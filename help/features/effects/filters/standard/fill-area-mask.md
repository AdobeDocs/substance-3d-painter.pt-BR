---
title: Máscara de área de preenchimento
description: Saiba como usar o filtro Máscara de área de preenchimento do Substance 3D Painter.
source-git-commit: 644a36a1dde953c1d793821e104049ebb6ec3c19
workflow-type: tm+mt
source-wordcount: '150'
ht-degree: 2%
---

# Máscara de área de preenchimento

<table>
<tr style="border: 0;">
<td width="33.33%" style="border: 0;" valign="top">

![Ícone de Máscara de área de preenchimento](./Resources/icon_fill_area_mask.png "Máscara de área de preenchimento")

<b>Entrada:</b> efeitos/preenchimento, forma, contorno, escala de cinza

</td>
<td width="100.00%" style="border: 0;" valign="top">

## Descrição

O filtro Máscara de área de preenchimento converte contornos em formas preenchidas. Qualquer área com uma borda contínua é preenchida.

É usado em uma camada de máscara (saída em preto e branco) após adicionar uma camada de tinta para preencher traçados pintados fechados.

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
| <b>Limite de Detecção de Borda UV:</b> | Ajuste o limite usado para ignorar áreas UV que, de outra forma, poderiam ser preenchidas pelo processo de detecção de área. |
