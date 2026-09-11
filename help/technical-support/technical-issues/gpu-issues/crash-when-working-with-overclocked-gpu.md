---
helpx_url: "https://helpx.adobe.com/br/substance-3d-painter/technical-support/technical-issues/gpu-issues/crash-when-working-with-overclocked-gpu.html"
breadcrumb-title: ''
description: Saiba como corrigir falhas do Substance 3D Painter ao trabalhar com GPUs com overclock para um desempenho de aplicativo estável.
helpx_creative_field: ""
helpx_description: Painter > Technical support > Technical Issues > GPU Issues > Crash when working with overclocked GPU
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Falha ao trabalhar com GPU em overclock
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '176'
ht-degree: 0%

---


# Falha ao trabalhar com GPU em overclock

GPUs com overclock geralmente podem ser mais instáveis, pois são executadas em frequências que não foram inicialmente projetadas pelo construtor da GPU. Se a GPU estiver com overclock e você tiver problemas de estabilidade, recomendamos voltar às frequências padrão de fábrica por um tempo.

## GPU NVIDIA

Nas GPUs Nvidia, a partir dos drivers 355.82, é possível desativar temporariamente o overclock da GPU ativando um modo de depuração nas configurações dos drivers. Isso permite verificar e determinar problemas relacionados às placas gráficas.

Para ativar o modo de depuração:

1. Abra o **Painel de Controle do Nvidia** (clique com o botão direito do mouse na área de trabalho).
1. Clique no menu **Ajuda**.
1. Clique em **Modo de Depuração**.

>[!NOTE]
>
> O Modo de depuração pode não estar disponível se a GPU for um cartão de referência. Ela estará disponível apenas se a GPU for executada em relógios não padrão ou com um BIOS modificado. Nesse caso, recomendamos desativar manualmente o overclock.
