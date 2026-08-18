---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/scripting-and-development/api-reference/shader-api/libraries-shader-api/lib-random-shader-api.html"
breadcrumb-title: ''
description: Acesse a referência de API de sombreamento Aleatória da biblioteca para que o Substance 3D Painter gere valores aleatórios no desenvolvimento de sombreador personalizado.
helpx_creative_field: ""
helpx_description: Painter > Scripting and development > API Reference > Shader API > Libraries - Shader API > Lib Random - Shader API
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Aleatório da biblioteca - API de sombreamento
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '128'
ht-degree: 0%

---


# Aleatório da biblioteca - API de sombreamento

## lib-random.glsl

**Funções Públicas:** *getBlueNoiseThreshold* *getBlueNoiseThresholdTemporal* *fibonacci1D* *fibonacci2D* *fibonacci2DDitheredTemporal*

Importar da biblioteca

```
import lib-defines.glsl
```


Uma textura de ruído azul 2D contendo valores escalares

```
//: param auto texture_blue_noise 

uniform sampler2D texture_blue_noise;
```


Resolução de textura de ruído azul

```
const ivec2 texture_blue_noise_size = ivec2(256);
```


Velocidade aleatória do quadro atual

```
//: param auto random_seed 

uniform int alg_random_seed;
```


Obtenha um valor aleatório uniforme com base nas coordenadas de pixel.

```
float getBlueNoiseThreshold() 

{ 

  return texture(texture_blue_noise, gl_FragCoord.xy / vec2(texture_blue_noise_size)).x + 0.5 / 65536.0; 

}
```


Obtenha um valor aleatório uniforme com base nas coordenadas de pixel e na ID do quadro.

```
float getBlueNoiseThresholdTemporal() 

{ 

  return fract(getBlueNoiseThreshold() + M_GOLDEN_RATIO * alg_random_seed); 

}
```


Retorna o número i *th* da sequência de fibonacci.

```
float fibonacci1D(int i) 

{ 

  return fract((float(i) + 1.0) * M_GOLDEN_RATIO); 

}
```


Retorna o par i *º* da sequência de fibonacci. nbSample é necessário para obter uma distribuição uniforme.

```
vec2 fibonacci2D(int i, int nbSamples) 

{ 

  return vec2( 

    (float(i)+0.5) / float(nbSamples), 

    fibonacci1D(i) 

  ); 

}
```


Retorna o par i *º* da sequência de fibonacci. nbSample é necessário para obter uma distribuição uniforme. Esta versão tem uma rotação pseudo-aleatória por quadro e por pixel aplicada.

```
vec2 fibonacci2DDitheredTemporal(int i, int nbSamples) 

{ 

  vec2 s = fibonacci2D(i, nbSamples); 

  s.x += getBlueNoiseThresholdTemporal(); 

  return s; 

} 

 
```
