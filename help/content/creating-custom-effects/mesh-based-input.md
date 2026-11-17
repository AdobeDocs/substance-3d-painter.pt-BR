---
breadcrumb-title: ""
description: Saiba como usar entradas baseadas em malha em efeitos personalizados para que o Substance 3D Painter crie efeitos de textura sensíveis à geometria.
title: Entrada baseada em malha
user-guide-description: ""
user-guide-title: ""
source-git-commit: 4432887b652896f77fc3c99010436ef44aeb8a3e
workflow-type: tm+mt
source-wordcount: '279'
ht-degree: 1%
---

# Entrada baseada em malha

A entrada baseada em malha é uma textura fornecida pelo mecanismo do Substance 3D Painter extraído da malha dentro do projeto atual. Essas texturas podem ser usadas para criar efeitos avançados com base na topologia de malha.

>[!NOTE]
>
> Essas informações de malha são baseadas na própria topologia e não levam em conta o mapa de malha (texturas feitas bake).
> 
> A entrada fornecida pelo mecanismo é uma textura de ponto flutuante de 32 bits que será reduzida/fixada ao valor da entrada no gráfico de Substance.

| Informações de malha | Identificador | Uso | Descrição |
| --- | --- | --- | --- |
| *Posição (RGB)* | **posição\_de_malha** | **meshPosition** | Recupera uma textura que contenha a posição do vértice. |
| *Espaço Mundial Normal (RGB)* | **mesh\_world\_space\_normal** | **meshNormalWS** | Recupera uma textura que contenha o vértice normal no espaço de mundo. |
| *Tangente do Espaço Mundial (RGB)* | **mesh\_world\_space\_tangent** | **meshTangentWS** | Recupera uma textura que contém a tangente de vértice no espaço de mundo. |
| *Bitangent (RGB) do Espaço Mundial* | **mesh\_world\_space\_bitangent** | **meshBitangentWS** | Recupera uma textura contendo o vértice bi-tangente (bi-normal) no espaço de mundo. |
| *Tamanho do texel (tons de cinza)* | **malha\_texel\_size** | **meshTexelSize** | Recupere uma textura que contenha o tamanho do texel (diferença entre a densidade de pixel e a malha UV). |
| *Máscara UV (Tons de Cinza)* | **malha\_uv\_mask** | **meshUVMask** | Recupere uma textura como uma máscara preta (externa) e branca (interna) das Ilhas UV de malha. |
| *Vizinho UV (RGB)* | **malha\_uv\_vizinho** | **meshUVNeighbor** | Recuperar uma textura com duas informações. O interior das coordenadas UV regulares da Ilha UV Store. O exterior do Ilha UV armazena as coordenadas UV do pixel no outro lado de uma emenda UV. Essa textura pode ser usada para criar efeitos perfeitos. |
