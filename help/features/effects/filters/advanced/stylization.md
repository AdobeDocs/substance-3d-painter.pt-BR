---

title: Estilização
description: Saiba como usar o filtro de estilização do Substance 3D Painter.
source-git-commit: 644a36a1dde953c1d793821e104049ebb6ec3c19
workflow-type: tm+mt
source-wordcount: '1055'
ht-degree: 1%
---

# Estilização

<table>
<tr style="border: 0;">
<td width="33.33%" style="border: 0;" valign="top">

![Ícone de estilização](./Resources/icon_stylization.png "Estilização")

<b>Em:</b> efeitos/estilizado, estilização, realista, mão, pintado, pincel

</td>
<td width="100.00%" style="border: 0;" valign="top">

## Descrição

O filtro Estilização dá a um material uma aparência pintada à mão e estilizada.

É usado em uma camada de textura para adicionar traçados de pincel de pintura, variação de smoothness, remapeamento de cores e efeitos de iluminação feita bake.

</td>
</tr>
</table>

## Entradas

| Nome de entrada | Descrição |
| --- | --- |
| <b>Base de Oclusão de ambiente:</b> Cor |  |
| <b>Curvatura:</b> Cor |  |
| <b>Cores de Base Normal:</b> |  |

<a name="parameters"></a>

## Parâmetros

| Nome do parâmetro | Descrição |
| --- | --- |
| <b>Estilização:</b> | Ajuste a intensidade global do filtro. |
| <b>Pinceladas:</b> | Ajuste a intensidade geral do efeito de traçado do pincel. |
| <b>Smoothness:</b> | Ajuste a intensidade geral do efeito smoothness. |
| <b>Colorir:</b> | Ajuste a intensidade geral do efeito de colorização. |
| <b>Gradiente:</b> | Ajuste a intensidade geral do efeito de gradiente. |
| <b>Iluminação Feita bake:</b> | Ajuste a intensidade geral do efeito de iluminação feito bake. |
| <b>Bordas e Cavidades:</b> | Ajuste a intensidade geral do efeito de bordas e cavidades. |

### Traçados de pincel

| Nome do parâmetro | Descrição |
| --- | --- |
| <b>Valor dos traços:</b> | Ajuste a quantidade de traçados de pincel usados pelo filtro. |
| <b>Modo de traçados:</b> | Selecione o tipo de traçado do pincel usado pelo filtro. |
| <b>Seleção de traços:</b> | Selecione as formas de traçado de pincel a serem projetadas ao usar vários traçados. |
| <b>Seleção de traços:</b> | Selecione a forma de traçado de pincel a ser projetada ao usar um único traçado. |
| <b>Escala de traçados:</b> | Ajuste a escala dos traçados do pincel. |
| <b>Tamanho Não Uniforme:</b> | Alterne o dimensionamento não uniforme para os traçados de pincel projetados. |
| <b>Tamanho dos traços:</b> | Ajuste a proporção dos traçados de pincel projetados. |
| <b>Escala de traçados aleatória:</b> | Ajuste a intensidade da variação de escala aleatória aplicada aos traçados de pincel. |
| <b>Os Traços Seguem A Superfície:</b> | Alterne o alinhamento dos traçados do pincel para a orientação da malha. |
| <b>Rotação de traçados:</b> | Ajuste o ângulo de rotação do traçado do pincel. |
| <b>Rotação de traçados aleatória:</b> | Ajuste a quantidade de rotação aleatória aplicada aos traçados de pincel. |
| <b>Dureza da Projeção:</b> | Ajuste a dureza da projeção do carimbo. |
| <b>Limite Normal:</b> | Ajuste o limite normal usado para projeção de traçado. |

### Efeitos de traçados de pincel

| Nome do parâmetro | Descrição |
| --- | --- |
| <b>Personalização de cores:</b> | Alterna o uso de uma cor personalizada nos traçados do pincel. |
| <b>Variação de cor:</b> | Ajuste o quanto os traçados de pincel se mesclam com a cor de base. |
| <b>Opacidade da cor:</b> | Ajuste a opacidade da cor personalizada aplicada aos traçados de pincel. |
| <b>Cor:</b> | Ajuste a cor personalizada aplicada aos traçados de pincel. |
| <b>Cores aleatórias:</b> | Ajuste a variação de cor aleatória aplicada aos traçados de pincel. |
| <b>Aspereza personalizada:</b> | Alterna o uso de um valor de aspereza personalizado nos traçados do pincel. |
| <b>Variação de aspereza:</b> | Ajuste a variação de aspereza nos traçados do pincel. |
| <b>Aspereza:</b> | Ajuste o valor de aspereza dos traçados do pincel. |
| <b>Metálico Personalizado:</b> | Alterna o uso de um valor metálico personalizado nos traçados de pincel. |
| <b>Variação Metálica:</b> | Ajuste a variação metálica nos traçados do pincel. |
| <b>Metálico:</b> | Ajuste o valor metálico dos traçados do pincel. |
| <b>Normal Personalizado:</b> | Alterne as opções adicionais de mapeamento normal para os traçados de pincel. |
| <b>Variação Normal:</b> | Ajuste a intensidade dos traçados com pincel no canal normal. |
| <b>Aleatório Normal:</b> | Ajuste a quantidade de variação normal aleatória aplicada aos traçados de pincel. |
| <b>Modo de Mesclagem (Normal):</b> | Selecione o modo de mesclagem normal usado para os traçados de pincel. |

### Suavização

| Nome do parâmetro | Descrição |
| --- | --- |
| <b>Smoothness de cores:</b> | Ajuste o efeito de suavização Kuwahara aplicado à Cor de base. |
| <b>Smoothness de aspereza:</b> | Ajuste o efeito de suavização Kuwahara aplicado à aspereza. |
| <b>Smoothness metálico:</b> | Ajuste o efeito de suavização Kuwahara aplicado a Metálico. |
| <b>Smoothness DO Height:</b> | Ajuste o efeito de suavização Kuwahara aplicado ao Height. |
| <b>Smoothness Normal:</b> | Ajuste o efeito de suavização Kuwahara aplicado ao Normal. |
| <b>Smoothness DE Oclusão de ambiente:</b> | Ajuste o efeito de suavização Kuwahara aplicado à Oclusão de ambiente. |

### Colorir

| Nome do parâmetro | Descrição |
| --- | --- |
| <b>Opacidade da cor:</b> | Ajuste a opacidade da substituição de cor aplicada à Cor de base. |
| <b>Cor:</b> | Selecione a cor usada para substituir a Cor de base. |
| <b>Variação de Desgaste:</b> | Selecione a forma de padrão usada para variação de cor. |
| <b>Opacidade do Desgaste:</b> | Ajuste a intensidade da variação de cor com base em padrão na Cor de base. |
| <b>Cor do Desgaste:</b> | Ajuste o matiz da variação de cor na Cor de base com base em padrão. |
| <b>Valor de Cobrança:</b> | Ajuste o número de padrões mapeados para a variação de cor. |
| <b>Escala de padrão:</b> | Ajuste a escala dos padrões mapeados para a variação de cor. |

### Gradiente

| Nome do parâmetro | Descrição |
| --- | --- |
| <b>Modo de gradiente:</b> | Selecione se o gradiente usa uma ou duas cores. |
| <b>Cor:</b> | Ajuste a cor do primeiro gradiente. |
| <b>Opacidade da cor:</b> | Ajuste a opacidade da primeira cor de gradiente. |
| <b>Modo de Mesclagem de Cores:</b> | Selecione o modo de mesclagem da primeira cor de gradiente. |
| <b>Cor 2:</b> | Ajuste a cor do segundo gradiente. |
| <b>Opacidade da Cor 2:</b> | Ajuste a opacidade da segunda cor de gradiente. |
| <b>Modo de mesclagem da Cor 2:</b> | Selecione o modo de mesclagem da segunda cor de gradiente. |
| <b>Rotação Horizontal:</b> | Ajuste a rotação horizontal do gradiente. |
| <b>Rotação Vertical:</b> | Ajuste a rotação vertical do gradiente. |
| <b>Inversão de gradiente:</b> | Alterna a inversão da máscara de gradiente. |
| <b>Deslocamento de gradiente:</b> | Ajuste o deslocamento da máscara de gradiente. |
| <b>Contraste de gradiente:</b> | Ajuste o contraste da máscara de gradiente. |

### Iluminação feita bake

| Nome do parâmetro | Descrição |
| --- | --- |
| <b>Traçados De Pincel Na Iluminação:</b> | Ajuste quanta variação do traçado de pincel aparece na iluminação feita bake. |
| <b>Intensidade da Difusão:</b> | Ajuste a intensidade da luz difusa. |
| <b>Cor da Difusão:</b> | Ajuste a cor da luz difusa. |
| <b>Raio da Difusão:</b> | Ajuste o raio da luz difusa. |
| <b>Contraste de Difusões:</b> | Ajuste o contraste da luz difusa. |
| <b>Intensidade de Specular:</b> | Ajuste a intensidade da luz de specular. |
| <b>Cor do Specular:</b> | Ajuste a cor da luz do specular. |
| <b>Raio do Specular:</b> | Ajuste o raio da luz do specular. |
| <b>Contraste de Specular:</b> | Ajuste o contraste da luz do specular. |
| <b>Rotação Horizontal:</b> | Ajuste a rotação horizontal da fonte de luz. |
| <b>Rotação Vertical:</b> | Ajuste a rotação vertical da fonte de luz. |
| <b>Nitidez de cores:</b> | Ajuste a nitidez aplicada à Cor de base. |
| <b>Nitidez da superfície:</b> | Ajuste o efeito de detalhes da superfície com base em malha na Cor de base. |

### Bordas E Cavidades

| Nome do parâmetro | Descrição |
| --- | --- |
| <b>Modo:</b> | Selecione se deseja mapear cavidades, bordas ou ambas na Cor de base. |
| <b>Contraste de bordas e cavidades:</b> | Ajuste o contraste da máscara de bordas e cavidades. |
| <b>Opacidade das Cavidades:</b> | Ajuste a intensidade das cavidades misturadas à Cor de base. |
| <b>Propagação de Cavidades:</b> | Ajuste a propagação das cavidades misturadas à Cor de base. |
| <b>Traçados De Pincel Em Cavidades:</b> | Ajuste quanto os traçados de pincel mascaram a mesclagem das cavidades. |
| <b>Cores de Cavidades Personalizadas:</b> | Alternar o uso de uma cor personalizada nas cavidades. |
| <b>Cor das Cavidades:</b> | Ajuste a cor personalizada mesclada nas cavidades. |
| <b>Opacidade Das Bordas:</b> | Ajuste a intensidade das bordas mescladas na Cor de base. |
| <b>Propagação de bordas:</b> | Ajuste a propagação das bordas mescladas na Cor de base. |
| <b>Traçados De Pincel Nas Bordas:</b> | Ajuste quanto os traçados de pincel mascaram a mesclagem de bordas. |
| <b>Cor de Bordas Personalizadas:</b> | Alternar o uso de uma cor personalizada nas bordas. |
| <b>Cor das Bordas:</b> | Ajuste a cor personalizada mesclada nas bordas. |

#### Assistentes

| Nome do parâmetro | Descrição |
| --- | --- |
| <b>Exibir Auxiliares:</b> | Selecione a máscara auxiliar ou as informações de depuração a serem exibidas no Cor de base. |

