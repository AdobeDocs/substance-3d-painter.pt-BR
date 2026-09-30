---
title: Edge Wear de Detalhes do MatFX
description: Saiba como usar o filtro Edge Wear de detalhes MatFX no Substance 3D Painter.
source-git-commit: 644a36a1dde953c1d793821e104049ebb6ec3c19
workflow-type: tm+mt
source-wordcount: '345'
ht-degree: 1%
---

# Edge Wear de Detalhes do MatFX

<table>
  <tr style="border: 0;">
    <td style="border: 0;" valign="top"><img src="./Resources/icon_matfx_detail_edge_wear.png" alt="Ícone de Edge Wear de Detalhes do MatFX" title="Edge Wear de Detalhes do MatFX"/><br><strong>Entrada:</strong> efeitos/desgaste, borda, material</td>
    <td style="border: 0;" valign="top">Descrição<br>O filtro MatFX Detail Edge Wear cria detalhes de borda desgastada que podem ser mesclados em um material.<br>É usado em uma camada de textura ou pilha de materiais para adicionar desgaste de borda, quebra de desgaste e ajustes de material de suporte orientados por máscaras e dados de curvatura.</td>
  </tr>
</table>

>[!NOTE]
>
> Para que o filtro Edge Wear de Detalhes MatFX tenha um efeito visível, é necessário que haja informações normais variadas existentes na pilha de camadas abaixo do filtro. Se não houver nenhum dado ou nenhuma variedade no canal normal, o filtro não conseguirá encontrar bordas danificadas e não terá nenhum efeito visível.

## Parâmetros

| Nome do parâmetro | Descrição |
| --- | --- |
| **Intensidade de desfoque:** | Ajuste a intensidade do efeito de desfoque. |
| **Quebra automática de linha:** | Alternar quebra automática de desfoque. Quando ativado, o efeito obtém amostras de pixels do lado oposto da textura. |
| **Modo de Entrada:** | Selecione o modo de entrada usado para orientar o efeito de desgaste. |
| **Nível de desgaste:** | Ajuste o nível de desgaste geral. |
| **Usar Contraste:** | Ajuste o contraste da máscara de desgaste. |
| **Smoothness de bordas:** | Ajuste o smoothness das bordas gastas. |
| **Valor do Desgaste:** | Ajuste a quantidade de desgaste adicionada ao desgaste. |
| **Escala do Desgaste:** | Ajuste a escala do padrão de desgaste. |

### Material

**Aspereza metálica PBR**

|  |  |
| --- | --- |
| **Cor de base:** | Ajuste a contribuição de cor de base. |
| **Metálico:** | Ajuste o valor metálico. |
| **Aspereza:** | Ajuste o valor de aspereza. |

**Brilho do Specular PBR**

|  |  |
| --- | --- |
| **Difusões:** | Ajuste a contribuição difusa. |
| **Cor do Specular:** | Ajuste a cor do specular. |
| **Textura reluzente:** | Ajuste o valor de brilho. |

### Configurações

|  |  |
| --- | --- |
| **Controle de Máscara de Gerador:** | Ajuste a influência da máscara do gerador. |
| **Contraste de máscara de gerador:** | Ajuste o contraste da máscara do gerador. |
| **Desfoque de Máscara do Gerador:** | Ajuste o desfoque aplicado à máscara do gerador. |
| **Valor do Plano de Fundo do Alpha:** | Ajuste o valor alfa do plano de fundo. |
| **Intensidade de curvatura:** | Ajuste a intensidade da entrada de curvatura. |
| **Inverter Curvatura:** | Alterna a inversão da entrada de curvatura. |
| **Combinar Curvatura:** | Alterne a combinação de dados de curvatura invertidos e não invertidos. |
| **Intensidade Normal:** | Ajuste a intensidade normal. |
| **Difusão de AO:** | Ajuste a propagação do efeito de oclusão de ambiente. |
