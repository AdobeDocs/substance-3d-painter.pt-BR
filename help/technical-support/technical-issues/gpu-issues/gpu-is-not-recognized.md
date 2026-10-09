---
breadcrumb-title: ""
description: Saiba como corrigir problemas de reconhecimento de GPU no Substance 3D Painter para permitir a aceleração e o desempenho adequados do hardware.
title: GPU não reconhecida
user-guide-description: ""
user-guide-title: ""
source-git-commit: 6b6d52207ca1d043aaa1b2b14145b6b49d4c1942
workflow-type: tm+mt
source-wordcount: '79'
ht-degree: 0%
---

# GPU não reconhecida

![](../../../assets/not-recognized-gpu.png){width="500px"}

Alguns usuários do **NVIDIA Optimus** podem ter problemas para executar o Substance 3D Painter na GPU correta. Uma solução alternativa é definir as seguintes chaves no Registro do Windows como 0:

* HKEY\_LOCAL\_MACHINE\SOFTWARE\Microsoft\Windows NT\CurrentVersion\Windows\RequireSignedAppInit
* HKEY\_LOCAL\_MACHINE\SOFTWARE\Wow6432Node\Microsoft\Windows NT\CurrentVersion\Windows\RequireSignedAppInit
