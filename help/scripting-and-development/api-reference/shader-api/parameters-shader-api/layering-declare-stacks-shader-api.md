---
breadcrumb-title: ""
description: Acesse a referência de API de sombreamento Declarar pilhas de camada para que o Substance 3D Painter crie pilhas de camadas de material personalizadas.
title: Camadas - Declarar pilhas - API de sombreamento
user-guide-description: ""
user-guide-title: ""
source-git-commit: 6b6d52207ca1d043aaa1b2b14145b6b49d4c1942
workflow-type: tm+mt
source-wordcount: '101'
ht-degree: 0%
---

# Camadas - Declarar pilhas - API de sombreamento

## Camadas de material: declarar pilhas editáveis

Uma pilha editável é definida por um identificador exclusivo e uma lista de canais de documentos. As identificações de canal possíveis são: *ambientoclusão* *anisotropiângulo* *anisotropinível* *basecolor* *mesclagem de máscaras* *difusas* *deslocamentos* *emissivos* *glossiness* *heights* *i* *metálico* *normal* *opacidade* *reflexo* *aspereza* *dispersão* *specular* *especularlevel* *transmissivo* *usuário0* *usuário1* *&lbrace;usuário2* usuário3 **&#x200B; usuário4 &#x200B;** usuário5 **&#x200B; usuário6 &#x200B;** usuário7 **

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


Para vincular um canal de uma pilha a um parâmetro de amostragem, coloque a tag de canal no identificador da pilha como prefixo:

```
//: param auto Mask1.channel_opacity 

uniform sampler2D mask_tex1; 

//: param auto Mask2.channel_opacity 

uniform sampler2D mask_tex2; 

 
```
