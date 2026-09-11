---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/pipeline-and-integration/resource-management/excluding-resources-in-a-resource-path.html"
breadcrumb-title: ''
description: Saiba como excluir recursos específicos de caminhos de recursos no Substance 3D Painter para uma melhor organização de prateleira.
helpx_creative_field: ""
helpx_description: Painter > Pipeline and integration > Resource management > Excluding resources in a resource path
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Excluindo recursos em um caminho de recurso
user-guide-description: ''
user-guide-title: ''
source-git-commit: 22871eab2f25d09bd82f1292d8b3e5f8c4f1c2cf
workflow-type: tm+mt
source-wordcount: '451'
ht-degree: 0%

---


# Excluindo recursos em um caminho de recurso

Esta página explica como configurar e ignorar arquivo para especificar recursos e pastas que serão ignorados durante o processo de rastreamento da janela [Ativos](../../interface/assets/assets.md). Permite evitar que recursos indesejados sejam exibidos.

>[!NOTE]
>
> Essa funcionalidade está disponível desde a versão 7.2.3.

## Criando um arquivo ignorado

Navegue até o local da pasta de recursos na qual deseja ocultar recursos. Em seguida, crie um arquivo com o seguinte nome:

```
.ignore_assets_pt
```


>[!NOTE]
>
> Observe que o nome do arquivo deve começar com um ponto.

Ele deve ficar parecido com o seguinte depois de criado:

![](../../assets/ignore-file-location.png)

## Exemplo

O conteúdo do arquivo a seguir descartará todos os recursos e pastas que não sejam as pastas de biblioteca padrão:

```
## exclude all

* 

 

## re-include library directories

!alphas 

!colorluts 

!effects 

!emitters 

!environments 

!export-presets 

!generators 

!materials 

!presets 

!procedurals 

!receivers 

!shaders 

!smart-masks 

!smart-materials 

!templates 

!textures
```


## Regras e diretrizes

A tabela a seguir mostra as regras gerais que se aplicam ao arquivo ignorado.

>[!NOTE]
>
> A correspondência de padrão do arquivo ignorado diferencia maiúsculas de minúsculas, independentemente do comportamento do Sistema Operacional.

| Regra | Descrição | Exemplo |
| --- | --- | --- |
| **Linha em Branco** | Linha vazia que não corresponde a nada. Pode ser usado como um separador para facilitar a leitura. |  |
| **Separador de diretório** | A barra é usada como separador de diretório. Os separadores podem ocorrer no início, no meio ou no fim de um padrão de pesquisa.Se houver um separador no início ou no meio (ou ambos) do padrão, o padrão é relativo ao nível de diretório do próprio arquivo ignorado. Caso contrário, o padrão também poderá corresponder a qualquer nível abaixo do nível de ignorar arquivo. Se houver um separador no fim do padrão, ele será ignorado; o padrão ainda corresponderá a arquivos e diretórios. | `folder/filename.extension   folder/sub-folder` |
| **Linha de comentário** | Uma linha que começa com o sinal numérico (ou hash) serve como comentário. | `# This is a comment` |
| **Asterisco** | Um asterisco corresponde a qualquer item, exceto uma barra. | `# Match anything starting with Alpha   alpha*   # Match any file with given extension   *.jpg` |
| **Intervalo de caracteres** | O intervalo de caracteres pode ser especificado entre colchetes para corresponder à pasta e aos nomes de arquivo.<ul data-preserve-html="true"> <li data-preserve-html="true"><b>[abc]</b>: corresponde a um caractere na lista fornecida</li> <li data-preserve-html="true"><b>[a-c]</b>: corresponde a um caractere no intervalo especificado</li> <li data-preserve-html="true"><b>[ !abc]</b>: um caractere não corresponde na lista fornecida</li> <li data-preserve-html="true"><b>[ !a-c]</b>: não corresponde a um caractere no intervalo especificado</li> </ul>O intervalo e a lista também podem ser números com o formato <b>[0-9]</b>. | `# Exclude any UDIM image in PNG   *_[0-9][0-9][0-9][0-9].png` |
| **Caractere de escape** | Indique caracteres literais que, de outra forma, seriam ignorados ou usados como regras. | `# This is a comment   [#]This/Is/A/Path` |
| **Espaços à direita** | Espaços à direita são ignorados, a menos que sejam prefixados por escape. | `# Match a subfolder with trailing space   folder/subfolder[ ]` |
| **Prefixo de Exclamação** | Prefixar um padrão com um ponto de exclamação permite negá-lo.Qualquer arquivo correspondente excluído por um padrão anterior será incluído novamente. Não é possível incluir novamente um arquivo se um diretório pai desse arquivo for excluído. O rastreamento não lista diretórios excluídos por motivos de desempenho, portanto, quaisquer padrões nos arquivos contidos não têm efeito, independentemente de onde estejam definidos. | `# Re-include specific file   !my_file_name.png` |
