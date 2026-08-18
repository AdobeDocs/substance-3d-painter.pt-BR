---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/baking/how-to-bake-mesh-maps.html"
breadcrumb-title: ''
description: Saiba como preparar mapas de malha no Substance 3D Painter para gerar oclusão ambiente, curvatura e outras texturas baseadas em geometria.
helpx_creative_field: ""
helpx_description: Painter > Baking > How to bake mesh maps
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Como preparar mapas de malha
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '520'
ht-degree: 0%

---


# Como preparar mapas de malha

O modo de cozimento dedicado do Substance 3D Painter facilita a construção de mapas de malha que podem fornecer materiais inteligentes incríveis e outras ferramentas. Continue lendo ou assista ao vídeo abaixo para saber como começar a assar com o Substance 3D Painter.

## 1 - Mudar para modo de cozedura

Por padrão, o Painter é iniciado no modo de Pintura ao criar ou abrir um projeto. Para poder preparar mapas de malha, é necessário alternar para o modo de cozimento. Use uma das seguintes opções para alternar para o modo de cozimento:

* Use o <b>botão Modo de cozimento</b> (<b>ícone do Croissant</b>) na barra de ferramentas contextual no canto superior direito da Janela de visualização

  ![](../assets/croissant-icon.png)

  >[!NOTE]
  >
  > Às vezes, o <b>botão Modo de cozimento</b> pode ficar oculto atrás de outros painéis, dependendo do layout do seu espaço de trabalho.
* Use o menu Modo e selecione <b>Criar mapas de malha.\
  </b>
* Use o atalho de teclado do <b>F8</b>.

### 2 - Selecionar Conjuntos de Textura e Blocos UV

Dentro da <b>lista do Conjunto de Texturas</b>, use a caixa de seleção ao lado de cada conjunto de Textura (e o número de Blocos UV, se houver) para selecionar quais partes assar:

![](../assets/texture-set-list-baking-selection.png)

### 3 - Selecionar padeiros

Dentro da janela Preparadores de mapas de malha, use as caixas de seleção para selecionar os mapas que deseja assar:

![](../assets/mesh-map-bakers-selection.png)

### 4 - Alterar configurações comuns

No painel Padeiros de mapas de malha, clique nas configurações comuns para alterar configurações como resolução de mapa baked, largura de dilatação e parâmetros de alto índice, que são compartilhadas em todos os mapas:

![](../assets/common-settings.png)

Nas configurações comuns, você pode definir quais arquivos serão usados como malhas de alta definição. A seleção de malhas de alta definição permite definir como a gaiola é gerada para as malhas:

* Distância com base: infle os vértices fora da malha a uma distância uniforme pelo modelo para criar uma caixa.
* Automático (experimental): o Painter analisará sua malha e gerará uma gaiola automaticamente, tentando mantê-la próxima à superfície sem criar interseções para obter melhores resultados.
* Arquivo personalizado: importe um arquivo que você criou para usar como o compartimento. Observe que os arquivos importados devem ter o mesmo número de vértices que a malha base para funcionar corretamente.

Se você não estiver assando a partir de uma malha de alto polígono, habilite a caixa de seleção <b>Usar malha de baixo polígono como malha de alto polígono</b>.

### 5 - Ajuste o compartimento

Há diferentes opções disponíveis para ajustar a gaiola com base no método de gaiola que você está usando. Com um compartimento com base na distância, é possível ajustar as distâncias Frontal e Traseira para minimizar a quantidade de interseção entre o compartimento e a malha.

![](../assets/cage-distance.gif)

>[!NOTE]
>
> Manchas vermelhas aparecem quando a gaiola cruza com a geometria do modelo. Uma gaiola de interseção geralmente leva a artefatos e problemas na área de interseção.

### 6 - Iniciar o processo de cozedura

Na parte inferior da viewport, clique no botão Bake para iniciar o processo de cozimento.

![](../assets/bake-button.png)

### 7 - Inspect o registro de preparo para erros

Assim que o processo de cozimento terminar, você pode dar uma olhada na janela Registro de cozedura para verificar se há algum erro relatado.

Se houver alguma, use a seta ao lado da mensagem de erro para exibir as configurações relevantes do panificador:

![](../assets/bake-failed.png)
