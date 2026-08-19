---
title: Ferrugem de gotejamento
description: Saiba como usar o gerador de Ferrugem de gotejamento da Substance 3D Painter.
source-git-commit: b7770a9497f0db047433aec32c31b57f8dc13ae7
workflow-type: tm+mt
source-wordcount: '247'
ht-degree: 2%

---


# Ferrugem de gotejamento

<table>
  <tr style="border: 0;">
    <td style="border: 0;" valign="top"><img src="../../../assets/generators/icon_dripping_rust.webp" alt=""/><br><strong>Em:</strong> gerador, tons de cinza, cor</td>
    <td style="border: 0;" valign="top"><strong>Descrição</strong><br>O gerador de Ferrugem de gotejamento cria faixas de ferrugem que fluem para baixo, simulando a corrosão causada pela gravidade e pelo escoamento de água.<br><br>O gerador de Ferrugem de gotejamento gera uma textura monocromática (preto e branco). Como resultado, é útil para gerar máscaras para criar um efeito de ferrugem de gotejamento.<br><br>A posição cozida, a curvatura e a oclusão ambiente são necessárias como entradas de imagem. <a href="../../../baking/baking.md">Saiba mais sobre como assar aqui</a>.</td>
  </tr>
</table>

## Entradas

| Nome de entrada | Descrição |
| --- | --- |
| **Curvatura** em tons de cinza | Use o mapa de curvatura assado. |
| **oclusão de ambiente** em tons de cinza | Use o mapa de Oclusão ambiente cozido. |
| Cor de **Posição** | Use o mapa de posição cozida. |

## Parâmetros

<table>
  <tr>
    <th>Nome do parâmetro</th>
    <th>Descrição</th>
  </tr>
  <tr>
    <td><strong>Semente</strong></td>
    <td>Defina o valor de propagação usado para gerar a textura do dirt. <br><ul><li>Clique em Aleatório para alternar para outra semente aleatória.</li><li>Clique no lápis para ver o valor de semente atual e insira um valor específico, se desejar.</li></ul></td>
  </tr>
  <tr>
    <td><strong>Inverter</strong></td>
    <td>Inverta mapas internos específicos (por exemplo, Curvatura, AO) antes que sejam combinados na máscara final.</td>
  </tr>
  <tr>
    <td><strong>Ferrugem propagação</strong></td>
    <td>Ajuste a expansão do efeito de ferrugem de gotejamento.</td>
  </tr>
  <tr>
    <td><strong>Contraste da ferrugem</strong></td>
    <td>Ajuste o contraste do efeito de ferrugem de gotejamento.</td>
  </tr>
  <tr>
    <td><strong>Espalhando Smoothness</strong></td>
    <td>Ajuste a suavidade de expansão do efeito de ferrugem de gotejamento.</td>
  </tr>
  <tr>
    <td><strong>Intensidade de gotejamento</strong></td>
    <td>Ajuste o comprimento do efeito de ferrugem de gotejamento.</td>
  </tr>
  <tr>
    <td><strong>Smoothness de gotas</strong></td>
    <td>Ajuste a suavidade do efeito de ferrugem de gotejamento.</td>
  </tr>
  <tr>
    <td><strong>Quantidade de amostras de gotas</strong></td>
    <td>Ajuste a qualidade do efeito (mais amostras para melhor qualidade).</td>
  </tr>
  <tr>
    <td><strong>Eixo de posição</strong></td>
    <td>Alterne entre o canal Y-Green, o canal X-Red e o canal B-Blue para alterar a direção do efeito de ferrugem de gotejamento.</td>
  </tr>
</table>
