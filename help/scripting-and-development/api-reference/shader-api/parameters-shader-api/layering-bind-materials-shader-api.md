---
breadcrumb-title: ""
description: Acesse a referência de API de sombreamento Materiais de vinculação de camada para que o Substance 3D Painter vincule materiais em fluxos de trabalho em camadas.
title: Materiais de vinculação de camada - API de sombreamento
user-guide-description: ""
user-guide-title: ""
source-git-commit: 6b6d52207ca1d043aaa1b2b14145b6b49d4c1942
workflow-type: tm+mt
source-wordcount: '106'
ht-degree: 0%
---

# Materiais de vinculação de camada - API de sombreamento

## Camadas de material: vincular materiais como parâmetros de sombreador

Um material é definido por um identificador exclusivo &#39;id&#39;. Parâmetros adicionais:

* &#39;default&#39;: o nome do recurso de material padrão a ser usado.
* &#39;tamanho&#39;: o tamanho de textura dos mapas de material.
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
