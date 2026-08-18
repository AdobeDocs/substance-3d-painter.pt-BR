---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/features/physical-size.html"
breadcrumb-title: ''
description: Saiba como definir o tamanho físico no Substance 3D Painter para definir dimensões reais para um dimensionamento de textura preciso.
helpx_creative_field: ""
helpx_description: Painter > Features > Physical size
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Tamanho físico
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '180'
ht-degree: 2%

---


# Tamanho físico

![](../assets/banner-physicalsize-2.png)

O tamanho físico é uma propriedade dentro de materiais de Substance que define seu tamanho real. Ele pode ser usado para corresponder com precisão o tamanho e a aparência dos materiais em superfícies 3D. O Painter usa centímetros como a unidade interna padrão.

Para usar tamanho físico, aplique um material que tenha essa propriedade com um valor diferente de 0,0,0 e ative o modo de tamanho físico na camada de preenchimento (ou efeito) em Transformação UV > Escala.

Para obter mais informações, consulte:

* <b>Parâmetros de {Tamanho físico</b> em [Projeções de preenchimento](../painting/fill-projections/fill-projections.md)
* Parâmetros da <b>grade</b> em [configurações do visor](../interface/display-settings/viewport-settings.md)
* <b>Deslocamento baseado no tamanho físico</b> em [Configurações do sombreador](../interface/shader-settings/shader-settings.md)

>[!NOTE]
>
> * A partir do Painter versão 8.3, o tamanho físico está disponível para todos os tipos de projeções.
> * A maioria dos formatos de arquivo de malha especifica a unidade usada durante a criação de malha. Essa unidade será convertida em centímetros automaticamente durante a importação.
> * Alguns formatos, como .obj, não possuem informações de unidade; portanto, quando um projeto é criado usando uma malha .obj, ele será medido em centímetros por padrão sem nenhuma conversão.
