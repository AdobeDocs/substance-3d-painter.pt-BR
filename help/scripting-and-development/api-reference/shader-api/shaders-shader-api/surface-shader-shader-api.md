---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/scripting-and-development/api-reference/shader-api/shaders-shader-api/surface-shader-shader-api.html"
breadcrumb-title: ''
description: Acesse a referência API de sombreamento de superfície do Substance 3D Painter para criar efeitos e materiais de sombreador de superfície personalizados.
helpx_creative_field: ""
helpx_description: Painter > Scripting and development > API Reference > Shader API > Shaders - Shader API > Surface Shader - Shader API
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Sombreador de Superfície - API de sombreamento
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '114'
ht-degree: 0%

---


# Sombreador de Superfície - API de sombreamento

## surface-shader.glsl

Para criar um recurso de sombreador que possa ser usado em Substance Painter, basta criar um arquivo glsl contendo uma única função chamada *sombra* com o seguinte perfil:

```
void shade(V2F inputs);
```


## Definição do tipo de entrada V2F:

```
struct V2F { 

  vec3 normal;               // interpolated normal 

  vec3 tangent;              // interpolated tangent 

  vec3 bitangent;            // interpolated bitangent 

  vec3 position;             // interpolated position 

  vec4 color[1];             // interpolated vertex colors (color0) 

  vec2 tex_coord;            // interpolated texture coordinates (uv0) 

  SparseCoord sparse_coord;  // interpolated sparse texture coordinates used by textureSparse() sampling function 

  vec2 multi_tex_coord[8];   // interpolated texture coordinates (uv0-uv7) 

};
```


Observação: para obter um SparseCoord para uv1-uv7, você deve chamar explicitamente *getSparseCoord(vec2)* definido em [lib-sparse.glsl](../libraries-shader-api/lib-sparse-shader-api.md)

## Saídas do sombreador de superfície:

As seguintes funções podem ser chamadas dentro da função *sombra* para descrever as propriedades do fragmento:

```
// fragment opacity. default value: 1.0 

void alphaOutput(float); 

// diffuse lighting contribution. default value: vec3(0.0) 

void diffuseShadingOutput(vec3); 

// specular lighting contribution. default value: vec3(0.0) 

void specularShadingOutput(vec3); 

// color emitted by the fragment. default value: vec3(0.0) 

void emissiveColorOutput(vec3); 

// fragment color. default value: vec3(1.0) 

void albedoOutput(vec3); 

// subsurface scattering properties, see lib-sss.glsl for details. default value: vec4(0.0) 

void sssCoefficientsOutput(vec4);
```


Como exemplo, a equação de renderização mais básica para calcular a cor do fragmento é: *emissiveColor + albedo \* diffuseShading + specularShading*
