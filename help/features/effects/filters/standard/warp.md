---
title: Distorcer
description: Saiba como usar o filtro Distorção do Substance 3D Painter.
source-git-commit: 644a36a1dde953c1d793821e104049ebb6ec3c19
workflow-type: tm+mt
source-wordcount: '261'
ht-degree: 2%
---

# Distorcer

<table>
<tr style="border: 0;">
<td width="33.33%" style="border: 0;" valign="top">

![Ícone de distorção](./Resources/icon_warp.png "Distorcer")

<b>Entrada:</b> efeitos/tons de cinza

</td>
<td width="100.00%" style="border: 0;" valign="top">

## Descrição

O filtro Distorção é usado para vários efeitos de deformação. O filtro Distorção fornece acesso à distorção regular, a uma distorção direcional que distorce em uma direção específica e a uma distorção multidirecional para mais variação.

A distorção é usada em uma camada de textura ou dentro de uma máscara (saída em preto e branco) para deformar materiais, formas, máscaras, contornos etc.

</td>
</tr>
</table>

## Entradas

| Nome de entrada | Descrição |
| --- | --- |
| <b>Ruído Personalizado</b> | Use uma textura personalizada como mapa de entrada de ruído. |

<a name="parameters"></a>

## Parâmetros

| Nome do parâmetro | Descrição |
| --- | --- |
| <b>Semente:</b> | Atribua um valor aleatório para criar uma variação diferente sem alterar as configurações gerais. |
| <b>Modo de distorção:</b> | Selecione o modo de distorção. |
| <b>Intensidade:</b> | Ajuste a intensidade da distorção. |
| <b>Divisor de Intensidade:</b> | Selecione como a intensidade de distorção é dividida. |
| <b>Ângulo:</b> | Ajuste o ângulo de distorção. |
| <b>Modo de Mesclagem:</b> | Selecione o modo de mesclagem usado pela distorção. |
| <b>Direções:</b> | Selecione o número de direções de distorção. |

### Parâmetros de Origem

<table>
<tr>
<td><b>Modo de Origem:</b></td>
<td>Determina o modo de origem.<br><br> - Ruído Padrão: usa o ruído padrão para o efeito de distorção.<br> - Entrada anterior: usa a entrada anterior para o efeito de distorção. Quando uma camada de preenchimento tem um padrão de ruído específico aplicado, o uso de um efeito de distorção no modo “Entrada anterior” fará com que o efeito use o mesmo padrão de ruído que a camada de preenchimento.<br> - Ruído personalizado: usa a entrada de ruído personalizado para o efeito de distorção.</td>
</tr>
<tr>
<td><b>Desfoque da origem:</b></td>
<td>Desfoca o ruído de origem.</td>
</tr>
<tr>
<td><b>Saldo de Origem:</b></td>
<td>Ajusta o equilíbrio do ruído de origem, deslocando o ponto médio em direção ao preto ou branco, como um controle de brilho.</td>
</tr>
<tr>
<td><b>Contraste da origem:</b></td>
<td>Ajusta o contraste do ruído de origem.</td>
</tr>
<tr>
<td><b>Cobrança de Origem:</b></td>
<td>Controla a divisão em blocos gráficos do ruído de origem.</td>
</tr>
</table>
