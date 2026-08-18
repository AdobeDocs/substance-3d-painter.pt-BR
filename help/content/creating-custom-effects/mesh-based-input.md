---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/content/creating-custom-effects/mesh-based-input.html"
breadcrumb-title: ''
description: Saiba como usar entradas baseadas em malha em efeitos personalizados do Substance 3D Painter para criar efeitos de textura sensíveis à geometria.
helpx_creative_field: ""
helpx_description: Painter > Content > Creating custom effects > Mesh Based Input
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Entrada baseada em malha
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '228'
ht-degree: 1%

---


# Entrada baseada em malha

A entrada baseada em malha é a textura fornecida pelo mecanismo do Substance 3D Painter extraído da malha dentro do projeto atual. Essas texturas podem ser usadas para criar efeitos avançados com base na topologia de malha.

>[!NOTE]
>
> Essas informações de malha são baseadas na própria topologia e não levam em conta o mapa de malha (texturas assadas).
> 
> A entrada fornecida pelo mecanismo é uma textura de ponto flutuante de 32 bits que será reduzida/fixada ao valor da entrada no gráfico de Substance.

| Informações de malha | Identificador | Uso | Descrição |
| --- | --- | --- | --- |
| *Posição (RGB)* | **posição\_de_malha** | **meshPosition** | Recupera uma textura que contém a posição do vértice. |
| *Espaço Mundial Normal (RGB)* | **mesh\_world\_space\_normal** | **meshNormalWS** | Recupera uma textura que contém o vértice normal no espaço de mundo. |
| *Tangente do Espaço Mundial (RGB)* | **mesh\_world\_space\_tangent** | **meshTangentWS** | Recupere uma textura que contenha a tangente de vértice no espaço global. |
| *Bitangent (RGB) do Espaço Mundial* | **mesh\_world\_space\_bitangent** | **meshBitangentWS** | Recupere uma textura contendo o vértice bi-tangente (bi-normal) no espaço de mundo. |
| *Tamanho do texel (tons de cinza)* | **malha\_texel\_size** | **meshTexelSize** | Recupere uma textura que contenha o tamanho do texel (diferença entre a densidade de pixel e a malha UV). |
| *Máscara UV (Tons de Cinza)* | **malha\_uv\_mask** | **meshUVMask** | Recupere uma textura como uma máscara preta (externa) e branca (interna) das Ilhas UV de malha. |
