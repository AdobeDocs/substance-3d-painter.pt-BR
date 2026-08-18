---
helpx_url: "https://helpx.adobe.com/br/substance-3d-painter/technical-support/workflow-issues/tools-issues/normal-map-looks-incorrect-when-loaded-in-layer-or-tool-properties.html"
breadcrumb-title: ''
description: Saiba como corrigir problemas de exibição normal de mapas nas propriedades de camada e ferramenta do Substance 3D Painter para obter detalhes precisos da superfície.
helpx_creative_field: ""
helpx_description: Painter > Technical support > Workflow Issues > Tools Issues > Normal map looks incorrect when loaded in layer or tool properties
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: O mapa normal parece incorreto quando carregado nas propriedades de camada ou ferramenta
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '105'
ht-degree: 0%

---


# O mapa normal parece incorreto quando carregado nas propriedades de camada ou ferramenta

Ao carregar um normal na ferramenta atual da camada fill (preenchimento), este pode parecer incorreto se for um mapa normal OpenGL.\
A razão é bastante simples : o mecanismo do Substance 3D Painter assume que o mapa normal carregado é DirectX por padrão.

Esse comportamento pode ser facilmente editado clicando na pequena seta ao lado do material do substance ou no canal dedicado:

![](../../../assets/channel-format-override.png)
