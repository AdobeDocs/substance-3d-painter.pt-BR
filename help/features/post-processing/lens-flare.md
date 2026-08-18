---
title: Flash de lente
description: ''
helpx_description: "Substance 3D Painter"
helpx_url: "https://helpx.adobe.com/substance-3d-painter/features/post-processing/lens-flare.html"
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '262'
ht-degree: 7%

---


# Reflexo da lente

![](../../assets/v12_post_flare.jpg)

Simula os artefatos ópticos produzidos quando fontes de luz brilhantes interagem com elementos da lente da câmera, criando halos, listras e reflexos de fantasma.

| <b>Parâmetro</b> | <b>Descrição</b> |
| --- | --- |
| <b>Resolução</b> | Define a resolução de renderização interna do efeito reflexo de flash. Valores mais altos produzem listras mais nítidas, mas podem afetar o desempenho. |
| <b>Câmera</b> | Seleciona o modelo de câmera usado para simular o clarão. Os valores possíveis são:<ul data-preserve-html="true"> <li data-preserve-html="true"><b>Lente Panorâmica</b> (distância focal mais curta) </li> <li data-preserve-html="true"><b>Lente telefoto</b> (distância focal mais longa).</li> </ul> |
| <b>Valor</b> | Controla a intensidade geral do efeito de reflexo. O valor pode ir além de 1,0 para aumentar a intensidade. |
| <b>Limite</b> | Determina a luminosidade mínima da imagem necessária para gerar um clarão. Valores mais baixos fazem com que mais áreas produzam clarões, enquanto valores mais altos restringem o efeito a fontes de luz muito brilhantes. |
| <b>Escala de abertura</b> | Dimensiona o tamanho da forma de abertura usada para o cálculo do clarão, afetando o tamanho geral dos elementos do clarão. |
| <b>Espessura do revestimento</b> | Simula o revestimento antirreflexo em elementos de lente. O thickness de revestimento afeta a forma como a luz dispersão e, portanto, altera a cor das clarões. |
| <b>Revestimento IOR</b> | Simula o índice de refração da lente: como a luz passa pelo seu thickness. Valores mais baixos produzem fantasmas mais concentrados. |
| <b>Escala de Oclusão</b> | Define o tamanho da área central afetada. |
| <b>smoothness DE Oclusão</b> | Controla o quão gradualmente o brilho da lente se desvanece. Valores mais altos criam transições mais suaves. |
| <b>Fantasmas exclusivos</b> | Define a variação das formas de clarão. Valores mais altos podem afetar significativamente o desempenho. |
| <b>Escala de posição fantasma</b> | Controla a propagação e o tamanho dos fantasmas do reflexo. |
| <b>Textura da abertura</b> | Define a forma da abertura da lente usada para gerar o padrão de brilho. A textura controla as formas de difração e fantasma. |
