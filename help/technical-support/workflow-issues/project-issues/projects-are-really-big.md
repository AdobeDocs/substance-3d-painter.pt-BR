---
helpx_url: "https://helpx.adobe.com/br/substance-3d-painter/technical-support/workflow-issues/project-issues/projects-are-really-big.html"
breadcrumb-title: ''
description: Saiba como reduzir o tamanho dos arquivos de projeto do Substance 3D Painter para otimizar os requisitos de desempenho e armazenamento.
helpx_creative_field: ""
helpx_description: Painter > Technical support > Workflow Issues > Project Issues > Projects are really big
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Projetos são realmente grandes
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '883'
ht-degree: 0%

---


# Projetos são realmente grandes

O projeto do Substance 3D Painter pode ser muito grande e usar muito espaço em disco. Esta página explica por que e como mitigá-la.

## Que tipo de recurso é armazenado em um projeto?

Cada ativo ou recurso usado durante a texturização é armazenado no arquivo de projeto, incluindo:

* **Malha de Origem** (não é o arquivo original, mas um arquivo processado)
* **Mapas de malha cozida**
* **Materiais** (como materiais de Substance)
* **Bitmaps** ou outros recursos usados por qualquer camada/predefinição/traçado de pincel.

As malhas de alto polietileno não estão incluídas no projeto. Eles estão apenas ligados.

## Por que um projeto armazena tantos recursos?

Armazenar todos os recursos usados torna um projeto completamente autônomo e facilmente móvel de um computador para outro sem quebrá-lo. A principal desvantagem é o espaço potencialmente grande do arquivo no disco.

A decisão de ter tudo incorporado no arquivo do projeto vem do fato de que tudo não é destrutivo. Isso significa que o projeto se “reconstrói” quando é reaberto. Se um único pincel ou material estiver ausente da prateleira, o projeto poderá se quebrar e não poderá ser regenerado corretamente. Armazenar uma duplicata do recurso garante que o projeto ainda possa ser restaurado quando foi salvo.

## Há uma maneira de reduzir o tamanho de um projeto?

Há algumas maneiras de reduzir o tamanho de um projeto:

### Limpar recursos não utilizados

Ao usar muitos recursos no projeto, o Substance 3D Painter os copia. Por exemplo, se você usou um alfa para pintar algo. Se, posteriormente, você excluir a camada quando o alfa for pintado, o Substance 3D Painter não removerá automaticamente o recurso.

Para remover o recurso não utilizado, use a ação **Limpar** no menu [Arquivo](https://substance3d.adobe.com/display/DRAFTPAINTER/File+menu). Em seguida, salve o projeto (isso acionará a remoção real do recurso).

Os recursos que ainda são usados em um projeto não podem ser removidos. Isso significa que o conjunto de texturas desativado ainda faz referência a recursos e impede que eles sejam excluídos. Para evitar isso, remova os Conjuntos de Textura desabilitados na [janela de reatribuição de Conjunto de Textura](../../../interface/texture-set/texture-set-reassignment.md).

### Reduzir a resolução do conjunto de textura

Quando um projeto é salvo, o resultado final da pilha de camadas de um conjunto de texturas é salvo no projeto. Isso permite preservar uma visualização no visor quando o projeto é reaberto sem ter que recalcular o conjunto de texturas. Quanto maior for a resolução do conjunto de texturas, maior será o cache de visualização.

Para reduzir o espaço ocupado pelo cache, basta alterar a resolução para um número menor, como 512, por exemplo. Como o Substance 3D Painter não é destrutivo, essa resolução pode ser alterada novamente sem perder a qualidade.

### Compactar o projeto

Salvar um projeto incrementalmente (via CTRL+S) pode fragmentar o arquivo de projeto. Embora não seja um problema crítico, isso pode introduzir espaço vazio no arquivo de projeto, o que pode aumentar o tamanho.

Use a função “Salvar e Compactar” no [Menu Arquivo](../../../interface/main-menu/file-menu.md) para salvar o projeto novamente e remover o espaço vazio desperdiçado. Essa ação de salvamento será mais longa do que o salvamento normal, mas pode reduzir significativamente o espaço ocupado pelo arquivo.

### Reduza o tamanho dos mapas de malha cozidos

Em geral, o maior culpado e a razão pela qual um projeto ocupa tanto espaço no disco é porque os mapas de malha assados são muitos e grandes.

Para reduzir o tamanho dos mapas de malha, algumas ações podem ser feitas:

* *Use uma resolução de cozimento mais baixa.*\
  Embora o mapa Normal possa se beneficiar de ser assado em 4K, este pode não ser o caso para o mapa de Posição, que geralmente é apenas sobre gradientes coloridos. Faça em dois passos com duas resoluções diferentes para misturar tamanhos de arquivo diferentes.
* *Exportar as texturas e reduzir manualmente o impacto.*\
  Por padrão, o Substance 3D Painter assenta todas as texturas como imagens RGBA em 16 bits, o que inclui os padeiros em tons de cinza, como a Oclusão ambiente.

  Para reduzir as texturas assadas para impressão, use este passo a passo:
  1. Desative a configuração “Aplicar difusão” na janela Padeiro
  1. Defina “Dilatação com” como um valor razoável (32 pixels para uma resolução de 2048, por exemplo)
  1. Faça todas as texturas na mesma resolução
  1. Exporte as texturas assadas com a predefinição de exportação “Mapas de malha” como PNG de 16 bits com o preenchimento definido como “Sem preenchimento (passagem)”
  1. Abra cada mapa em um software de edição de fotos ou no Substance 3D Designer
  1. Reduza a resolução das texturas para as quais ela parece encaixada. Certifique-se de alternar a Oclusão ambiente, a Curvatura e o Thickness de colorido para tons de cinza.
  1. Salve as novas versões de textura como PNG de 16 bits.
  1. Reimporte as texturas e substitua-as sobre as texturas de cozimento originais nas configurações do Conjunto de texturas.
  1. Use a ação Limpar no menu Arquivo para remover os antigos Mapas de malha.
  1. Use a ação Salvar e compactar no menu Arquivo para compactar o arquivo de projeto.\
     Depois de todas essas etapas, o impacto no projeto deve ser reduzido significativamente.

É importante que os mapas de malha permaneçam com texturas de pelo menos 16 bits. Embora as texturas de 8 bits possam ter um impacto menor, elas introduzirão artefatos em materiais inteligentes e geradores de máscaras. Recomendamos o PNG porque ele é um formato de compactação sem perdas, o que significa que ainda compactará as texturas sem introduzir artefatos e também é compatível com 16 bits.
