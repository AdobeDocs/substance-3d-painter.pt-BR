---
helpx_url: "https://helpx.adobe.com/br/substance-3d-painter/interface/viewport/2d-view.html"
breadcrumb-title: ''
description: Aprenda a usar a visualização 2D no Substance 3D Painter para visualizar e editar texturas no espaço UV para uma pintura com textura precisa.
helpx_creative_field: ""
helpx_description: Painter > Interface > Viewport > 2D view
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Exibição 2D
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '285'
ht-degree: 0%

---


# Exibição 2D

![](../../assets/2d-view.jpg){width="450px"}

A Exibição 2D exibe as Ilhas UV de malha do [Conjunto de Textura](../texture-set/texture-set.md) atualmente selecionado. Ele permite ver as texturas da pilha de camadas, mas também pintar nas Ilhas UV de malha.

## Modo de exibição

![](../../assets/display-mode-1.png)

No canto superior direito da viewport está o menu suspenso do modo de exibição. Esse controle permite alterar as informações que devem estar visíveis na viewport. Permite exibir canais únicos, mapas de malha ou o resultado final do material com iluminação.

## Informações do Eixo

![](../../assets/2d-axis.png)

Na parte inferior direita do visor estão as **Informações do Eixo**, que indicam a direção dos eixos bidimensionais. No caso da visualização 2D, os eixos são U e V.

## Informações de Bloco UV

![](../../assets/2d-view-button.png)

Ao lado do **Modo de Exibição** está o botão **Informações de Bloco UV** que permite mostrar/ocultar informações relacionadas aos Blocos UV. Este botão não é visível com projetos regulares.

## Fluxo de trabalho do projeto

Dependendo do fluxo de trabalho definido ao criar um projeto, a exibição 2D pode ter uma aparência e um comportamento diferentes:

| *Fluxo de Trabalho do Projeto* | *Comportamentos* |
| --- | --- |
| **Projeto regular** | Com o projeto regular, somente o UV com o intervalo UV [0-1] pode ser pintado. Qualquer item fora desse intervalo será visível, mas não será interativo.Neste exemplo, somente as Ilhas UV à esquerda podem ser pintadas (com o fundo cinza claro atrás). <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r1-column-c1_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/2d-view-range-regular.jpg" width="500px"/></div> |
| **Projeto de Bloco UV** | Com o projeto UV Tile, cada gama UV é um novo conjunto de texturas, que pode ser pintado. A exibição 2D também exibe uma grade para ver melhor como cada bloco está organizado. Cada bloco terá um número UDIM atribuído. <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r2-column-c1_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/2d-view-range-uvtiles.jpg" width="500px"/></div> |
