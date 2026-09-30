---
title: Dinâmica de gradiente
description: Saiba como usar o filtro dinâmico Gradiente do Substance 3D Painter.
source-git-commit: 644a36a1dde953c1d793821e104049ebb6ec3c19
workflow-type: tm+mt
source-wordcount: '117'
ht-degree: 4%
---

# Dinâmica de gradiente

<table>
<tr style="border: 0;">
<td width="33.33%" style="border: 0;" valign="top">

![Ícone de Gradiente dinâmico](./Resources/icon_gradient_dynamic.png "Gradiente dinâmico")

<b>Entrada:</b> efeitos/gradiente, tons de cinza, remapear

</td>
<td width="100.00%" style="border: 0;" valign="top">

## Descrição

O filtro Dinâmico do Gradiente remapeia os valores de tons de cinza de uma imagem para um gradiente definido pelas cores colocadas em pontos específicos ao longo do gradiente.

É usado em uma camada de textura ou dentro de uma máscara (saída em preto e branco) para remapear valores de tons de cinza com um gradiente amostrado de outra imagem.

</td>
</tr>
</table>

## Entradas

| Nome de entrada | Descrição |
| --- | --- |
| <b>Origem do Gradiente:</b> Cor | Use um mapa de cores personalizado ou um ponto de ancoragem. |

<a name="parameters"></a>

## Parâmetros

| Nome do parâmetro | Descrição |
| --- | --- |
| <b>Orientação do Gradiente:</b> | Selecione se a origem do gradiente será amostrada horizontal ou verticalmente. |
| <b>Posição de entrada do gradiente:</b> | Ajuste a posição da amostra de entrada do gradiente. |
