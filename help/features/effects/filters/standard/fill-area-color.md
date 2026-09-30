---
title: Cor da área de preenchimento
description: Saiba como usar o filtro Cor da área de preenchimento do Substance 3D Painter.
source-git-commit: 644a36a1dde953c1d793821e104049ebb6ec3c19
workflow-type: tm+mt
source-wordcount: '212'
ht-degree: 1%
---

# Cor da área de preenchimento

<table>
<tr style="border: 0;">
<td width="33.33%" style="border: 0;" valign="top">

![Ícone de Cor da Área de Preenchimento](./Resources/icon_fill_area_color.png "Cor da Área de Preenchimento")

<b>Em:</b> efeitos/preenchimento, forma, contorno, rgba, cor

</td>
<td width="100.00%" style="border: 0;" valign="top">

## Descrição

O filtro Cor da área de preenchimento converte contornos em formas preenchidas. Qualquer área com uma borda contínua é preenchida. A versão de cores usa alfa para determinar as bordas da área.

É usado em uma camada de tinta (canal de cor) para preencher traçados pintados fechados.

</td>
</tr>
</table>

<a name="parameters"></a>

## Parâmetros

| Nome do parâmetro | Descrição |
| --- | --- |
| <b>Detecção de Área:</b> | Selecione como a área a ser preenchida é identificada. |
| <b>Limite de Detecção de Área:</b> | Ajuste o limite de detecção de área. |
| <b>Detecção de Área de Depuração:</b> | Alterna para a exibição do contorno detectado pela configuração de Detecção de área. Isso pode ajudar a identificar áreas que podem não estar totalmente fechadas. |
| <b>Comportamento de Borda UV:</b> | Selecione como as bordas UV são tratadas durante o preenchimento de área. |
| <b>Limite de Borda UV:</b> | Ajuste o limite usado para ignorar áreas UV que, de outra forma, poderiam ser preenchidas pelo processo de detecção de área. |
| <b>Modo de cores:</b> | Selecione o método usado para preencher o interior da área. |
| <b>Cor de Preenchimento:</b> | Ajuste a cor de preenchimento. |
| <b>Intensidade de desfoque:</b> | Ajuste a intensidade do desfoque. |
| <b>Amostras de desfoque:</b> | Ajuste o número de amostras de desfoque. |
| <b>Iterações de Difusão:</b> | Ajuste o número de iterações de difusão a serem executadas. Valores mais altos melhoram o resultado, mas são mais lentos. Os valores úteis estão no intervalo [8, 48]. |
