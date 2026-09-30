---
title: Validação do PBR
description: Saiba como usar o filtro de Validações do PBR do Substance 3D Painter.
source-git-commit: 644a36a1dde953c1d793821e104049ebb6ec3c19
workflow-type: tm+mt
source-wordcount: '117'
ht-degree: 2%
---

# Validação do PBR

<table>
<tr style="border: 0;">
<td width="33.33%" style="border: 0;" valign="top">

![ícone de Validação do PBR](./Resources/icon_pbr_validate.png "Validação do PBR")

<b>Em:</b> efeitos/pbr, metálico, aspereza

</td>
<td width="100.00%" style="border: 0;" valign="top">

## Descrição

O filtro Validação do PBR valida os dados de PBR verificando os valores escuros do albedo e os intervalos de refletância metálica.

É usado em uma camada de preenchimento para verificar se os valores de material permanecem dentro dos intervalos de PBR esperados. As Validações do PBR não devem ser ativadas ao exportar materiais.

</td>
</tr>
</table>

<a name="parameters"></a>

## Parâmetros

| Nome do parâmetro | Descrição |
| --- | --- |
| <b>Modo de Validação:</b> | Selecione se deseja validar o albedo, a refletância metálica ou ambos. |
| <b>Limite de Intervalo Escuro do Albedo:</b> | Selecione o limite mínimo de valor escuro permitido para validação de albedo. |
| <b>Intervalo de Reflexão Metálica:</b> | Selecione o intervalo de refletância usado para validar valores metálicos. |
| <b>Sobrepor Mapa:</b> | Alterna a sobreposição de validação sobre os dados do mapa. |

