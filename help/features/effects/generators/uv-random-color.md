---
title: Cor aleatória UV
description: Aprenda a usar o gerador de cores aleatórias UV do Substance 3D Painter.
source-git-commit: b7770a9497f0db047433aec32c31b57f8dc13ae7
workflow-type: tm+mt
source-wordcount: '182'
ht-degree: 2%

---


# Cor aleatória UV

<table>
  <tr style="border: 0;">
    <td style="border: 0;" valign="top"><img src="../../../assets/generators/icon_uv_random_color.png" alt=""/><br><strong>No utilitário:</strong>, máscara</td>
    <td style="border: 0;" valign="top"><strong>Descrição</strong><br>O gerador de Cores Aleatórias UV atribui cores únicas sólidas a cada Ilha UV. Isso geralmente é útil como uma ferramenta de diagnóstico com malhas complexas.<br><br>A cor aleatória UV pode ser usada para criar uma máscara (saída em preto e branco) ou diretamente como uma camada de preenchimento para aplicar a variação de cor à malha com base em Ilhas UV, por exemplo, para randomizar cada prancha de um piso de madeira.</td>
  </tr>
</table>

## Entradas

| Nome de entrada | Descrição |
| --- | --- |
| **Gradiente personalizado** | Use um mapa de degradê para definir o intervalo de cores. |

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
    <td><strong>Modo de origem de cores</strong></td>
    <td>Determina o modo de origem de cores usado. <br><ul><li><strong>Aleatório</strong>: no modo Aleatório, as cores são definidas e atribuídas aleatoriamente.</li><li><strong>Gradiente personalizado</strong>: no modo Gradiente personalizado, você tem uma entrada adicional para adicionar um mapa de gradiente personalizado no qual as cores são escolhidas.</li></ul></td>
  </tr>
</table>
