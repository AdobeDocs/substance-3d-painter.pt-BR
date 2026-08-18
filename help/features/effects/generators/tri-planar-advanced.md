---
title: Tri-Planar Avançado
description: Saiba como usar o gerador avançado triplanar da Substance 3D Painter.
source-git-commit: b7770a9497f0db047433aec32c31b57f8dc13ae7
workflow-type: tm+mt
source-wordcount: '372'
ht-degree: 2%

---


# Tri-Planar Avançado

<table>
  <tr style="border: 0;">
    <td style="border: 0;" valign="top">Máscara de <img src="../../../assets/generators/icon_tri_planar_advanced.png" alt=""/><br><strong>entrada:</strong>, gerador</td>
    <td style="border: 0;" valign="top"><strong>Descrição</strong><br>O gerador Avançado Triplanar é uma versão autônoma do modo de mesclagem triplanar com controles manuais para a projeção completa, incluindo controle sobre todos os valores de rotação e deslocamento para cada eixo separado. Comparado com a projeção de preenchimento nativa, o gerador Tri-Planar Advanced usa normais de espaço-mundo para mesclar os três eixos de projeção, enquanto a implementação nativa depende apenas da geometria de baixo-poli. Isso resulta em mais controle e resultados mais precisos.<br><br>O gerador Avançado Triplanar gera uma textura monocromática (preto e branco). Como resultado, é útil para gerar uma mesclagem triplanar de uma máscara personalizada ou de um ponto de ancoragem para usar como máscara.<br><br>Mapas normais de posição cozida e espaço global são necessários como entradas de imagem. <a href="../../../baking/baking.md">Saiba mais sobre como assar aqui</a>.</td>
  </tr>
</table>

## Entradas

| Nome de entrada | Descrição |
| --- | --- |
| Cor **Normal Do Espaço Mundial** | Use o mapa World Space Normals assado. |
| Cor de **Posição** | Use o mapa de posição cozida. |
| **máscara** em tons de cinza | Use uma textura personalizada ou um ponto de ancoragem. |

## Parâmetros

<table>
  <tr>
    <th>Nome do parâmetro</th>
    <th>Descrição</th>
  </tr>
  <tr>
    <td><strong>Projeção</strong></td>
    <td>Selecione se projetará todos os eixos ou apenas um único eixo.</td>
  </tr>
  <tr>
    <td><strong>Modo de mesclagem</strong></td>
    <td>Selecione o Modo de mesclagem para mesclar entre eixos.<br><ul><li><strong>Linear</strong>: no modo de mesclagem linear, a linha de transição de mesclagem é reta.</li><li><strong>Avançado</strong>: no modo de mesclagem Avançado, os eixos são mesclados com base no valor máximo entre os 3 eixos e o ângulo normal no local especificado.</li></ul></td>
  </tr>
  <tr>
    <td><strong>Contraste de mesclagem</strong></td>
    <td>Ajuste quanto a linha de transição de mesclagem ficará desfocada.</td>
  </tr>
  <tr>
    <td><strong>Textura lado a lado</strong></td>
    <td>Ajuste a divisão em blocos da textura da máscara.</td>
  </tr>
</table>

### Eixo X

| Nome do parâmetro | Descrição |
| --- | --- |
| **Rotação X** | Gire a projeção de textura do Eixo X. |
| **Deslocamento X X** | Mova a projeção da textura do Eixo X para a esquerda ou direita. |
| **Deslocamento X Y** | Mova a projeção de textura do Eixo X para cima ou para baixo. |

### Eixo Y

| Nome do parâmetro | Descrição |
| --- | --- |
| **Rotação X** | Gire a projeção de textura do Eixo Y. |
| **Deslocamento Y X** | Mova a projeção da textura do Eixo Y para a esquerda ou direita. |
| **Deslocamento Y** | Mova a projeção de textura do Eixo Y para cima ou para baixo. |

### Eixo Z

| Nome do parâmetro | Descrição |
| --- | --- |
| **Rotação X** | Gire a projeção de textura do eixo Z. |
| **Deslocamento Z X** | Mova a projeção de textura do Eixo Z para a esquerda ou direita. |
| **Deslocamento Z Y** | Mova a projeção de textura do Eixo Z para cima ou para baixo. |
