---
helpx_url: "https://helpx.adobe.com/br/substance-3d-painter/features/effects/compare-mask.html"
breadcrumb-title: ''
description: Saiba como usar o efeito Comparar máscara no Substance 3D Painter para criar máscaras com base em operações de comparação de textura.
helpx_creative_field: ""
helpx_description: Painter > Features > Effects > Compare Mask
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Comparar máscara
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '376'
ht-degree: 1%

---


# Comparar máscara

![](../../assets/compare-mask.png)

Esse efeito permite comparar dois canais de maneira rápida e fácil e, como resultado, produzir uma máscara. Esse efeito só está disponível para a Máscara em camadas.

Abaixo estão as configurações disponíveis para este efeito:

| Configuração | Descrição |
| --- | --- |
| **Canal** | O canal a ser comparado entre a origem e o destino a partir do qual uma máscara será criada. Esta lista é baseada no canal disponível nas [configurações do Conjunto de Texturas](../../interface/texture-set/texture-set-settings.md). |
| **Comparar** | Três parâmetros estão disponíveis aqui para escolher como a máscara deve ser calculada. A lista suspensa no meio define a operação de comparação (menor que, dentro da tolerância, maior que). <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r2-column-c1_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/compare-mode.png"/></div> Os modos de Origem e Destino são:<ul data-preserve-html="true"><li data-preserve-html="true"><strong>Camadas Abaixo</strong>: leve em consideração a versão achatada de todas as camadas abaixo da atual.</li><li data-preserve-html="true"><strong>Esta Camada</strong>: leve em consideração apenas esta camada.</li><li data-preserve-html="true"><strong>Esta máscara</strong>: leve em consideração o conteúdo existente da Máscara (por exemplo, se um efeito de Preenchimento ou um efeito Gerador já estiver presente).</li><li data-preserve-html="true"><strong>Constante</strong>: valor uniforme.</li></ul>As operações são:<ul data-preserve-html="true"><li data-preserve-html="true"><strong>Menor que</strong>: se o menu suspenso Origem (à esquerda) tiver valores inferiores ao Destino (menu suspenso à direita), ele exibirá valores brancos na máscara.</li><li data-preserve-html="true"><strong>Dentro da tolerância</strong>: se o menu suspenso Origem (à esquerda) tiver valores semelhantes aos do menu suspenso Destino (à direita), ele exibirá valores brancos na máscara.</li><li data-preserve-html="true"><strong>Maior que</strong>: se o menu suspenso Origem (à esquerda) tiver valores mais altos que o menu suspenso Destino (à direita), ele exibirá valores brancos na máscara.</li></ul> |
| **Constante** | Valor a ser comparado quando a configuração de comparação estiver definida como “constante”. |
| **Dureza** | Controla o smoothness/dureza da comparação de máscara resultante. |
| **Histograma de Canais de Origem** | Forneça uma exibição de histograma da origem e do destino. Útil para saber se eles se sobrepõem um pouco ou não se sobrepõem (se não se sobrepuserem, a máscara estará vazia).Para obter mais informações sobre como o histograma funciona, consulte: [Níveis](https://experienceleague.adobe.com/pt-br/docs/substance-3d-designer/using/substance-graphs/nodes-reference-for-substance-graphs/atomic-nodes/levels). |

>[!NOTE]
>
> É possível clicar com o botão direito do mouse em uma camada e escolher o atalho “**Adicionar máscara com combinação de height**” para adicionar rapidamente esse novo efeito em uma camada. Este atalho também mudará o canal de Height **modo de mesclagem** para “**Normal**” em vez do padrão “**Subexposição Linear (Adicionar)**”.\
> ![](../../assets/compare-shortcut.png)
