---
breadcrumb-title: ""
description: Saiba como configurar o Substance 3D Painter para sistemas de várias GPUs e BiGPU para otimizar o desempenho de renderização.
title: MultiBi-GPU
user-guide-description: ""
user-guide-title: ""
source-git-commit: 6b6d52207ca1d043aaa1b2b14145b6b49d4c1942
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
