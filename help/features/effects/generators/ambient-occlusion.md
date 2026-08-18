---
title: Oclusão de ambiente
description: Saiba como usar o gerador de Oclusão ambiente do Substance 3D Painter.
source-git-commit: b095b9b437f75bbb3a3b85ee84a6850026c3bf98
workflow-type: tm+mt
source-wordcount: '542'
ht-degree: 4%

---


# Oclusão de ambiente

<table>
  <tr style="border: 0;">
    <td style="border: 0;" valign="top"><img src="../../../assets/generators/icon_ambient_occlusion.webp" alt=""/><br><strong>Entrada:</strong> máscara, gerador, tons de cinza, mesclagem</td>
    <td style="border: 0;" valign="top"><strong>Descrição</strong><br>O gerador de Oclusão ambiente cria uma máscara com base no mapa de Oclusão ambiente assado com a opção de mesclar uma textura ou microdetalhes na máscara.<br><br>Se estiver usando o gerador de Oclusão ambiente para criar uma máscara de camada, talvez seja necessário inverter a saída da Oclusão ambiente. Por padrão, o gerador gera a saída de áreas ocultas como áreas escuras e não ocultadas como claras. Se usada como máscara, a camada mascarada ficará visível somente em áreas não ocultadas. Inverter a saída garantirá que a camada mascarada apareça apenas em áreas ocultadas.<br><br>Mapas normais de posição cozida, oclusão ambiente e espaço global são necessários como entradas de imagem. <a href="../../../baking/baking.md">Saiba mais sobre como assar aqui</a>.</td>
  </tr>
</table>

## Entradas

| Nome de entrada | Descrição |
| --- | --- |
| Cor da textura | Use uma textura personalizada ou um ponto de ancoragem. |
| Micro cor normal | Use uma textura normal personalizada ou um ponto de ancoragem. |
| Cor do Height Micro | Use uma textura personalizada ou um ponto de ancoragem. |
| Escala de cinza da Oclusão ambiente | Use o mapa de Oclusão ambiente cozido. |
| Cor dos normais do espaço mundial | Use o mapa World Space Normals assado. |
| Cor do gradiente da posição | Use o mapa de posição cozida. |

## Parâmetros

| Nome do parâmetro | Descrição |
| --- | --- |
| **Inversão global** | Inverta o resultado final depois que todos os efeitos forem combinados. |
| **Desfoque global** | Suavize a máscara final uniformemente depois de combinar todos os efeitos. |
| **Saldo Global** | Altere o equilíbrio da máscara final depois que todos os efeitos forem combinados entre preto ou branco, como um ajuste de brilho. |
| **Contraste global** | Ajuste o contraste da máscara final depois que todos os efeitos forem combinados. |
| **Usar Textura** | Ativar ou desativar o uso de um mapa de textura personalizado. |
| **Usar Microdetalhes** | Ativar ou desativar o uso de microdetalhes personalizados. |

### Oclusão de ambiente

| Nome do parâmetro | Descrição |
| --- | --- |
| **Inverter** | Inverta apenas a Oclusão ambiente e os microdetalhes. |
| **Desfoque** | Suavize apenas a Oclusão ambiente e os microdetalhes. |
| **Saldo** | Ajuste o equilíbrio apenas da Oclusão ambiente e dos microdetalhes, deslocando o ponto médio em direção ao preto ou branco, como um controle de brilho. |
| **Contraste** | Ajuste o contraste/declínio apenas da Oclusão ambiente e dos microdetalhes. |

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
    <td>Inverta apenas a textura personalizada.</td>
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
    <td>Quando o Triplanar está ativado, a textura é projetada a partir de três direções (eixos X, Y, Z) em vez de depender apenas de UVs.<br><ul><li>Sem o triplanar, a textura segue o layout UV.</li><li>Com o triplanar, a textura é projetada a partir de vários ângulos e misturada.</li></ul></td>
  </tr>
  <tr>
    <td><strong>Contraste triplanar</strong></td>
    <td>Controle a suavidade de mesclagem de uma textura quando projetada usando o mapeamento triplanar. Essa configuração ajusta a suavidade da mesclagem entre as projeções de cada direção.</td>
  </tr>
</table>

### Microdetalhes

| Nome do parâmetro | Descrição |
| --- | --- |
| **Micro Height** | Ativar ou desativar o uso de um mapa personalizado de Micro Height. |
| **Micro normal** | Ativa ou desativa a utilização de um mapa Micro Normal personalizado. |
| **Raio do AO** | Ajuste o raio (intervalo) da Oclusão ambiente em microdetalhes. |
| **Profundidade AO** | Ajuste a profundidade (intensidade) da Oclusão ambiente em microdetalhes. |
