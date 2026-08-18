---
helpx_url: "https://helpx.adobe.com/br/substance-3d-painter/scripting-and-development/api-reference/shader-api/libraries-shader-api/lib-emissive-shader-api.html"
breadcrumb-title: ''
description: Acesse a referência Lib Emissive API de sombreamento para o Substance 3D Painter para criar materiais emissivos e efeitos brilhantes.
helpx_creative_field: ""
helpx_description: Painter > Scripting and development > API Reference > Shader API > Libraries - Shader API > Lib Emissive - Shader API
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Lib Emissive - API de sombreamento
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '54'
ht-degree: 0%

---


# Lib Emissive - API de sombreamento

## lib-emissive.glsl

**Funções Públicas:** *pbrComputeEmissive*

Importar da biblioteca

```
import lib-sparse.glsl
```


A textura emissiva do canal.

```
//: param auto channel_emissive 

uniform SamplerSparse emissive_tex;
```


Um valor usado para ajustar a intensidade emissiva.

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


Calcular a radiância emissiva para o olho do espectador

```
vec3 pbrComputeEmissive(SamplerSparse emissive, SparseCoord coord) 

{ 

  return emissive_intensity * textureSparse(emissive, coord).rgb; 

} 

 
```
