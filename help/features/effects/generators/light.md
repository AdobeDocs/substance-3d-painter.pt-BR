---
title: Luz
description: Saiba como usar o gerador de luz da Substance 3D Painter.
source-git-commit: b095b9b437f75bbb3a3b85ee84a6850026c3bf98
workflow-type: tm+mt
source-wordcount: '192'
ht-degree: 3%

---


# Luz

<table>
  <tr style="border: 0;">
    <td style="border: 0;" valign="top">Máscara de <img src="../../../assets/generators/icon_light.webp" alt=""/><br><strong>entrada:</strong>, gerador</td>
    <td style="border: 0;" valign="top"><strong>Descrição</strong><br>O gerador de Luz simula uma luz direcional que brilha na sua malha, com base nos mapas de Espaço Mundial Normal e Posição.<br><br>O gerador de Luz pode ser usado em uma camada de preenchimento ou para criar uma máscara. Quando usado em uma camada de preenchimento, o gerador gera os canais de cor, metalidade, aspereza do specular, normal e height, que podem ser usados em várias combinações para criar efeitos diferentes. Recomendamos percorrer as exibições de canal no Visor para entender como cada canal é impactado pelo gerador de luz.<br><br>Mapas normais de posição cozida e espaço global são necessários como entradas de imagem. <a href="../../../baking/baking.md">Saiba mais sobre como assar aqui</a>.</td>
  </tr>
</table>

## Entradas

| Nome de entrada | Descrição |
| --- | --- |
| Cor **Normal Do Espaço Mundial** | Use o mapa World Space Normals assado. |
| Cor de **Posição** | Use o mapa de posição cozida. |

## Parâmetros

| Nome do parâmetro | Descrição |
| --- | --- |
| **Inverter** | Inverta o mapa de cores de saída. |
| **Ângulo Horizontal** | Defina o ângulo horizontal da luz falsa. |
| **Ângulo Vertical** | Defina o ângulo vertical da luz falsa. |
| **Brilho do destaque** | Ajuste a página espelhada inferior da área realçada. |
| **Nível de realce** | Ajuste o contraste do realce. |
| **Atenuação da luz** | Ajuste a queda de luz. |
