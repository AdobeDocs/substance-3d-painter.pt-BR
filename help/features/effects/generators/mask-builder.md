---
title: Construtor de máscaras
description: Saiba como usar o gerador de Construtor de máscaras do Substance 3D Painter.
source-git-commit: b7770a9497f0db047433aec32c31b57f8dc13ae7
workflow-type: tm+mt
source-wordcount: '1146'
ht-degree: 2%

---


# Construtor de máscaras

<table>
  <tr style="border: 0;">
    <td style="border: 0;" valign="top">Máscara de <img src="../../../assets/generators/icon_mask_builder_dark.png" alt=""/><strong>entrada:</strong>, gerador</td>
    <td style="border: 0;" valign="top"><strong>Descrição</strong><br>O gerador do Construtor de máscaras é uma versão herdada do gerador do Editor de Máscaras. É um gerador de máscara multiuso que permite combinar Desgaste, AO, Curvatura, Gradiente, Espaço Mundial Normal, Scratches, Dispersão e Micro Detalhes em uma única máscara.<br><br>O gerador de Construtor de máscaras é muito flexível, mas devido à sua complexidade, ele pode afetar mais o desempenho do que a maioria dos geradores.<br><br>O gerador de Construtor de máscaras gera uma textura monocromática (preto e branco). Como resultado, é útil para gerar máscaras com base nos vários mapas baked. <br><br>Mapas normais de posição cozida, curvatura, oclusão ambiente e espaço global são necessários como entradas de imagem. <a href="../../../baking/baking.md">Saiba mais sobre como assar aqui</a>.</td>
  </tr>
</table>

## Entradas

| Nome de entrada | Descrição |
| --- | --- |
| Cor **normal do espaço global** | Use o mapa World Space Normals assado. |
| **desgaste personalizado 1** em tons de cinza | Use uma textura personalizada ou um ponto de ancoragem. |
| **desgaste personalizado 2** em tons de cinza | Use uma textura personalizada ou um ponto de ancoragem. |
| **Entrada de Dispersão** em tons de cinza | Use uma textura personalizada ou um ponto de ancoragem. |
| Cor de **Posição** | Use o mapa de posição cozida. |
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
    <td><strong>Nível</strong></td>
    <td>Ajuste o nível do ponto médio da máscara final depois que todos os efeitos forem combinados entre preto ou branco, como um ajuste de brilho.</td>
  </tr>
  <tr>
    <td><strong>Contraste</strong></td>
    <td>Ajuste o contraste/declínio da máscara final.</td>
  </tr>
  <tr>
    <td><strong>Inverter</strong></td>
    <td>Inverta o resultado final da máscara combinada.</td>
  </tr>
  <tr>
    <td><strong>Usar Triplanar</strong></td>
    <td>Quando <strong>Usar Triplanar </strong> está habilitado, a textura é projetada a partir de três direções (eixos X, Y, Z) em vez de depender apenas de UVs. <br><ul><li>Sem o triplanar ativado, a textura segue o layout UV.</li><li>Com o triplanar ativado, a textura é projetada a partir de vários ângulos e mesclada.</li></ul></td>
  </tr>
  <tr>
    <td><strong>Contraste de mesclagem triplanar</strong></td>
    <td>Ajuste a suavidade de uma textura quando projetada usando o mapeamento triplanar. Ela ajusta a suavidade da mesclagem entre as projeções de cada direção.</td>
  </tr>
  <tr>
    <td><strong>Grunge</strong></td>
    <td>Ajuste quanto as configurações de Desgaste afetam o resultado final da máscara.</td>
  </tr>
  <tr>
    <td><strong>AO</strong></td>
    <td>Ajuste quanto as configurações de AO (Oclusão ambiente) afetam o resultado final da máscara.</td>
  </tr>
  <tr>
    <td><strong>Curvatura</strong></td>
    <td>Ajuste quanto as configurações de Curvatura afetam o resultado final da máscara.</td>
  </tr>
  <tr>
    <td><strong>Gradiente superior/inferior</strong></td>
    <td>Ajuste quanto o Gradiente superior/inferior afeta o resultado final da máscara.</td>
  </tr>
  <tr>
    <td><strong>Normal do Espaço Global</strong></td>
    <td>Ajuste quanto as configurações do Espaço global normal afetam o resultado final da máscara.</td>
  </tr>
  <tr>
    <td><strong>Arranhões</strong></td>
    <td>Ajuste quanto as configurações de Scratches afetam o resultado final da máscara. Para os Scratches serem visíveis, Desgaste, AO ou Curvatura precisam estar acima de 0.</td>
  </tr>
  <tr>
    <td><strong>Dispersão</strong></td>
    <td>Ajusta o quanto a Dispersão afeta a máscara.</td>
  </tr>
</table>

### Grunge

| Nome do parâmetro | Descrição |
| --- | --- |
| **Escala** | Ajuste o tamanho da textura do desgaste. |
| **Usar Desgaste Personalizado** | Ativar ou desativar o uso de um mapa de Desgaste personalizado. É apenas a visibilidade do Desgaste Personalizado 1. Para controlar a visibilidade do Desgaste Personalizado 2, ajuste o controle deslizante Desgaste Personalizado Secundário. |
| **Desgaste Personalizado Secundário** | Ajuste a visibilidade da textura do Desgaste Personalizado 2. |
| **Inverter** | Inverta os mapas de desgaste. |

### Oclusão de ambiente

| Nome do parâmetro | Descrição |
| --- | --- |
| **Intervalo** | Ajuste o intervalo da máscara de AO. |
| **Contraste** | Ajuste o contraste/declínio da máscara do AO. |
| **Ruído** | Adicione ruído ao resultado do AO, diminuindo efetivamente o brilho da máscara. |
| **Inverter** | Inverta a máscara de AO. |

### Curvatura

| Nome do parâmetro | Descrição |
| --- | --- |
| **Intervalo Convexo** | Ajuste o ângulo convexo mínimo necessário para ser realçado pela máscara. |
| **Contraste convexo** | Ajuste o contraste da máscara convexa. |
| **Inversão Convexa** | Inverte a máscara convexa. |
| **Intervalo côncavo** | Ajuste o ângulo côncavo mínimo a ser destacado pela máscara. |
| **Contraste côncavo** | Ajuste o contraste da máscara côncava. |
| **Inversão côncava** | Inverta a máscara côncava. |
| **Smoothness** | Ajuste a mesclagem entre as áreas claras e escuras da máscara de Curvatura. |
| **Aumento de Nível** | Use isso para estender o intervalo da área mascarada. Isso funciona como um multiplicador para os parâmetros **Intervalo convexo** e **Intervalo côncavo**. |
| **Ruído** | Adicione ruído ao resultado Curvatura, diminuindo efetivamente o brilho da máscara. |

### Gradiente

A posição do gradiente é baseada no mapa de posição, que pode ser cozido com Cena completa ou com escala de normalização Por material. Se o material aparecer apenas em uma pequena área da cena, mas o mapa de posição for assado com uma escala de Normalização de cena completa, pode ser difícil ajustar o Intervalo de degradê para obter o resultado desejado.

| Nome do parâmetro | Descrição |
| --- | --- |
| **Intervalo** | Ajuste o intervalo de gradientes. |
| **Contraste** | Ajusta o contraste do gradiente. |
| **Inverter** | Inverte o gradiente. |

### Normal do Espaço Global

Os valores de **frontal**, **traseira**, **esquerda** e **direita** podem não corresponder aos valores de frente, trás, esquerda e direita da malha. Por padrão, **Frente** corresponde ao eixo X positivo, e Direita corresponde ao eixo Z positivo.

| Nome do parâmetro | Descrição |
| --- | --- |
| **Intensidade Superior** | Ajuste o intervalo (intensidade) do gradiente de cima para baixo. |
| **Intensidade inferior** | Ajuste o intervalo (intensidade) do gradiente de baixo para cima. |
| **Intensidade frontal** | Ajuste o intervalo (intensidade) do gradiente traseiro frontal. |
| **Intensidade de fundo** | Ajuste o intervalo (intensidade) do gradiente frontal traseiro. |
| **Intensidade correta** | Ajuste o intervalo (intensidade) do gradiente à esquerda à direita. |
| **Intensidade da esquerda** | Ajuste o intervalo (intensidade) do gradiente à esquerda e à direita. |

### Arranhões

| Nome do parâmetro | Descrição |
| --- | --- |
| **Valor** | Ajuste a densidade dos arranhões. |
| **Escala** | Ajuste o tamanho dos arranhões. |

### Dispersão

| Nome do parâmetro | Descrição |
| --- | --- |
| **Escala** | Ajuste o tamanho do efeito de dispersão. Uma escala mais alta resulta em carimbos maiores e menores, enquanto uma escala mais baixa aumenta o tamanho do carimbo individual com menos itens visíveis. |
| **Densidade** | Ajuste o número dos carimbos dispersos. |
| **Tamanho** | Ajuste o tamanho dos carimbos dispersos. |
| **Variação de Tamanho** | Ajuste quanta aleatoriedade há no tamanho de cada ocorrência do carimbo disperso. Uma variação de tamanho maior reduz aleatoriamente os tamanhos do carimbo, portanto, aumentar a variação de tamanho pode significar que você também precisa aumentar o valor do tamanho para manter o mesmo tamanho médio. |
| **Variação de opacidade** | Ajuste quanta aleatoriedade há na opacidade de cada ocorrência do carimbo disperso. |

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
