---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/interface/layer-stack.html"
breadcrumb-title: ''
description: Saiba como usar a pilha de camadas no Substance 3D Painter para organizar e gerenciar várias camadas de pintura de textura.
helpx_creative_field: ""
helpx_description: Painter > Interface > Layer stack
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Pilha de camadas
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '615'
ht-degree: 5%

---


# Pilha de camadas

![](../../assets/layer-stack.png)

A **Pilha de camadas** permite manipular as camadas de um Conjunto de Texturas. Uma camada contém a pintura e os efeitos que criarão a textura no objeto 3D na cena. Você pode ocultar e reexibir camadas, colocá-las em pastas e alterar a opacidade e o modo de mesclagem.

Consulte as páginas a seguir para obter informações adicionais:

* [Criação de camadas](creating-layers.md)
* [Gerenciamento de camadas](managing-layers.md)
* [Mascaramento e efeitos](masking-and-effects.md)
* [Modos de mesclagem](blending-modes.md)
* [Instância de camada](layer-instancing.md)
* [Máscara de geometria](geometry-mask.md)

## Visão geral

As camadas de exibição da pilha de camadas com uma hierarquia específica: a camada na parte inferior será desenhada primeiro na malha e a camada na parte superior seguirá. Portanto, a camada no topo da pilha é o último item, enquanto a camada na parte inferior é o primeiro. O mesmo princípio se aplica às pastas; no entanto, o conteúdo da pasta tem prioridade. Isso significa que o conteúdo de uma pasta será processado antes das camadas que estiverem no mesmo nível.

**Características comuns:**

* Cada camada tem **vários canais**.
* A ferramenta de pintura pintará **em todos os seus respectivos canais**, dependendo das configurações do material (qual canal você está visualizando atualmente na Pilha de Camadas não tem impacto).
* Cada camada tem um **modo de mesclagem** e uma **opacidade** por canal (você pode alternar entre canais por meio do menu suspenso superior esquerdo).

**Tipos de camadas:**

* **Camada de pintura** : este tipo de camada pode ser pintado com pincéis e partículas
* **Camada de preenchimento**: esta camada não pode ser pintada; em vez disso, você pode carregar um material nela para preencher os canais. (Você também pode manipular a transformação para repetir o material, por exemplo.)
* **Pasta** : este tipo de camada tem como única finalidade conter outras camadas, sendo usado principalmente para organizar a pilha de camadas

Em cada camada, você pode **adicionar uma máscara** que permita aplicar o conteúdo apenas a partes específicas dos canais do conjunto de textura atual.\
É possível pintar a máscara manualmente (em tons de cinza com um pincel) ou usar filtros e substâncias para obter resultados mais dinâmicos/de procedimentos.

## Modo de visualização

![](../../assets/switch-viewmode-optim.gif)

O menu suspenso superior esquerdo da Pilha de camadas controla o modo de exibição da pilha de camadas. Como uma camada pode cobrir vários canais, não é possível exibir todas essas propriedades de uma vez. Portanto, o modo de exibição pode ser usado para definir o contexto de exibição atual. Ao usar esse menu suspenso, é possível especificar quais canais devem ser usados para exibir as miniaturas de camada, bem como controlar o modo de mesclagem e a opacidade somente desse canal.

A lista neste menu suspenso é baseada na lista de canais disponíveis nas [configurações do Conjunto de Texturas](../texture-set/texture-set-settings.md).

## Ações

![](../../assets/image2020-9-30-12-2-13.png)

A lista de ícones no canto superior direito é uma das ações comuns que podem ser executadas na Pilha de camadas:

| Ação | Descrição |
| --- | --- |
| Adicionar efeito <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r1-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/icon-effect.png"/></div> | Crie um novo efeito e adicione-o à camada atualmente selecionada. Para obter mais informações sobre efeitos, consulte as[páginas dedicadas](../../features/effects/effects.md). |
| Criar máscara <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r2-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/icon-mask.png"/></div> | Abra o menu de ação Máscara que contém os seguintes itens:<ul data-preserve-html="true"><li data-preserve-html="true">Adicionar máscara branca</li><li data-preserve-html="true">Adicionar máscara preta</li><li data-preserve-html="true">Adicionar máscara de bitmap</li><li data-preserve-html="true">Adicionar máscara com seleção de cor</li><li data-preserve-html="true">Adicionar máscara com combinação de altura</li></ul> |
| Criar nova camada de pintura <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r3-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/image2020-9-30-11-52-41.png"/></div> | Crie uma nova camada de pintura acima da camada atualmente selecionada. |
| Criar nova camada de preenchimento <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r4-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/image2020-9-30-12-0-49.png"/></div> | Crie uma nova [camada de preenchimento](../../painting/fill-projections/fill-projections.md) acima da selecionada atualmente. |
| Adicionar novos materiais inteligentes <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r5-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/icon-smartmat.png"/></div> | Insira um novo Material inteligente acima da camada atualmente selecionada.Clicar neste botão abrirá uma miniprateleira para procurar a lista de Materiais Inteligentes disponíveis nos [Ativos](../../interface/assets/assets.md) atuais. |
| Adicionar Nova Pasta <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r6-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/image2020-9-30-12-1-13.png"/></div> | Cria uma nova pasta vazia acima da camada atualmente selecionada. |
| Excluir camada <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r7-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/icon-trash.png"/></div> | Exclui o item atualmente selecionado (camada, pasta ou efeito). |
