---
title: Editor de máscara
description: Saiba como usar o gerador de editor de máscaras do Substance 3D Painter.
source-git-commit: b7770a9497f0db047433aec32c31b57f8dc13ae7
workflow-type: tm+mt
source-wordcount: '1494'
ht-degree: 3%

---


# Editor de máscara

<table>
  <tr style="border: 0;">
    <td style="border: 0;" valign="top">Máscara de <img src="../../../assets/generators/icon_mask_editor_dark.png" alt=""/><strong>entrada:</strong>, gerador</td>
    <td style="border: 0;" valign="top"><strong>Descrição</strong><br>O gerador de Editor de Máscara é um gerador de máscara multiuso que permite combinar Texturas, Oclusão ambiente, Curvatura, Espaço mundial normal, Gradiente, Thickness e Microdetalhes em uma única máscara.<br>O gerador de Construtor de máscaras é muito flexível, mas devido à sua complexidade, ele pode afetar mais o desempenho do que a maioria dos geradores.<br><br>O gerador do Editor de Máscara gera uma textura monocromática (preto e branco). Como resultado, é útil para gerar máscaras com base nos vários mapas baked. <br><br>Mapas normais de posição cozida, thickness, curvatura, oclusão ambiente e espaço global são necessários como entradas de imagem. <a href="../../../baking/baking.md">Saiba mais sobre como assar aqui</a>.</td>
  </tr>
</table>

## Entradas

| Nome de entrada | Descrição |
| --- | --- |
| Cor de **Textura** | Use uma textura personalizada ou um ponto de ancoragem. |
| **Cor de textura (secundária)** | Use uma textura personalizada ou um ponto de ancoragem. |
| **Cores Normais do Espaço Mundial** | Use o mapa World Space Normals assado. |
| Cor do **Gradiente de posição** | Use o mapa de posição cozida. |
| **Thickness** em tons de cinza | Use o mapa de Thicknesss assados. |
| **Curvatura** em tons de cinza | Use o mapa de curvatura assado. |
| **Oclusão de ambiente** em tons de cinza | Use o mapa de Oclusão ambiente cozido. |
| Cor **Micro Normal** | Use uma textura normal personalizada ou um ponto de ancoragem. |
| Cor do **Micro Height** | Use uma textura personalizada ou um ponto de ancoragem. |

## Parâmetros

| Nome do parâmetro | Descrição |
| --- | --- |
| **Inversão global** | Inverta o resultado final depois que todas as camadas forem combinadas. |
| **Desfoque global** | Desfoque a máscara final de maneira uniforme depois que todas as camadas forem combinadas. |
| **Saldo Global** | Ajuste o equilíbrio da máscara final depois que todas as camadas forem combinadas entre preto ou branco, como um ajuste de brilho. |
| **Contraste global** | Ajuste o contraste da máscara final depois que todas as camadas forem combinadas. |
| **Opacidade da textura** | Ajuste a visibilidade da textura personalizada. |
| **Opacidade da textura 2** | Ajuste a visibilidade da segunda textura personalizada. |
| **Opacidade da Oclusão do ambiente** | Ajuste a visibilidade dos detalhes da oclusão ambiente. |
| **Opacidade da curvatura** | Ajuste a visibilidade dos detalhes da curvatura. |
| **Opacidade Normal Do Espaço Mundial** | Ajuste a visibilidade dos detalhes normais do espaço global. |
| **Posição Da Opacidade Do Gradiente** | Ajuste a visibilidade dos detalhes da posição. |
| **Opacidade do Thickness** | Ajuste a visibilidade dos detalhes do thickness. |

### Textura

<table>
  <tr>
    <th>Nome do parâmetro</th>
    <th>Descrição</th>
  </tr>
  <tr>
    <td><strong>Inverter</strong></td>
    <td>Inverte a textura personalizada.</td>
  </tr>
  <tr>
    <td><strong>Conversão em tons de cinza</strong></td>
    <td>Defina o método usado para converter cores inteiras em tons de cinza. O <a href="grayscale-conversion.md">Gerador de conversão de tons de cinza tem mais informações sobre como cada método funciona</a>.</td>
  </tr>
  <tr>
    <td><strong>Modo de mesclagem</strong></td>
    <td>Selecione o <a href="../../../interface/layer-stack/blending-modes.md">modo de mesclagem</a> a ser usado para a camada atual.</td>
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
  <tr>
    <td><strong>Lado a lado não quadrado</strong></td>
    <td>Ativar ou desativar a divisão em blocos gráficos não quadrados.</td>
  </tr>
</table>

### Textura 2

<table>
  <tr>
    <th>Nome do parâmetro</th>
    <th>Descrição</th>
  </tr>
  <tr>
    <td><strong>Inverter</strong></td>
    <td>Inverta a textura secundária personalizada.</td>
  </tr>
  <tr>
    <td><strong>Conversão em tons de cinza</strong></td>
    <td>Defina o método usado para converter cores inteiras em tons de cinza. O <a href="grayscale-conversion.md">Gerador de conversão de tons de cinza tem mais informações sobre como cada método funciona</a>.</td>
  </tr>
  <tr>
    <td><strong>Modo de mesclagem</strong></td>
    <td>Selecione o <a href="../../../interface/layer-stack/blending-modes.md">modo de mesclagem</a> a ser usado para a camada atual.</td>
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
  <tr>
    <td><strong>Lado a lado não quadrado</strong></td>
    <td>Ativar ou desativar a divisão em blocos gráficos não quadrados.</td>
  </tr>
</table>

### Oclusão de ambiente

| Nome do parâmetro | Descrição |
| --- | --- |
| **Inverter** | Inverta as camadas Oclusão ambiente e Microdetalhes. |
| **Modo de Mesclagem** | Selecione o [modo de mesclagem](../../../interface/layer-stack/blending-modes.md) a ser usado para a camada atual. |
| **Desfoque** | Ajuste a Oclusão ambiente e a suavidade de microdetalhes. |
| **Saldo** | Ajuste o equilíbrio da Oclusão ambiente e dos microdetalhes, deslocando o ponto médio em direção ao preto ou branco, como um controle de brilho. |
| **Contraste** | Ajuste o contraste/declínio da Oclusão ambiente e microdetalhes. |

### Curvatura

<table>
  <tr>
    <th>Nome do parâmetro</th>
    <th>Descrição</th>
  </tr>
  <tr>
    <td><strong>Inverter</strong></td>
    <td>Inverta a curvatura.</td>
  </tr>
  <tr>
    <td><strong>Modo de mesclagem</strong></td>
    <td>Selecione o <a href="../../../interface/layer-stack/blending-modes.md">modo de mesclagem</a> a ser usado para a camada atual.</td>
  </tr>
  <tr>
    <td><strong>Modo</strong></td>
    <td>Defina o modo Curvatura. <br><ul><li><strong>Bordas</strong>: mascara as bordas (áreas convexas)</li><li><strong>Cavidades</strong>: mascara as cavidades (áreas côncavas)</li><li><strong>Duplo</strong>: máscaras em áreas côncavas e convexas.</li><li><strong>Não processado</strong>: máscara de curvatura normal.</li></ul></td>
  </tr>
  <tr>
    <td><strong>Nítida</strong></td>
    <td>Ajuste a visibilidade dos detalhes de curvatura nítidos.</td>
  </tr>
  <tr>
    <td><strong>Fina</strong></td>
    <td>Ajuste a visibilidade dos detalhes de curvatura fina.</td>
  </tr>
  <tr>
    <td><strong>Suave</strong></td>
    <td>Ajuste a visibilidade dos detalhes da curvatura suave.</td>
  </tr>
  <tr>
    <td><strong>Média</strong></td>
    <td>Ajuste a visibilidade dos detalhes de curvatura média.</td>
  </tr>
  <tr>
    <td><strong>Grande</strong></td>
    <td>Ajuste a visibilidade dos detalhes de curvatura grandes.</td>
  </tr>
  <tr>
    <td><strong>Grande</strong></td>
    <td>Ajuste a visibilidade dos detalhes das curvaturas grandes.</td>
  </tr>
  <tr>
    <td><strong>Enorme</strong></td>
    <td>Ajuste a visibilidade dos detalhes de curvatura enormes.</td>
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

### Normal do Espaço Global

| Nome do parâmetro | Descrição |
| --- | --- |
| **Inverter** | Inverta os normais do espaço global. |
| **Modo de Mesclagem** | Selecione o [modo de mesclagem](../../../interface/layer-stack/blending-modes.md) a ser usado para a camada atual. |
| **Desfoque** | Ajuste a suavidade normal do espaço global. |
| **Saldo** | Ajuste o equilíbrio dos normais de espaço, deslocando o ponto médio em direção ao preto ou branco, como um controle de brilho. |
| **Contraste** | Ajuste o contraste/declínio das normais de espaço. |
| **Brilho** | Ajuste a luminosidade dos normais do espaço do mundo. |
| **Da direita para a esquerda** | Ajuste como o efeito é aplicado da esquerda para a direita na malha. |
| **De Cima Para Baixo** | Ajuste como o efeito é aplicado de cima para baixo na Malha. |
| **Da frente para trás** | Ajuste como o efeito é aplicado da frente para trás na malha. |

### Espaço mundial Normal/Direita para a esquerda

| Nome do parâmetro | Descrição |
| --- | --- |
| **Inverter** | Inverta a direção da direita para a esquerda. |
| **Modo de Mesclagem** | Selecione o [modo de mesclagem](../../../interface/layer-stack/blending-modes.md) a ser usado para a camada atual. |

### Espaço mundial normal/de cima para baixo

| Nome do parâmetro | Descrição |
| --- | --- |
| **Inverter** | Inverta a direção de cima para baixo. |
| **Modo de Mesclagem** | Selecione o [modo de mesclagem](../../../interface/layer-stack/blending-modes.md) a ser usado para a camada atual. |

### Espaço mundial normal/da frente para trás

| Nome do parâmetro | Descrição |
| --- | --- |
| **Inverter** | Inverta a direção da frente para trás. |
| **Modo de Mesclagem** | Selecione o [modo de mesclagem](../../../interface/layer-stack/blending-modes.md) a ser usado para a camada atual. |

### Gradiente de posição

| Nome do parâmetro | Descrição |
| --- | --- |
| **Inverter** | Inverta a camada de gradiente de posição. |
| **Saldo** | Ajuste o equilíbrio da camada de gradiente de posição, deslocando o ponto médio em direção ao preto ou branco, como um controle de brilho. |
| **Contraste** | Ajuste o contraste/declínio da camada de gradiente de posição. |
| **Brilho** | Ajuste a luminosidade da camada de degradê de posição. |
| **Modo de mesclagem** | Selecione o [modo de mesclagem](../../../interface/layer-stack/blending-modes.md) a ser usado para a camada atual. |
| **Da direita para a esquerda** | Ajuste como o efeito é aplicado da esquerda para a direita na malha. |
| **De Cima Para Baixo** | Ajuste como o efeito é aplicado de cima para baixo na Malha. |
| **Da frente para trás** | Ajuste como o efeito é aplicado da frente para trás na malha. |

>[!TIP]
>
> O gradiente de posição é formado por até três gradientes: da direita para a esquerda, de cima para baixo e de frente para trás. Cada um dos subgradientes tem seu próprio modo de mesclagem, que pode ser usado para criar diferentes efeitos ou mascarar diferentes áreas do modelo. Os modos de mesclagem desses gradientes interagem uns com os outros apenas para criar uma camada de gradiente de Posição final, eles não interagem diretamente com outras camadas no gerador fora do gradiente de posição.

### Gradiente de posição - da direita para a esquerda

| Nome do parâmetro | Descrição |
| --- | --- |
| **Inverter** | Inverta a direção do gradiente da direita para a esquerda. |
| **Modo de Mesclagem** | Selecione o [modo de mesclagem](../../../interface/layer-stack/blending-modes.md) a ser usado para o gradiente da direita para a esquerda. |

### Gradiente de Posição - De Cima para Baixo

| Nome do parâmetro | Descrição |
| --- | --- |
| **Inverter** | Inverta a direção do gradiente de cima para baixo. |
| **Modo de Mesclagem** | Selecione o [modo de mesclagem](../../../interface/layer-stack/blending-modes.md) a ser usado para o gradiente de cima para baixo. |

### Gradiente de posição - da frente para trás

| Nome do parâmetro | Descrição |
| --- | --- |
| **Inverter** | Inverta a direção do gradiente da frente para trás. |
| **Modo de Mesclagem** | Selecione o [modo de mesclagem](../../../interface/layer-stack/blending-modes.md) a ser usado para o gradiente da frente para trás. |

### Espessura

| Nome do parâmetro | Descrição |
| --- | --- |
| **Inverter** | Inverta a thickness. |
| **Desfoque** | Ajuste a suavidade dos detalhes na camada de thickness. |
| **Contraste** | Ajuste o contraste/declínio da camada de thickness. |
| **Brilho** | Ajuste a luminosidade da camada de thickness. |

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
    <td>Ajuste a intensidade da Curvatura no <strong>Padrão</strong> e no <strong>modo de Curvatura Sobel </strong>.</td>
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
