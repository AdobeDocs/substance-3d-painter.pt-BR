---
title: Grampo
description: Saiba como usar o filtro de Restrinjo do Substance 3D Painter.
source-git-commit: 644a36a1dde953c1d793821e104049ebb6ec3c19
workflow-type: tm+mt
source-wordcount: '170'
ht-degree: 2%
---

# Grampo

<table>
<tr style="border: 0;">
<td width="33.33%" style="border: 0;" valign="top">

![Ícone de Restrinjo](./Resources/icon_clamp.png "Restrinjo")

<b>Entrada:</b> efeitos/ajustes

</td>
<td width="100.00%" style="border: 0;" valign="top">

## Descrição

O filtro Restringido fixa os valores nos limites definidos.

É usado diretamente em uma camada de preenchimento para limitar aspectos específicos de um material ou em uma máscara para restringir valores a um intervalo específico.

</td>
</tr>
</table>

>[!NOTE]
>
> Quando usado em uma camada de preenchimento ou como uma passagem para informações de cores, o grampo afeta cada canal de cor individualmente. Assim, se um determinado pixel tiver uma cor de (R 0, G 0,5, B 1,0), e estiver preso a 0,5, a cor resultante desse pixel será (R 0, G 0,5, B 0,5). Isso ocorre porque o canal Azul tinha um valor alto o suficiente para ser bloqueado, mas os outros canais não. Isso significa que o filtro Restrinjo pode alterar o matiz do conteúdo colorido.
>
>Se você não deseja modificar o matiz, outros filtros, como Níveis, podem ser a melhor opção.

<a name="parameters"></a>

## Parâmetros

| Nome do parâmetro | Descrição |
| --- | --- |
| <b>Mín:</b> | Ajuste o valor mínimo. |
| <b>Máx:</b> | Ajuste o valor máximo. |
