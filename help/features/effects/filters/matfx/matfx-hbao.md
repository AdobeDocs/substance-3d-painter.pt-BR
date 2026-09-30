---
title: MatFX HBAO
description: Saiba como usar o filtro MatFX HBAO da Substance 3D Painter.
source-git-commit: 644a36a1dde953c1d793821e104049ebb6ec3c19
workflow-type: tm+mt
source-wordcount: '145'
ht-degree: 2%
---

# MatFX HBAO

<table>
<tr style="border: 0;">
<td width="33.33%" style="border: 0;" valign="top">

![Ícone MatFX HBAO](./Resources/icon_matfx_hbao.png "MatFX HBAO")

<b>Entrada:</b> Efeitos/oclusão de ambiente, height, sombreamento

</td>
<td width="100.00%" style="border: 0;" valign="top">

## Descrição

O filtro MatFX HBAO gera uma oclusão de ambiente baseada em horizonte a partir de informações do height.

É usado em camadas ou máscaras de textura para adicionar sombras de profundidade e contato com base nas informações do canal de origem ou do height.

</td>
</tr>
</table>

<a name="parameters"></a>

## Parâmetros

| Nome do parâmetro | Descrição |
| --- | --- |
| <b>Intensidade de desfoque:</b> | Ajuste a intensidade do desfoque do resultado. |
| <b>Quebra automática de linha:</b> | Alternar quebra automática de desfoque. Quando ativado, o efeito obtém amostras de pixels do lado oposto da textura. |
| <b>Fonte do Canal:</b> | Selecione a origem de canal usada para gerar a oclusão. |
| <b>Usar Unidades Mundiais:</b> | Alternar o uso de unidades de espaço global. |
| <b>Profundidade DE Height:</b> | Ajuste a profundidade percebida da entrada do height. |
| <b>Raio:</b> | Ajuste o raio de amostragem do efeito de oclusão. |
| <b>Intensidade:</b> | Ajuste a força da oclusão. |
| <b>Saldo do Relevo:</b> | Ajuste o saldo da contribuição do relevo. |
