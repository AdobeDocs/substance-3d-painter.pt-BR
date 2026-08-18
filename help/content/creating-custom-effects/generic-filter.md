---
helpx_url: "https://helpx.adobe.com/br/substance-3d-painter/content/creating-custom-effects/generic-filter.html"
breadcrumb-title: ''
description: Saiba como criar efeitos de filtro genéricos para que o Substance 3D Painter aplique processamento de imagem personalizado e filtros de textura.
helpx_creative_field: ""
helpx_description: Painter > Content > Creating custom effects > Generic filter
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Filtro genérico
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '144'
ht-degree: 0%

---


# Filtro genérico

Um efeito genérico será aplicado em todos os canais de documento, incluindo a opacidade. Um filtro genérico pode ser:

* **tons de cinza**, ele será aplicado a cada componente (R, G, B e A) de cada canal (cor base, metálico, aspereza e assim por diante)
* **colorido**, será aplicado no canal colorido como está ou convertido em tons de cinza internamente para afetar os canais em tons de cinza

O nó de entrada do efeito deve ter o **identificador** ou o **uso** definido como **entrada** e seu nó de saída deve ter **saída**. Observe que filtros baseados em **cores** não podem ser usados na máscara de uma camada; somente filtros de **tons de cinza** serão compatíveis.

>[!NOTE]
>
> É possível usar o **uso** ou o **identificador** em um nó de entrada (o uso tem a prioridade).

Exemplo:

![](../../assets/generic-filter.png)![](../../assets/generic-rgba.png){width="575px"}
