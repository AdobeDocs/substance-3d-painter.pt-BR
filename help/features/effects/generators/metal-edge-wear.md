---
title: Edge Wear de metal
description: Saiba como usar o gerador de Edge Wear de Metal da Substance 3D Painter.
source-git-commit: b7770a9497f0db047433aec32c31b57f8dc13ae7
workflow-type: tm+mt
source-wordcount: '541'
ht-degree: 1%

---


# Edge Wear de metal

<table>
  <tr style="border: 0;">
    <td style="border: 0;" valign="top">Máscara de <img src="../../../assets/generators/icon_metal_edge_wear.webp" alt=""/><br><strong>entrada:</strong>, gerador</td>
    <td style="border: 0;" valign="top"><strong>Descrição</strong><br>O gerador de Edge Wear metálico cria a aparência de dano e desgaste nas áreas da malha com maior probabilidade de serem derrubadas ou arranhadas.<br><br>O gerador de Edge Wear Metal gera uma textura monocromática (preto e branco). Como resultado, é útil para gerar máscaras para adicionar detalhes de desgaste de borda a uma camada.<br><br>Mapas normais de posição cozida, curvatura, oclusão ambiente e espaço global são necessários como entradas de imagem. <a href="../../../baking/baking.md">Saiba mais sobre como assar aqui</a>.</td>
  </tr>
</table>

## Entradas

| Nome de entrada | Descrição |
| --- | --- |
| Cor **normal do espaço global** | Use o mapa do espaço do mundo normal assado. |
| Cor de **Posição** | Use o mapa de posição cozida. |
| **desgaste personalizado** em tons de cinza | Use uma textura personalizada ou um ponto de ancoragem. |
| **Curvatura** em tons de cinza | Use o mapa de curvatura assado. |
| **Oclusão de ambiente** em tons de cinza | Use o mapa de Oclusão ambiente cozido. |
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
    <td>Inverta a máscara de desgaste de borda de metal.</td>
  </tr>
  <tr>
    <td><strong>Nível de desgaste</strong></td>
    <td>Defina a quantidade total de desgaste.</td>
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
    <td>Ajuste a quantidade de detalhes do desgaste.</td>
  </tr>
  <tr>
    <td><strong>Escala de desgaste</strong></td>
    <td>Ajuste a escala dos detalhes do desgaste.</td>
  </tr>
  <tr>
    <td><strong>Usar Desgaste personalizado</strong></td>
    <td>Ativar ou desativar o uso de um mapa de desgaste personalizado.</td>
  </tr>
  <tr>
    <td><strong>Smoothness de bordas</strong></td>
    <td>Ajuste o smoothness das bordas gerais.</td>
  </tr>
  <tr>
    <td><strong>Mascaramento de Oclusão ambiente</strong></td>
    <td>Use a oclusão ambiente como máscara para evitar que áreas ocultadas recebam o efeito de intemperismo.</td>
  </tr>
  <tr>
    <td><strong>Espessura da curvatura</strong></td>
    <td>Ajuste o quanto o mapa de curvatura afeta o resultado final. O mapa de curvatura é o que o gerador usa para definir as bordas, portanto, um peso de curvatura muito baixo pode remover todo o desgaste das bordas, deixando apenas o desgaste.</td>
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
    <td>Ajuste a intensidade da Curvatura no <strong>modo Padrão </strong> e no <strong>modo Curvatura Sobel </strong>.</td>
  </tr>
  <tr>
    <td><strong>Intensidade de detalhes do height</strong></td>
    <td>Ajuste a intensidade dos detalhes do Micro Height.</td>
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
