---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/painting/tool-list/polygon-fill.html"
breadcrumb-title: ''
description: Use a ferramenta Preenchimento de polígono no Substance 3D Painter para preencher polígonos selecionados com pintura, proporcionando uma textura eficiente.
helpx_creative_field: ""
helpx_description: Painter > Painting > Tool list > Polygon fill
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Preenchimento de polígono
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '251'
ht-degree: 1%

---


# Preenchimento de polígono

A ferramenta **Preenchimento de Polígono** (![](../../assets/image2018-6-12-18-15-12.png)) permite desenhar máscaras rapidamente, transformando polígonos selecionados em uma máscara de pixel. Pode parecer uma ferramenta de seleção 3D de outros aplicativos 3DCC, mas na verdade é uma ferramenta de preenchimento de pintura que resulta em dados de pixels. Isso significa selecionar e cancelar a seleção de trabalhos usando-a para pintar de branco ou preto.

A ferramenta de preenchimento de polígono funciona em [Camadas de pintura](../../interface/layer-stack/layer-stack.md), mas está limitada apenas a basecolor e não se destina a essa finalidade. [Use-o somente para máscaras](../../interface/layer-stack/masking-and-effects.md).

Ele tem 4 modos de seleção:

* ![](../../assets/image2020-9-30-11-31-53.png) **Preenchimento triangular** - preenche triplas de malha individuais.
* ![](../../assets/image2020-9-30-11-32-12.png) **Preenchimento de Polígono** - preenche polígonos inteiros. Não faz nada diferente do Preenchimento triangular se a malha já estiver triangulada na exportação.
* **![](../../assets/image2020-9-30-11-32-42.png)Preenchimento de Malha** - preenche todas as sub-malhas conectadas. Como o modo de “subobjeto” em aplicativos 3D, preencherá cada polígono conectado ao que foi clicado.
* **![](../../assets/image2020-9-30-11-32-54.png)Preenchimento de parte UV** - preenche todo o bloco UV ou “ilha”. Funciona como preenchimento de malha, mas observando polígonos conectados no espaço UV. O preenchimento pára nas bordas UV.

![](../../assets/polygon-fill.gif)

Esses 4 modos podem ser combinados e alternados, o que significa que algum uso inteligente permite marcar e desmarcar rapidamente seções em uma máscara usando o modo de Malha e parte UV.

As teclas de atalho (padrão) associadas à ferramenta Preenchimento de polígono são:

* *Chave numérica 4* - seleciona a ferramenta Preenchimento de Polígono.
* *X* - Inverte a cor atual ao pintar máscaras. Trocará rapidamente preto por branco. No modo de pintura de material, essa tecla de atalho não tem efeito.
