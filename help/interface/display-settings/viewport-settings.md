---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/interface/display-settings/viewport-settings.html"
breadcrumb-title: ''
description: Saiba como definir as configurações de visor no Substance 3D Painter para personalizar as opções de exibição e a qualidade de renderização.
helpx_creative_field: ""
helpx_description: Painter > Interface > Display settings > Viewport settings
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Configurações da janela de visualização
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '734'
ht-degree: 2%

---


# Configurações da janela de visualização

Esta seção das **Configurações de Exibição** controla várias configurações relacionadas à exibição do visor, como a filtragem de textura e o wireframe de malha.

## Filtragem de textura

![](../../assets/texture-filtering.png)

A Filtragem Anisotrópica e o MipMap Bias permitem controlar a exibição de texturas na viewport. Essas configurações não afetam diretamente as texturas e não serão aplicadas na exportação, apenas refinam o processo de renderização no visor. A configuração de polarização do MipMap permite forçar o uso de texturas muito nítidas para pixels que estão longe ou em ângulos oblíquos. No entanto, em alguns casos, elas podem criar padrões Moiré ou tremulação.

As configurações padrão são um comprometimento da qualidade e dos desempenhos e só devem ser alteradas quando realmente necessário.

| *Configuração* | *Descrição* |
| --- | --- |
| **Filtragem Anisotrópica** | A filtragem anisotrópica melhora a qualidade da textura ao visualizar em ângulos oblíquos. Valores de alta qualidade fornecem uma filtragem melhor, mas podem resultar em perda de desempenho. Essa configuração controla a quantidade de amostras por pixel (spp) usada para a filtragem:<ul data-preserve-html="true"><li data-preserve-html="true"><strong>Desabilitado</strong> : Sem filtragem</li><li data-preserve-html="true"><strong>Baixo</strong> (2spp)</li><li data-preserve-html="true"><strong>Médio</strong> (4spp): valor padrão</li><li data-preserve-html="true"><strong>Alta</strong> (8spp)</li><li data-preserve-html="true"><strong>Muito Alta</strong> (16spp)</li></ul> <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r1-column-c1_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/quality-anisotropic-filtering.jpg"/></div> |
| **Polarização de MipMap** | Desloque o Nível do mipmap de detalhes para melhorar a qualidade da textura. Valores nítidos podem resultar em perda de desempenho e texturas irregulares.<ul data-preserve-html="true"><li data-preserve-html="true"><strong>0 - Flexível</strong> (Desempenho Leve): valor padrão</li><li data-preserve-html="true"><strong>1 - Médio suave</strong></li><li data-preserve-html="true"><strong>2 - Nítido</strong></li><li data-preserve-html="true"><strong>3 - Muito Nítido</strong> (Desempenho Intensivo)</li></ul>(De 0 a -3) |

## Moldura da câmera

![](../../assets/camera-frame.png)

Para obter mais informações sobre o Gerenciamento de Câmera, consulte: [Gerenciamento de câmera](../viewport/camera-management.md)

## Exibição de ferramentas

![](../../assets/viewport-tool.png)

| *Configuração* | *Descrição* |
| --- | --- |
| **Ocultar estêncil ao pintar** | Ao usar um estêncil (consulte as propriedades da ferramenta de pintura), esta configuração permite ocultá-lo temporariamente ao pintar na malha. |
| **Opacidade de exibição de estêncil** | Controla a visibilidade do estêncil sobre a renderização do visor quando não estiver pintando. |
| **Canal de visualização de projeção** | Controla qual canal do material deve ser exibido ao usar a ferramenta de projeção. |

## Wireframe das malha

![](../../assets/viewport-mesh.png)

| *Configuração* | *Descrição* |
| --- | --- |
| **Mostrar wireframe de malha** | Habilitar ou desabilitar a exibição do wireframe de malha no visor. |
| **Cor do Wireframe** | Controla a cor usada para desenhar o wireframe de malha. |
| **Opacidade do Wireframe** | Controla o quanto o wireframe ficará visível quando desenhado sobre a malha. |

## Exibição do canal

![](../../assets/viewport-channel.png)

>[!NOTE]
>
> As configurações de exibição do canal só estão disponíveis ao usar o modo de exibição **canal único**.

| *Configuração* | *Descrição* |
| --- | --- |
| **Exibir exibição solo sem iluminação (sem iluminação)** | Ao visualizar no modo de canal único, ativar essa configuração removerá a iluminação e exibirá o canal como cores simples. Se desativada, um sombreamento será aplicado à borda da malha. |
| **Dimensionar valores HDR** | Ao visualizar no modo de canal único uma textura **HDR** (como o height), essa configuração dimensionará os valores totais. Isso é útil para visualizar valores que vão acima de 1 ou abaixo de -1. O resultado é igual a **Canal dividido por escala**.Com o exemplo abaixo, o canal de height tem valores até 3. No entanto, por padrão, eles não podem ser visualizados a menos que o valor da escala seja alterado: <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table1_row-r2-column-c1_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/scale-hdr.jpg"/></div> |
| **Usar cor +/- para valores HDR** | Essa configuração permite exibir mais facilmente a textura HDR substituindo valores positivos pela primeira cor e valores negativos pela segunda cor. Os valores neutros (0) são pretos.Exemplo: <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table1_row-r3-column-c1_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/colored-hdr.jpg"/></div> |
| **Canais de cores** | Modifique o modo de visualização do visor para exibir apenas individualmente o componente R, G, B ou Alpha do canal atual. Esta configuração não está disponível no modo de exibição de material. Quando ativado, o nome do canal de cor selecionado é exibido na viewport:  <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table1_row-r4-column-c1_image" src="../../assets/color-channel.png"/></div>  Valores possíveis:<ul data-preserve-html="true"><li data-preserve-html="true"><strong>RGBA</strong> (padrão): em canais de cores, exibe todos os componentes com transparência.</li><li data-preserve-html="true"><strong>Tons de cinza+Alpha</strong> (padrão): no canal de Tons de Cinza, exiba os valores de tons de cinza com a transparência.</li><li data-preserve-html="true"><strong>R</strong>: em canais de cores, exibe somente o componente vermelho.</li><li data-preserve-html="true"><strong>G</strong>: em canais de cores, exibe somente o componente Verde.</li><li data-preserve-html="true"><strong>B</strong>: em canais de cores, exibe somente o componente Azul.</li><li data-preserve-html="true"><strong>Alpha</strong>: em qualquer canal, exibe apenas a transparência da textura.</li></ul> |

## Grade

![](../../assets/display-settings-grid.png)

As configurações de grade permitem exibir e controlar o desenho de uma grade 3D dentro da janela de visualização 3D.

As divisões da grade são automáticas com base no nível atual da câmera de zoom e ângulo. A unidade de grade atual é exibida na parte inferior esquerda da viewport.

| Configuração | Descrição |
| --- | --- |
| **Mostrar grade** | Se ativada, torne a grade visível na viewport 3D. |
| **Eixo** | Defina ao longo de qual eixo a grade fica visível na viewport. O valor padrão é Y, pois esse é o eixo superior do aplicativo. |
| **Cor da grade** | A cor da grade quando desenhada no visor. |
| **Opacidade da grade** | A opacidade da grade no visor. |
