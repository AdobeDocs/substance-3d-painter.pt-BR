---
title: Conversão em tons de cinza
description: Saiba como usar o gerador de conversão em tons de cinza do Substance 3D Painter.
source-git-commit: b7770a9497f0db047433aec32c31b57f8dc13ae7
workflow-type: tm+mt
source-wordcount: '229'
ht-degree: 5%

---


# Conversão em tons de cinza

<table>
  <tr style="border: 0;">
    <td style="border: 0;" valign="top"><img src="../../../assets/generators/icon_grayscale_conversion.png" alt=""/><br><strong>Em:</strong> gerador, tons de cinza, cor</td>
    <td style="border: 0;" valign="top"><strong>Descrição</strong><br>O gerador de Conversão em Tons de Cinza converte uma textura ou um mapa em valores de tons de cinza.<br><br>O gerador de Conversão em Tons de Cinza gera uma textura monocromática (preto e branco). Como resultado, é útil para gerar máscaras a partir de um mapa de entrada de cores completo.</td>
  </tr>
</table>

## Entradas

| Nome de entrada | Descrição |
| --- | --- |
| Cor de **Origem** | Use uma textura de cor personalizada ou um ponto de ancoragem. |

## Parâmetros

<table>
  <tr>
    <th>Nome do parâmetro</th>
    <th>Descrição</th>
  </tr>
  <tr>
    <td><strong>Tipo de tons de cinza</strong></td>
    <td>Defina o método de conversão de tons de cinza: <br><ul><li><strong>Dessaturação</strong>: usa o valor na metade do caminho entre os canais mais fortes e mais fracos do RGB.</li><li><strong>Luma</strong>: usa coeficientes de RGB ponderados que correspondem ao brilho percebido pelo olho humano (favorecendo o verde).</li><li><strong>Média</strong>: mistura os canais vermelho, verde e azul em quantidades iguais.</li><li><strong>Máx</strong>: usa o valor mais alto dos canais de RGB.</li><li><strong>Min</strong>: usa o menor valor dos canais de RGB.<ul><li>Canal vermelho: usa somente o canal vermelho.</li><li>Canal verde: usa somente o canal verde.</li><li>Canal azul: usa somente o canal azul.</li></ul></li></ul></td>
  </tr>
  <tr>
    <td><strong>Inverter</strong></td>
    <td>Inverte a máscara.</td>
  </tr>
  <tr>
    <td><strong>Equilíbrio</strong></td>
    <td>Ajusta o equilíbrio da imagem de origem convertida, deslocando o ponto médio em direção ao preto ou branco, como um controle de brilho.</td>
  </tr>
  <tr>
    <td><strong>Contraste</strong></td>
    <td>Define o contraste/declínio da imagem de origem convertida.</td>
  </tr>
  <tr>
    <td><strong>Lado a lado</strong></td>
    <td>Define a divisão em blocos gráficos da imagem de origem convertida.</td>
  </tr>
  <tr>
    <td><strong>Giro</strong></td>
    <td>Ajusta o ângulo da imagem de origem convertida.</td>
  </tr>
  <tr>
    <td><strong>Rotação segura</strong></td>
    <td>Ativa ou desativa o modo de rotação de segurança. Quando verdadeiro, a Rotação segura bloqueia a rotação em ângulos de 45 graus.</td>
  </tr>
</table>
