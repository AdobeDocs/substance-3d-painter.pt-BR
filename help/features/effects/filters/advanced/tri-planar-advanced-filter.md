---
title: Avançado Tri-Planar
description: Saiba como usar o filtro avançado Tri-Planar do Substance 3D Painter.
source-git-commit: 644a36a1dde953c1d793821e104049ebb6ec3c19
workflow-type: tm+mt
source-wordcount: '544'
ht-degree: 0%
---

# Avançado Tri-Planar

<table>
<tr style="border: 0;">
<td width="33.33%" style="border: 0;" valign="top">

![Ícone Avançado Triplo-Planar](./Resources/icon_tri_planar_advanced_filter.png "Avançado Triplo-Planar")

<b>Entrada:</b> efeitos/projeção

</td>
<td width="100.00%" style="border: 0;" valign="top">

## Descrição

O filtro Avançado Tri-Planar é a versão de filtro do gerador Avançado Tri-Planar, com controles manuais para a projeção completa. Ele permite controlar os valores de rotação e de deslocamento de cada eixo. Ao contrário do gerador, esse filtro funciona diretamente no conteúdo da camada, enquanto o gerador requer uma entrada de máscara personalizada para mesclagem.

É usado em uma camada de textura ou dentro de uma máscara para adicionar uma mesclagem tripla planar.

</td>
</tr>
</table>

## Entradas

| Nome de entrada | Descrição |
| --- | --- |
| <b>Espaço Mundial Normal:</b> | Use o mapa do Espaço Mundial feito bake - Normal. |
| <b>Posição:</b> | Use o mapa de Posição feita bake. |

<a name="parameters"></a>

## Parâmetros

| Nome do parâmetro | Descrição |
| --- | --- |
| <b>Projeção:</b> | Selecione os eixos pelos quais projetar. |
| <b>Modo de Mesclagem:</b> | Selecione como as projeções de eixo se mesclam. |
| <b>Contraste de Mesclagem:</b> | Ajuste o contraste da mesclagem de projeção. |
| <b>Divisão em blocos gráficos da Textura:</b> | Ajuste a divisão em blocos gráficos da textura projetada. |
| <b>Rotação X:</b> | Ajuste a rotação da projeção do eixo X. |
| <b>Deslocamento X:</b> | Ajuste o deslocamento da projeção do eixo X. |
| <b>Rotação Y:</b> | Ajuste a rotação da projeção do eixo Y. |
| <b>Deslocamento Y:</b> | Ajuste o deslocamento da projeção do eixo Y. |
| <b>Rotação Z:</b> | Ajuste a rotação da projeção do eixo Z. |
| <b>Deslocamento Z:</b> | Ajuste o deslocamento da projeção do eixo Z. |

### Eixo X

<table>
<tr>
<td><b>Rotação X:</b></td>
<td>Ajuste a rotação da projeção de textura do eixo X.</td>
</tr>
<tr>
<td><b>Deslocamento X X:</b></td>
<td>Ajuste o deslocamento da projeção do eixo X ao longo do eixo X.</td>
</tr>
<tr>
<td><b>Deslocamento X Y:</b></td>
<td>Ajuste o deslocamento da projeção do eixo X ao longo do eixo Y.</td>
</tr>
</table>

>[!NOTE]
>
> Os parâmetros de deslocamento contêm dois eixos em seu título. O primeiro define o eixo de projeção, e o segundo define o eixo de deslocamento. Portanto, o **Deslocamento X Y** olha especificamente para a projeção no eixo X e desloca essa projeção ao longo das projeções no eixo Y local.
>
>Outra maneira de pensar sobre isso é que o **Deslocamento X X** compensa a projeção X **horizontalmente**, e o **Deslocamento X Y** compensa a projeção X **verticalmente**.

### Eixo Y

<table>
<tr>
<td><b>Rotação X:</b></td>
<td>Ajuste a rotação da projeção de textura do eixo Y.</td>
</tr>
<tr>
<td><b>Deslocamento Y X:</b></td>
<td>Ajuste o deslocamento da projeção do eixo Y ao longo do eixo X.</td>
</tr>
<tr>
<td><b>Deslocamento Y Y:</b></td>
<td>Ajuste o deslocamento da projeção do eixo Y ao longo do eixo Y.</td>
</tr>
</table>

>[!NOTE]
>
> Os parâmetros de deslocamento contêm dois eixos em seu título. O primeiro define o eixo de projeção, e o segundo define o eixo de deslocamento. Portanto, o **Deslocamento Y X** olha especificamente para a projeção no eixo Y e desloca essa projeção ao longo das projeções no eixo X local.
>
>Outra maneira de pensar sobre isso é que o **Deslocamento Y X** compensa a projeção Y **horizontalmente**, e o **Deslocamento Y Y** compensa a projeção Y **verticalmente**.

### Eixo Z

<table>
<tr>
<td><b>Rotação X:</b></td>
<td>Ajuste a rotação da projeção da textura do eixo Z.</td>
</tr>
<tr>
<td><b>Deslocamento Z X:</b></td>
<td>Ajuste o deslocamento da projeção do eixo Z ao longo do eixo X.</td>
</tr>
<tr>
<td><b>Deslocamento Z Y:</b></td>
<td>Ajuste o deslocamento da projeção do eixo Z ao longo do eixo Y.</td>
</tr>
</table>

>[!NOTE]
>
> Os parâmetros de deslocamento contêm dois eixos em seu título. O primeiro define o eixo de projeção, e o segundo define o eixo de deslocamento. Portanto, o **Deslocamento Z Y** olha especificamente para a projeção no eixo Z e desloca essa projeção ao longo das projeções no eixo Y local.
>
>Outra maneira de pensar sobre isso é que o **Deslocamento Z X** compensa a projeção Z **horizontalmente**, e o **Deslocamento Z Y** compensa a projeção Z **verticalmente**.
