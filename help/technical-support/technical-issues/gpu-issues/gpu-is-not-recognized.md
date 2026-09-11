---
helpx_url: "https://helpx.adobe.com/br/substance-3d-painter/technical-support/technical-issues/gpu-issues/gpu-is-not-recognized.html"
breadcrumb-title: ''
description: Saiba como corrigir problemas de reconhecimento de GPU no Substance 3D Painter para permitir a aceleração e o desempenho adequados do hardware.
helpx_creative_field: ""
helpx_description: Painter > Technical support > Technical Issues > GPU Issues > GPU is not recognized
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: GPU não reconhecida
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '79'
ht-degree: 0%

---


# GPU não reconhecida

![](../../../assets/not-recognized-gpu.png){width="500px"}

Alguns usuários do **NVIDIA Optimus** podem ter problemas para executar o Substance 3D Painter na GPU correta. Uma solução alternativa é definir as seguintes chaves no Registro do Windows como 0:

* HKEY\_LOCAL\_MACHINE\SOFTWARE\Microsoft\Windows NT\CurrentVersion\Windows\RequireSignedAppInit
* HKEY\_LOCAL\_MACHINE\SOFTWARE\Wow6432Node\Microsoft\Windows NT\CurrentVersion\Windows\RequireSignedAppInit
