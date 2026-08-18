---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/painting/fill-projections/spherical-projection.html"
breadcrumb-title: ''
description: Use projeção esférica no Substance 3D Painter para projetar texturas de uma esfera para quebrar texturas em torno de objetos.
helpx_creative_field: ""
helpx_description: Painter > Painting > Fill projections > Spherical projection
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Projeção esférica
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '855'
ht-degree: 2%

---


# Projeção esférica

![](../../assets/spherical-proj.jpg)

A Projeção esférica de preenchimento permite projetar imagens e padrões ao redor de um objeto. Pode ser útil projetar em objetos redondos ou distorcer a textura em padrões circulares.

## Propriedades

| Configuração | Descrição |
| --- | --- |
| **Filtragem** | Controla como a textura ou o material será filtrado. Essa configuração pode afetar a aparência da textura quando repetida várias vezes. Com valores de dimensionamento altos, o uso de um filtro diferente do padrão pode produzir resultados com melhor aparência. Configurações atuais disponíveis:<ul data-preserve-html="true"><li data-preserve-html="true"><strong>Bilinear | HQ</strong> (padrão): filtragem bilinear avançada que tenta melhorar a qualidade da textura quando os valores de divisão em blocos gráficos estão altos.</li><li data-preserve-html="true"><strong>Bilinear | Nítido</strong>: filtragem bilinear simples que suaviza ligeiramente a textura, mas tenta preservar os detalhes.</li><li data-preserve-html="true"><strong>Mais próximo</strong>: sem filtragem, útil se a filtragem Bilinear fornecer um resultado desfocado e quebrar detalhes finos. É possível introduzir suavização na textura.</li></ul> |
| **Envoltório UV** | Controla como a textura se repete dentro da projeção. Os valores possíveis são:<ul data-preserve-html="true"><li data-preserve-html="true"><strong>Nenhuma</strong>: a textura não se repete. Qualquer item fora da textura é preto/transparente.</li><li data-preserve-html="true"><strong>Repetir horizontalmente</strong>: a textura se repete apenas horizontalmente.</li><li data-preserve-html="true"><strong>Repetir verticalmente</strong>: a textura só se repete verticalmente.</li><li data-preserve-html="true"><strong>Repetição</strong> (padrão): a textura se repete em ambos os eixos.</li></ul> <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r2-column-c1_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/spherical-repeat.jpg" width="500px"/></div> |
| **Corte De Formas** | Defina se a textura projetada deve ser visível fora da área de projeção. Os valores possíveis são:<ul data-preserve-html="true"><li data-preserve-html="true"><strong>Projeto cortado na forma</strong>: a projeção está confinada dentro da área de projeção.</li><li data-preserve-html="true"><strong>A projeção se estende para fora da forma</strong> (padrão): a projeção continua além da área de projeção.</li></ul> <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r3-column-c1_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/spherical-shape-crop.jpg" width="500px"/></div> |

### Transformação UV

As configurações de transformação UV controlam a textura dentro da projeção.

| *Configuração* | *Descrição* |
| --- | --- |
| **Escala** | Defina quantas vezes a textura se repetirá dentro da projeção. |
| **Rotação** | Controle o ângulo da textura aplicada à projeção. |
| **Deslocamento** | Controle a origem da textura projetada. O valor padrão significa que a textura está no meio da projeção. |

### Configurações de projeção 3D

As configurações de projeção 3D controlam a transformação da projeção no espaço 3D.

| Configuração | Descrição |
| --- | --- |
| **Deslocamento** | Posição da origem da projeção no espaço 3D. As unidades são baseadas na caixa delimitadora de toda a cena. 0 é o centro desta caixa. |
| **Rotação** | Ângulos em graus para girar toda a projeção em cada eixo. |
| **Escala** | Tamanho de toda a projeção em cada eixo. |

## Barra de ferramentas Contextual

Várias configurações e ferramentas estão disponíveis na [barra de ferramentas contextual](../../interface/toolbars.md) localizada na parte superior da viewport, que fornece controles sobre o manipulador e a projeção:

| Ícone | Nome | Descrição |
| --- | --- | --- |
| <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table1_row-r1-column-c0_image" src="../../assets/icon-hide-manipulator.png" width="50px"/></div> | Mostrar/Ocultar manipulador | Se ativado, o manipulador fica visível e é controlável na viewport. |
| <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table1_row-r2-column-c0_image" src="../../assets/icon-manipulator-settings.png" width="50px"/></div> | Configurações do manipulador | Esse menu contém três configurações:<ul data-preserve-html="true"><li data-preserve-html="true"><strong>Tamanho do manipulador</strong>: controla o tamanho do manipulador no visor.</li><li data-preserve-html="true"><strong>Etapas de grade</strong>: defina o tamanho da etapa ao traduzir com uma restrição.</li><li data-preserve-html="true"><strong>Etapas de ângulo</strong>: defina o ângulo da etapa ao girar com uma restrição.</li></ul> |
| <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table1_row-r3-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/icon-translate.png" width="50px"/></div> | Manipulador de tradução | Permitir mover a projeção na cena ao longo dos eixos principais (X, Y, Z). |
| <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table1_row-r4-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/icon-rotate.png" width="50px"/></div> | Manipulador de rotação | Permitir girar a projeção na cena ao longo dos eixos principais (X, Y, Z). |
| <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table1_row-r5-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/icon-scale.png" width="50px"/></div> | Manipulador de escala | Permitir dimensionar a projeção na cena ao longo dos eixos principais (X, Y, Z). |
| <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table1_row-r6-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/icon-surface.png" width="50px"/></div> | Manipulador de superfície | Permita mover a projeção ajustando-a à superfície do modelo 3D.  **Observação:** este manipulador só está disponível com os tipos de projeção Planar e Distorcer. |
| <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table1_row-r7-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/icon-space.png" width="50px"/></div> | Espaço do manipulador | Defina em qual espaço a transformação é executada. Os valores possíveis são:<ul data-preserve-html="true"><li data-preserve-html="true"><strong>Espaço local</strong>: os eixos estão alinhados com a transformação atual.</li><li data-preserve-html="true"><strong>Espaço global</strong>: os eixos estão alinhados com a cena.</li></ul> |
| <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table1_row-r8-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/icon-flip-x.png" width="50px"/></div> | Espelho em X | Vire a transformação no eixo X. |
| <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table1_row-r9-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/icon-flip-y.png" width="50px"/></div> | Espelho em Y | Vire a transformação no eixo Y. |
| <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table1_row-r10-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/icon-flip-z.png" width="50px"/></div> | Espelho em Z | Vire a transformação no eixo Z. |
| <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table1_row-r11-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/icon-reset.png" width="50px"/></div> | Redefinir transformação | Restaure a transformação de projeção de volta ao seu estado padrão. |

## Manipulador

Este manipulador de projeção só está disponível no [visor 3D](../../interface/viewport/3d-view.md).

| Ação | Atalho | Descrição |
| --- | --- | --- |
| **Tradução** | Clique do mouse | Com o manipulador de tradução, clique nos eixos para mover a projeção:<ul data-preserve-html="true"><li data-preserve-html="true"><strong>Um eixo</strong>: mover apenas em uma direção a projeção.</li><li data-preserve-html="true"><strong>Dois eixos</strong>: mova a projeção nos planos alinhados aos eixos.</li><li data-preserve-html="true"><strong>Três eixos</strong>: mova a projeção no espaço da câmera (plano de frente para ela).</li></ul>   <table> <tr style="border: 0;"> <td style="border: 0;" valign="top">  <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table2_row-r1-column-c2_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/3d-translate.gif" width="200px"/></div>  </td> <td style="border: 0;" valign="top">  <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table2_row-r1-column-c2_dynamic_grid_items_grid-cell1_position-par_image" src="../../assets/3d-translate-2axes.gif" width="200px"/></div>  </td> <td style="border: 0;" valign="top">  <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table2_row-r1-column-c2_dynamic_grid_items_grid-cell2_position-par_image" src="../../assets/3d-translate-3axes.gif" width="200px"/></div>  </td> </tr> </table> |
| **Tradução restrita** | Clique com a tecla SHIFT pressionada | Com o manipulador Translação, mova a projeção ao longo dos eixos selecionados, mas somente em intervalos específicos (revisão). O tamanho do intervalo é definido através das configurações do manipulador. <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table2_row-r2-column-c2_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/3d-translate-step.gif" width="200px"/></div> |
| **Rotação** | Clique do mouse | Com o manipulador de rotação, clique em um eixo para girar a projeção. Clique entre os eixos para girar todos os eixos ao mesmo tempo.   <table> <tr style="border: 0;"> <td style="border: 0;" valign="top">  <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table2_row-r3-column-c2_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/3d-rotate.gif" width="200px"/></div>  </td> <td style="border: 0;" valign="top">  <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table2_row-r3-column-c2_dynamic_grid_items_grid-cell1_position-par_image" src="../../assets/3d-rotate-3axes.gif" width="200px"/></div>  </td> </tr> </table> |
| **Rotação restrita** | Clique com a tecla SHIFT pressionada | Com o manipulador de rotação, clicar em um eixo para girar a projeção só acontecerá em intervalos específicos. O passo é definido por um ângulo através das configurações do manipulador. <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table2_row-r4-column-c2_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/3d-rotate-step.gif" width="200px"/></div> |
| **Escala** | Clique do mouse | Com o manipulador de Escala, clique em uma alça de eixo para redimensionar a projeção ao longo do eixo fornecido.   <table> <tr style="border: 0;"> <td style="border: 0;" valign="top">  <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table2_row-r5-column-c2_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/scale-one-axis.gif" width="200px"/></div>  </td> <td style="border: 0;" valign="top">  <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table2_row-r5-column-c2_dynamic_grid_items_grid-cell1_position-par_image" src="../../assets/scale-two-axis.gif" width="200px"/></div>  </td> <td style="border: 0;" valign="top">  <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table2_row-r5-column-c2_dynamic_grid_items_grid-cell2_position-par_image" src="../../assets/scale-3-axes.gif" width="200px"/></div>  </td> </tr> </table> |
| **Escala restrita** | Clique com a tecla SHIFT pressionada | Com o manipulador de Escala, clicar em uma alça de eixo enquanto mantém o atalho redimensionará a projeção em etapas. O tamanho da etapa é o mesmo usado para o manipulador de tradução. <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table2_row-r6-column-c2_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/scale-1-axis-constrained.gif" width="200px"/></div> |
| **Superfície** | Clique do mouse | Com o manipulador de Superfície, clicar e arrastar sobre o modelo 3D o ajustará à superfície. <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table2_row-r7-column-c2_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/surface.gif" width="200px"/></div> **Observação:** este manipulador só está disponível com os tipos de projeção **Planar** e **Distorcer**. |
