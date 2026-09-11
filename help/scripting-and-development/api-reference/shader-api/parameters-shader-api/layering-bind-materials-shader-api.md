---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/scripting-and-development/api-reference/shader-api/parameters-shader-api/layering-bind-materials-shader-api.html"
breadcrumb-title: ''
description: Acesse a referência de API de sombreamento Materiais de vinculação de camada para que o Substance 3D Painter vincule materiais em fluxos de trabalho em camadas.
helpx_creative_field: ""
helpx_description: Painter > Scripting and development > API Reference > Shader API > Parameters - Shader API > Layering Bind Materials - Shader API
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Materiais de vinculação de camada - API de sombreamento
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '106'
ht-degree: 0%

---


# Materiais de vinculação de camada - API de sombreamento

## Camadas de material: vincular materiais como parâmetros de sombreador

Um material é definido por um identificador exclusivo &#39;id&#39;. Parâmetros adicionais:

* &#39;default&#39;: o nome do recurso de material padrão a ser usado.
* &#39;size&#39;: o tamanho da textura dos mapas de materiais.
* “group”: o grupo da interface do usuário do widget de seleção de material.

Exemplo:

```
//:  materials [ 

//:    { 

//:       "id": "Material1", 

//:       "default": "Concrete 044", 

//:       "size": 512, 

//:       "group": "Material 1" 

//:    }, { 

//:       "id": "Material2", 

//:       "default": "Leaves elm", 

//:       "size": 1024, 

//:       "group": "Material 2" 

//:    } 

//:  ]
```


Para vincular um canal de um material a um amostrador, defina um parâmetro automático com a ID do material seguida pela tag de canal (consulte os canais disponíveis em [all-engine-params.glsl](all-engine-params-shader-api.md)):

```
//: param auto Material1.channel_basecolor 

uniform sampler2D basecolor_tex1; 

//: param auto Material1.channel_metallic 

uniform sampler2D metallic_tex1; 

//: param auto Material1.channel_roughness 

uniform sampler2D roughness_tex1; 

 

//: param auto Material2.channel_basecolor 

uniform sampler2D basecolor_tex2; 

//: param auto Material2.channel_metallic 

uniform sampler2D metallic_tex2; 

//: param auto Material2.channel_roughness 

uniform sampler2D roughness_tex2; 

 
```
