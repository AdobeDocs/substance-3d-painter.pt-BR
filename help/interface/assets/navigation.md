---
helpx_url: "https://helpx.adobe.com/br/substance-3d-painter/interface/assets/navigation.html"
breadcrumb-title: ''
description: Saiba como navegar no painel Ativos no Substance 3D Painter para navegar e acessar sua biblioteca de recursos com eficiência.
helpx_creative_field: ""
helpx_description: Painter > Interface > Assets > Navigation
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Navegação
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '830'
ht-degree: 1%

---


# Navegação

Há vários meios de navegação na janela Ativos: navegação estrutural, campo de pesquisa e ícone de tipos de ativo. Todos os tipos de navegação são codependentes, para que você possa combinar essas pesquisas a seu favor.\
Por exemplo, se você tiver Materiais selecionados nos ícones de tipo de ativo, mas tiver usado as trilhas para navegar até a pasta Máscaras inteligentes, o painel Ativos não exibirá nenhum resultado; você terá que voltar para Todas as bibliotecas se quiser exibir Materiais ou desmarcar Materiais se quiser navegar pelas Máscaras inteligentes.

## Trilhas de navegação

As trilhas permitem navegar rapidamente pela biblioteca. Clicar nas setas exibe como os ativos são armazenados no disco e permite que você selecione qualquer um dos locais exibidos. Se estiver acinzentado, significa que não há ativos do tipo selecionado nessa pasta, mas você ainda pode navegar até esse local.

![](../../assets/00-05-breadcrumbs.jpg)

## Campo Pesquisar

O campo de pesquisa pode ser usado para filtrar recursos que contenham a consulta digitada. Observe que ele não pesquisa apenas pelo título dos recursos, mas também seu local e qualquer tag contida no recurso.\
As pesquisas digitadas também podem ser mais avançadas do que apenas palavras-chave. Consulte [Consultas de pesquisa avançada](advanced-search-queries.md).

![](../../assets/00-05-searchfield.jpg)

## Tipos de ativo

>[!NOTE]
>
> Os ícones de tipo de ativo podem ser selecionados por meio da manutenção da **Ctrl** ao clicar.

A seleção padrão é Materiais, mas clicar em outros ícones de tipo de ativo exibe outros tipos de recursos.

![](../../assets/00-05-assettypeicons.jpg)

| Tipos de ativo | Descrição |
| --- | --- |
| Materiais <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r1-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/00-05-assettypes-1-1.png"/></div> | Conter .sbsar importado como *material base* e materiais criados a partir de uma camada de preenchimento (você pode saber mais sobre a criação de predefinições [aqui](https://helpx.adobe.com/br/substance-3d/unlisted/documentation/spdoc/creating-and-saving-a-preset-180191514.html)).Eles são materiais básicos que podem ser usados em camadas de preenchimento e serão aplicados a toda a superfície da sua malha ou conjunto de texturas. |
| Materiais inteligentes <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r2-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/00-05-assettypes-7.png"/></div> | Contêm materiais mais complexos que consistem em várias camadas salvas em uma pasta (materiais inteligentes também são predefinições que você pode criar).Como materiais de base, materiais inteligentes serão aplicados a toda a malha/conjunto de texturas, mas também levam em consideração as informações individuais da malha, como curvatura, Oclusão ou qualquer outro detalhe da superfície. Para obter esses detalhes de superfície e usar materiais inteligentes corretamente, primeiro sua malha precisa ser [assada](../../baking/baking.md). |
| Máscaras inteligentes <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r3-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/00-05-assettypes-2.png"/></div> | Contêm máscaras mais complexas que usam vários efeitos de camada e/ou geradores. Você mesmo pode [criar](https://helpx.adobe.com/br/substance-3d/unlisted/documentation/spdoc/managing-assets-217187091.html) predefinições de máscaras inteligentes.Semelhante aos materiais inteligentes, as máscaras inteligentes precisam de informações preparadas na malha para funcionar corretamente. |
| Filtros <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r4-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/00-05-assettypes-3.png"/></div> | Contém arquivos .sbsar importados como *filtro*.Os filtros são efeitos que pegam a textura já presente e a transformam de alguma forma. Alguns filtros funcionarão somente com informações em preto e branco, outros somente com entradas de material, o que significa que nem todos os filtros podem ser usados em máscaras. |
| Pincéis <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r5-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/00-05-assettypes-4.png"/></div> | Contém pincéis, partículas e ferramentas. Todas estas são predefinições que podem ser [criadas](https://helpx.adobe.com/br/substance-3d/unlisted/documentation/spdoc/managing-assets-217187091.html) no Painter.**Os pincéis** são predefinições básicas em preto e branco que usam um alfabeto. É possível usar pincéis para pintar em qualquer um ou todos os canais ou em uma máscara.**Partículas** têm as mesmas características dos Pincéis, mas também têm um conjunto adicional de parâmetros que simulam a interação física com a malha. Eles podem produzir os efeitos de vazamentos, gotejamentos, chuva ou qualquer outro que exija simulação física.As **Ferramentas** podem conter o comportamento Pincel e/ou Partícula, mas além disso essa predefinição também é salva com informações de canais de material. |
| Alfas <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r6-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/00-05-assettypes-5.png"/></div> | Contêm diversas alfas, além de vários Criadores de pincéis que permitem [criar](https://helpx.adobe.com/br/substance-3d/unlisted/documentation/spdoc/managing-assets-217187091.html) pincéis com efeitos mais elaborados (tipo Photoshop, traçados dinâmicos, cilindro de pintura).Alpha são imagens em tons de cinza nas quais as partes pretas aparecem transparentes quando usadas. |
| Texturas <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r7-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/00-05-assettypes-6.png"/></div> | Contêm grunges, procedimentos, mapas baked, normais de superfície dura e LUTs.**Grunges** são imagens em tons de cinza com ruídos e texturas interessantes. Eles podem ser usados para adicionar variação à superfície da malha, seja por meio de uma máscara ou conectando-os diretamente a um canal.**Procedimentos** também são texturas em tons de cinza que compreendem ruídos ou até mesmo padrões regulares. Entretanto, diferentemente de alguns grunges estáticos, os procedimentos são bitmaps dinâmicos que podem ser dimensionados sem repetição e têm variações infinitas (por meio de propagação aleatória).**Mapas baked** representam as informações de superfície e forma extraídas da sua malha. Para saber mais sobre panificação, veja aqui.**Normais de superfície dura** são detalhes que você pode carimbar diretamente na malha usando o canal Normal.**LUTs** (tabelas de consulta) são texturas de perfil de cores que podem ser usadas nas Configurações de Exibição para simular um comportamento de perfil de cores na janela de visualização. Você pode saber mais sobre perfis de cores [aqui](../../features/post-processing/color-profile.md). |
| Mapas do ambiente <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r8-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/00-05-assettypes-1.jpg"/></div> | Contêm imagens importadas como *ambiente* (mais comumente .hdr ou .exr). Mapas de ambiente são imagens de plano de fundo que geram automaticamente uma configuração de iluminação. Você pode usar um mapa de ambiente arrastando-o diretamente para a viewport ou percorrendo as Configurações de exibição. |
