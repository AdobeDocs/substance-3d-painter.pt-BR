---
helpx_url: "https://helpx.adobe.com/br/substance-3d-painter/technical-support/technical-issues/stability-issues/crash-during-export.html"
breadcrumb-title: ''
description: Saiba como corrigir falhas do Substance 3D Painter durante as operações de exportação para fluxos de trabalho de exportação de textura confiáveis.
helpx_creative_field: ""
helpx_description: Painter > Technical support > Technical Issues > Stability Issues > Crash during export
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Falha durante a exportação
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '318'
ht-degree: 0%

---


# Falha durante a exportação

Alguns casos específicos podem fazer com que o Substance 3D Painter falhe durante a exportação, especialmente em uma resolução muito alta (como 4K ou 8K). Veja abaixo uma lista das fontes mais comuns desse problema.

## TDR (Timeout Detection and Recovery, Detecção e recuperação de tempo limite)

A Detecção e recuperação de tempo limite (TDR) é um mecanismo de segurança do Microsoft Windows para impedir que uma GPU bloqueie o sistema com uma computação sem fim. Infelizmente, esse mecanismo é muito restritivo para o Substance 3D Painter por padrão.

Para obter mais informações, consulte: [Falha dos drivers de GPU com cálculos longos (falha de TDR)](https://helpx.adobe.com/br/substance-3d/unlisted/documentation/spdoc/gpu-drivers-crash-with-long-computations-128745489.html).

## Pouca memória virtual

A exportação pode consumir uma grande quantidade de RAM (memória do computador); nesse caso, o sistema tentará executar fallback na memória virtual se o sistema ficar sem RAM. A memória virtual é geralmente memória adicional armazenada em unidades de disco rígido. Se o tamanho da memória virtual for muito pequeno, o Substance 3D Painter falhará porque está sem memória total.

Para obter mais informações, consulte: [Falha com pouca memória virtual](crash-with-low-virtual-memory.md).

## Falta de espaço em disco

Desde a introdução do SVT (Sparse Virtual Textures), o Substance 3D Painter pode transmitir no disco um pouco de cache para equilibrar o desempenho. Se não houver espaço livre suficiente no disco, isso pode levar a uma falha porque o aplicativo não conseguiu transferir e gravar o cache.

O local do cache pode ser movido da pasta de arquivos temporários padrão do sistema. Para obter mais informações, consulte: [Texturas Virtuais Esparsas](../../../features/sparse-virtual-textures.md).

## Frequência da GPU com overclock

GPUs com overclock geralmente podem ser mais instáveis, pois são executadas em frequências que não foram inicialmente projetadas pelo construtor da GPU. Pode ajudar a desativar o overclock por um tempo.

Para obter mais informações, consulte: [Falha ao trabalhar com GPU com overclock](../gpu-issues/crash-when-working-with-overclocked-gpu.md).
