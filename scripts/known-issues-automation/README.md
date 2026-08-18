---
source-git-commit: 0376fe6500551442b28831d5742ecbbc9363ab19
workflow-type: tm+mt
source-wordcount: '828'
ht-degree: 1%

---
# Gerador de problemas conhecidos — Substance 3D Painter

Automatiza a geração do documento de marcação de problemas conhecidos para o Substance 3D Painter, publicado em:
`https://helpx.adobe.com/substance-3d-painter/release-notes/know-issues.html`

Os problemas foram originados do épico Jira `SBSFOUR-6267`. O script busca todos os problemas, filtra tudo o que já foi corrigido na versão de destino e gera um arquivo de markdown formatado pronto para confirmação.

---

## Início rápido

Estas etapas pressupõem que você já tenha concluído a configuração única abaixo.

1. Conectar à **GlobalProtect VPN**
2. Defina `TARGET_VERSION` no arquivo `.env` para a versão para a qual você está gerando documentos (por exemplo, `12.0.3`)
3. Executar o script a partir do diretório `scripts/known-issues-automation/`:

   ```
   python fetch_known_issues.py
   ```
4. Verifique o resumo de saída, ele relatará quantos problemas foram buscados e quantos foram excluídos
5. Copiar o `known-issues.md` gerado para `help/release-notes/known-issues.md`

> Se algum problema estiver ausente ou inesperado, inspecione `raw_issues.json` para ver exatamente o que o Jira retornou antes da aplicação da filtragem.

---

## Configuração única

### &#x200B;1. Instalar dependências

```bash
pip install requests python-dotenv
```

### &#x200B;2. Criar seu arquivo `.env`

```bash
cp .env.example .env
```

### &#x200B;3. Obter um token de acesso pessoal do Jira

1. Fazer logon em `https://jira.corp.adobe.com`
2. Vá para seu perfil → **Tokens de acesso pessoal** na barra lateral esquerda
3. Clique em **Criar token**, dê um nome a ele e copie o valor gerado

> Os PATs não expiram quando a sessão do navegador termina, tornando-os mais confiáveis do que os cookies de sessão para acesso à API com script.

### &#x200B;4. Preencha seu arquivo `.env`

```
JIRA_PAT=your-personal-access-token
TARGET_VERSION=12.0.3
OUTPUT_FILE=known-issues.md
```

`TARGET_VERSION` é a versão do Substance 3D Painter para a qual você está gerando a página de problemas conhecidos. Ele controla quais problemas corrigidos são excluídos — consulte a [Lógica de Filtragem](#filtering-logic) abaixo.

---

## Estrutura do repositório

```
.
├── README.md                  # This file
├── fetch_known_issues.py      # Main script
├── .env.example               # Environment variable template (safe to commit)
├── .env                       # Your local credentials — never commit this
├── raw_issues.json            # Raw Jira dump from last run — gitignored
└── known-issues.md            # Generated output from last run — gitignored
```

---

## Referência do Jira

| Campo | Valor |
|---|---|
| Instância do Jira | `https://jira.corp.adobe.com` |
| Chave do projeto | `SBSFOUR` |
| Problemas conhecidos épicos | `SBSFOUR-6267` |

Todos os problemas conhecidos devem ser vinculados a este épico para aparecerem no documento gerado. Se um problema precisar ser adicionado ou removido da página, atualize o épico no Jira em vez de editar a redução manualmente.

---

## Como o script funciona

### Etapa 1 — Buscar

O script consulta a API REST Jira usando JQL:

```
"Epic Link" = SBSFOUR-6267 ORDER BY created ASC
```

Os resultados são paginados em 50 ocorrências por página. Os seguintes campos são recuperados para cada problema: `summary`, `issuetype`, `status`, `affectedVersions`, `fixVersions`, `labels`.

A autenticação usa um token de Portador de `JIRA_PAT`. A instância corporativa do Jira usa um certificado SSL interno, de modo que a verificação do certificado está desabilitada para essas solicitações — esse é o comportamento esperado na rede Adobe.

### Passo 2 — Despejo de lixo em bruto

Antes de qualquer filtragem ou formatação, o script grava `raw_issues.json`. Esta é uma captura de tela simplificada de cada problema retornado pelo Jira e é sempre gerada, independentemente do que acontecer a seguir. Se a saída parecer errada, inspecione este arquivo primeiro — ele mostra exatamente quais dados Jira forneceu.

### Etapa 3 — Filtro

Os problemas são filtrados usando duas regras aplicadas juntas:

1. **Filtro de status** — somente problemas `Backlog` e `Dev In Progress` são conhecidos ativos. Problemas com o status `Fixed` são candidatos à exclusão, sujeitos à verificação de versão abaixo.

2. **Filtro de versão** — um problema de `Fixed` será excluído somente se uma de suas versões de correção for menor ou igual a `TARGET_VERSION`. Se a versão de correção for superior a `TARGET_VERSION`, o problema ainda será incluído porque a correção não foi enviada para a versão que está sendo documentada.

Isso manipula o caso em que duas versões estão em desenvolvimento simultaneamente: um problema corrigido no `12.1.0` permanece um problema conhecido para `12.0.3`.

Consulte [Lógica de Filtragem](#filtering-logic) para obter a tabela de decisão completa.

### Etapa 4 — analisar categorias

Cada resumo de ocorrência é analisado para marcas de categoria no início da sequência de caracteres:

- `[Shader] Some description` → categorias: `["Shader"]`, descrição: `"Some description"`
- `[Crash][Engine] Some description` → categorias: `["Crash", "Engine"]`, descrição: `"Some description"`
- `No brackets here` → nenhuma categoria, tratada como não categorizada

A **categoria primária** é sempre a primeira marca. Determina o agrupamento e o posicionamento da seção.

### Etapa 5 — Agrupar e classificar

As questões estão organizadas da seguinte forma:

- As ocorrências são agrupadas por categoria principal
- Os grupos são classificados por contagem de ocorrências, decrescente (maiores grupos primeiro)
- Os grupos com mais de um problema aparecem na parte superior do documento
- Grupos com apenas um problema, além de quaisquer problemas não categorizados, aparecem após os grupos de vários problemas sem cabeçalho de seção
- Problemas com `[Crash]` como categoria primária são sempre colocados por último, em uma seção `## Stability`

### Etapa 6 — Formatar e gravar

O script gera a saída de `known-issues.md` com:

- Interface do YAML (metadados helpx)
- Um cabeçalho `# Known issues` com um parágrafo de introdução que nomeia a versão de destino
- Problemas formatados como: `` * `[Category]` Description ``
- Problemas de várias categorias: `` * `[Category1]` `[Category2]` Description ``
- Linhas em branco entre grupos de categorias
- Uma seção `## Stability` no final para problemas de falha

---

## Lógica de Filtragem

| Status | Corrigir conjunto de versões? | Corrigir versão versus destino | Incluído? |
|---|---|---|---|
| `Backlog` | — | — | Sim |
| `Dev In Progress` | — | — | Sim |
| `Fixed` | Não | — | Não (excluído de forma conservadora) |
| `Fixed` | Sim | Corrigir versão ≤ destino | Não (já enviado) |
| `Fixed` | Sim | Corrigir versão > destino | Sim (a correção está em uma versão futura) |

---

## Formato de saída

```markdown
---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/release-notes/know-issues.html"
...
---

# Known issues

This page lists all the active known issues present in v12.0.3 of Substance 3D Painter:

* `[Engine]` Error when using Smart Materials if Texture Set has no tile 1001
* `[Engine]` Geometry mask shows artifacts at UV borders with instanced layers

* `[Shader]` user0 channel always can not be read as sRGB with specific shader

* `[Export]` GLTF exports at the wrong size
* `[Import]` Cannot import obj file with "nan" values

## Stability

* `[Crash]` Select "Export mesh" when mesh failed to load
```

**Observação de formatação:** as marcas de categoria usam a disposição de backtick único — `` `[Category]` `` — não são backticks duplos. O documento legado mantido manualmente continha erros de duplo backtick; o script sempre produz o formato correto.

---

## Solução de problemas

**401 Não Autorizado**
- Confirme se você está conectado ao **GlobalProtect VPN**
- Seu PAT pode ter expirado ou sido revogado. Gere um novo em `https://jira.corp.adobe.com/secure/ViewProfile.jspa` e atualize o `.env`

**`JIRA_PAT is not set`erro**
- Verifique se você criou um arquivo `.env` de `.env.example` e preencheu o token
- Confirme se você está executando o script de dentro do diretório `scripts/known-issues-automation/` para que `python-dotenv` possa localizar o arquivo `.env`

**Problemas ausentes na saída**
- Verificar `raw_issues.json` — se o problema não existir, ele não está vinculado ao épico `SBSFOUR-6267` no Jira
- Se o problema estiver em `raw_issues.json`, mas não na saída, ele foi excluído pelo filtro — verifique seu status e corrija a versão em relação ao `TARGET_VERSION`

**`TARGET_VERSION`aviso em tempo de execução**
- O script será executado, mas excluirá de forma conservadora todos os `Fixed` problemas se `TARGET_VERSION` não estiver definido. Sempre defina antes de gerar o documento final.
