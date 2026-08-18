---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/scripting-and-development/api-reference/shader-api/parameters-shader-api/layering-declare-stacks-shader-api.html"
breadcrumb-title: ''
description: Acesse a referência de API de sombreamento Declarar pilhas de camada para que o Substance 3D Painter crie pilhas de camadas de material personalizadas.
helpx_creative_field: ""
helpx_description: Painter > Scripting and development > API Reference > Shader API > Parameters - Shader API > Layering Declare Stacks - Shader API
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Camadas - Declarar pilhas - API de sombreamento
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '101'
ht-degree: 0%

---


# Camadas - Declarar pilhas - API de sombreamento

## Camadas de material: declarar pilhas editáveis

Uma pilha editável é definida por um identificador exclusivo e uma lista de canais de documentos. As identificações de canal possíveis são: *ambientoclusão* *anisotropiângulo* *anisotropinível* *basecolor* *mesclagem de máscaras* *difusas* *deslocamentos* *emissivas* *glossiness* *heights* *i* *metálico* *normal* *opacidade* *reflexão* *aspereza* *dispersão* *specular* *especularlevel* *transmissivo* *usuário0* *usuário1* *{usuário2* usuário3 ** usuário4 ** usuário5 ** usuário6 ** usuário7 **

Exemplo:

```
//:  stacks [ 

//:    { 

//:      "id": "Mask1", 

//:      "channels": [ 

//:        {"id": "opacity"} 

//:      ] 

//:    }, { 

//:      "id": "Mask2", 

//:      "channels": [ 

//:        {"id": "opacity"}, 

//:        {"id": "user0"} 

//:      ] 

//:    } 

//:  ]
```


Para vincular um canal de uma pilha a um parâmetro de amostragem, coloque o prefixo da tag de canal com o identificador da pilha:

```
//: param auto Mask1.channel_opacity 

uniform sampler2D mask_tex1; 

//: param auto Mask2.channel_opacity 

uniform sampler2D mask_tex2; 

 
```
