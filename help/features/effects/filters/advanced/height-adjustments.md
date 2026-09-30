---
title: Ajuste de height
description: Saiba como usar o filtro Ajuste de Height do Substance 3D Painter.
source-git-commit: 644a36a1dde953c1d793821e104049ebb6ec3c19
workflow-type: tm+mt
source-wordcount: '159'
ht-degree: 1%
---

# Ajuste de height

<table>
<tr style="border: 0;">
<td width="33.33%" style="border: 0;" valign="top">

![Ícone de Ajuste de Height](./Resources/icon_height_adjust.png "Ajuste de Height")

<b>Entrada:</b> efeitos/ajustes, escala, deslocamento, inversão

</td>
<td width="100.00%" style="border: 0;" valign="top">

## Descrição

O filtro Ajuste de Height inverte, desloca ou multiplica o canal de height por um valor escolhido.

É usado em uma camada de textura ou dentro de uma máscara (saída em preto e branco) para ajustar as informações do height de forma não destrutiva.

</td>
</tr>
</table>

<a name="parameters"></a>

## Parâmetros

| Nome do parâmetro | Descrição |
| --- | --- |
| <b>Inverter:</b> | Alterna a inversão do resultado. |
| <b>Deslocamento:</b> | Ajuste o valor do height adicionando ou subtraindo o valor especificado. |
| <b>Multiplicar:</b> | Multiplique os valores de height por esse valor. Como um multiplicador, isso torna as áreas mais altas mais altas e as áreas mais baixas mais baixas. |

>[!NOTE]
>
> Os parâmetros **Multiplicar** e **Deslocamento** são empilhados com o Deslocamento aplicado primeiro. Se o deslocamento resultar em um valor de height de zero em um determinado ponto, a multiplicação será multiplicada por zero, o que significa que não causará nenhuma alteração nesse ponto. Para multiplicar e depois deslocar os valores multiplicados, você pode adicionar um segundo filtro de Ajuste de Height.
