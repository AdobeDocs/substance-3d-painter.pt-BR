---
helpx_url: "https://helpx.adobe.com/br/substance-3d-painter/release-notes/old-versions/version-2-6.html"
breadcrumb-title: ''
description: Consulte as notas de versão do Substance 3D Painter versão 2.6 para saber mais sobre novos recursos, aprimoramentos e correções de erros.
helpx_creative_field: ""
helpx_description: Painter > Release notes > Old versions > Version 2.6
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Versão 2.6
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '1055'
ht-degree: 0%

---


# Versão 2.6

Com o **Substance Painter 2.6**, nosso foco era fornecer uma maneira de gerenciar os conjuntos de texturas diretamente no Substance Painter, sem a necessidade de criar um novo projeto ou reimportar sua malha com nomes de material atualizados. Também queríamos fornecer uma maneira de atualizar os recursos usados em projetos, algo que vimos como solicitado muito no passado.

Data de lançamento: *27 de abril de 2017*

## Principais recursos

### Novo projeto de amostra “Meet Mat”

![](../../assets/meetmat-render.jpg)

Este novo projeto de amostra oferece um novo personagem brilhante e adorável chamado “**Mat**”. Contém três conjuntos de texturas prontos para serem pintados.\
Participe do concurso **Meet Mat** com ele para ganhar alguns prêmios muito legais : <https://www.allegorithmic.com/contest/meet-mat-2017-substance-3d-painting-contest>

### Nova API de script com capacidade de atualizar recursos em projetos

![](../../assets/resources-updater-ui.jpg)

A API de script do Substance Painter foi aprimorada para adicionar novas funções que permitem **substituir recursos** no projeto por outras versões. Para demonstrar esse novo recurso, um novo **plug-in** criado com a API de script foi adicionado e permite procurar todos os recursos contidos em um determinado projeto. Os recursos marcados como vermelhos são detectados como “desatualizados” e podem ser substituídos automaticamente. Esse recurso não se limita a recursos “desatualizados”; qualquer ativo pode ser substituído por outro. Isso oferece muitas possibilidades novas e mostra ainda mais como o Substance Painter é uma **ferramenta de pintura não destrutiva**!

O **plug-in** está disponível no GitHub. Não hesite em ajudar se você vir possíveis melhorias: <https://github.com/AllegorithmicSAS/painter-plugin-resources-updater>

![](../../assets/resource-update-demo.gif)

### Nova capacidade de renomear e reatribuir conjuntos de texturas

![](../../assets/texture-set-rename-description.png)

Agora é possível alterar o nome de um conjunto de texturas diretamente dentro do Substance Painter. Renomear um conjunto de texturas afetará o nome das texturas exportadas no disco (dependendo da predefinição de exportação usada).\
Para renomear um conjunto de texturas, basta clicar duas vezes no nome para modificá-lo ou usar o botão direito do mouse para abrir o menu de contexto. Também é possível adicionar descrições personalizadas para fornecer mais informações sobre o que os conjuntos de texturas fazem. Isso pode ser muito útil ao trabalhar em um [projeto UDIM](https://helpx.adobe.com/br/substance-3d/unlisted/documentation/spdoc/uv-tile-udim-legacy-144310352.html). Use o botão “**configurações**” para configurar a maneira como as descrições são exibidas na lista.

![](../../assets/reasign-texture-set.png)

Os conjuntos de textura agora podem ser reatribuídos a diferentes materiais de malha. Isso significa que é possível **recuperar** conjuntos de texturas desabilitados anteriormente (porque estavam ausentes na malha) ou até mesmo **trocá-los**. Basta clicar no novo botão “**configurações**” na janela Lista de Conjuntos de Texturas e clicar na entrada “**Reatribuir Conjuntos de Texturas**”. Ele abrirá uma nova janela dedicada ao gerenciamento dos conjuntos de texturas e como eles são vinculados aos materiais de malha. O gerenciamento pode ser feito **arrastando e soltando** um nome de conjunto de texturas onde você quiser.

## Tutorial

Os novos recursos principais são abordados em nosso tutorial em vídeo mais recente:

## Notas de versão

### 2.6.2

(Lançado em 20 de outubro de 2017)

**Adicionado:**

* [Conjunto de texturas] Permite excluir conjuntos de texturas desativados
* [Prateleira] Permite que vários usuários gravem dentro da mesma pasta de prateleira
* [Script] Poder recarregar a pasta de plug-ins
* [Script] Adicione uma versão mínima necessária da API nos metadados do plug-in para garantir a compatibilidade
* [IRay] Melhorias na caixa de diálogo Exportar imagem

**Corrigido:**

* [Engine] Problema de desaparecimento de traços, ao alterar a resolução (4K>2K)
* [Padeiros] Falha no cozimento do mapa de ID com a opção Corresponder pelo nome ativada
* [Padeiros] As mensagens de erro não são suficientemente explícitas
* [Exibição 3D] O espaço tangente não é sincronizado com padeiros
* [Ferramenta] Artefatos pretos ao usar a ferramenta de borrar
* [Shader] O sombreador não PBR não funciona mais
* [Shader] “pbr-coated” está quebrado
* [Shader] A aspereza do revestimento do sombreador “revestido com pbr” não tem mais impacto
* [Shader] O sombreador de brilho de especificação não corresponde a Iray e SD
* [Prateleira] Falha ao carregar dois arquivos com o mesmo nome, mas com extensões diferentes
* [Prateleira] Não é mais possível editar a predefinição nas prateleiras
* [Prateleira] Não é possível definir uma visualização personalizada para ativos importados na prateleira
* Os recursos carregados do cache perdem seus usos
* Salvar um projeto antes de criar um modelo retorna erros de permissão de gravação
* Salvar projeto incorreto se o nome do arquivo contiver dois pontos
* Importação de arquivos com vários pontos (.) no nome do arquivo causa problemas

### 2.6.1

(Lançado em 12 de maio de 2017)

**Adicionado:**

* [TextureSet] Não permitir a reatribuição de materiais de malha a nada

**Corrigido:**

* Falha ao alternar o TextureSet após substituir o mapa baked
* Falha ao fazer “Desfazer e Refazer” após alterar o modo de mesclagem da camada
* Falha ou congelamento ao usar o efeito “seleção de cores” com um mapa de ID grande
* [Exportar] Os conjuntos de texturas renomeados não são classificados em ordem alfabética na janela de exportação
* [TextureSet] Redefinir para o nome padrão não verifica a unicidade
* [TextureSet] O conjunto de texturas renomeado é desativado após a reabertura do projeto
* [Prateleira] Conteúdo de modelos padrão ausente
* [Prateleira] As texturas não quadradas são exibidas como quadradas
* [Shader] Depois que um conjunto de textura é desativado, o sombreador associado é destruído
* [Scripting] alg.baking.setTextureSetBakingParameters() não funciona mais
* [Script] Erro de digitação no tutorial do websocket
* [Scripting] Vários problemas em AlgWidgets
* [Log] Detecção incorreta de memória virtual disponível em alguns casos

### 2.6.0

(Lançado em 27 de abril de 2017)

**Adicionado**:

* Adicionar novo projeto de amostra “Meet Mat”
* [Plug-in] Novo plug-in “Atualizador de recursos”
* [TextureSet] Permite renomear e adicionar uma descrição a conjuntos de textura
* [TextureSet] Permitir a reatribuição de materiais
* [TextureSet] Adiciona um botão de configuração na janela de lista do conjunto de textura
* [TextureSet] Mostra os conjuntos de texturas “desativados” na parte inferior da lista
* [Substance] Use mapas adicionais na resolução atual do conjunto de texturas para melhorar o desempenho
* [Script] Permite atualizar um recurso usado em um projeto (material, gerador etc.)
* [Script] Adicionar uma maneira de adicionar/remover uma prateleira
* [Scripts] Permitir a consulta de informações do recurso em projetos
* [Scripting] Permite recuperar uma lista de prateleiras disponíveis
* [Script] Tutorial de aprimoramento de miniatura do AlgWidget
* [Export] Desativar/ativar profundidade de bits com base no suporte ao formato de arquivo
* [Log] Adicionar nome de plug-in para imprimir no console
* [Log] Remover erro sobre conjuntos de texturas ocultos
* Atualizar “Tela de boas-vindas” com novos ícones e texto para amostras

**Corrigido**:

* Falha ao atualizar uma malha em projetos específicos
* [Janela de visualização] A cor interna do plano de simetria não está mais visível
* [Janela de visualização] Alguns efeitos de pós-processo são ativados ao usar a visualização individual
* [Shaders] A mesclagem “over\_premult” não funciona corretamente
* [Shaders] Aviso sobre o teste alfa com o sombreador padrão
* [Prateleira] Análise incorreta de marcas de Substance
* [Shelf] O Envolvimento de Ferrugem do MatFX não funciona corretamente
* [Prateleira] O filtro HSL está habilitado em canais incorretos por padrão
* [Prateleira] A nitidez está ativada no canal Height/Normal por padrão
* [Exportar] As predefinições de exportação do Vray não usam um mapa normal do OpenGL
* [Ferramenta] Problemas de imprecisão com a ferramenta clonar/borrar criam artefatos
