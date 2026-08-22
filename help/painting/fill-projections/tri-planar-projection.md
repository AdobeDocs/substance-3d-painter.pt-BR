---
helpx_url: "https://helpx.adobe.com/br/substance-3d-painter/painting/fill-projections/tri-planar-projection.html"
breadcrumb-title: ''
description: Use a projeção triplanar no Substance 3D Painter para projetar texturas de três planos ortogonais para uma cobertura contínua.
helpx_creative_field: ""
helpx_description: Painter > Painting > Fill projections > Tri-planar projection
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Projeção triplanar
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '1091'
ht-degree: 3%

---


# Projeção triplanar

![](../../assets/triplanar.jpg)

A projeção triplanar do preenchimento é uma projeção 3D que combina várias projeções planares juntas e as mescla para cobrir toda a malha 3D. É muito útil projetar ruídos e padrões sem criar emendas visíveis.

## Propriedades

| *Configuração* | *Descrição* |
| --- | --- |
| **Filtragem** | Controla como a textura ou o material será filtrado. Essa configuração pode afetar a aparência da textura quando repetida várias vezes. Com valores de dimensionamento altos, o uso de um filtro diferente do padrão pode produzir resultados com melhor aparência. Configurações atuais disponíveis:<ul data-preserve-html="true"> <li data-preserve-html="true"><b>Bilinear - HQ</b> (padrão): uma filtragem bilinear avançada que tenta melhorar a qualidade da textura quando os valores de divisão em blocos gráficos estão altos.</li> <li data-preserve-html="true"><b>Bilinear - Nítido</b>: filtragem bilinear simples que suaviza ligeiramente a textura, mas tenta preservar os detalhes.</li> <li data-preserve-html="true"><b>Mais próximo</b>: sem filtragem, útil se a filtragem Bilinear fornecer um resultado desfocado e quebrar detalhes finos. É possível introduzir suavização na textura.</li> </ul> |
| **Corte da forma** | Defina se a textura projetada deve ser visível fora da área de projeção. Os valores possíveis são:<ul data-preserve-html="true"><li data-preserve-html="true"><strong>Projeto cortado na forma</strong>: a projeção está confinada dentro da área de projeção.</li><li data-preserve-html="true"><strong>A projeção se estende para fora da forma</strong> (padrão): a projeção continua além da área de projeção.</li></ul>   <table> <tr style="border: 0;"> <td style="border: 0;" valign="top">  <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r2-column-c1_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/cropped.jpg" width="200px"/></div>  </td> <td style="border: 0;" valign="top">  <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r2-column-c1_dynamic_grid_items_grid-cell1_position-par_image" src="../../assets/extend-1.jpg" width="200px"/></div>  </td> </tr> </table> |
| **Dureza** | Controle a intensidade e a suavidade das transições entre planos da projeção. Um valor ou 1,0 significa que haverá um corte claro entre cada plano. <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r3-column-c1_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/hardness-fill.gif"/></div> **Observação:** a transição de cada plano é definida pelo vértice de malha normal (sem levar em conta o mapa de malha normal). Isso significa que normais de vértice abruptos ou quebrados podem levar a resultados inesperados ao mesclar planos juntos. |

### Transformação UV

As configurações de transformação UV controlam a textura/material dentro da projeção.

<table data-preserve-html="true" style="width: 100.0%;"><colgroup> <col style="width: 40.0%;"/> <col style="width: 20.0%;"/> <col style="width: 40.0%;"/> </colgroup><tbody><tr><th>Modo de dimensionamento</th><th>Configuração</th><th>Descrição</th></tr><tr><td><p><strong>Divisão em blocos gráficos</strong> (padrão)<strong> <br/></strong></p><p>Permite definir manualmente o valor de repetição para a textura atual.</p></td><td><strong>Revestimento</strong></td><td>Controla o número de vezes que a textura é repetida.</td></tr><tr><td rowspan="2"><br/><br/></td><td colspan="1"><strong>Giro</strong></td><td colspan="1">Controla o ângulo em que a textura é projetada na malha.</td></tr><tr><td colspan="1"><strong>Deslocamento</strong></td><td colspan="1">Controla a partir de onde a textura será projetada. O valor padrão significa que o centro da textura está no centro dos UVs da malha.</td></tr><tr><th colspan="1"><br/></th><th colspan="1"><br/></th><th colspan="1"><br/></th></tr><tr><td rowspan="4"><p><strong>Tamanho físico</strong></p><p>Ajuste automático de uma textura de acordo com o tamanho da malha e o tamanho físico incorporado. Ele usa a largura e o comprimento (medidas X e Y) para calcular o tamanho físico correto. A medição Z não é levada em conta.</p><p>(Para obter mais informações, consulte a [página de documentação](https://experienceleague.adobe.com/pt-br/docs/substance-3d-painter/using/features/physical-size) dedicada</p></td><td><strong>Tamanho personalizado</strong></td><td><p>Se ativada, permite inserir um tamanho físico manualmente e substituir o fornecido por um ativo.</p><p>Ela é selecionada automaticamente se nenhum tamanho físico for detectado ou se vários ativos com tamanhos físicos diferentes forem usados na mesma camada/efeito.</p></td></tr><tr><td colspan="1"><strong>Tamanho (cm)</strong></td><td colspan="1">Os tamanhos físicos incorporados são expressos em centímetros. É possível trabalhar com um arquivo de malha que foi criado usando diferentes unidades de medida - ele reterá as proporções corretas. No entanto, o tamanho do ativo é exibido atualmente apenas em centímetros.</td></tr><tr><td colspan="1"><strong>Giro</strong></td><td colspan="1">Controla o ângulo em que a textura é projetada na malha.</td></tr><tr><td colspan="1"><strong>Deslocamento</strong></td><td colspan="1"><p>Controla a partir de onde a textura será projetada. O valor padrão significa que o centro da textura está no centro dos UVs da malha.</p></td></tr></tbody></table>

>[!NOTE]
>
> A configuração **Deslocamento** não está disponível com a projeção Triplanar.

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
| **Escala** | Clique do mouse | Com o manipulador de Escala, clique em uma alça de eixo para redimensionar a projeção ao longo do eixo fornecido.   <table> <tr style="border: 0;"> <td style="border: 0;" valign="top">  <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table2_row-r5-column-c2_dynamic_grid_items_image_1881993640" src="../../assets/scale-one-axis.gif" width="200px"/></div>  </td> <td style="border: 0;" valign="top">  <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table2_row-r5-column-c2_dynamic_grid_items_image_518594828" src="../../assets/scale-two-axis.gif" width="200px"/></div>  </td> <td style="border: 0;" valign="top">  <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table2_row-r5-column-c2_dynamic_grid_items_image" src="../../assets/scale-3-axes.gif" width="200px"/></div>  </td> </tr> </table> |
| **Escala restrita** | Clique com a tecla SHIFT pressionada | Com o manipulador de Escala, clicar em uma alça de eixo enquanto mantém o atalho redimensionará a projeção em etapas. O tamanho da etapa é o mesmo usado para o manipulador de tradução. <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table2_row-r6-column-c2_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/scale-1-axis-constrained.gif" width="200px"/></div> |
| **Superfície** | Clique do mouse | Com o manipulador de Superfície, clicar e arrastar sobre o modelo 3D o ajustará à superfície. <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table2_row-r7-column-c2_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/surface.gif" width="200px"/></div> **Observação:** este manipulador só está disponível com os tipos de projeção **Planar** e **Distorcer**. |
