---
breadcrumb-title: ""
description: Saiba como corrigir problemas de exibição de mapas normais nas propriedades de camada e ferramenta do Substance 3D Painter para obter detalhes precisos da superfície.
title: A mapa normal parece incorreta quando carregada nas propriedades de camada ou ferramenta
user-guide-description: ""
user-guide-title: ""
source-git-commit: 6b6d52207ca1d043aaa1b2b14145b6b49d4c1942
workflow-type: tm+mt
source-wordcount: '105'
ht-degree: 0%
---

# A mapa normal parece incorreta quando carregada nas propriedades de camada ou ferramenta

Ao carregar um normal na ferramenta atual da camada fill (preenchimento), esta pode parecer incorreta, se for uma mapa normal OpenGL.\
A razão é bastante simples : o mecanismo do Substance 3D Painter assume que o mapa normal carregado é DirectX por padrão.

Esse comportamento pode ser facilmente editado clicando na pequena seta ao lado do material do substance ou no canal dedicado:

![](../../../assets/channel-format-override.png)
