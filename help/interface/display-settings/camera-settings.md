---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/interface/display-settings/camera-settings.html"
breadcrumb-title: ''
description: Saiba como definir as configurações da câmera no Substance 3D Painter para controlar o comportamento e a projeção da câmera no visor.
helpx_creative_field: ""
helpx_description: Painter > Interface > Display settings > Camera settings
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Configurações da câmera
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '348'
ht-degree: 3%

---


# Configurações da câmera

Esta seção das **Configurações de exibição** controla o comportamento da câmera, bem como a aparência final do visor.

## Câmera

| *Configuração* | *Descrição* |
| --- | --- |
| **Campo de Exibição** | Permite controlar o campo de visão da câmera (em graus) |
| **Distância do foco** | Define a distância na qual o ponto de foco está localizado.  Esse ponto é usado pelo efeito Profundidade de campo. <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r2-column-c1_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/focus-distance-optim.gif"/></div> **Observação:** a distância de foco pode ser definida automaticamente clicando em um ponto da malha com o atalho **CTRL + botão do meio do mouse** |
| **Abertura** | Define a largura da Profundidade de Campo. <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r3-column-c1_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/dof-aperture-optim.gif"/></div> **Observação:** se Iray estiver controlando este parâmetro, alterá-lo disparará novamente um cálculo. |

## Pós-efeitos

![](../../assets/post.png)

Consulte a [página Pós-efeito](../../features/post-processing/post-processing.md) para obter mais informações.

## Suavização temporal

![](../../assets/taa.png)

Quando habilitada, a **Suavização temporal** (**TAA**) removerá as bordas irregulares no visor.\
O **TAA** funciona acumulando informações em vários quadros de renderização. Isso significa que o efeito está desabilitado até que a câmera pare de se mover ou que outra operação seja executada.

| *Configuração* | *Descrição* |
| --- | --- |
| **Acúmulos** | Define quantos quadros serão acumulados para reduzir a suavização.<ul data-preserve-html="true"> <li data-preserve-html="true">16: Valor recomendado para a maioria dos casos</li> <li data-preserve-html="true">64: útil para limpar valores de alto contraste (como sombreador de teste de Alpha e pontilhamento combinados)</li> </ul>  **Observação:** esta configuração não tem nenhum impacto no desempenho; no entanto, um valor alto pode levar mais tempo para produzir bons resultados. |

![](../../assets/temporal-anti-aliasing.gif){width="500px"}

A Suavização de borda também pode ser usada para filtrar o sombreador **Alpha-Test** se a configuração “**Pontilhamento alfa**” estiver habilitada:

![](../../assets/dithering-aa.gif){width="500px"}

## Dispersão de subsuperfície

![](../../assets/subscat.png)

Consulte a página [Dispersão da Subsuperfície](../../features/subsurface-scattering/subsurface-scattering.md) para obter mais informações.

## Perfil de cores

![](../../assets/profile-13.png)

Consulte a [página Perfil de Cores](../../features/post-processing/color-profile.md) para obter mais informações.

## Mapeamento de tons

| Configuração | Descrição |
| --- | --- |
| **Função** | Especifique a função usada para ajustar valores de cor que excedem os recursos de exibição do monitor (remapeamento de valores HDR para um intervalo de LDR). Os valores possíveis são:<ul data-preserve-html="true"><li data-preserve-html="true"><strong>Linear</strong> (padrão): nenhuma transformação; valores acima de 1.0 são fixados.</li><li data-preserve-html="true"><strong>ACES</strong>: use a curva de mapeamento de tom do Filmic ACES.</li></ul> <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table2_row-r1-column-c1_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/linear-vs-aces.jpg" width="450px"/></div> **Observação:** alguns mecanismos de jogos e softwares de renderização usam o mapeador de tons ACES. Habilitar essa função ajudará a combinar cores entre aplicativos e evitará diferenças. |
