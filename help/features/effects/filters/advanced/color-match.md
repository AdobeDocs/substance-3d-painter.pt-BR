---
title: Correspondência de cores
description: Saiba como usar o filtro Correspondência de cores no Substance 3D Painter.
source-git-commit: 644a36a1dde953c1d793821e104049ebb6ec3c19
workflow-type: tm+mt
source-wordcount: '273'
ht-degree: 1%
---

# Correspondência de cores

<table>
  <tr style="border: 0;">
    <td style="border: 0;" valign="top"><img src="./Resources/icon_color_match.png" alt="Ícone Correspondência de cores" title="Correspondência de cores"/><br><strong>Entrada:</strong> efeitos/ajustes</td>
    <td style="border: 0;" valign="top">Descrição<br>O filtro Correspondência de Cores corresponde a um intervalo de cores de origem definido a um intervalo de cores de destino, com suporte para slots de entrada para definir valores de origem e de destino. A Correspondência de cores permite que você mantenha detalhes ao alterar a cor de uma superfície, com controle sobre como a Matiz, a Croma e a Luma são tratadas.<br>A Correspondência de cores é usada em uma camada de preenchimento para fazer ajustes de cores finos.</td>
  </tr>
</table>

## Entradas

| Nome de entrada | Descrição |
| --- | --- |
| **Cor de Origem:** | Slot de entrada para a cor de origem. Use um mapa de cores personalizado ou um ponto de ancoragem. |
| **Cor de Destino:** | Slot de entrada para a cor de destino. Use um mapa de cores personalizado ou um ponto de ancoragem. |

## Parâmetros

<table>
  <tr>
    <th>Nome do parâmetro</th>
    <th>Descrição</th>
  </tr>
  <tr>
    <td><strong>Modo de cores de origem:</strong></td>
    <td>Selecione a origem da cor de origem.<br><ul><li><strong>Média</strong>: use a cor de material existente como cor de origem. Observe que isso requer que o modo de mesclagem de camada seja definido como <strong>Transparência</strong>.</li><li><strong>Parâmetro</strong>: defina a cor de origem usando um parâmetro.</li><li><strong>Entrada</strong>: defina a cor de origem com uma entrada de imagem.</li></ul></td>
  </tr>
  <tr>
    <td><strong>Cor de origem:</strong></td>
    <td>Ajuste a cor de origem quando o <strong>Modo de Cor de Origem</strong> estiver definido como <strong>Parâmetro</strong>.</td>
  </tr>
  <tr>
    <td><strong>Modo de cor de destino:</strong></td>
    <td>Selecione a origem da cor de destino.<br><ul><li><strong>Parâmetro</strong>: defina a cor de destino usando um parâmetro.</li><li><strong>Entrada</strong>: defina a cor de destino com uma entrada de imagem.</li></ul></td>
  </tr>
  <tr>
    <td><strong>Cor de destino:</strong></td>
    <td>Ajuste a cor de destino quando o <strong>Modo de Cor de Destino</strong> estiver definido como <strong>Parâmetro</strong>.</td>
  </tr>
  <tr>
    <td><strong>Variação de cor personalizada:</strong></td>
    <td>Alterne os controles personalizados de matiz, croma e variação de luma.</td>
  </tr>
  <tr>
    <td><strong>Matiz:</strong></td>
    <td>Ajuste a variação de matiz aplicada ao resultado.</td>
  </tr>
  <tr>
    <td><strong>Croma:</strong></td>
    <td>Ajuste a variação de croma aplicada ao resultado.</td>
  </tr>
  <tr>
    <td><strong>Luma:</strong></td>
    <td>Ajuste a variação de luma aplicada ao resultado.</td>
  </tr>
</table>