---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/technical-support/technical-issues/rendering-issues/mesh-flash-to-white-when-moving-camera.html"
breadcrumb-title: ''
description: Saiba como corrigir a malha piscando para branco ao mover a câmera no visor do Substance 3D Painter para uma renderização estável.
helpx_creative_field: ""
helpx_description: Painter > Technical support > Technical Issues > Rendering Issues > Mesh flash to white when moving camera
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: A malha flash para branco ao mover a câmera
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '140'
ht-degree: 0%

---


# A malha flash para branco ao mover a câmera

![](../../../assets/white-flash-svt-optim.gif){width="300px"}

Com projetos antigos se movendo pela câmera na viewport poderão mostrar brevemente flashes brancos criados por texturas brancas/vazias. Isso ocorre porque o sistema SVT (Texturas Virtuais Esparsas) [depende de configurações específicas de sombreador que sombreadores mais antigos não usam.](https://substance3d.adobe.com/display/DRAFTPAINTER/Sparse+Virtual+Textures)

Para se livrar do flash branco, basta **atualizar** o **sombreador de projeto**:

* Para **sombreadores padrão**: siga o procedimento passo a passo na página [Atualizando um sombreador](../../../interface/shader-settings/updating-a-shader.md).
* Para **sombreadores personalizados**: observe a(s) mensagem(ns) de erro no log e na página [API de sombreamento](https://helpx.adobe.com/substance-3d/unlisted/documentation/spdoc/custom-shader-api-89686018.html).
