---
helpx_url: "https://helpx.adobe.com/br/substance-3d-painter/painting/tool-list/path.html"
breadcrumb-title: ''
description: Use a ferramenta Caminho no Substance 3D Painter para criar e editar caminhos para uma pintura de textura precisa e o posicionamento do traçado.
helpx_creative_field: ""
helpx_description: Painting > Path tools list > Path tool
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Visão geral da ferramenta Caminho
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '1699'
ht-degree: 0%

---


# Visão geral da ferramenta Caminho

![Imagem mostrando a ferramenta de caminho usada em um sapato](../../assets/v90_banner_path.jpg)

<table>
<tr style="border: 0;">
<td style="border: 0;" valign="top">

<b>Áudio</b>

Ajuste ou adicione áudio ao seu projeto.


* Ajuste o volume do vídeo de origem se ele tiver áudio.
* Adicionar, remover ou substituir um arquivo de áudio externo.
* Ajuste o volume do arquivo de áudio externo.

</td>
<td style="border: 0;" valign="top">

![](../../assets/image_180.png)

</td>
</tr>
</table>

As <b>ferramentas de caminho</b> permitem definir uma curva com pontos na superfície da malha. Depois que a curva é criada, as diferentes ferramentas de Caminho permitem criar diferentes efeitos ao longo da curva.

## Criação de um caminho

Caminhos podem ser criados em camadas e efeitos de pintura. Há duas maneiras de acessar a ferramenta Caminho:

* <b>Pela interface</b>: navegue até a barra de ferramentas da ferramenta no lado esquerdo e clique no terceiro ícone na parte superior.
* <b>Por meio de um atalho de teclado</b>: por padrão, a ferramenta não tem nenhuma atribuída. Isso pode ser alterado no menu Configurações ao editar o atalho “Selecionar ferramenta Pintar ao longo do caminho”.

Depois que a ferramenta é selecionada, os pontos podem ser colocados clicando na superfície do modelo 3D na janela de visualização 3D. Pelo menos dois pontos (ou vértices) são necessários para criar um caminho.

![Gif mostrando a seleção da ferramenta de caminho e a criação de pontos](../../assets/path_create_points.gif)

A ferramenta Caminho tem modos diferentes, que podem ser semelhantes às outras ferramentas de pintura disponíveis no aplicativo:

* Pintar ao longo do caminho: desenhe um traçado de pincel regular ao longo de um caminho definido.
* [Caminho da faixa](ribbon-tool.md): desenha uma imagem repetida ou esticada ao longo de um caminho.
* [Caminho preenchido](filled-path.md): preencha o interior de um caminho com uma cor uniforme.
* Apagar ao longo do caminho: desenhe um traçado que apaga/remove informações ao longo de um caminho definido.
* Borrar ao longo do caminho: desenhe um traçado que borra/desfoca as informações ao longo de um caminho definido.

![Captura de tela da barra de ferramentas da ferramenta mostrando os diferentes modos de ferramentas de caminho](../../assets/PathTools.png)

Por exemplo, esta é a ferramenta de caminho no modo <b>Borrar</b> afetando outras informações da pintura:

![Gif mostrando uma ferramenta de caminho no modo de borrar](../../assets/v90_path_smudge.gif)

>[!NOTE]
>
> As <b>ferramentas de caminho</b> funcionam somente no espaço 3D na superfície da geometria. No momento, não é possível criar um caminho no espaço UV ou como uma projeção de espaço de tela.

### Edição de um demarcador

Os pontos de caminho (ou vértices) aderem automaticamente à superfície da malha. Eles podem ser movidos e ajustados a qualquer momento. É possível adicionar novos vértices a um caminho existente clicando em qualquer lugar ao longo da linha. 

* Pressionar <b>Esc </b> ou <b>Enter </b> sairá da edição de caminho.
* Uma vez encerrado, clicar em uma superfície em branco da malha iniciará um novo caminho.
* Passar o mouse e clicar em um caminho existente o selecionará, permitindo continuar ou editar esse caminho. Os caminhos também podem ser selecionados novamente por meio do painel <b>Caminhos</b> (veja abaixo).

![Gif mostrando a adição de novos pontos e a movimentação de pontos existentes em um caminho](../../assets/path_edit_move_points.gif)

Algumas propriedades são específicas de um caminho como um todo. Este é o caso das opções encontradas na janela <b>Propriedades </b>. Assim como com um traçado regular (consulte a [documentação da ferramenta Pintura](paint-brush.md)), é possível definir as seguintes propriedades para um caminho:

* <b>Pincel</b>
* <b>Alpha</b>
* <b>Material</b>

A seção <b>pincel </b> contém opções adicionais que estão disponíveis apenas com a ferramenta Caminho:

| <b>Configuração</b> | <b>Descrição</b> |
| --- | --- |
| <b>profundidade de projeção</b> | Determina o quão próximo o caminho precisa estar da superfície da malha para que as marcas de pincel sejam exibidas. Para ver esse feedback visual diretamente no visor, é possível habilitar <b>Normais</b> nas <b>configurações de exibição do caminho </b>(veja abaixo). |
| <b>Eixo para cima</b> | O eixo usado para orientar carimbos de pincel quando <b>Seguir caminho</b> está desativado.   Em algum contexto, faz mais sentido ter todos os carimbos alinhados ao longo de um eixo/direção global e não ao longo do caminho. Por exemplo, com rebites em uma superfície metálica. |

Outras propriedades são definidas por pontos (vértices) no caminho, como a pressão. Para editar um ponto específico, basta clicar nele (ou usar a seleção retangular). Em seguida, use a barra de ferramentas contextual para editar os valores de pontos selecionados.

![Gif mostrando a edição da pressão por vértice](../../assets/path_point_pressure_example.gif)

### Controle de tangentes

Pode haver momentos em que um caminho suave não é ideal, seja porque não segue da melhor maneira a superfície de modelo 3D ou porque não se ajusta a uma aparência específica. Para resolver esses problemas, é possível modificar as tangentes de um determinado vértice. As tangentes são as direções de um ponto que controlam a curvatura do caminho.

Para alternar entre tangentes suaves ou lineares/quebradas, basta clicar duas vezes em um vértice (ou usar o botão dedicado na barra de ferramentas contextual):

![Grade mostrando como controlar tangentes em um caminho](../../assets/path_break_tangents.gif)

Para controlar com mais precisão a orientação das tangentes, use o botão Tangentes personalizadas na barra de ferramentas contextual para substituí-las manualmente:

![Grade mostrando como controlar tangentes em um caminho](../../assets/path_control_tangents.gif)

Use o atalho de teclado <b>ALT</b> para quebrar as tangentes enquanto se move, se o ponto ainda não estiver pronto.

Use o atalho de teclado <b>CTRL</b> para dimensionar as duas tangentes ao mesmo tempo.

>[!NOTE]
>
> Os controles de tangente são definidos ao longo do plano, alinhados com o normal do ponto especificado no caminho. Isso significa que as tangentes não podem se curvar em algumas direções.

### Barra de ferramentas contextual

![Captura de tela da barra de ferramentas contextual no modo de caminho](../../assets/path_contextual_toolbar_overview.png)

A <b>barra de ferramentas contextual</b> quando a ferramenta <b>Caminho</b> está selecionada fornece várias configurações que permitem controlar o caminho atualmente selecionado:

| <b>Parâmetro</b> | <b>Descrição</b> |
| --- | --- |
| <b>Mostrar/ocultar interface do visor</b>  <div><img alt="Ferramenta Caminho mostra o ícone de ocultar" class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_table_row-1k12728-column-xc227lz_image" src="../../assets/path_contextual_toolbar_showhide.png"/></div> | Se ativada, a sobreposição de caminhos e vértices ficará visível na viewport. |
| <b>Configurações de exibição</b>  <div><img alt="Ícone de configurações de exibição de caminho" class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_table_row-uj427cc-column-xc227lz_image" src="../../assets/path_contextual_toolbar_display.png"/></div> | Controle a aparência do feedback visual do caminho na viewport:<ul data-preserve-html="true"> <li data-preserve-html="true"><b>Tamanho da alça</b>: controla o tamanho dos pontos do caminho.</li> <li data-preserve-html="true"><b>Largura do caminho</b>: controle o thickness da linha do caminho.<br/> </li> <li data-preserve-html="true"><b>Cor do caminho</b>: controle a cor da linha do caminho.<br/> </li> <li data-preserve-html="true"><b>Cor de caminho não selecionada</b>: controle a cor dos caminhos não ativos.<br/> </li> <li data-preserve-html="true"><b>Normais</b>: se habilitado, mostra a direção de projeção em cada ponto de um caminho.<br/> </li> <li data-preserve-html="true"><b>Tangentes</b>: se habilitada, mostra a direção da curva dos pontos de controle do caminho.<br/> </li> <li data-preserve-html="true"><b>Direção do caminho</b>: se habilitada, mostra uma pequena seta no final do caminho para indicar a direção da pintura. Isso é útil para saber como os carimbos dentro do traçado serão orientados.</li> </ul>  <div><img alt="Captura de tela do painel de configurações de exibição de caminho" class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_table_row-uj427cc-column-vo327hy_image" src="../../assets/path_contextual_toolbar_display_settings.png"/></div> |
| <b>Inverter direção do caminho</b>  <div><img alt="Ícone de direção do caminho inverso" class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_table_row-5xb27rp-column-xc227lz_image" src="../../assets/path_contextual_toolbar_direction.png"/></div> | Inverter a direção do caminho atual. A direção define a orientação geral usada para pintar os carimbos dentro do traçado. Inverter o caminho pode ajudar a reorientar o padrão desenhado. |
| <b>Alternar canto/suave</b>  <div><img alt="Ícone de alternância de canto suave" class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_table_row-8wd27al-column-xc227lz_image" src="../../assets/path_contextual_toolbar_smoothcorner.png"/></div> | Quebrar ou alinhar a tangente dos vértices atualmente selecionados, permitindo alternar entre uma curva suave ou linear.  <div><img alt="Captura de tela de um caminho com um caminho suave e linear " class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_table_row-8wd27al-column-vo327hy_image" src="../../assets/path_smooth_corner_demo.png"/></div>  **Observação:** a alternância entre o comportamento de canto/suave também pode ser feita clicando duas vezes em um ponto diretamente no caminho. |
| <b>Tangentes personalizadas</b>  <div><img alt="Ícone da ferramenta Caminho para tangentes personalizadas" class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_table_row-r302zw8-column-xc227lz_image" src="../../assets/path_icon_custom_tangents.png"/></div> | Se habilitada, permite controlar manualmente as tangentes de um determinado ponto no caminho.  <div><img alt="Imagem mostrando tangentes de caminho personalizado" class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_table_row-r302zw8-column-vo327hy_image" src="../../assets/paht_cutom_tangents_demo.png"/></div> |
| <b>Abrir/fechar caminho</b>  <div><img alt="Ícone de abrir e fechar caminho" class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_table_row-7ve27oq-column-xc227lz_image" src="../../assets/path_contextual_toolbar_close.png"/></div> | Abrir ou fechar o caminho atual. Para fechar um caminho, um dos dois pontos finais do caminho atual precisa ser selecionado primeiro.  <div><img alt="Gif mostrando um caminho aberto e fechado" class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_table_row-7ve27oq-column-vo327hy_image" src="../../assets/v90_path_open_close.gif"/></div> |
| <b>Excluir vértice</b>  <div><img alt="Ícone do vértice de exclusão de caminho" class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_table_row-v0f273z-column-xc227lz_image" src="../../assets/path_contextual_toolbar_delete.png"/></div> | Remove os vértices atualmente selecionados de um caminho. |
| <b>Simetria</b>  <div><img alt="Ícone do recurso de simetria" class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_table_row-hkg27qa-column-xc227lz_image" src="../../assets/path_contextual_toolbar_symmetry.png"/></div> | Habilite ou desabilite a simetria para o caminho atual. Consulte a [documentação de simetria](../symmetry/symmetry.md) para obter mais informações.  <div><img alt="Gif mostrando um caminho sendo desenhado em simetria" class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_table_row-hkg27qa-column-vo327hy_image" src="../../assets/v90_path_symmetry.gif"/></div> |
| <b>Ocultar/ignorar geometria excluída</b>  <div><img alt="Ícone do recurso de exclusão da máscara de geometria" class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_table_row-52h27be-column-xc227lz_image" src="../../assets/path_contextual_toolbar_exclude.png"/></div> | Se esta opção estiver ativada, faça com que o caminho atual pinte através da geometria oculta. Consulte a [Documentação de máscara de geometria](../../interface/layer-stack/geometry-mask.md) para obter mais informações. |

### Painel Demarcadores

![Painel Caminho](../../assets/path_panel_visibility.png)

>[!NOTE]
>
> O painel fica oculto quando a ferramenta atual não for a ferramenta Caminho ou se uma camada/pasta de preenchimento estiver selecionada.

Dentro do visor há o painel <b>Caminhos</b>, onde são listados todos os caminhos da camada/efeito de pintura atualmente selecionado. Ele fornece uma maneira fácil de selecionar e gerenciar caminhos.

Com esse painel, é possível:

* Clique duas vezes em um caminho para <b>renomear</b>.
* <b>Exclua</b> um caminho selecionando-o e pressionando a tecla Delete.
* <b>Copiar</b>/<b>Colar</b>/<b>Duplicar</b> um caminho com os atalhos de teclado dedicados.
* <b>Mostre</b> ou <b>oculte</b> um caminho com o ícone de olho (que controla se o caminho é aplicado à texturização).

Por conveniência, também é possível clicar com o botão direito do mouse em um caminho para abrir o menu contextual que oferece as mesmas ações:

![Menu do botão direito do mouse do painel Caminho](../../assets/path_panel_rightclick_menu_copy_properties.png)

O menu de contexto também abre ações para copiar as propriedades ou a posição de um caminho em outro caminho. Isso permite compartilhar ou sincronizar recursos facilmente entre diferentes caminhos:

![Gif mostrando como copiar e colar propriedades de caminho](../../assets/path_copy_paste_properties.gif)

![Gif mostrando como copiar e colar posições de caminho](../../assets/path_copy_paste_vertices.gif)

>[!NOTE]
>
> As propriedades de copiar e colar só funcionam quando os caminhos se baseiam na mesma ferramenta de pintura. Por exemplo, não é possível compartilhar propriedades entre um caminho usando as configurações de borrar e outro usando as configurações de pincel.

## Predefinições de ferramenta

![Uma captura de tela da seção de predefinições do painel de propriedades quando uma ferramenta de caminho é selecionada](../../assets/path_presets.png){width="400px"}

Quando uma ferramenta de demarcador é selecionada, uma seção Predefinições fica disponível na parte superior do painel Propriedades. A partir daí, você pode acessar rapidamente as predefinições de várias ferramentas de caminho.

### Adicionar predefinições de caminho aos favoritos

A opção Favoritos na seção Predefinições contém apenas as predefinições que você favoritou para um acesso ainda mais rápido. Para começar a adicionar favoritos, selecione Favoritos e, em seguida, “Mostrar predefinições compatíveis em ativos” para obter uma lista completa de predefinições de caminho disponíveis.

Para adicionar uma predefinição aos favoritos, clique com o botão direito na predefinição no painel Ativos ou na seção Predefinições do painel Propriedades e selecione “Adicionar aos favoritos”. 

Você também pode remover predefinições da lista de favoritos. Clique com o botão direito do mouse em uma predefinição Favorita e selecione “Remover dos favoritos”.

![Uma captura de tela da seção de predefinições do painel de propriedades quando uma ferramenta de caminho está selecionada. A opção Favoritos está selecionada, e o botão “Mostrar predefinições compatíveis em ativos” está destacado.](../../assets/ShowCompatiblePresets.png){width="400px"}

### Criação de predefinições de caminho

Como outras ferramentas, as predefinições podem ser criadas para restaurar rapidamente as configurações/definições do pincel. Para fazer isso, basta clicar com o botão direito do mouse na janela <b>Propriedades</b> e escolher a predefinição de ferramenta <b>Criar.</b> Esta predefinição recém-criada mudará automaticamente para a ferramenta Caminho quando selecionada na janela <b>Ativos</b>.
