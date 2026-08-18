---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/painting/advanced-channel-painting/flow-map-painting.html"
breadcrumb-title: ''
description: Aprenda a pintar mapas de fluxo no Substance 3D Painter para controlar a direção do fluxo do material e os efeitos anisotrópicos.
helpx_creative_field: ""
helpx_description: Painter > Painting > Advanced channel painting > Flow Map Painting
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Pintura de mapa de fluxo
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '174'
ht-degree: 0%

---


# Pintura de mapa de fluxo

Um canal dedicado é planejado, mas, ao mesmo tempo, usando o canal Normal e alguns parâmetros de pincel, é possível pintar mapas de fluxo no Substance 3D Painter.

## Etapa 1: Criar o mapa normal

Crie uma textura de mapa normal de 16 por 16 pixels. A cor deve ser 128, 255, 128, o que deve apresentar a seguinte cor: ![](../../assets/up-dx.png)\
(Esta cor é o equivalente a um vetor olhando para cima, em DirectX)

## Etapa 2: Adicionar canal normal

Em seu projeto do Substance 3D Painter, adicione um canal **Normal** por meio das **configurações do conjunto de texturas** se esse canal ainda não existir.

## Etapa 3: Configuração do pincel

Ative o recurso Seguir caminho nos parâmetros do pincel. Carregue a textura normal do mapa (etapa 1) no slot de canal normal. Desative os outros canais.

![](../../assets/brush-settings-1.png){width="300px"}

## Etapa 4: Pintar!

Ao pintar na malha com a configuração do caminho de acompanhamento ativada, os traçados de pincel desenharão direções no mapa normal.

![](../../assets/painting-1.png){width="700px"}
