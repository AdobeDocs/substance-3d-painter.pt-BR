---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/painting/dynamic-strokes/enabling-dynamic-stroke-feature.html"
breadcrumb-title: ''
description: Saiba como ativar o recurso de traçado dinâmico no Substance 3D Painter para criar traçados de pincel responsivos com efeitos variáveis.
helpx_creative_field: ""
helpx_description: Painter > Painting > Dynamic strokes > Enabling Dynamic Stroke Feature
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Ativação do recurso Traçado dinâmico
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '448'
ht-degree: 2%

---


# Ativação do recurso Traçado dinâmico

Para ativar o recurso Traçados dinâmicos, um recurso específico é necessário primeiro.

## Encontrando recursos compatíveis com Traçados dinâmicos

Ao navegar na janela [Ativos](../../interface/assets/assets.md), um ícone dedicado na parte inferior direita de uma miniatura indica o tipo de compatibilidade do recurso. Se não houver um ícone visível, significa que o recurso não pode aproveitar o recurso.

| *Ícone* | *Descrição* |
| --- | --- |
| <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r1-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/icon-dyn.png"/></div> | Este recurso pode usar um ou mais dos seguintes comportamentos:<ul data-preserve-html="true"><li data-preserve-html="true">Índice de carimbo</li><li data-preserve-html="true">Hora</li><li data-preserve-html="true">Distribuição aleatória</li></ul> |
| <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r2-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/icon-random.png"/></div> | Este recurso só expõe o parâmetro de Distribuição Aleatória. |

Também é possível pesquisar recursos usando o campo de pesquisa na Prateleira com as seguintes palavras-chave:

* dynamicstroke
* semente aleatória

## parâmetros de traçados dinâmicos

![](../../assets/dynamic-strokes-settings.png)

Quando um recurso Traçado dinâmico é carregado, uma nova lista de parâmetros é adicionada logo antes do grupo de parâmetros Substance.

| *Parâmetro* | *Descrição* |
| --- | --- |
| **Controles Dinâmicos** | Lista os parâmetros que estão disponíveis com o arquivo de Substance atualmente usado. |
| **Início do carimbo** | Disponível apenas se o recurso tiver o controle dinâmico “Índice de carimbo”. Indica a partir de qual valor o índice dos carimbos dentro do traçado do pincel deve começar:<ul data-preserve-html="true"><li data-preserve-html="true"><strong>Do início (0)</strong>: padrão. O índice começa a partir de zero a cada novo traçado.</li> <li data-preserve-html="true"><strong>Do Índice Aleatório</strong>: o índice começa com base em um valor aleatório (com seu máximo definido pela Contagem de Ciclos de Carimbo). Observe que os seguintes valores ainda estarão na sequência e não serão totalmente aleatórios.</li> </ul> |
| **Contagem de Ciclos de Carimbo** | Disponível apenas se o recurso tiver o controle dinâmico “Índice de carimbo”. Estes parâmetros controlam quando o Substance 3D Painter deve parar de gerar novas variações de Substance e começar a reciclar as existentes. Este parâmetro tem um grande impacto nas performances, que você pode ler mais sobre [Desempenho de traçados dinâmicos](dynamic-stroke-performances.md). |
| **Tipo de Distribuição Aleatória** | Disponível apenas se o recurso tiver o controle dinâmico “Distribuição aleatória”. Controla como a Distribuição aleatória deve ser alterada:<ul data-preserve-html="true"><li data-preserve-html="true"><strong>Único</strong>: padrão. Use um único valor de Distribuição aleatória que pode ser definido manualmente por meio dos parâmetros Substance.</li> <li data-preserve-html="true"><strong>Aleatório por traço</strong>: gera um novo valor de Distribuição aleatória para cada novo traçado de pincel.</li> <li data-preserve-html="true"><strong>Aleatório por carimbo</strong>: gera um novo valor de Distribuição aleatória para cada carimbo dentro de um traçado de pincel. <em><strong>Tenha cuidado com o parâmetro, pois ele pode ser muito caro</strong>.</em></li> </ul> |
| **Hora** | O controle dinâmico de tempo não tem nenhum parâmetro. O tempo é determinado pelo tempo que dura a pintura de um traçado de pincel. |

## Lista de ferramentas compatíveis

As configurações de Traçado dinâmico estão disponíveis apenas com as seguintes ferramentas e contextos:

| *Tipo de ferramenta* | *Slot de Recurso Compatível* |
| --- | --- |
| **Pintar** | <ul data-preserve-html="true"><li data-preserve-html="true">Alfa</li><li data-preserve-html="true">Material</li></ul> |
| **Borracha** | <ul data-preserve-html="true"><li data-preserve-html="true">Alfa</li><li data-preserve-html="true">Material</li></ul> |
| **Projeção** | <ul data-preserve-html="true"><li data-preserve-html="true">Alfa</li></ul> |
| **Borrar** | <ul data-preserve-html="true"><li data-preserve-html="true">Alfa</li></ul> |
| **Clonar** | <ul data-preserve-html="true"><li data-preserve-html="true">Alfa</li></ul> |

>[!NOTE]
>
> Traçados dinâmicos não são compatíveis com **Partículas**, e é por isso que o recurso é desabilitado ao usar qualquer ferramenta no modo Física.
