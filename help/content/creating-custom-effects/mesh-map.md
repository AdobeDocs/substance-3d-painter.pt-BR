---
breadcrumb-title: ""
description: Saiba como usar mapas de malha em efeitos personalizados para que o Substance 3D Painter acesse informações de textura baseadas em geometria.
title: Mapa de malha
user-guide-description: ""
user-guide-title: ""
source-git-commit: 6b6d52207ca1d043aaa1b2b14145b6b49d4c1942
workflow-type: tm+mt
source-wordcount: '120'
ht-degree: 3%
---

# Mapa de malha

Para conectar automaticamente mapas de malha (texturas feitas bake) quando um efeito é adicionado a uma camada, uma convenção de nomenclatura específica deve ser seguida.

>[!NOTE]
>
> É possível usar o **uso** ou o **identificador** em um nó de entrada (o uso tem a prioridade).

Esta é a convenção de nomenclatura de cada mapa de malha:

| Mapa de malha | Uso | Identificador |
| --- | --- | --- |
| *Oclusão de ambiente* | **ambientOcclusionBase** | **ambiente\_oclusão** |
| *ID* | **id** | **id** |
| *Curvatura* | **curvatura** | **curvatura** |
| *Normal* | **BaseNormal** | **normal\_base** |
| *Normais de espaço mundial* | **normalWS** | **mundo\_espaço\_normais** |
| *Posição* | **posição** | **posição** |
| *Thickness* | **thickness** | **thickness** |
| *Height* | **heightBase** | **height\_base** |
| *Dobras normais* | **bentNormalsBase** | **curvo\_normal\_base** |
| *Opacidade* | **opacityBase** | **opacidade\_base** |
