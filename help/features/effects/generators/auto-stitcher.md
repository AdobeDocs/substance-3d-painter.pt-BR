---
title: Auto Stitcher
description: Saiba mais sobre como usar o gerador de autocolante do Substance 3D Painter.
source-git-commit: b095b9b437f75bbb3a3b85ee84a6850026c3bf98
workflow-type: tm+mt
source-wordcount: '329'
ht-degree: 1%

---


# Auto Stitcher

<table>
  <tr style="border: 0;">
    <td style="border: 0;" valign="top"><img src="../../../assets/generators/icon_auto_stitcher.png" alt=""/><br><strong>Em:</strong> stitch, stitches</td>
    <td style="border: 0;" valign="top"><strong>Descrição</strong><br>O gerador de Autocostura cria automaticamente um efeito de costura ao longo de caminhos gerados proceduralmente. Esses caminhos podem ser gerados com base em emendas UV, Curvatura ou um mapa de entrada personalizado.<br><br>O gerador de Autocostura gera uma textura monocromática (preto e branco). Como resultado, é útil gerar máscaras para aplicar efeitos de costura.<br><br>Para usar o Modo Máscara de Curvatura, é necessário um mapa de curvatura preparada. <a href="../../../baking/baking.md">Saiba mais sobre como assar aqui</a>.</td>
  </tr>
</table>

## Entradas

<table>
  <tr>
    <th>Nome de entrada</th>
    <th>Descrição</th>
  </tr>
  <tr>
    <td><strong>Curvatura</strong> em tons de cinza</td>
    <td>Selecione como gerar os caminhos de costura:<br><ul><li><strong>Máscara UV</strong> gera os caminhos ao longo das emendas UV.</li><li><strong>A curvatura </strong> gera caminhos perto das bordas sólidas.</li><li><strong>A entrada personalizada</strong> permite controlar onde os caminhos são gerados usando um mapa.<br>Ao usar a <strong>Entrada personalizada</strong>, os caminhos são gerados em áreas de alto contraste.</li></ul></td>
  </tr>
  <tr>
    <td><strong>Entrada personalizada</strong> em tons de cinza</td>
    <td>Use uma textura personalizada ou um ponto de ancoragem.</td>
  </tr>
</table>

## Parâmetros

<table>
  <tr>
    <th>Nome do parâmetro</th>
    <th>Descrição</th>
  </tr>
  <tr>
    <td><strong>Modo Máscara</strong></td>
    <td>Selecione o modo Máscara.<br><ul><li>Máscara UV: máscaras baseadas em Ilhas UV.</li><li>Curvatura: máscaras baseadas no mapa de curvatura.</li><li>Entrada personalizada: máscaras com base em uma textura de entrada personalizada.</li></ul></td>
  </tr>
  <tr>
    <td><strong>Smoothness de caminho</strong></td>
    <td>Suavize o caminho onde os pontos são aplicados.</td>
  </tr>
  <tr>
    <td><strong>Posição do caminho</strong></td>
    <td>Desloque a posição do caminho.</td>
  </tr>
  <tr>
    <td><strong>Tamanho da costura</strong></td>
    <td>Ajuste a escala dos pontos.</td>
  </tr>
  <tr>
    <td><strong>Largura da costura</strong></td>
    <td>Ajuste a largura dos pontos.</td>
  </tr>
  <tr>
    <td><strong>Comprimento da costura</strong></td>
    <td>Ajuste o comprimento dos pontos.</td>
  </tr>
  <tr>
    <td><strong>Arredondamento da costura</strong></td>
    <td>Ajuste o arredondamento dos pontos.</td>
  </tr>
  <tr>
    <td><strong>Tremulação</strong></td>
    <td>Ajuste a tremulação na direção do fluxo de pontos.</td>
  </tr>
</table>

## Exemplos

<table>
  <tr>
    <td><img src="../../../assets/generators/examples/auto-stitcher/custom-input2.png" alt=""/></td>
    <td>Este exemplo mostra como a entrada personalizada cria caminhos de junção. <br><ul><li>A cor base em preto e branco mostra as texturas de ruído que estamos usando como uma entrada personalizada para o gerador de autostitcher.</li><li>O gerador de autostitcher está mascarando a camada vermelha, deixando os caminhos costurados vermelhos visíveis.</li><li>Observe que os caminhos com costura vermelha se ajustam a regiões preto ou branco suficientemente grandes da textura de ruído de entrada personalizada. A costura vermelha nunca cruza de branco para preto ou preto para branco.</li></ul><br>A imagem abaixo mostra a configuração de camada simples usada para criar esse exemplo.<br><br><img src="../../../assets/generators/examples/auto-stitcher/custom-input-layer-stack.png" alt=""/></td>
  </tr>
</table>
