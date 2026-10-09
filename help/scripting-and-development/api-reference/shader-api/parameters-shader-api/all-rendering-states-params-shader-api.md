---
breadcrumb-title: ""
description: Acesse a referência Todos os parâmetros de estados de renderização para que o Substance 3D Painter controle os parâmetros de estado de renderização.
title: Todos os parâmetros de estados de renderização - API de sombreamento
user-guide-description: ""
user-guide-title: ""
source-git-commit: 6b6d52207ca1d043aaa1b2b14145b6b49d4c1942
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


## localidade de amostragem de sombreador

Por padrão, os canais de documento são amostrados usando coordenadas de textura não transformadas para renderização de otimizações durante a pintura.

Se aparecerem artefatos, defina o estado *não local* para *ativado*.

```
//: state nonlocal on 

 
```
