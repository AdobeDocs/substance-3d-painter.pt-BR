---
description: Saiba como usar o gerador de normais do espaço mundial da Substance 3D Painter.
title: Normas globais de espaço
source-git-commit: b7770a9497f0db047433aec32c31b57f8dc13ae7
workflow-type: tm+mt
source-wordcount: '567'
ht-degree: 4%

---


# Normas globais de espaço

<table>
  <tr style="border: 0;">
    <td style="border: 0;" valign="top"><img src="../../../assets/generators/icon_world_space_normals.png" alt=""/><br><strong>Entrada:</strong> máscara, gerador, tons de cinza, mesclagem</td>
    <td style="border: 0;" valign="top"><strong>Descrição</strong><br>O gerador normal de espaço global usa o mapa normal de espaço global cozido para colorir o modelo ou aplicar efeitos com base na direção para a qual cada superfície está voltada no espaço 3D. Por exemplo, de cima para baixo.<br><br>O gerador de World Space Normals gera uma textura monocromática (preto e branco). Como resultado, é útil para gerar máscaras para aplicar vários efeitos como dirt, dust, neve ou ferrugem com base nas direções do rosto.<br><br>Mapas normais de posição cozida e espaço global são necessários como entradas de imagem. <a href="../../../baking/baking.md">Saiba mais sobre como assar aqui</a>.</td>
  </tr>
</table>

## Entradas

| Nome de entrada | Descrição |
| --- | --- |
| Cor de **Textura** | Use uma textura personalizada ou um ponto de ancoragem. |
| **Cores Normais do Espaço Mundial** | Use o mapa World Space Normals assado. |
| Cor do **Gradiente de posição** | Use o mapa de posição cozida. |

## Parâmetros

| Nome do parâmetro | Descrição |
| --- | --- |
| **Inversão global** | Inverta o resultado final depois que todos os efeitos forem combinados. |
| **Desfoque global** | Suavize a máscara final uniformemente depois de combinar todos os efeitos. |
| **Saldo Global** | Altere o equilíbrio da máscara final depois que todos os efeitos forem combinados entre preto ou branco, como um ajuste de brilho. |
| **Contraste global** | Ajuste o contraste da máscara final depois que todos os efeitos forem combinados. |
| **Usar Textura** | Ativar ou desativar o uso de um mapa de textura personalizado. |

### Normal do Espaço Global

| Nome do parâmetro | Descrição |
| --- | --- |
| **Inverter** | Inverta apenas os normais do espaço global. |
| **Desfoque** | Suavize somente os normais de espaço do mundo. |
| **Saldo** | Ajuste o equilíbrio dos normais de espaço apenas, deslocando o ponto médio em direção ao preto ou branco, como um controle de brilho. |
| **Contraste** | Ajuste somente o contraste/declínio das normais de espaço global. |
| **Brilho** | Ajuste apenas a luminosidade dos normais do espaço do mundo. |
| **Da direita para a esquerda** | Ajuste como o efeito é aplicado da esquerda para a direita na malha. |
| **De Cima Para Baixo** | Ajuste como o efeito é aplicado de cima para baixo na Malha. |
| **Da frente para trás** | Ajuste como o efeito é aplicado da frente para trás na malha. |

#### Espaço mundial Normal/Direita para a esquerda

| Nome do parâmetro | Descrição |
| --- | --- |
| **Inverter** | Inverta a direção do gradiente da direita para a esquerda. |
| **Modo de Mesclagem** | Selecione o [modo de mesclagem](../../../interface/layer-stack/blending-modes.md) a ser usado para a camada atual. |

#### Espaço mundial normal/de cima para baixo

| Nome do parâmetro | Descrição |
| --- | --- |
| **Inverter** | Inverta a direção do gradiente de cima para baixo. |
| **Modo de Mesclagem** | Selecione o [modo de mesclagem](../../../interface/layer-stack/blending-modes.md) a ser usado para a camada atual. |

#### Espaço mundial normal/da frente para trás

| Nome do parâmetro | Descrição |
| --- | --- |
| **Inverter** | Inverta a direção do gradiente da frente para trás. |
| **Modo de Mesclagem** | Selecione o [modo de mesclagem](../../../interface/layer-stack/blending-modes.md) a ser usado para a camada atual. |

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
    <td>Inverta somente a textura personalizada.</td>
  </tr>
  <tr>
    <td><strong>Conversão em tons de cinza</strong></td>
    <td>Defina o método usado para converter cores inteiras em tons de cinza. O <a href="grayscale-conversion.md">Gerador de conversão de tons de cinza tem mais informações sobre como cada método funciona</a>.</td>
  </tr>
  <tr>
    <td><strong>Modo de mesclagem</strong></td>
    <td>Ajuste a operação de mesclagem a ser usada. Consulte a página dedicada sobre modos de mesclagem.</td>
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
    <td>Quando o Triplanar está ativado, a textura é projetada a partir de três direções (eixos X, Y, Z) em vez de depender apenas de UVs.<br><ul><li>Sem o triplanar, a textura segue o layout UV.</li><li>Com o triplanar, a textura é projetada a partir de vários ângulos e misturada.</li></ul></td>
  </tr>
  <tr>
    <td><strong>Contraste triplanar</strong></td>
    <td>Ajuste a suavidade com que uma textura se mescla quando é projetada usando o mapeamento triplanar. Isso ajusta a suavidade da mesclagem entre as projeções de cada direção.</td>
  </tr>
</table>
