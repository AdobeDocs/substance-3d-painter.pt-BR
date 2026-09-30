---
title: Kuwahara anisotrópico
description: Saiba como usar o filtro Kuwahara anisotrópico da Substance 3D Painter.
source-git-commit: 644a36a1dde953c1d793821e104049ebb6ec3c19
workflow-type: tm+mt
source-wordcount: '258'
ht-degree: 1%
---

# Kuwahara anisotrópico

<table>
<tr style="border: 0;">
<td width="33.33%" style="border: 0;" valign="top">

![Ícone Anisotrópico do Kuwahara](./Resources/icon_anisotropic_kuwahara.png "Kuwahara Anisotrópico")

<b>Em:</b> efeitos/tons de cinza, kuwahara, anisotrópico, estilizado

</td>
<td width="100.00%" style="border: 0;" valign="top">

## Descrição

O filtro Kuwahara anisotrópico cria efeitos de estilização de pintura, preservando características direcionais fortes.

É usado em uma camada de textura ou dentro de uma máscara (saída em preto e branco) para criar uma aparência estilizada para materiais completos, ruídos e máscaras.

</td>
</tr>
</table>

## Entradas

| Nome de entrada | Descrição |
| --- | --- |
| <b>Mapa de Raio:</b> Tons de Cinza | Use uma textura personalizada ou um ponto de ancoragem. |
| <b>Entrada personalizada:</b> cor | Use uma textura personalizada ou um ponto de ancoragem. |

<a name="parameters"></a>

## Parâmetros

| Nome do parâmetro | Descrição |
| --- | --- |
| <b>Extrair Direção:</b> | Selecione como o filtro deriva a direção do desfoque. |
| <b>Raio:</b> | Ajuste o raio do desfoque. Valores mais altos produzem um efeito de desfoque mais forte. O valor máximo é 32. |
| <b>Smoothness:</b> | Ajuste a quantidade de cores misturadas na direção calculada. Em 0, as cores são principalmente deslocadas nessa direção com muito pouca mesclagem. |
| <b>Nitidez:</b> | Ajuste o contraste nas áreas desfocadas para que pareçam mais planas e definidas com mais clareza. |
| <b>Smoothness de sensor:</b> | Ajuste a quantidade de desfoque aplicada às direções computadas a partir da imagem e armazenadas na mapa de orientação. Valores mais altos produzem um resultado mais suave quando a imagem contém muitos detalhes de alta frequência. |
| <b>Anisotropia:</b> | Ajuste a intensidade de influência do desfoque no mapa de orientação. O mapa de orientação e seus modificadores ainda afetam o resultado mesmo quando este valor é 0, porque o mapa é usado no kernel do filtro Kuwahara. |
| <b>Ângulo de anisotropia:</b> | Ajuste a rotação aplicada ao mapa de orientação em rotações. Essa rotação é adicionada ao valor da entrada do Mapa de Ângulos de anisotropia. |

