---
title: Desfocar Inclinação
description: Saiba como usar o filtro Inclinação de desfoque do Substance 3D Painter.
source-git-commit: 644a36a1dde953c1d793821e104049ebb6ec3c19
workflow-type: tm+mt
source-wordcount: '215'
ht-degree: 2%
---

# Desfocar Inclinação

<table>
<tr style="border: 0;">
<td width="33.33%" style="border: 0;" valign="top">

![Ícone de Inclinação de desfoque](./Resources/icon_blur_slope.png "Inclinação de desfoque")

<b>Entrada:</b> efeitos/desfoque, tons de cinza

</td>
<td width="100.00%" style="border: 0;" valign="top">

## Descrição

O filtro Desfoque de Inclinação cria um efeito de mancha ou desbotamento, especialmente perceptível nas bordas de alto contraste entre as cores.

É usado diretamente em uma camada de textura para desfocar materiais completos ou texturas específicas, ou em uma máscara para manchar a máscara. Ela pode criar efeitos, como bordas lascadas ou envelhecidas, vazamento de dirt ou ferrugem manchada.

</td>
</tr>
</table>

## Entradas

| Nome de entrada | Descrição |
| --- | --- |
| <b>Ruído Personalizado:</b> Tons de Cinza | Use uma textura personalizada ou um ponto de ancoragem como ruído personalizado. |

<a name="parameters"></a>

## Parâmetros

| Nome do parâmetro | Descrição |
| --- | --- |
| <b>Semente:</b> | Atribua um valor aleatório para criar uma variação diferente sem alterar as configurações gerais. |
| <b>Intensidade:</b> | Ajuste a intensidade do desfoque. |
| <b>Divisor de Intensidade:</b> | Selecione como a intensidade do desfoque é dividida. |
| <b>Modo de Mesclagem:</b> | Selecione o modo de mesclagem usado pelo desfoque de inclinação. |
| <b>Qualidade:</b> | Ajuste a qualidade do efeito. |

### Parâmetros de Origem

<table>
<tr>
<td><b>Tipo de Origem:</b></td>
<td>Selecione se a origem usa o ruído padrão, a entrada anterior ou um ruído personalizado.</td>
</tr>
<tr>
<td><b>Desfoque:</b></td>
<td>Ajuste a intensidade do desfoque do ruído de origem ou da entrada.</td>
</tr>
<tr>
<td><b>Posição:</b></td>
<td>Ajuste o ponto médio do ruído ou da entrada da origem, semelhante a um controle de brilho.</td>
</tr>
<tr>
<td><b>Contraste:</b></td>
<td>Ajuste o contraste do ruído ou da entrada de origem.</td>
</tr>
<tr>
<td><b>Cobrança de Origem:</b></td>
<td>Ajuste a divisão em blocos gráficos do ruído ou da entrada de origem.</td>
</tr>
</table>
