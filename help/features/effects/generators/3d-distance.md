---
title: Distância 3D
description: Saiba como usar o gerador de distância 3D do Substance 3D Painter.
source-git-commit: b095b9b437f75bbb3a3b85ee84a6850026c3bf98
workflow-type: tm+mt
source-wordcount: '222'
ht-degree: 1%

---


# Distância 3D

<table>
  <tr style="border: 0;">
    <td style="border: 0;" valign="top">Máscara de <img src="../../../assets/generators/icon_3d_distance.webp" alt=""/><br><strong>entrada:</strong>, gerador</td>
    <td style="border: 0;" valign="top"><strong>Descrição</strong><br>O gerador de Distância 3D define um ponto no espaço 3D (ponto de origem) e exibe a distância desse ponto com um gradiente monocromático. As áreas na superfície da malha mais próximas ao ponto são mais escuras e as áreas mais distantes são mais claras (por padrão).<br><br>Um mapa de posição cozido é necessário como entrada de imagem. <a href="../../../baking/baking.md">Saiba mais sobre como assar aqui</a>.<br><br>A Distância 3D gera uma textura monocromática (preto e branco). Como resultado, é útil para gerar máscaras que criam um gradiente longe de uma determinada posição.<br><br></td>
  </tr>
</table>

## Entradas

| Nome de entrada | Descrição |
| --- | --- |
| **Posição** | Use o mapa de posição cozida para calcular a distância. |

## Parâmetros

| Nome do parâmetro | Descrição |
| --- | --- |
| **Inverter** | Inverta o gradiente. |
| **Posição X** | Transforme o ponto de origem ao longo do eixo x. |
| **Posição Y** | Transforme o ponto de origem ao longo do eixo y. |
| **Posição Z** | Transforme o ponto de origem ao longo do eixo z. |
| **Raio** | Ajuste o tamanho da queda de distância. |
| **Deslocamento** | Mova as posições inicial e final do gradiente em direção ao ponto de origem ou para longe dele. Afastar-se do ponto de origem (aumentando o deslocamento) resulta em uma área escura maior perto do ponto de origem. Aproximar-se do ponto de origem clareia o gradiente, possivelmente removendo-o totalmente se o **Deslocamento** estiver definido como 0. |
| **Contraste** | Ajuste o contraste do gradiente esférico. |
