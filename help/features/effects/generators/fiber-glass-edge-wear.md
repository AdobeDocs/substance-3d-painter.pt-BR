---
title: Edge Wear de fibra de vidro
description: Saiba como usar o gerador de Edge Wear de fibra de vidro da Substance 3D Painter.
source-git-commit: b7770a9497f0db047433aec32c31b57f8dc13ae7
workflow-type: tm+mt
source-wordcount: '533'
ht-degree: 1%

---


# Edge Wear de fibra de vidro

<table>
  <tr style="border: 0;">
    <td style="border: 0;" valign="top">Máscara de <img src="../../../assets/generators/icon_fiber_glass_edge_wear.webp" alt=""/><br><strong>entrada:</strong>, gerador</td>
    <td style="border: 0;" valign="top"><strong>Descrição</strong><br>O gerador de Edge Wear de fibra de vidro adiciona detalhes realistas de desgaste de borda de fibra de vidro e desgaste com base em mapas de curvatura assada e Oclusão ambiente. Opcionalmente, você também pode usar os mapas Micro Height e Micro Normal para obter detalhes adicionais.<br><br>O gerador de Edge Wear de fibra de vidro gera uma textura monocromática (preto e branco). Como resultado, é útil para gerar máscaras para adicionar detalhes de desgaste de bordas de fibra de vidro a uma camada.<br><br>Mapas normais de posição cozida, curvatura, oclusão ambiente e espaço global são necessários como entradas de imagem. <a href="../../../baking/baking.md">Saiba mais sobre como assar aqui</a>.</td>
  </tr>
</table>

## Entradas

| Nome de entrada | Descrição |
| --- | --- |
| **desgaste personalizado** em tons de cinza | Use uma textura personalizada ou um ponto de ancoragem. |
| **Curvatura** em tons de cinza | Use o mapa de curvatura assado. |
| **Oclusão de ambiente** em tons de cinza | Use o mapa de Oclusão ambiente cozido. |
| Cor **Normal Do Espaço Mundial** | Use o mapa World Space Normals assado. |
| Cor de **Posição** | Use o mapa de posição cozida. |
| Cor **Micro Normal** | Use uma textura normal personalizada ou um ponto de ancoragem. |
| Cor do **Micro Height** | Use uma textura personalizada ou um ponto de ancoragem. |

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
    <td><strong>Nível de desgaste</strong></td>
    <td>Ajuste a quantidade total de desgaste e visibilidade geral do efeito gerador.</td>
  </tr>
  <tr>
    <td><strong>Desgaste de contraste</strong></td>
    <td>Ajuste o contraste do resultado final de desgaste.</td>
  </tr>
  <tr>
    <td><strong>Usar Triplanar</strong></td>
    <td>Quando <strong>Usar Triplanar </strong> está habilitado, a textura é projetada a partir de três direções (eixos X, Y, Z) em vez de depender apenas de UVs. <br><ul><li>Sem o triplanar ativado, a textura segue o layout UV.</li><li>Com o triplanar ativado, a textura é projetada a partir de vários ângulos e mesclada.</li></ul></td>
  </tr>
  <tr>
    <td><strong>Contraste de mesclagem triplanar</strong></td>
    <td>Ajuste a suavidade com que uma textura se mescla quando é projetada usando o mapeamento triplanar. Isso ajusta a suavidade da mesclagem entre as projeções de cada direção.</td>
  </tr>
  <tr>
    <td><strong>Quantidade de desgaste</strong></td>
    <td>Ajuste a intensidade dos detalhes do desgaste.</td>
  </tr>
  <tr>
    <td><strong>Usar Desgaste personalizado</strong></td>
    <td>Ativar ou desativar o uso de um mapa de desgaste personalizado.</td>
  </tr>
  <tr>
    <td><strong>Smoothness de bordas</strong></td>
    <td>Ajuste a suavidade do efeito de desgaste de borda.</td>
  </tr>
  <tr>
    <td><strong>Mascaramento de Oclusão ambiente</strong></td>
    <td>Ajuste quanto o mapa de oclusão ambiente afeta o resultado.</td>
  </tr>
  <tr>
    <td><strong>Espessura da curvatura</strong></td>
    <td>Ajuste o quanto o mapa de curvatura afeta o resultado.</td>
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
    <td>Determina o tipo de curvatura. <br><ul><li><strong>Padrão</strong>: produz um resultado geralmente bastante nítido, mas pode não apresentar detalhes mais amplos.</li><li><strong>Sobel</strong>: produz resultados semelhantes em comparação com o padrão, mas um pouco mais desfocado, pois avalia o mapa normal usando um filtro Sobel.</li><li><strong>Suave</strong>: produz níveis diferentes de desfoque (como mipmaps) para acumular informações. Isso geralmente fornece curvas mais suaves, mas os detalhes podem ser perdidos.</li></ul></td>
  </tr>
  <tr>
    <td><strong>Intensidade de curvatura</strong></td>
    <td>Ajuste a intensidade da Curvatura nos modos de Curvatura padrão e Sobel.</td>
  </tr>
  <tr>
    <td><strong>Intensidade de detalhes do height</strong></td>
    <td>Ajuste a quantidade de detalhes do Micro Height.</td>
  </tr>
  <tr>
    <td><strong>Raio AO</strong></td>
    <td>Ajuste o raio (intervalo) da Oclusão ambiente em microdetalhes.</td>
  </tr>
  <tr>
    <td><strong>PROFUNDIDADE AO</strong></td>
    <td>Ajuste a profundidade (intensidade) da Oclusão ambiente em microdetalhes.</td>
  </tr>
</table>
