---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/painting/fill-projections/uv-projection.html"
breadcrumb-title: ''
description: Use o recurso Projeção UV no Substance 3D Painter para projetar texturas com base em coordenadas UV para um posicionamento preciso da textura.
helpx_creative_field: ""
helpx_description: Painter > Painting > Fill projections > UV projection
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Projeção UV
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '788'
ht-degree: 4%

---


# Projeção UV

![](../../assets/uv-proj.png)

A Projeção UV do preenchimento é uma Projeção 2D que funciona apenas no espaço de textura 2D. Ela oferece controles para mover, girar e dimensionar uma imagem.

## Propriedades

| *Configuração* | *Descrição* |
| --- | --- |
| **Filtragem** | Controla como a textura ou o material será filtrado. Essas configurações podem afetar a aparência da textura quando repetidas várias vezes. Com valores de escala altos, o uso de um método de filtragem diferente do padrão pode produzir resultados com melhor aparência. Configurações disponíveis no momento:<ul data-preserve-html="true"><li data-preserve-html="true"><strong>Bilinear | HQ </strong>: (padrão) Filtragem bilinear avançada que tenta melhorar a qualidade da textura quando os valores de divisão em blocos gráficos são altos.</li><li data-preserve-html="true"><strong>Bilinear | Sharp </strong>: Filtragem bilinear simples que suaviza ligeiramente a textura, mas tenta preservar os detalhes.</li><li data-preserve-html="true"><strong>Mais próximo </strong>: sem filtragem, útil se a filtragem Bilinear fornecer um resultado desfocado e quebrar detalhes finos. É possível introduzir suavização na textura.</li></ul> |
| **Envoltório UV** | Controla como o Material/Imagem projetado deve se repetir dentro da forma de projeção. Os valores possíveis são:<ul data-preserve-html="true"><li data-preserve-html="true"><strong>Nenhum</strong> : não há repetição da projeção.</li><li data-preserve-html="true"><strong>Repetir horizontalmente</strong> : repetir apenas horizontalmente.</li><li data-preserve-html="true"><strong>Repetir verticalmente</strong> : repetir apenas verticalmente.</li><li data-preserve-html="true"><strong>Repetir</strong> (padrão): repita horizontal e verticalmente.</li></ul> <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r2-column-c1_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/2d-repeat.jpg" width="500px"/></div> |

### Transformação UV

As configurações de transformação UV controlam a textura/material dentro da projeção.

<table data-preserve-html="true" style="width: 100.0%;"><colgroup> <col style="width: 40.0%;"/> <col style="width: 20.0%;"/> <col style="width: 40.0%;"/> </colgroup><tbody><tr><th>Modo de dimensionamento</th><th>Configuração</th><th>Descrição</th></tr><tr><td><p><strong>Divisão em blocos gráficos</strong> (padrão)<strong> <br/></strong></p><p>Permite definir manualmente o valor de repetição para a textura atual.</p></td><td><strong>Revestimento</strong></td><td>Controla o número de vezes que a textura é repetida.</td></tr><tr><td rowspan="2"><br/><br/></td><td colspan="1"><strong>Giro</strong></td><td colspan="1">Controla o ângulo em que a textura é projetada na malha.</td></tr><tr><td colspan="1"><strong>Deslocamento</strong></td><td colspan="1">Controla a partir de onde a textura será projetada. O valor padrão significa que o centro da textura está no centro dos UVs da malha.</td></tr><tr><th colspan="1"><br/></th><th colspan="1"><br/></th><th colspan="1"><br/></th></tr><tr><td rowspan="4"><p><strong>Tamanho físico</strong></p><p>Ajuste automático de uma textura de acordo com o tamanho da malha e o tamanho físico incorporado. Ele usa a largura e o comprimento (medidas X e Y) para calcular o tamanho físico correto. A medição Z não é levada em conta.</p><p>(Para obter mais informações, consulte a [página de documentação](https://experienceleague.adobe.com/en/docs/substance-3d-painter/using/features/physical-size) dedicada</p></td><td><strong>Tamanho personalizado</strong></td><td><p>Se ativada, permite inserir um tamanho físico manualmente e substituir o fornecido por um ativo.</p><p>Ela é selecionada automaticamente se nenhum tamanho físico for detectado ou se vários ativos com tamanhos físicos diferentes forem usados na mesma camada/efeito.</p></td></tr><tr><td colspan="1"><strong>Tamanho (cm)</strong></td><td colspan="1">Os tamanhos físicos incorporados são expressos em centímetros. É possível trabalhar com um arquivo de malha que foi criado usando diferentes unidades de medida - ele reterá as proporções corretas. No entanto, o tamanho do ativo é exibido atualmente apenas em centímetros.</td></tr><tr><td colspan="1"><strong>Giro</strong></td><td colspan="1">Controla o ângulo em que a textura é projetada na malha.</td></tr><tr><td colspan="1"><strong>Deslocamento</strong></td><td colspan="1"><p>Controla a partir de onde a textura será projetada. O valor padrão significa que o centro da textura está no centro dos UVs da malha.</p></td></tr></tbody></table>

## Barra de ferramentas Contextual

Várias configurações e ferramentas estão disponíveis na [barra de ferramentas contextual](../../interface/toolbars.md) localizada na parte superior da viewport, que dão controle sobre o manipulador e a projeção:

| Ícone | Nome | Descrição |
| --- | --- | --- |
| <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table1_row-r1-column-c0_image" src="../../assets/icon-manipulator-2d-hide.png" width="50px"/></div> | Mostrar/Ocultar manipulador | Se ativado, o manipulador fica visível e é controlável na viewport. |
| <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table1_row-r2-column-c0_image" src="../../assets/icon-manipulator-settings-2d.png" width="50px"/></div> | Tamanho das alças do manipulador | Esse menu contém três configurações que definem o tamanho das alças da transformação na viewport:<ul data-preserve-html="true"><li data-preserve-html="true"><strong>Pequeno</strong></li><li data-preserve-html="true"><strong>Médio</strong></li><li data-preserve-html="true"><strong>Grande</strong></li></ul> |
| <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table1_row-r3-column-c0_image" src="../../assets/icon-flip-x.png" width="50px"/></div> | Espelho em X | Vire a transformação no eixo X. |
| <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table1_row-r4-column-c0_image" src="../../assets/icon-flip-y.png" width="50px"/></div> | Espelho em Y | Vire a transformação no eixo Y. |
| <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table1_row-r5-column-c0_image" src="../../assets/icon-pivot.png" width="50px"/></div> | Redefina o ponto de articulação | Restaure o ponto de giro de volta ao meio da transformação. |
| <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table1_row-r6-column-c0_image" src="../../assets/icon-reset.png" width="50px"/></div> | Redefinir transformação | Restaure a transformação de projeção de volta ao seu estado padrão. |

## Manipulador

A Projeção UV usa um manipulador que só está disponível na [exibição 2D](../../interface/viewport/2d-view.md).

| Ação | Atalho | Descrição |
| --- | --- | --- |
| **Traduzir** | Clique do mouse | Clique e arraste qualquer área dentro da transformação para movê-la. <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table2_row-r1-column-c2_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/uv-translate.gif"/></div> |
| **Traduzir restrito** | Clique com a tecla SHIFT pressionada | Clique e arraste qualquer área dentro da transformação enquanto pressiona e mantém o atalho para movê-lo apenas ao longo de um eixo. O eixo pode ser horizontal ou vertical e, alinhado com a câmera, baseia-se na direção do mouse. <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table2_row-r2-column-c2_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/uv-translate-constrained.gif"/></div> |
| **Rotação** | Clique do mouse | Clicar e arrastar de fora da transformação permite girá-la. Mover a tabela dinâmica também permite alterar o ponto de origem da rotação.   <table> <tr style="border: 0;"> <td style="border: 0;" valign="top">  <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table2_row-r3-column-c2_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/uv-rotation.gif"/></div>  </td> <td style="border: 0;" valign="top">  <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table2_row-r3-column-c2_dynamic_grid_items_grid-cell1_position-par_image" src="../../assets/uv-rotation-pivot.gif"/></div>  </td> </tr> </table> |
| **Rotação restrita** | Clique com a tecla SHIFT pressionada | Clicar e arrastar de fora da transformação enquanto pressiona e mantém o atalho permite girá-lo apenas a cada 45 graus. <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table2_row-r4-column-c2_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/uv-rotation-constrained.gif"/></div> |
| **Escala** | Clique do mouse | Clicar e arrastar qualquer alça do manipulador permite deformar a transformação.   <table> <tr style="border: 0;"> <td style="border: 0;" valign="top">  <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table2_row-r5-column-c2_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/uv-scale-free.gif"/></div>  </td> <td style="border: 0;" valign="top">  <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table2_row-r5-column-c2_dynamic_grid_items_grid-cell1_position-par_image" src="../../assets/uv-scale-middle.gif"/></div>  </td> </tr> </table> |
| **Escala restrita** | Clique com a tecla SHIFT pressionada | Ao pressionar e manter o atalho ao arrastar uma alça, a transformação é forçada a manter sua proporção.   <table> <tr style="border: 0;"> <td style="border: 0;" valign="top">  <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table2_row-r6-column-c2_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/uv-scale-ratio.gif"/></div>  </td> <td style="border: 0;" valign="top">  <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table2_row-r6-column-c2_dynamic_grid_items_grid-cell1_position-par_image" src="../../assets/uv-scale-middle-ratio.gif"/></div>  </td> </tr> </table> |
| **Escala espelhada** | CTRL+clique do mouse | Ao mover uma alça enquanto pressiona o atalho, as outras alças executarão um movimento semelhante. Permite deformar a transformação em simetria ao redor do ponto pivô.   <table> <tr style="border: 0;"> <td style="border: 0;" valign="top">  <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table2_row-r7-column-c2_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/uv-scale-mirror.gif"/></div>  </td> <td style="border: 0;" valign="top">  <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table2_row-r7-column-c2_dynamic_grid_items_grid-cell1_position-par_image" src="../../assets/uv-scale-mirror-pivot.gif"/></div>  </td> </tr> </table> |
| **Escala espelhada e restrita** | SHIFT+CTRL+Clique do mouse | A combinação de ambos os atalhos permite deformar a transformação em simetria, preservando a proporção. <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table2_row-r8-column-c2_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/uv-scale-mirror-ratio.gif"/></div> |
