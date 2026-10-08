---
breadcrumb-title: ""
description: Saiba como corrigir a exibição incorreta de miniaturas na prateleira do Substance 3D Painter para garantir visualizações precisas de recursos.
title: As miniaturas na prateleira parecem incorretas
user-guide-description: ""
user-guide-title: ""
source-git-commit: 6b6d52207ca1d043aaa1b2b14145b6b49d4c1942
workflow-type: tm+mt
source-wordcount: '131'
ht-degree: 0%
---

# As miniaturas na prateleira parecem incorretas

Se as miniaturas na prateleira parecem ser diferentes do habitual, pode ser por causa do sombreador usado para renderizar as visualizações.

| Miniaturas quebradas | Miniaturas normais |
| --- | --- |
| <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r1-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../../assets/shelf-broken-preview.png"/></div> | <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r1-column-c1_dynamic_grid_items_grid-cell_position-par_image" src="../../../assets/shelf-normal-preview.png" width="300px"/></div> |

## 1 - Abra a janela principal de configurações

Vá para **Editar** e clique em **Configurações**:

![](../../../assets/pref-menu.png)

## 2 - Remover o sombreador de visualização da prateleira

Na exibição **Geral**, role para baixo até que a seção “Opções de visualização” esteja visível.\
Clique no botão **cruz** em frente ao &quot; **Sombreamento de visualização do material** &quot; para remover o sombreador atual especificado.

![](../../../assets/remove-preview-shader.png){width="450px"}

## 3 - Reiniciar o Substance 3D Painter

Para regenerar as miniaturas para que elas pareçam corretas, o Substance 3D Painter precisa ser reiniciado.
