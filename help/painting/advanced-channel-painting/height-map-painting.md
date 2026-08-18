---
helpx_url: "https://helpx.adobe.com/br/substance-3d-painter/painting/advanced-channel-painting/height-map-painting.html"
breadcrumb-title: ''
description: Aprenda a pintar mapas de height diretamente no Substance 3D Painter para criar efeitos de elevação de superfície e de deslocamento.
helpx_creative_field: ""
helpx_description: Painter > Painting > Advanced channel painting > Height Map Painting
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Pintura de mapa de heights
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '313'
ht-degree: 0%

---


# Pintura de mapa de heights

## Ideia geral

Trabalhar em um mapa de altura em vez de trabalhar diretamente em um normal oferece várias vantagens, como melhor qualidade, melhor controle, flexibilidade e melhor consistência entre os recursos.

O processo é o seguinte:

* Um mapa normal, assado a partir de uma malha poli alta, é carregado na malha poli baixa.
* Você pintará detalhes adicionais no canal do mapa de altura.
* O Height que você pinta é composto por todas as camadas e convertido em um mapa normal em tempo real e, finalmente, mesclado com o normal da malha de alta poli.

Tudo que você tem que se preocupar é pintar aquele height, todo o resto é feito automaticamente.

### Formato HDR do height

O canal de Height usa um formato de cor **HDR**, que permite pintar valores positivos e negativos sem nunca atingir um limite de brilho, diferentemente dos mapas de height tradicionais, que saturarão entre 0 e 255.

* Ao pintar com um bitmap ou substância em um height, essa origem é remapeada de seu intervalo original [0,255] para um intervalo [-1,1].

Um cinza médio será remapeado para 0. Portanto, valores abaixo de 127 **subtrairão** do mapa de altura, enquanto valores acima de 127 **adicionarão** a ele ao usar o modo de mistura padrão definido para os mapas de height, **Subexposição Linear (Adicionar)**.

* Ao pintar com cor simples, você poderá selecionar valores entre -1 e 1 diretamente.

### Visualização de height

Ao visualizar o mapa de Heights no modo Solo, a visualização padrão mostrará apenas valores positivos, com forte saturação em preto para valores negativos.

A configuração **+/- cor** permite visualizar o intervalo completo usando uma cor diferente para os valores positivos e negativos.

A configuração de **Escala** permite modificar o intervalo visível desse mapa HDR caso você tenha adicionado ou subtraído mais do que o intervalo padrão [-1,1].

<table>
<tr style="border: 0;">
<td style="border: 0;" valign="top">

![](../../assets/height1.png)

</td>
<td style="border: 0;" valign="top">

![](../../assets/height2.png)

</td>
</tr>
</table>
