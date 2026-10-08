---
breadcrumb-title: ""
description: Acesse a API de sombreamento Lib para que o Substance 3D Painter funcione com canais alfa e transparência em sombreadores personalizados.
title: Alpha da biblioteca - API de sombreamento
user-guide-description: ""
user-guide-title: ""
source-git-commit: 6b6d52207ca1d043aaa1b2b14145b6b49d4c1942
workflow-type: tm+mt
source-wordcount: '72'
ht-degree: 0%
---

# Alpha da biblioteca - API de sombreamento

## lib-alpha.glsl

**Funções Públicas:** *alphaKill*

```
import lib-sampler.glsl 

import lib-random.glsl
```


Mapa de opacidade fornecido pelo mecanismo.

```
//: param auto channel_opacity 

uniform SamplerSparse opacity_tex;
```


Limite de teste de Alpha.

```
//: param custom { 

//:   "default": 0.33, 

//:   "label": "Alpha threshold", 

//:   "min": 0.0, 

//:   "max": 1.0, 

//:   "group": "Common Parameters" 

//: } 

uniform float alpha_threshold;
```


pontilhamento de teste Alpha.

```
//: param custom { 

//:   "default": false, 

//:   "label": "Alpha dithering", 

//:   "group": "Common Parameters" 

//: } 

uniform bool alpha_dither;
```


Emular teste alfa : descarta o fragmento atual se sua opacidade estiver abaixo de um limite definido pelo usuário. Deve ser chamado APÓS chamadas de amostragem de textura: pode quebrar derivados

```
void alphaKill(float alpha) 

{ 

  float threshold = alpha_dither ? getBlueNoiseThresholdTemporal() : alpha_threshold; 

  if (alpha < threshold) discard; 

} 

 

void alphaKill(SparseCoord coord) 

{ 

  alphaKill(getOpacity(opacity_tex, coord)); 

} 

 
```
