---
title: 3D linear gradient
description: Saiba como usar o gerador de 3D linear gradient da Substance 3D Painter.
source-git-commit: b095b9b437f75bbb3a3b85ee84a6850026c3bf98
workflow-type: tm+mt
source-wordcount: '260'
ht-degree: 1%

---


# 3D linear gradient

<table>
  <tr style="border: 0;">
    <td style="border: 0;" valign="top"><img src="../../../assets/generators/icon_3d_linear_gradient.webp" alt=""/><br><strong>Dentro:</strong> gradiente, escala de cinza</td>
    <td style="border: 0;" valign="top"><strong>Descrição</strong><br>O gerador de 3D linear gradient usa o mapa de posições para criar um gradiente entre dois pontos na malha. <br><br>O 3D linear gradient gera uma textura monocromática (preto e branco). Como resultado, é útil para gerar máscaras para colocar um gradiente linear em uma área específica.<br><br>Um mapa de posição cozida é necessário como entrada de imagem. <a href="../../../baking/baking.md">Saiba mais sobre como assar aqui</a>.<br><br>O mapa de Posição atribui uma cor a cada ponto da malha que corresponde à sua posição entre 0 e 1 ao longo dos eixos X, Y e Z. Isso significa que cada ponto na malha tem uma cor única. É possível definir os pontos inicial e final do gradiente linear selecionando a cor do mapa de posições nos locais inicial e final.</td>
  </tr>
</table>

## Entradas

| Nome de entrada | Descrição |
| --- | --- |
| **Posição** | Use o mapa de posição cozida. |

## Parâmetros

| Nome do parâmetro | Descrição |
| --- | --- |
| **Inverter** | Inverta o gradiente linear. |
| **Saldo** | Desloque a posição do ponto médio do gradiente linear. |
| **Contraste** | Ajuste o contraste do gradiente linear. |
| **Início da Posição 3D** | Defina o ponto inicial do gradiente com base nas cores do mapa de posições. Para definir facilmente o ponto inicial, exiba o mapa de posições na tela no visor e use o seletor de cores para escolher o ponto inicial. |
| **Fim da Posição 3D** | Defina o ponto final do gradiente com base nas cores do mapa de posições. Para definir facilmente o ponto final, exiba o mapa de posições na tela no visor e use o seletor de cores para escolher o ponto final. |
