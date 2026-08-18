---
helpx_url: "https://helpx.adobe.com/br/substance-3d-painter/technical-support/technical-issues/gpu-issues/gpu-drivers-compatibility.html"
breadcrumb-title: ''
description: Saiba mais sobre os requisitos de compatibilidade de driver de GPU para o Substance 3D Painter para garantir renderização e desempenho estáveis.
helpx_creative_field: ""
helpx_description: Painter > Technical support > Technical Issues > GPU Issues > GPU drivers compatibility
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Compatibilidade de drivers de GPU
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '144'
ht-degree: 2%

---


# Compatibilidade de drivers de GPU

Esta página agrupa informações sobre drivers de GPU que podem levar a problemas com o Substance 3D Painter.

## Nvidia

A tabela abaixo lista todas as versões de driver conhecidas por criar problemas para a GPU Nvidia (modelos GeForce ou Quadro):

| *Versão do driver* | *Descrição do problema* |
| --- | --- |
| <b> 425.xx </b> | artefatos de Rastreamento de raios do GPU. |
| <b> 429.xx ou anterior </b> | Artefatos de bloco de textura preta. |
| <b> 435.xx ou anterior </b> | Problemas de cores sRGB ao calcular texturas. |
| <b> 439.xx </b> | Corrupção de texturas. |
| <b> 441.08 </b> | Problemas de falha ou estabilidade. |
| <b> 442.19 </b> | Problemas de falha ou estabilidade. |
| <b>528.09</b> | Congelamento do sistema operacional. |
| <b>572.16 a 572.42</b> | Artefatos ou falha ao assar texturas. |

### AMD

| *Versão do driver* | *Descrição do problema* |
| --- | --- |
| **20.7.x** a **20.11.2** | Texturas com problemas ou corrupção. |
| **20.11.3** a **21.2.1** | Texturas com falha ou corrupção, além de problemas de falha ou estabilidade. |
| **21.2.3** a **21.6.1** | Problemas de falha ou estabilidade. |
