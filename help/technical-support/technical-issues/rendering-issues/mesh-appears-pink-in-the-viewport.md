---
helpx_url: "https://helpx.adobe.com/br/substance-3d-painter/technical-support/technical-issues/rendering-issues/mesh-appears-pink-in-the-viewport.html"
breadcrumb-title: ''
description: Saiba como corrigir a aparência da malha rosa no visor do Substance 3D Painter para restaurar a renderização adequada do material.
helpx_creative_field: ""
helpx_description: Painter > Technical support > Technical Issues > Rendering Issues > Mesh appears pink in the viewport
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: A malha aparece em rosa no visor
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '125'
ht-degree: 0%

---


# A malha aparece em rosa no visor

![](../../../assets/pink-mesh.jpg){width="400px"}

A malha pode aparecer **rosa** dentro do visor porque o **sombreador** usado para desenhá-lo **não é mais compilado** (conforme mencionado pela **janela de log** ). Isso pode ser causado por um sombreador desatualizado que não oferece suporte à versão mais recente do API de sombreamento.

Veja como corrigir isso:

* Para **sombreadores padrão**: siga o procedimento passo a passo na página [Atualizando um sombreador](../../../interface/shader-settings/updating-a-shader.md).
* Para **sombreador personalizado**: observe a mensagem de erro na janela de log e na página [API de sombreamento](https://helpx.adobe.com/br/substance-3d/unlisted/documentation/spdoc/custom-shader-api-89686018.html).
