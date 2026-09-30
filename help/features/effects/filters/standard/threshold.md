---
title: Limiar
description: Saiba como usar o filtro Limite do Substance 3D Painter.
source-git-commit: 644a36a1dde953c1d793821e104049ebb6ec3c19
workflow-type: tm+mt
source-wordcount: '157'
ht-degree: 3%
---

# Limite

<table>
<tr style="border: 0;">
<td width="33.33%" style="border: 0;" valign="top">

![Ícone de limite](./Resources/icon_threshold.png "Limite")

<b>Entrada:</b> efeitos/ajustes

</td>
<td width="100.00%" style="border: 0;" valign="top">

## Descrição

O filtro Limite retorna branco quando os critérios de comparação definidos no parâmetro Modo são atendidos pelo valor do pixel de entrada relativo ao valor Limite. É semelhante à Varredura de histograma, mas com contraste sempre em seu nível máximo, fornecendo uma maneira mais rápida e precisa de obter resultados semelhantes.

É usado diretamente em uma camada de preenchimento ou em uma máscara (saída em preto e branco) para criar rapidamente uma máscara de alto contraste a partir de canais específicos.

</td>
</tr>
</table>

<a name="parameters"></a>

## Parâmetros

| Nome do parâmetro | Descrição |
| --- | --- |
| <b>Limite:</b> | Ajuste o valor de luminância com o qual o valor do pixel de entrada é comparado. |
| <b>Modo:</b> | Selecione o critério de comparação usado em relação ao valor limite: Maior, Maior ou igual, Menor ou Inferior ou igual. |
| <b>_mode:</b> | Selecione o valor do modo interno. |
| <b>_threshold:</b> | Ajuste o valor do limite interno. |
| <b>_threshold_min:</b> | Ajuste o valor do limite mínimo interno. |
| <b>_threshold_max:</b> | Ajuste o valor do limite máximo interno. |
