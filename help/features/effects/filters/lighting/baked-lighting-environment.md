---
title: Ambiente de iluminação baked
description: Saiba como usar o filtro de Ambiente de iluminação baked do Substance 3D Painter.
source-git-commit: 644a36a1dde953c1d793821e104049ebb6ec3c19
workflow-type: tm+mt
source-wordcount: '186'
ht-degree: 2%
---

# Ambiente de iluminação baked

<table>
<tr style="border: 0;">
<td width="33.33%" style="border: 0;" valign="top">

![Ícone de Ambiente de iluminação baked](./Resources/icon_baked_lighting_environment.png "Ambiente de iluminação baked")

<b>Entrada:</b> efeitos/iluminação, faço bake, ambiente, PBR

</td>
<td width="100.00%" style="border: 0;" valign="top">

## Descrição

O filtro Ambiente de iluminação baked faz bake as informações de iluminação do material e do ambiente no canal de cores.

É usado em uma camada de tinta definida para o modo de passagem e aplicado a todos os canais. É útil para fluxos de trabalho estilizados em que não é necessária iluminação simulada precisa ou quando os recursos são limitados, como em projetos para dispositivos móveis ou ativos que dependem apenas de um mapa de cores.

</td>
</tr>
</table>

## Entradas

| Nome de entrada | Descrição |
| --- | --- |
| <b>Oclusão de ambiente:</b> tons de cinza | Use o mapa de Oclusão de ambiente feito bake. |
| <b>Mapa de ambiente:</b> tons de cinza | Usar o mapa de ambiente. |
| <b>Normal:</b> Cor | Use o Mapa normal feito bake. |

<a name="parameters"></a>

## Parâmetros

| Nome do parâmetro | Descrição |
| --- | --- |
| <b>Rotação Horizontal:</b> | Ajuste a rotação horizontal da iluminação ambiente. |
| <b>Rotação Vertical:</b> | Ajuste a rotação vertical da iluminação do ambiente. |
| <b>Exposição:</b> | Ajuste a exposição do resultado feito bake. |
| <b>Intensidade do Height:</b> | Ajuste a intensidade com que as informações de height afetam o resultado. |
| <b>Intensidade de Oclusão de ambiente:</b> | Ajuste a intensidade da oclusão de ambiente no faço bake. |
| <b>Intensidade de Oclusão do Specular:</b> | Ajuste a intensidade da oclusão de specular no faço bake. |
