---
title: Curvatura
description: Saiba como usar o gerador de curvatura do Substance 3D Painter.
source-git-commit: b095b9b437f75bbb3a3b85ee84a6850026c3bf98
workflow-type: tm+mt
source-wordcount: '597'
ht-degree: 4%

---


# Curvatura

<table>
  <tr style="border: 0;">
    <td style="border: 0;" valign="top"><img src="../../../assets/generators/icon_curvature.webp" alt=""/><br><strong>Entrada:</strong> máscara, gerador, tons de cinza, mesclagem</td>
    <td style="border: 0;" valign="top"><strong>Descrição</strong><br>O gerador de curvatura cria uma máscara com base no mapa de curvatura assado com a opção de mesclar uma textura ou microdetalhes na máscara.<br><br>O gerador de curvatura gera uma textura monocromática (preto e branco). Como resultado, é útil para gerar máscaras em vez de aplicá-las diretamente a uma camada.<br><br>Um mapa de posição preparada é necessário como entrada. <a href="../../../baking/baking.md">Saiba mais sobre como assar aqui</a>.</td>
  </tr>
</table>

## Entradas

| Nome de entrada | Descrição |
| --- | --- |
| Cor de **Textura** | Use uma textura personalizada ou um ponto de ancoragem. |
| Cor **Micro Normal** | Use uma textura normal personalizada ou um ponto de ancoragem. |
| Cor do **Micro Height** | Use uma textura personalizada ou um ponto de ancoragem. |
| **Curvatura** em tons de cinza | Use o mapa de curvatura assado. |
| **Cores Normais do Espaço Mundial** | Use o mapa World Space Normals assado. |
| Cor do **Gradiente de posição** | Use o mapa de posição cozida. |

## Parâmetros

| Nome do parâmetro | Descrição |
| --- | --- |
| **Inversão global** | Inverte o resultado final depois que todos os efeitos são combinados. |
| **Desfoque global** | Suaviza uniformemente a máscara final depois que todos os efeitos são combinados. |
| **Saldo Global** | Alterna o equilíbrio da máscara final depois que todos os efeitos são combinados entre preto ou branco, como um ajuste de brilho. |
| **Contraste global** | Ajusta o contraste da máscara final depois que todos os efeitos são combinados. |
| **Usar Textura** | Ativar ou desativar o uso de um mapa de textura personalizado. |
| **Usar Microdetalhes** | Ativar ou desativar o uso do mapa de microdetalhes personalizado. |

### Curvatura

<table>
  <tr>
    <th>Nome do parâmetro</th>
    <th>Descrição</th>
  </tr>
  <tr>
    <td><strong>Inverter</strong></td>
    <td>Inverta o mapa de curvatura gerado.</td>
  </tr>
  <tr>
    <td><strong>Modo</strong></td>
    <td>Defina o modo Curvatura. <br><ul><li><strong>Bordas</strong>: mascara as bordas (áreas convexas)</li><li><strong>Cavidades</strong>: mascara as cavidades (áreas côncavas)</li><li><strong>Duplo</strong>: máscaras em áreas côncavas e convexas.</li><li><strong>Não processado</strong>: máscara de curvatura normal.</li></ul></td>
  </tr>
  <tr>
    <td><strong>Nítida</strong></td>
    <td>Ajuste a intensidade dos detalhes de curvatura nítidos.</td>
  </tr>
  <tr>
    <td><strong>Fina</strong></td>
    <td>Ajuste a força dos detalhes finos de curvatura.</td>
  </tr>
  <tr>
    <td><strong>Suave</strong></td>
    <td>Ajuste a força dos detalhes da curvatura suave.</td>
  </tr>
  <tr>
    <td><strong>Média</strong></td>
    <td>Ajuste a força dos detalhes de curvatura média.</td>
  </tr>
  <tr>
    <td><strong>Grande</strong></td>
    <td>Ajuste a força dos detalhes de curvatura grandes.</td>
  </tr>
  <tr>
    <td><strong>Grande</strong></td>
    <td>Ajuste a força dos detalhes de curvatura grandes.</td>
  </tr>
  <tr>
    <td><strong>Enorme</strong></td>
    <td>Ajuste a força dos detalhes de curvatura enormes.</td>
  </tr>
  <tr>
    <td><strong>Contraste</strong></td>
    <td>Ajuste o contraste/declínio da curvatura.</td>
  </tr>
  <tr>
    <td><strong>Brilho</strong></td>
    <td>Ajuste a luminosidade da Curvatura.</td>
  </tr>
</table>

### Textura

<table>
  <tr>
    <th>Nome do parâmetro</th>
    <th>Descrição</th>
  </tr>
  <tr>
    <td><strong>Opacidade da textura</strong></td>
    <td>Controle a visibilidade da textura personalizada.</td>
  </tr>
  <tr>
    <td><strong>Inverter</strong></td>
    <td>Inverta apenas a textura personalizada.</td>
  </tr>
  <tr>
    <td><strong>Conversão em tons de cinza</strong></td>
    <td>Selecione o método usado para converter da entrada de cores para preto e branco. </td>
  </tr>
  <tr>
    <td><strong>Modo de mesclagem</strong></td>
    <td>Defina o modo de mesclagem para a textura personalizada.</td>
  </tr>
  <tr>
    <td><strong>Dimensionar</strong></td>
    <td>Ajuste o tamanho da textura personalizada.</td>
  </tr>
  <tr>
    <td><strong>Contraste</strong></td>
    <td>Defina o contraste/declínio da textura personalizada.</td>
  </tr>
  <tr>
    <td><strong>Brilho</strong></td>
    <td>Defina a luminosidade da textura personalizada.</td>
  </tr>
  <tr>
    <td><strong>Triplanar</strong></td>
    <td>Quando o Triplanar está ativado, a textura é projetada a partir de três direções (eixos X, Y, Z) em vez de depender apenas de UVs. <br><ul><li>Sem o triplanar ativado, a textura segue o layout UV.</li><li>Com o triplanar ativado, a textura é projetada a partir de vários ângulos e mesclada.</li></ul></td>
  </tr>
  <tr>
    <td><strong>Contraste triplanar</strong></td>
    <td>Ajuste a suavidade com que uma textura se mescla quando é projetada usando o mapeamento triplanar. Isso ajusta a suavidade da mesclagem entre as projeções de cada direção.</td>
  </tr>
</table>

### Microdetalhes

<table>
  <tr>
    <th>Nome do parâmetro</th>
    <th>Descrição</th>
  </tr>
  <tr>
    <td><strong>Micro Height</strong></td>
    <td>Ativar ou desativar o uso de um mapa personalizado de Micro Height.</td>
  </tr>
  <tr>
    <td><strong>Micro normal</strong></td>
    <td>Ativa ou desativa a utilização de um mapa Micro Normal personalizado.</td>
  </tr>
  <tr>
    <td><strong>Tipo de curvatura</strong></td>
    <td>Defina o tipo de Curvatura. <br><ul><li><strong>Padrão</strong>: produz um resultado geralmente bastante nítido, mas pode não apresentar detalhes mais amplos.</li><li><strong>Sobel</strong>: produz resultados semelhantes em comparação com o padrão, mas um pouco mais desfocado, pois avalia o mapa normal usando um filtro Sobel.</li><li><strong>Suave</strong>: produz níveis diferentes de desfoque (como mipmaps) para acumular informações. Isso geralmente fornece curvas mais suaves, mas os detalhes podem ser perdidos.</li></ul></td>
  </tr>
  <tr>
    <td><strong>Intensidade de curvatura</strong></td>
    <td>Ajuste a intensidade da Curvatura nos modos de curvatura <strong>Padrão </strong> e <strong>Sobel </strong>.</td>
  </tr>
  <tr>
    <td><strong>Intensidade de detalhes do height</strong></td>
    <td>Ajuste a intensidade dos detalhes do Micro Height.</td>
  </tr>
</table>
