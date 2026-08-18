---
title: Terra
description: Saiba como usar o gerador de Dirt da Substance 3D Painter.
source-git-commit: b7770a9497f0db047433aec32c31b57f8dc13ae7
workflow-type: tm+mt
source-wordcount: '528'
ht-degree: 1%

---


# Terra

<table>
  <tr style="border: 0;">
    <td style="border: 0;" valign="top">Máscara de <img src="../../../assets/generators/icon_dirt.webp" alt=""/><br><strong>entrada:</strong>, gerador</td>
    <td style="border: 0;" valign="top"><strong>Descrição</strong><br>O gerador de Dirt adiciona um acúmulo realista de dirt e desgaste em fendas, bordas e superfícies planas com base na curvatura, oclusão ambiente. Opcionalmente, você também pode usar os mapas Micro Height e Micro Normal para adicionar mais detalhes.<br><br>O gerador de Dirt gera uma textura monocromática (preto e branco). Como resultado, é útil para gerar máscaras para adicionar detalhes de dirt ou desgaste ao modelo.<br><br>Mapas normais de posição cozida, curvatura, oclusão ambiente e espaço global são necessários como entradas de imagem. <a href="../../../baking/baking.md">Saiba mais sobre como assar aqui</a>.</td>
  </tr>
</table>

>[!NOTE]
>
> O gerador de Dirt é uma ferramenta poderosa para adicionar dirt rapidamente à sua malha. Para obter os melhores resultados, recomendamos o uso de máscaras adicionais para controlar como o dirt é aplicado, sempre considerando o ambiente e o histórico do ativo.

## Entradas

| Nome de entrada | Descrição |
| --- | --- |
| **Curvatura** em tons de cinza | Use o mapa de curvatura assado. |
| **Oclusão de ambiente** em tons de cinza | Use o mapa de Oclusão ambiente cozido. |
| Cor **Normal Do Espaço Mundial** | Use o mapa World Space Normals assado. |
| Cor de **Posição** | Use o mapa de posição cozida. |
| **desgaste personalizado** em tons de cinza | Use uma textura personalizada ou um ponto de ancoragem. |
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
    <td>Inverta a máscara de dirt.</td>
  </tr>
  <tr>
    <td><strong>Nível do dirt</strong></td>
    <td>Ajuste a intensidade do efeito dirt.</td>
  </tr>
  <tr>
    <td><strong>Contraste do dirt</strong></td>
    <td>Ajuste o contraste do efeito dirt.</td>
  </tr>
  <tr>
    <td><strong>Usar Triplanar</strong></td>
    <td>Quando o Triplanar está ativado, a textura é projetada a partir de três direções (eixos X, Y, Z) em vez de depender apenas de UVs. <br><ul><li>Sem o triplanar ativado, a textura segue o layout UV.</li><li>Com o triplanar ativado, a textura é projetada a partir de vários ângulos e mesclada.</li></ul></td>
  </tr>
  <tr>
    <td><strong>Contraste de mesclagem triplanar</strong></td>
    <td>Ajuste a suavidade com que uma textura se mescla quando é projetada usando o mapeamento triplanar. Ela ajusta a suavidade da mesclagem entre as projeções de cada direção.</td>
  </tr>
  <tr>
    <td><strong>Quantidade de desgaste</strong></td>
    <td>Ajuste a intensidade dos detalhes do desgaste.</td>
  </tr>
  <tr>
    <td><strong>Escala de desgaste</strong></td>
    <td>Ajuste o tamanho dos detalhes do desgaste.</td>
  </tr>
  <tr>
    <td><strong>Usar Desgaste personalizado</strong></td>
    <td>Ativar ou desativar o uso de um mapa de desgaste personalizado.</td>
  </tr>
  <tr>
    <td><strong>Mascaramento de bordas</strong></td>
    <td>Ajuste o mascaramento das bordas com base no mapa de curvatura.</td>
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
