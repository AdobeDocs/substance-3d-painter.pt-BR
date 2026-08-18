---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/baking/baking-visualization-settings.html"
breadcrumb-title: ''
description: Saiba como definir as configurações de visualização de panificação no Substance 3D Painter para visualizar e depurar os resultados da panificação do mapa de malha.
helpx_creative_field: ""
helpx_description: Painter > Baking > Baking visualization settings
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Configurações de visualização de preparo
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '597'
ht-degree: 6%

---


# Configurações de visualização de preparo

![](../assets/viewport-vizu.png)

A visualização de cozimento é um painel dentro da viewport do Painter quando em modo de cozimento. Ele permite ajustar as configurações relacionadas à exibição de malhas na viewport.

## Configurações gerais

| Configuração | Descrição |
| --- | --- |
| **Ocultar malhas de cozimento** | Se habilitado, este ícone ocultará a malha alta do poli e do compartimento na viewport. <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r1-column-c1_dynamic_grid_items_grid-cell_position-par_image" src="../assets/hide-baking-meshes.png"/></div> |
| **Mostrar apenas para o Conjunto de Texturas selecionado** | Se ativada, somente o compartimento e as malhas de alto polígono do conjunto de texturas atualmente ativo ficarão visíveis no visor. |

### Malha de alta definição (HP)

| Configuração | Descrição |
| --- | --- |
| <b>Malha</b> | Se ativada, exiba as malhas de alto polígono na visualização 3D. Quando desativadas, as malhas de alto polígono também são descarregadas da memória e podem ajudar a melhorar o desempenho. Use a opção de cor ao lado dessa configuração para controlar a cor da superfície da malha no visor. |
| <b>Erro correspondente</b> | Se ativado, exibe áreas das malhas de alto polígono que estão fora do shell da malha da gaiola na cor dada. Esta configuração ajuda a identificar as áreas que não serão tratadas durante o processo de cozimento e pode resultar em perda de detalhes/informações. Use a opção de cor ao lado dessa configuração para controlar a cor das áreas de interseção na viewport. |

### Gaiola

| Configuração | Descrição |
| --- | --- |
| <b>Superfície da gaiola</b> | Se ativada, a superfície da malha do compartimento será exibida na exibição 3D. A superfície da gaiola é definida pelo botão de cor ao lado da configuração. |
| <b>Opacidade da superfície da caixa</b> | Torne a malha mais ou menos transparente para gerenciar a visibilidade dos detalhes na malha subjacente. |
| <b>wireframe da gaiola</b> | Se ativado, o wireframe da malha do compartimento ficará visível no visor. A cor do wireframe pode ser ajustada com o botão de cor ao lado dessa configuração. |
| <b>Opacidade do wireframe da gaiola</b> | Torne o wireframe mais ou menos transparente. |

### Emendas UV

| Configuração | Descrição |
| --- | --- |
| <b>Fendas ausentes em bordas sólidas</b> | Se ativadas, as bordas sólidas na superfície da malha que não sejam emendas UV serão destacadas com a cor definida pelo botão ao lado da configuração. As bordas realçadas são visíveis apenas na gaiola e na malha de baixo polímero. As bordas podem ser vistas nas exibições 2D e 3D. Esta configuração ajuda a identificar as bordas que têm vértice dividido normal sem uma costura de desembrulho UV, o que poderia levar a problemas de cozimento mais tarde. |

### Malha do projeto

<table data-preserve-html="true">
<colgroup><col/><col/><col/></colgroup><tbody><tr><th scope="col">Configuração</th>
<th scope="col">Configuração secundária</th>
<th scope="col">Descrição</th>
</tr><tr><td><b>Malha do projeto</b></td>
<td> </td>
<td><p>Se ativadas, as malhas de baixo polígono nas quais as malhas de alto polígono são assadas ficarão visíveis no visor. Se a opção <b>Ocultar malhas de cozimento</b> estiver habilitada, essa configuração também será habilitada automaticamente para evitar uma viewport vazia.</p>
<p>Use a opção de cor ao lado dessa configuração para ajustar a cor da malha do projeto.</p>
</td>
</tr><tr><td rowspan="7"><b>Material neutro</b></td>
<td><b>Qualidade</b></td>
<td>Controla a qualidade do reflexo do specular na superfície da malha de baixo polígono. Usar um valor alto proporcionará melhor fidelidade nos reflexos, mas um valor alto poderá afetar o desempenho. Um valor baixo pode introduzir emendas no sombreamento com mapas normais (Observação: este é apenas um problema de exibição).</td>
</tr><tr><td><b>Rugosidade</b></td>
<td>Controla a aspereza do material de malha de baixo polígono nas viewports.</td>
</tr><tr><td><b>Metálico</b></td>
<td>Controla a metalidade do material de malha de baixo polígono nas viewports.</td>
</tr><tr><td><b>Intensidade AO</b></td>
<td>Controla o quanto a Oclusão ambiente cozida contribui para o sombreamento de malha de baixo polígono na Janela de visualização.</td>
</tr><tr><td><b>Dobra normal</b></td>
<td>Se ativada, use Valores normais tortos para melhorar o sombreamento de malha de baixo polígono no visor.</td>
</tr><tr><td><b>Quantidade difusa normal dobrada</b></td>
<td>Controla o quanto os Normais Curvados afetam o sombreamento difuso.</td>
</tr><tr><td><b>Quantidade especular normal dobrada</b></td>
<td>Controla o quanto os Normais Curvados afetam o sombreamento de specular.</td>
</tr></tbody></table>
