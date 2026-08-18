---
helpx_url: "https://helpx.adobe.com/br/substance-3d-painter/content/creating-custom-effects/mesh-map.html"
breadcrumb-title: ''
description: Saiba como usar mapas de malha em efeitos personalizados para que o Substance 3D Painter acesse informações de textura baseadas em geometria.
helpx_creative_field: ""
helpx_description: Painter > Content > Creating custom effects > Mesh Map
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Mapa de malha
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '120'
ht-degree: 3%

---


# Mapa de malha

Para conectar automaticamente mapas de malha (texturas preparadas) quando um efeito é adicionado a uma camada, é necessário seguir uma convenção de nomenclatura específica.

>[!NOTE]
>
> É possível usar o **uso** ou o **identificador** em um nó de entrada (o uso tem a prioridade).

Esta é a convenção de nomenclatura de cada mapa de malha:

| Mapa de malha | Uso | Identificador |
| --- | --- | --- |
| *oclusão de ambiente* | **ambientOcclusionBase** | **ambiente\_oclusão** |
| *ID* | **id** | **id** |
| *Curvatura* | **curvatura** | **curvatura** |
| *Normal* | **BaseNormal** | **normal\_base** |
| *Normais de espaço mundial* | **normalWS** | **mundo\_espaço\_normais** |
| *Posição* | **posição** | **posição** |
| *Thickness* | **thickness** | **thickness** |
| *Height* | **heightBase** | **height\_base** |
| *Normais Tortos* | **bentNormalsBase** | **curvo\_normal\_base** |
| *Opacidade* | **opacityBase** | **opacidade\_base** |
