---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/scripting-and-development/api-reference/shader-api/shaders-shader-api/pixelated-shader-api.html"
breadcrumb-title: ''
description: Acesse a referência de API de sombreamento pixelada para o Substance 3D Painter para criar efeitos de renderização pixelados personalizados.
helpx_creative_field: ""
helpx_description: Painter > Scripting and development > API Reference > Shader API > Shaders - Shader API > Pixelated - Shader API
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Pixelizado - API de sombreamento
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '179'
ht-degree: 0%

---


# Pixelizado - API de sombreamento

## Sombreador de pixelização básico

Importar das bibliotecas.

```
import lib-sampler.glsl
```


Definimos a posição de luz global

```
const vec3 light_pos = vec3(10.0, 10.0, 10.0);
```


Nós **vinculamos** a posição do olho do mundo auto param ao nosso uniforme **câmera\_pos**.

```
//: param auto world_eye_position 

uniform vec3 camera_pos;
```


**Associamos** a **cor base** do canal do documento ao nosso **basecolor\_tex** uniforme.

```
//: param auto channel_basecolor 

uniform SamplerSparse basecolor_tex;
```


Definimos um novo ajuste personalizado para esse sombreador, juntamente com seu valor padrão. Esse é usado para ajustar o thickness de contorno, quando sombreado.

```
//: param custom { 

//:  "default": 0.4, 

//:   "min": 0.0, 

//:   "max": 1.0, 

//:   "label": "Unlit outline thickness" 

//: } 

uniform float unlit_outline_thickness;
```


Definimos um novo ajuste personalizado para esse sombreador, juntamente com seu valor padrão. Este é usado para ajustar o thickness de contorno, quando iluminado.

```
//: param custom { 

//:   "default": 0.1, 

//:   "min": 0.0, 

//:   "max": 1.0, 

//:   "label": "Lit outline thickness" 

//: } 

uniform float lit_outline_thickness;
```


Ponto de entrada do sombreador.

```
void shade(V2F inputs) 

{
```


Calculamos alguns valores úteis.

```
  vec3 V = normalize(camera_pos - inputs.position); 

  vec3 N = normalize(inputs.normal); 

  vec3 L = normalize(light_pos - inputs.position); 

  float NdV = dot(N, V); 

  float NdL = max(0.0, dot(N, L));
```


**Prioridade** é executar a **detecção de estrutura de tópicos**. Se a condição do contorno for atingida, saia com a cor preta.

```
  if (NdV < mix(unlit_outline_thickness, lit_outline_thickness, NdL)) { 

    return; 

  } 

 

  vec3 baseColor = getBaseColor(basecolor_tex, inputs.sparse_coord);
```


Introduza alguma tremulação no tamanho da máscara, com base na luminância da cor de base

```
  float maskRadiusJitter = pow(dot(baseColor, vec3(0.3333)), 0.1);
```


Calcular um valor de máscara com base na posição do espaço da tela do fragmento. Isso criará uma grade como padrão.

```
  float mask = pow(1.0 - length(fract(gl_FragCoord.xy / 7.0) - vec2(0.5)), maskRadiusJitter * 5.0) * 5.0;
```


Aqui, obtemos uma amostra da cor base e aplicamos uma atenuação difusa simples

```
  vec3 color = baseColor * NdL; 

 

  diffuseShadingOutput(mask * color); 

} 

 
```
