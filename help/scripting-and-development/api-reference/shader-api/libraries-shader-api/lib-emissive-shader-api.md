---
helpx_url: "https://helpx.adobe.com/br/substance-3d-painter/scripting-and-development/api-reference/shader-api/libraries-shader-api/lib-emissive-shader-api.html"
breadcrumb-title: ''
description: Acesse a referência API de sombreamento de Emissivo de biblioteca do Substance 3D Painter para criar materiais de emissivo e efeitos brilhantes.
helpx_creative_field: ""
helpx_description: Painter > Scripting and development > API Reference > Shader API > Libraries - Shader API > Lib Emissive - Shader API
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Emissivo de biblioteca - API de sombreamento
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '54'
ht-degree: 0%

---


# Emissivo de biblioteca - API de sombreamento

## lib-emissivo.glsl

**Funções Públicas:** *pbrComputeEmissive*

Importar da biblioteca

```
import lib-sparse.glsl
```


A textura do canal de emissivo.

```
//: param auto channel_emissive 

uniform SamplerSparse emissive_tex;
```


Um valor usado para ajustar a intensidade do emissivo.

```
//: param custom { 

//:   "default": 1.0, 

//:   "label": "Emissive Intensity", 

//:   "min": 0.0, 

//:   "max": 100.0, 

//:   "group": "Common Parameters" 

//: } 

uniform float emissive_intensity;
```


Calcular a radiância do emissivo para o olho do espectador

```
vec3 pbrComputeEmissive(SamplerSparse emissive, SparseCoord coord) 

{ 

  return emissive_intensity * textureSparse(emissive, coord).rgb; 

} 

 
```
