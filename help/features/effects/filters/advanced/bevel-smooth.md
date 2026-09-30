---
title: Suavização de chanfro
description: Saiba como usar o filtro de Suavizações de chanfro do Substance 3D Painter.
source-git-commit: 644a36a1dde953c1d793821e104049ebb6ec3c19
workflow-type: tm+mt
source-wordcount: '180'
ht-degree: 2%
---

# Suavização de chanfro

<table>
<tr style="border: 0;">
<td width="33.33%" style="border: 0;" valign="top">

![ícone de Suavização de chanfro](./Resources/icon_bevel_smooth.png "Suavização de chanfro")

<b>Entrada:</b> efeitos/chanfro, suave, distância, tons de cinza

</td>
<td width="100.00%" style="border: 0;" valign="top">

## Descrição

O filtro Suavização de chanfro desenha um gradiente das bordas de uma máscara para fora, para dentro ou para ambos.

É usado em uma camada de textura ou dentro de uma máscara (saída em preto e branco) para criar um gradiente chanfrado suave a partir das bordas de uma máscara.

</td>
</tr>
</table>

## Entradas

| Nome de entrada | Descrição |
| --- | --- |
| <b>Mapa de distância:</b> tons de cinza | Use uma textura personalizada ou um ponto de ancoragem. |

<a name="parameters"></a>

## Parâmetros

| Nome do parâmetro | Descrição |
| --- | --- |
| <b>Direção:</b> | Selecione o lado da borda da máscara que deve ser dilatado. |
| <b>Distância:</b> | Ajuste a distância de dilatação do bisel. |
| <b>Suavização:</b> | Ajuste a intensidade da suavização aplicada à máscara. |
| <b>Deslocamento da curva:</b> | Ajuste as bordas da máscara para dentro ou para fora. |
| <b>Forma da curva:</b> | Selecione se a inclinação de chanfro usará uma curva comprimida ou arredondada. |
| <b>Limite de Máscara:</b> | Ajuste o valor usado para detectar as bordas da máscara a partir da Entrada. |
| <b>Multiplicador de Mapa de distância:</b> | Ajuste o impacto do Mapa de distância na Distância máxima. |
| <b>Quebra de chanfro:</b> | Se marcada, o chanfro será ladrilhado horizontal e verticalmente. |
