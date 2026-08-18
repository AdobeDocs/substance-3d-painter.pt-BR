---
helpx_url: "https://helpx.adobe.com/br/substance-3d-painter/getting-started/export.html"
breadcrumb-title: ''
description: Saiba como exportar texturas do Substance 3D Painter em vários formatos para uso em outros aplicativos e mecanismos de jogo.
helpx_creative_field: ""
helpx_description: Painter > Getting Started > Export
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Exportar
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '292'
ht-degree: 1%

---


# Exportar

## Exportar texturas

As texturas são exportadas como uma coleção de bitmaps. O Painter oferece muita flexibilidade ao exportar texturas graças a Modelos de saída. Os modelos de saída permitem controlar coisas como a nomeação de arquivos exportados, como as texturas são empacotadas em canais e o formato e a profundidade de bits dos arquivos exportados. Se isso soar intimidante, não se preocupe, o Painter inclui dezenas de Modelos de saída padrão configurados para aplicativos 3D usados com frequência e casos de uso.

Você abre a <b>janela Exportar</b> e começa a exportar texturas com <b>Arquivo > Exportar Texturas</b> ou usa o atalho de teclado <b>CTRL + SHIFT + E</b>. Use os links a seguir para saber mais sobre a Exportação de texturas:

* [Janela Exportar](../export/export-window/export-window.md)
* [Modelos de saída](../export/export-presets/export-presets.md)
* [Modificar ou criar Modelos de saída](creating-export-presets.md)

### Exportar sua malha

O Painter pode modificar sua malha importada, por exemplo, gerando UVs automaticamente. Se você fez alterações na malha no Painter, poderá exportá-la com <b>Arquivo > Exportar malha</b>.

Ao exportar uma malha, você terá algumas opções:

* <b>Sem deslocamento/mosaico</b>: exporta a malha de base sem modificar a geometria baseada em materiais.
  * <b>Aplicar triangulação</b>: se a malha importada foi feita de quads ou polígonos, você pode habilitar esta opção para exportar a versão triangulada do Painter da malha. Isso pode ajudar a evitar erros baseados em triangulação visual caso outros aplicativos triangulem de forma diferente.
* <b>Com deslocamento/mosaico</b>: o Painter mosaico a malha, adicionando mais polígonos, e usa deslocamento ou height para alterar a geometria da superfície da malha.
  * <b>Recalcular normais de vértice</b>: modificar a superfície da malha pode resultar em normais incorretos de vértices pré-existentes. Ao ativar essa opção, o Painter atualizará automaticamente os normais de vértice para o valor correto da nova superfície.

![](../assets/export-render.jpg){width="500px"}
