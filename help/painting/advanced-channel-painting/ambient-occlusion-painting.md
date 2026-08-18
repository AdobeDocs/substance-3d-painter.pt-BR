---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/painting/advanced-channel-painting/ambient-occlusion-painting.html"
breadcrumb-title: ''
description: Aprenda a pintar mapas de oclusão ambiente diretamente no Substance 3D Painter para adicionar sombreamento e profundidade realistas às texturas.
helpx_creative_field: ""
helpx_description: Painter > Painting > Advanced channel painting > Ambient Occlusion Painting
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Pintura de Oclusão ambiente
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '522'
ht-degree: 0%

---


# Pintura de Oclusão ambiente

O canal da oclusão ambiente permite pintar detalhes nas sombras ambientes de um objeto. Ele pode ser usado para adicionar detalhes do AO provenientes de materiais ou simplesmente corrigir erros de cozimento manual quando necessário.

>> 

Em gráficos de computador, a oclusão ambiente é uma técnica de sombreamento e renderização usada para calcular como cada ponto exposto em uma cena é à iluminação ambiente. Normalmente, o interior de um tubo é mais ocluído (e, portanto, mais escuro) do que as superfícies externas expostas, e quanto mais fundo você vai no interior do tubo, mais ocluída (e mais escura) se torna a iluminação. A oclusão ambiente pode ser vista como um valor de acessibilidade calculado para cada ponto da superfície.\
Fonte: &lt;https://en.wikipedia.org/wiki/Ambient_occlusion>

O **resultado** desta computação está armazenado em um bitmap denominado mapa de “Oclusão ambiente”. Este mapa pode ser cozido diretamente no aplicativo, consulte: [Preparação](../../baking/baking.md).

## Pintura Oclusão ambiente

Para pintar detalhes de oclusão personalizados, é necessário um canal de Oclusão ambiente. Ele pode ser adicionado por meio das [configurações do Conjunto de Texturas](../../interface/texture-set/texture-set-settings.md):

![](../../assets/add-ao-channel.png)

Depois que o canal for adicionado a um Conjunto de texturas, qualquer camada poderá ser usada para pintar novas informações. Como o canal AO contém apenas informações de tons de cinza, o modo de mesclagem recomendado é **Normal** (pintar sobre) e **Multiplicar** (combinar).

Para saber mais sobre eles e como alterá-los por canal, consulte: [Modos de mesclagem](../../interface/layer-stack/blending-modes.md).

## Pintura sobre o mapa adicional da Oclusão ambiente

Em algumas situações, pode ser útil pintar sobre a Oclusão ambiente cozida para ocultar detalhes ou até mesmo corrigir problemas de cozimento.

A configuração padrão de um projeto no Substance 3D Painter combinará o **canal** da Oclusão ambiente com o mapa de Oclusão ambiente dos **mapas adicionais**. Isso significa que a pintura sobre o mapa adicional cozido não é possível por padrão, os resultados de cada mapa (os mapas baked e os canais) serão multiplicados juntos. No entanto, isso pode ser alterado com a seguinte configuração:

### 1 - Adicionar um canal de Oclusão ambiente

Adicionar um canal de oclusão ambiente no conjunto de texturas atual:\
![](../../assets/edit-ao-channel-optimized.gif)

Defina seu modo de mistura como &quot; **substituir** &quot; em vez de &quot; **multiplicar** &quot; :\
![](../../assets/ao-mix-mode.gif)

### 2 - Definir uma camada de preenchimento com a oclusão ambiente assada

Crie uma nova camada de preenchimento e coloque a oclusão ambiente assada dentro do slot de “oclusão ambiente” por meio do painel de propriedades. Não se esqueça de alterar a divisão padrão da camada de preenchimento, se ainda não estiver definida como 1.\
![](../../assets/ao-stack.png)

### 3 - Alterar o modo de mesclagem da camada de preenchimento

Por padrão, o modo de mesclagem do canal AO em qualquer nova camada é definido como &quot; **Multiplicar** “. Como é preferível usar a camada de preenchimento como base, escolhemos o modo de mesclagem “normal”, pois o bitmap não tem nenhum alfa, ele substituirá tudo abaixo (incluindo a cor padrão do sombreador).\
![](../../assets/ao-blend-mode.gif)

### 4 - Criar uma camada para pintar sobre o mapa de oclusão ambiente assado

Crie uma nova camada (regular ou de preenchimento) e altere o modo de mesclagem para “normal” para o canal AO. Depois que essa configuração for feita, qualquer coisa pintada no canal AO assumirá o mapa do AO assado que está na camada abaixo.\
![](../../assets/paint-over-ao-optimized.gif)
