---
helpx_url: "https://helpx.adobe.com/br/substance-3d-painter/scripting-and-development/api-reference/shader-api/parameters-shader-api/all-engine-params-shader-api.html"
breadcrumb-title: ''
description: Acesse a referência da API de sombreamento Todos os parâmetros de mecanismo do Substance 3D Painter para controlar os parâmetros de sombreador no nível do mecanismo.
helpx_creative_field: ""
helpx_description: Painter > Scripting and development > API Reference > Shader API > Parameters - Shader API > All Engine Params - Shader API
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Todos os Parâmetros de Mecanismo - API de sombreamento
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '511'
ht-degree: 0%

---


# Todos os Parâmetros de Mecanismo - API de sombreamento

## Exemplos de parâmetros de mecanismo

## Parâmetros de textura

O Substance Painter usa um sistema SVT (Textura Virtual Esparsa) para exibir texturas na viewport.

Para obter mais informações sobre este sistema, vá para a [documentação online](../../../../features/sparse-virtual-textures.md).

Este sistema tem repercussões em como escrever código de sombreador. Estamos fornecendo auxiliares para simplificar seu uso com as funções de pesquisa de textura e estrutura do *SamplerSparse* (consulte [lib-sparse.glsl](../libraries-shader-api/lib-sparse-shader-api.md)).

Uso básico:

```
// Defines the SamplerSparse structure 

import lib-sparse.glsl 

 

//: param auto TEXTURE_TAG 

uniform SamplerSparse uniform_tex;   // Texture sampler and its information
```


Os parâmetros de textura permitem usar o operador &#39;or&#39; para definir um fallback:

```
//: param auto TEXTURE_TAG_1 or TEXTURE_TAG_2 

uniform SamplerSparse uniform_tex; // if TEXTURE_TAG_1 exists then TEXTURE_TAG_1 else TEXTURE_TAG_2
```


Em que *TEXTURE\_TAG* é uma das marcas descritas abaixo.

### Tags de canais do documento

Todas essas texturas são **pré-multiplicadas** e **dilatadas** para evitar problemas de emendas.

**Canais do conjunto de texturas**

*channel\_ambientocclusion* *channel\_anisotropyangle* *channel\_anisotropylevel* *channel\_basecolor* *channel\_blendingmask* *channel\_diffuse* *channel\_deslocamento* *channel\_emissive* *channel\_glossiness* *channel\_height* *canal\_i* *canal\_metálico* *canal\_normal* *canal\_opacidade* *canal\_reflexão* *canal\_aspereza* *canal\_dispersão* *canal\_specular* *canal\_espéarlevel* *canal\_transmissivo*

**Canais de usuário**

*canal\_usuário0* *canal\_usuário1* *canal\_usuário2* *canal\_usuário3* *canal\_usuário4* *canal\_usuário5* *canal\_usuário6* *canal\_usuário7*

### Mapas de malha

*textura\_ambientocclusion* : mapa de Oclusão de ambiente\
*textura\_curvatura* : mapa de curvatura\
*textura\_id* : mapa de ID\
*textura\_normal* : mapa de espaço tangente normal\
*textura\_normal\_ws* : mapa normal do espaço global\
*textura\_posição* : mapa de posição do espaço global\
*textura\_thickness* : mapa de Thickness

## Parâmetros de textura adicionais

Uso básico:

```
//: param auto TEXTURE_TAG 

uniform sampler2D uniform_tex;   // The texture itself 

 

//: param auto TEXTURE_TAG_size 

uniform vec4 uniform_tex_size;   // The size of the texture (width, height, 1/width, 1/height)
```


Os parâmetros de textura permitem usar o operador &#39;or&#39; para definir um fallback:

```
//: param auto TEXTURE_TAG_1 or TEXTURE_TAG_2 

uniform sampler2D uniform_tex; // if TEXTURE_TAG_1 exists then TEXTURE_TAG_1 else TEXTURE_TAG_2 

 

//: param auto TEX_TAG_1_size or TEX_TAG_2_size 

uniform vec4 uniform_tex_size; // if TEX_TAG_1 exists then TEX_TAG_1_size else TEX_TAG_2_size
```


Em que *TEXTURE\_TAG* é uma das marcas descritas abaixo.

*textura\_azul\_noise* : uma textura de ruído azul\
*textura\_ambiente* : mapa de ambiente, **mip-mapped**, use [lib-env.glsl](../libraries-shader-api/lib-env-shader-api.md) para usar este

## Outros parâmetros

*proporção\_ratio* : uma *flutuante* contendo a proporção de visor *largura / height*

```
//: param auto aspect_ratio 

uniform float uniform_aspect_ratio;
```


*câmera\_view\_matrix* : um *mat4* representando a transformação do espaço global para o espaço da câmera

```
//: param auto camera_view_matrix 

uniform mat4 uniform_camera_view_matrix;
```


*camera\_view\_matrix\_it* : versão de transposição inversa da *câmera\_exibição\_matriz*

```
//: param auto camera_view_matrix_it 

uniform mat4 uniform_camera_view_matrix_it;
```


*camera\_vp\_matrix\_inverse* : inverso da matriz *projeção \* câmera\_exibição\_matriz*

```
//: param auto camera_vp_matrix_inverse 

uniform mat4 uniform_camera_vp_matrix_inverse;
```


*exposição\_ambiente* : um *flutuar* representando a exposição do mapa de ambiente

```
//: param auto environment_exposure 

uniform float uniform_environment_exposure;
```


*environment\_max\_lod* : um *float* representando a profundidade do mapa de ambiente da pirâmide do mapa de mip

```
//: param auto environment_max_lod 

uniform float uniform_max_lod;
```


*environment\_rotation* : um *float* representando a rotação do mapa de ambiente no eixo superior\
o valor está no intervalo [0,1] e deve ser mapeado para o intervalo [0, 2\*pi]

```
//: param auto environment_rotation 

uniform float uniform_environment_rotation;
```


*face* : um *inteiro* indicando faces renderizadas (-1: faces traseiras, 0: indefinidas, 1: faces frontais)\
o valor 0 significa que você pode confiar com segurança na variável interna glsl *gl\_FrontFacing*

```
//: param auto facing 

uniform int uniform_facing;
```


*fovy* : um *float* representando o campo de visão da câmera ao longo do eixo Y

```
//: param auto fovy 

uniform float uniform_fovy;
```


*is\_2d\_view* : um *bool* indicando se a renderização é executada para exibição 2D ou não

```
//: param auto is_2d_view 

uniform bool uniform_2d_view;
```


*is\_perspective\_projection* : um *bool* indicando se a projeção é em perspectiva ou ortográfica

```
//: param auto is_perspective_projection 

uniform bool uniform_perspective_projection;
```


*luz\_principal* : um *vec4* indicando a posição da luz principal no ambiente

```
//: param auto main_light 

uniform vec4 uniform_main_light;
```


*mvp\_matrix* : um *mat4* representando a matriz de projeção de exibição de modelo

```
//: param auto mvp_matrix 

uniform mat4 uniform_mvp_matrix;
```


*cena\_original\_radius* : um *flutuante* representando o raio da esfera delimitadora da cena antes de sua normalização

```
//: param auto scene_original_radius 

uniform float uniform_scene_original_radius;
```


*tamanho\_da_tela* : um *vec4* contendo dados de tamanho da tela *(largura, height, 1/largura, 1/height)*

```
//: param auto screen_size 

uniform vec4 uniform_screen_size;
```


*world\_camera\_direction* : um *vec3* representando a orientação mundial da câmera

```
//: param auto world_camera_direction 

uniform vec3 uniform_world_camera_direction;
```


*world\_eye\_position* : um *vec3* que representa a posição do olho do mundo

```
//: param auto world_eye_position 

uniform vec3 uniform_world_eye_position; 

 
```
