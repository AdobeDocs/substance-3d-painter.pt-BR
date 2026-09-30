---
title: Quantize
description: Saiba como usar o filtro Quantizar do Substance 3D Painter.
source-git-commit: 644a36a1dde953c1d793821e104049ebb6ec3c19
workflow-type: tm+mt
source-wordcount: '220'
ht-degree: 1%
---

# Quantize

<table>
<tr style="border: 0;">
<td width="33.33%" style="border: 0;" valign="top">

![Ícone Quantizar](./Resources/icon_quantize.png "Quantizar")

<b>Em:</b> efeitos/quantizar, cor

</td>
<td width="100.00%" style="border: 0;" valign="top">

## Descrição

O filtro Quantificar reduz uma imagem a um conjunto limitado de cores.

É usado em uma camada de textura para criar regiões de cores mais planas, posterizadas ou estilizadas.

</td>
</tr>
</table>

<a name="parameters"></a>

## Parâmetros

| Nome do parâmetro | Descrição |
| --- | --- |
| <b>Quantidade de cores:</b> | Ajuste o número máximo de cores usadas na imagem quantizada. Esse valor também orienta a paleta extraída, embora a contagem real possa ser menor dependendo do método de quantização. Verifique a saída do Valor de cor da paleta para o número final de cores extraídas. |
| <b>Suavização do Contorno:</b> | Ajuste o raio de suavização aplicado à imagem de entrada para simplificar o resultado quantificado em formas mais sólidas e coesas. Valores mais altos aumentam consideravelmente o tempo de computação. |
| <b>Pontilhamento:</b> | Ajuste a intensidade de pontilhamento usada para recriar gradientes e misturas de cores enquanto ainda usa apenas as cores deixadas após a quantização. Use um valor de Suavização do contorno de 0 para o efeito de pontilhamento esperado. |
| <b>Padrão de Pontilhamento:</b> | Selecione o padrão de pontilhamento usado para recriar degradês e misturas de cores na imagem original. |
| <b>Espaço de cores à distância:</b> | Selecione o espaço de cores usado para comparar e distribuir cores durante a quantificação. Use Lab (Cor) para imagens de cores perceptuais e RGB (Dados) para dados brutos, como mapas normais. |
| <b>Aplicar ao Alpha:</b> | Alterna a quantização do canal alfa da camada. |
| <b>Limite de Alpha:</b> | Ajuste o limite alfa. |

