---
helpx_url: "https://helpx.adobe.com/br/substance-3d-painter/technical-support/workflow-issues/viewport-issues/mesh-faces-disappear-when-looking-at-them-from-behind.html"
breadcrumb-title: ''
description: Saiba como corrigir faces de malha que desaparecem quando vistas de trás na viewport do Substance 3D Painter para uma visibilidade de malha adequada.
helpx_creative_field: ""
helpx_description: Painter > Technical support > Workflow Issues > Viewport Issues > Mesh faces disappear when looking at them from behind
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Os rostos de malha desaparecem ao olhar para eles por trás
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '86'
ht-degree: 0%

---


# Os rostos de malha desaparecem ao olhar para eles por trás

Por padrão, as malhas no visor podem não exibir a parte de trás dos polígonos de malha (face de fundo). Isso ocorre porque eles são removidos pelo sombreador atual.

Para exibir a parte de trás dos rostos, basta alterar o sombreador atual para **pbr-metal-rough-alpha-test** nas [configurações do sombreador](../../../interface/shader-settings/shader-settings.md).
