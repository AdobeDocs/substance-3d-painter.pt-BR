---
helpx_url: "https://helpx.adobe.com/br/substance-3d-painter/technical-support/workflow-issues/viewport-issues/viewports-and-textures-are-blurry-or-lack-sharpness.html"
breadcrumb-title: ''
description: Saiba como corrigir viewports e texturas desfocadas no Substance 3D Painter para garantir uma qualidade visual nítida e clara.
helpx_creative_field: ""
helpx_description: Painter > Technical support > Workflow Issues > Viewport Issues > Viewports and textures are blurry or lack sharpness
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: As viewports e as texturas são desfocadas ou não possuem nitidez
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '137'
ht-degree: 1%

---


# As viewports e as texturas são desfocadas ou não possuem nitidez

As viewports podem parecer desfocadas por diferentes motivos.

## Configurações de telas de alto DPI (retina)

Por padrão, o Substance 3D Painter reduz a resolução da viewport na tela High-DPI/Retina para melhorar o desempenho.

Este comportamento pode ser alterado nas [configurações principais](https://helpx.adobe.com/br/substance-3d/unlisted/documentation/spdoc/general-71008262.html) alterando o parâmetro **Escala de Visor**.

## Filtragem de textura

As viewports usam mipmaps e filtragem de textura para serem capazes de transmitir e receber [Texturas Virtuais Esparsas](../../../features/sparse-virtual-textures.md) para melhorar o desempenho. Em alguns casos, isso pode resultar em texturas desfocadas.

A filtragem de textura pode ser ajustada pela janela Configurações de Exibição nos parâmetros [Configurações de Visor](../../../interface/display-settings/viewport-settings.md).
