---
helpx_url: "https://helpx.adobe.com/br/substance-3d-painter/scripting-and-development/api-reference/shader-api/parameters-shader-api/all-rendering-states-params-shader-api.html"
breadcrumb-title: ''
description: Acesse a referência Todos os parâmetros de estados de renderização para que o Substance 3D Painter controle os parâmetros de estado de renderização.
helpx_creative_field: ""
helpx_description: Painter > Scripting and development > API Reference > Shader API > Parameters - Shader API > All Rendering States Params - Shader API
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Todos os parâmetros de estados de renderização - API de sombreamento
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '107'
ht-degree: 2%

---


# Todos os parâmetros de estados de renderização - API de sombreamento

## Exemplos de estados de renderização

## Seleção da face posterior

Retirar faces:

```
//: state cull_face on
```


Desenhe as faces frontal e traseira:

```
//: state cull_face off
```


## Mesclagem

Sem mistura, objetos totalmente opacos:

```
//: state blend none
```


Modo de mesclagem padrão para ordem de desenho de trás para frente:

```
//: state blend over
```


Modo de mesclagem padrão para ordem de desenho de frente para trás. Suponha que a cor seja pré-multiplicada por alfa:

```
//: state blend over_premult
```


Modo de mesclagem aditiva:

```
//: state blend add
```


Modo de mesclagem multiplicativo:

```
//: state blend multiply
```


## Localidade de amostragem do sombreador

Por padrão, os canais de documento são amostrados usando coordenadas de textura não transformadas para renderizar otimizações durante a pintura.

Se aparecerem artefatos, defina o estado *não local* para *ativado*.

```
//: state nonlocal on 

 
```
