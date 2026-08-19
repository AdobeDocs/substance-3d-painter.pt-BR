---
helpx_url: "https://helpx.adobe.com/br/substance-3d-painter/scripting-and-development/api-reference/shader-api/shaders-shader-api/toon-shader-api.html"
breadcrumb-title: ''
description: Acesse a referência de API de sombreamento de animação do Substance 3D Painter para criar efeitos de renderização personalizados no estilo de animação.
helpx_creative_field: ""
helpx_description: Painter > Scripting and development > API Reference > Shader API > Shaders - Shader API > Toon - Shader API
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Toon - API de sombreamento
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '195'
ht-degree: 0%

---


# Toon - API de sombreamento

## Sombreador de tom básico

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


Nós **vinculamos** a **curvatura da malha** ao nosso **curvatura\_tex** uniforme. Se nenhuma curvatura estiver disponível, a textura transparente será fornecida.

```
//: param auto texture_curvature 

uniform SamplerSparse curvature_tex;
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


Se preferimos usar a curvatura ou não.

```
//: param custom { 

//:   "default": false, 

//:   "label": "Use curvature" 

//: } 

uniform bool use_curvature;
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


**Prioridade** é executar a **detecção de estrutura de tópicos**. Permitir que o usuário escolha se prefere usar o mapa de curvatura para detecção de contorno ou não.

```
  if (use_curvature) { 

    float curv = textureSparse(curvature_tex, inputs.sparse_coord).r; 

    NdV = 1.0 - curv; 

  }
```


Se a condição do contorno for atingida, saia com a cor preta.

```
  if (NdV < mix(unlit_outline_thickness, lit_outline_thickness, NdL)) { 

    return; 

  }
```


Aqui, executamos uma discretização de cores de 4 etapas.

```
  vec3 color = getBaseColor(basecolor_tex, inputs.sparse_coord); 

  if (NdL > 0.75) { 

    color = color; 

  } else if (NdL > 0.5) { 

    color = color * 0.5; 

  } else if (NdL > 0.1) { 

    color = color * 0.1; 

  } 

  else
```


O fallback é preto.

```
    color = vec3(0.0); 

 

  diffuseShadingOutput(color); 

} 

 
```
