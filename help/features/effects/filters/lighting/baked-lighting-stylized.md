---
title: Iluminação feita bake Estilizada
description: Saiba como usar o filtro estilizado de iluminação Feita bake do Substance 3D Painter.
source-git-commit: 644a36a1dde953c1d793821e104049ebb6ec3c19
workflow-type: tm+mt
source-wordcount: '651'
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
| <b>Ângulo Horizontal:</b> | Ajuste o ângulo horizontal da luz adicional. |
| <b>Ângulo Vertical:</b> | Ajuste o ângulo vertical da luz adicional. |
| <b>Intensidade:</b> | Ajuste a intensidade da luz adicional. |
| <b>Cor:</b> | Ajuste a cor da luz adicional. |
| <b>Ângulo Horizontal:</b> | Ajuste o ângulo horizontal da segunda luz adicional. |
| <b>Ângulo Vertical:</b> | Ajuste o ângulo vertical da segunda luz adicional. |
| <b>Intensidade:</b> | Ajuste a intensidade da segunda luz adicional. |
| <b>Cor:</b> | Ajuste a cor da segunda luz adicional. |

### Material

<table>
<tr>
<td><b>Reflexão dielétrica:</b></td>
<td>Defina a quantidade de refletância dielétrica.</td>
</tr>
<tr>
<td><b>Difusão AO:</b></td>
<td>Controle quanto a oclusão de ambiente afeta os detalhes difusos.</td>
</tr>
<tr>
<td><b>Cavidade da Difusão:</b></td>
<td>Controle quanto as áreas de cavidade influenciam os detalhes difusos.</td>
</tr>
<tr>
<td><b>AO specular:</b></td>
<td>Controle quanto a oclusão de ambiente afeta os detalhes do specular.</td>
</tr>
<tr>
<td><b>Cavidade do specular:</b></td>
<td>Ajuste quanto as áreas de cavidade influenciam os detalhes do specular.</td>
</tr>
<tr>
<td><b>Smoothness da cavidade:</b></td>
<td>Ajuste a suavidade das áreas da cavidade.</td>
</tr>
<tr>
<td><b>Intensidade das bordas:</b></td>
<td>Defina a intensidade dos detalhes da borda.</td>
</tr>
<tr>
<td><b>Smoothness de bordas:</b></td>
<td>Ajuste o smoothness das áreas das bordas.</td>
</tr>
<tr>
<td><b>Tipo de Detalhes Normal:</b></td>
<td>Selecione quais detalhes são usados para os normais: somente malha ou Malha + Height + normal.</td>
</tr>
<tr>
<td><b>Height para intensidade normal:</b></td>
<td>Ajuste a intensidade dos detalhes normais gerados.</td>
</tr>
</table>

### Sol e céu

<table>
<tr>
<td><b>Intensidade do Sol:</b></td>
<td>Controle a força do sol.</td>
</tr>
<tr>
<td><b>Ângulo horizontal do sol:</b></td>
<td>Ajuste o ângulo horizontal do sol.</td>
</tr>
<tr>
<td><b>Ângulo vertical do sol:</b></td>
<td>Ajuste o ângulo vertical do sol.</td>
</tr>
<tr>
<td><b>Cor do Sol:</b></td>
<td>Controle a cor do sol.</td>
</tr>
<tr>
<td><b>Intensidade do céu:</b></td>
<td>Ajuste a força do céu.</td>
</tr>
<tr>
<td><b>Cor do céu:</b></td>
<td>Defina a cor do céu.</td>
</tr>
<tr>
<td><b>Cor do horizonte:</b></td>
<td>Ajuste a cor do horizonte.</td>
</tr>
<tr>
<td><b>Cor do solo:</b></td>
<td>Defina a cor do chão.</td>
</tr>
</table>

### Luz 1

<table>
<tr>
<td><b>Ângulo horizontal:</b></td>
<td>Ajuste o ângulo horizontal da luz adicional.</td>
</tr>
<tr>
<td><b>Ângulo Vertical:</b></td>
<td>Ajuste o ângulo vertical da luz adicional.</td>
</tr>
<tr>
<td><b>Intensidade:</b></td>
<td>Ajuste a intensidade da luz adicional.</td>
</tr>
<tr>
<td><b>Cor:</b></td>
<td>Defina a cor da luz adicional.</td>
</tr>
</table>

### Claro 2

<table>
<tr>
<td><b>Ângulo horizontal:</b></td>
<td>Ajuste o ângulo horizontal da segunda luz adicional.</td>
</tr>
<tr>
<td><b>Ângulo Vertical:</b></td>
<td>Ajuste o ângulo vertical da segunda luz adicional.</td>
</tr>
<tr>
<td><b>Intensidade:</b></td>
<td>Ajuste a intensidade da segunda luz adicional.</td>
</tr>
<tr>
<td><b>Cor:</b></td>
<td>Defina a cor da segunda luz adicional.</td>
</tr>
</table>
