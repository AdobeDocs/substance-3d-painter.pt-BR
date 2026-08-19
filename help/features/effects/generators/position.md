---
title: Posição
description: Saiba como usar o gerador de posição da Substance 3D Painter.
source-git-commit: b7770a9497f0db047433aec32c31b57f8dc13ae7
workflow-type: tm+mt
source-wordcount: '537'
ht-degree: 3%

---


# Posição

<table>
  <tr style="border: 0;">
    <td style="border: 0;" valign="top"><img src="../../../assets/generators/icon_position.webp" alt=""/><br><strong>Entrada:</strong> malha, uv, distância</td>
    <td style="border: 0;" valign="top"><strong>Descrição</strong><br>O gerador de Posição usa os mapas normais de posição cozida e de espaço global para criar uma máscara de gradiente com base na posição do material no espaço 3D (como de cima para baixo ou de lado para lado).<br><br>O gerador de Posição gera uma textura monocromática (preto e branco). Como resultado, é útil para gerar máscaras de gradiente com base na posição do espaço mundial.<br><br>Mapas normais de posição cozida e espaço global são necessários como entradas de imagem. <a href="../../../baking/baking.md">Saiba mais sobre como assar aqui</a>.</td>
  </tr>
</table>

## Entradas

| Nome de entrada | Descrição |
| --- | --- |
| Cor de **Textura** | Use uma textura personalizada ou um ponto de ancoragem. |
| Cor do **Gradiente de posição** | Use o mapa de posição cozida. |
| **Cores Normais do Espaço Mundial** | Use o mapa World Space Normals assado. |

## Parâmetros

| Nome do parâmetro | Descrição |
| --- | --- |
| **Inversão global** | Inverta o resultado final depois que todos os efeitos forem combinados. |
| **Desfoque global** | Desfoque a máscara final de maneira uniforme depois que todos os gradientes forem combinados. |
| **Saldo Global** | Ajuste o equilíbrio da máscara final depois que todos os gradientes forem combinados entre preto ou branco, como um ajuste de brilho. |
| **Contraste global** | Ajuste o contraste da máscara final depois que todos os gradientes forem combinados. |
| **Usar Textura** | Ativar ou desativar o uso de um mapa de textura personalizado. |

### Gradiente de posição

| Nome do parâmetro | Descrição |
| --- | --- |
| **Inverter** | Inverta apenas o gradiente de posição. |
| **Saldo** | Ajuste o equilíbrio apenas do gradiente de posição, deslocando o ponto médio em direção ao preto ou branco, como um controle de brilho. |
| **Contraste** | Ajuste o contraste/declínio apenas do gradiente de posição. |
| **Brilho** | Ajuste apenas a luminosidade do gradiente de posição. |
| **Da direita para a esquerda** | Ajuste como o efeito é aplicado da esquerda para a direita na malha. |
| **De Cima Para Baixo** | Ajuste como o efeito é aplicado de cima para baixo na Malha. |
| **Da frente para trás** | Ajuste como o efeito é aplicado da frente para trás na malha. |

#### Posicionar gradiente/da direita para a esquerda

| Nome do parâmetro | Descrição |
| --- | --- |
| **Inverter** | Inverta a direção do gradiente da direita para a esquerda. |
| **Modo de Mesclagem** | Selecione o [modo de mesclagem](../../../interface/layer-stack/blending-modes.md) a ser usado para o gradiente da direita para a esquerda. |

#### Posicionar Gradiente/De Cima Para Baixo

| Nome do parâmetro | Descrição |
| --- | --- |
| **Inverter** | Inverta a direção do gradiente de cima para baixo. |
| **Modo de Mesclagem** | Selecione o [modo de mesclagem](../../../interface/layer-stack/blending-modes.md) a ser usado para o gradiente de cima para baixo. |

#### Posicionar gradiente/da frente para trás

| Nome do parâmetro | Descrição |
| --- | --- |
| **Inverter** | Inverta a direção do gradiente da frente para trás. |
| **Modo de Mesclagem** | Selecione o [modo de mesclagem](../../../interface/layer-stack/blending-modes.md) a ser usado para o gradiente da frente para trás. |

### Textura

<table>
  <tr>
    <th>Nome do parâmetro</th>
    <th>Descrição</th>
  </tr>
  <tr>
    <td><strong>Opacidade da textura</strong></td>
    <td>Ajuste a visibilidade da textura personalizada.</td>
  </tr>
  <tr>
    <td><strong>Inverter</strong></td>
    <td>Inverta o mapa de textura personalizado.</td>
  </tr>
  <tr>
    <td><strong>Conversão em tons de cinza</strong></td>
    <td>Defina o método usado para converter cores inteiras em tons de cinza. O <a href="grayscale-conversion.md">Gerador de conversão de tons de cinza tem mais informações sobre como cada método funciona</a>.</td>
  </tr>
  <tr>
    <td><strong>Modo de mesclagem</strong></td>
    <td>Selecione o <a href="../../../interface/layer-stack/blending-modes.md">modo de mesclagem</a> a ser usado.</td>
  </tr>
  <tr>
    <td><strong>Dimensionar</strong></td>
    <td>Ajuste o tamanho da textura personalizada.</td>
  </tr>
  <tr>
    <td><strong>Contraste</strong></td>
    <td>Ajuste o contraste/declínio da textura personalizada.</td>
  </tr>
  <tr>
    <td><strong>Brilho</strong></td>
    <td>Ajuste a luminosidade da textura personalizada.</td>
  </tr>
  <tr>
    <td><strong>Triplanar</strong></td>
    <td>Quando <strong>Usar Triplanar </strong> está habilitado, a textura é projetada a partir de três direções (eixos X, Y, Z) em vez de depender apenas de UVs. <br><ul><li>Sem o triplanar ativado, a textura segue o layout UV.</li><li>Com o triplanar ativado, a textura é projetada a partir de vários ângulos e mesclada.</li></ul></td>
  </tr>
  <tr>
    <td><strong>Contraste triplanar</strong></td>
    <td>Ajuste a suavidade com que uma textura se mescla quando é projetada usando o mapeamento triplanar. Isso ajusta a suavidade da mesclagem entre as projeções de cada direção.</td>
  </tr>
</table>
