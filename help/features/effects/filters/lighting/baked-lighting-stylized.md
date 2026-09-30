---
title: Iluminação feita bake Estilizada
description: Saiba como usar o filtro estilizado de iluminação Feita bake do Substance 3D Painter.
source-git-commit: 5078774d081555f586a50965b91d85f7c340ef13
workflow-type: tm+mt
source-wordcount: '662'
ht-degree: 1%
---

# Iluminação feita bake Estilizada

<table>
<tr style="border: 0;">
<td width="33.33%" style="border: 0;" valign="top">

![Ícone de Iluminação Estilizada Feita bake](./Resources/icon_baked_lighting_stylized.png "Iluminação Estilizada Feita bake")

<b>Em:</b> efeitos/estilizados, luz, cor

</td>
<td width="100.00%" style="border: 0;" valign="top">

## Descrição

O filtro Estilizado de Iluminação Feito bake faz bake material e informações de iluminação no canal de cor.

É usado em uma camada de tinta definida para o modo de passagem e aplicado a todos os canais. É útil para fluxos de trabalho estilizados em que não é necessária iluminação simulada precisa ou quando os recursos são limitados, como em projetos para dispositivos móveis ou ativos que dependem apenas de um mapa de cores.

</td>
</tr>
</table>

## Entradas

| Nome de entrada | Descrição |
| --- | --- |
| <b>Oclusão de ambiente:</b> tons de cinza | Use o mapa de Oclusão de ambiente feito bake. |
| <b>Curvatura:</b> tons de cinza | Use o mapa de curvatura feita bake. |
| <b>Normal:</b> Cor | Use o Mapa normal feito bake. |
| <b>Normais do Espaço Mundial:</b> Cor | Use o mapa do World Space Normals feito bake. |

<a name="parameters"></a>

## Parâmetros

| Nome do parâmetro | Descrição |
| --- | --- |
| <b>Entrada:</b> | Selecione o fluxo de trabalho de material de entrada. |
| <b>Saída:</b> | Selecione o modo de saída. |
| <b>Reflexão Dielétrica:</b> | Ajuste a refletância dielétrica. |
| <b>Difusão AO:</b> | Ajuste a contribuição da oclusão de ambiente para a iluminação difusa. |
| <b>Cavidade da Difusão:</b> | Ajuste a contribuição da cavidade para a iluminação difusa. |
| <b>AO de Specular:</b> | Ajuste a contribuição de oclusão de ambiente para a iluminação do specular. |
| <b>Cavidade do Specular:</b> | Ajuste a contribuição da cavidade para a iluminação do specular. |
| <b>Smoothness de cavidade:</b> | Ajuste o smoothness do efeito de cavidade. |
| <b>Intensidade das bordas:</b> | Ajuste a intensidade do efeito de borda. |
| <b>Smoothness de bordas:</b> | Ajuste o smoothness do efeito de borda. |
| <b>Tipo de Detalhes Normais:</b> | Selecione quais detalhes normais são usados. |
| <b>Height para Intensidade Normal:</b> | Ajuste a intensidade da conversão de height em normal. |
| <b>Intensidade do Sol:</b> | Ajuste a intensidade da luz solar. |
| <b>Ângulo Horizontal Do Sol:</b> | Ajuste o ângulo horizontal da luz do sol. |
| <b>Ângulo Vertical Do Sol:</b> | Ajuste o ângulo vertical da luz do sol. |
| <b>Cor do Sol:</b> | Ajuste a cor da luz do sol. |
| <b>Intensidade do céu:</b> | Ajuste a intensidade da luz do céu. |
| <b>Cor do céu:</b> | Ajuste a cor da luz do céu. |
| <b>Cor horizontal:</b> | Ajuste a cor da luz do horizonte. |
| <b>Cor do solo:</b> | Ajuste a cor da luz do solo. |
| <b>Ângulo Horizontal:</b> | Ajuste a intensidade da luz adicional. |
| <b>Ângulo Vertical:</b> | Ajuste o ângulo vertical da luz adicional. |
| <b>Intensidade:</b> | Ajuste a intensidade da luz adicional. |
| <b>Cor:</b> | Ajuste a cor da luz adicional. |
| <b>Ângulo Horizontal:</b> | Ajuste o ângulo horizontal da segunda luz adicional. |
| <b>Ângulo Vertical:</b> | Ajuste o ângulo vertical da segunda luz adicional. |
| <b>Intensidade:</b> | Ajuste a intensidade da segunda luz adicional. |
| <b>Cor:</b> | Ajuste a cor da segunda luz adicional. |

### Material

| Nome do parâmetro | Descrição |
| --- | --- |
| **Reflexão Dielétrica:** | Defina a quantidade de refletância dielétrica. |
| **Difusão AO:** | Controle quanto a oclusão de ambiente afeta os detalhes difusos. |
| **Cavidade da Difusão:** | Controle quanto as áreas de cavidade influenciam os detalhes difusos. |
| **AO de Specular:** | Controle quanto a oclusão de ambiente afeta os detalhes do specular. |
| **Cavidade do Specular:** | Ajuste quanto as áreas de cavidade influenciam os detalhes do specular. |
| **Smoothness de cavidade:** | Ajuste a suavidade das áreas da cavidade. |
| **Intensidade das bordas:** | Defina a intensidade dos detalhes da borda. |
| **Smoothness de bordas:** | Ajuste o smoothness das áreas das bordas. |
| **Tipo de Detalhes Normais:** | Selecione quais detalhes são usados para os normais: somente malha ou Malha + Height + normal. |
| **Height para Intensidade Normal:** | Ajuste a intensidade dos detalhes normais gerados. |

### Sol e céu

| Nome do parâmetro | Descrição |
| --- | --- |
| **Intensidade do Sol:** | Controle a força do sol. |
| **Ângulo Horizontal Do Sol:** | Ajuste o ângulo horizontal do sol. |
| **Ângulo Vertical Do Sol:** | Ajuste o ângulo vertical do sol. |
| **Cor do Sol:** | Controle a cor do sol. |
| **Intensidade do céu:** | Ajuste a força do céu. |
| **Cor do céu:** | Defina a cor do céu. |
| **Cor horizontal:** | Ajuste a cor do horizonte. |
| **Cor do solo:** | Defina a cor do chão. |

### Luz 1

| Nome do parâmetro | Descrição |
| --- | --- |
| **Ângulo Horizontal:** | Ajuste o ângulo horizontal da luz adicional. |
| **Ângulo Vertical:** | Ajuste o ângulo vertical da luz adicional. |
| **Intensidade:** | Ajuste a intensidade da luz adicional. |
| **Cor:** | Defina a cor da luz adicional. |

### Claro 2

| Nome do parâmetro | Descrição |
| --- | --- |
| **Ângulo Horizontal:** | Ajuste o ângulo horizontal da segunda luz adicional. |
| **Ângulo Vertical:** | Ajuste o ângulo vertical da segunda luz adicional. |
| **Intensidade:** | Ajuste a intensidade da segunda luz adicional. |
| **Cor:** | Defina a cor da segunda luz adicional. |
