---
helpx_url: "https://helpx.adobe.com/br/substance-3d-painter/technical-support/technical-issues/rendering-issues/some-hdpi-scaling-values-are-not-working.html"
breadcrumb-title: ''
description: Saiba como corrigir problemas de valor de escala HDPI no Substance 3D Painter para suporte adequado à exibição de alta resolução.
helpx_creative_field: ""
helpx_description: Painter > Technical support > Technical Issues > Rendering Issues > Some HDPI scaling values are not working
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Alguns valores de escala HDPI não estão funcionando
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '127'
ht-degree: 0%

---


# Alguns valores de escala HDPI não estão funcionando

No Windows, alguns valores de escala HDPI (usados para dimensionar a interface em monitores com altas resoluções) podem não funcionar corretamente.\
Isto ocorre porque a nossa estrutura de janelas (Qt) não suporta as mesmas. Não podemos corrigi-lo até que ele seja realmente gerenciado pelos provedores da própria estrutura.

Portanto, aqui está o comportamento que você pode encontrar, dependendo de suas configurações:

* 120 DPI (**125%** de escala) - renderizado como 96 DPI (**100%** de escala)
* 144 DPI (**150%** dimensionamento) - renderizado como 192 DPI (**200%** dimensionamento)
* 168 DPI (**175%** de escala) - renderizado como 192 DPI (**200%** de escala)

Para obter mais detalhes, consulte: <https://bugreports.qt.io/browse/QTBUG-55654>
