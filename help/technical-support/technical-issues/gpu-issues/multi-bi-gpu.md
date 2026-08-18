---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/technical-support/technical-issues/gpu-issues/multi-bi-gpu.html"
breadcrumb-title: ''
description: Saiba como configurar o Substance 3D Painter para sistemas de várias GPUs e BiGPU para otimizar o desempenho de renderização.
helpx_creative_field: ""
helpx_description: Painter > Technical support > Technical Issues > GPU Issues > MultiBi-GPU
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: MultiBi-GPU
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '93'
ht-degree: 0%

---


# Multi/Bi-GPU

Algumas configurações de GPU e/ou modelos de GPU são incompatíveis com o Substance 3D Painter e resultarão em instabilidades e falhas. Veja abaixo uma lista das configurações incompatíveis:

| ***Configuração*** | ***Solução*** |
| --- | --- |
| **Nvidia SLI/AMD Crossfire** (pontes de placa gráfica) | Desative SLI ou Crossfire nas configurações do driver da GPU. |
| **Bi-GPU** (dois chipsets de GPU em uma placa gráfica) | Desative o uso dos dois chipsets de GPU nas configurações de drivers para apenas um. |
