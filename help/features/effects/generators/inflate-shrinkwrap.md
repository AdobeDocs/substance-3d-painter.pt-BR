---
title: Inflar contorno
description: Aprenda a usar o gerador de quebra automática do Substance 3D Painter Inflate.
source-git-commit: b7770a9497f0db047433aec32c31b57f8dc13ae7
workflow-type: tm+mt
source-wordcount: '279'
ht-degree: 3%

---


# Inflar contorno

<table>
  <tr style="border: 0;">
    <td style="border: 0;" valign="top"><img src="../../../assets/generators/icon_inflate_shrinkwrap.webp" alt=""/><br><strong>Em:</strong> encolher, inflar, gerador, randomseed</td>
    <td style="border: 0;" valign="top"><strong>Descrição</strong><br>O gerador de Inflar Shrinkwrap adiciona rugas que imitam o efeito de um material fino sendo esticado sobre a superfície da sua malha.<br><br>O gerador Inflar Encolhimento gera uma textura monocromática (preto e branco). Como resultado, é útil para gerar máscaras que criam o efeito de quebra. No entanto, ele também pode ser colocado diretamente em uma camada de preenchimento para adicionar rugas ao height e aos canais normais.<br><br>Um mapa de curvatura assado é necessário como entrada de imagem. <a href="../../../baking/baking.md">Saiba mais sobre como assar aqui</a>.</td>
  </tr>
</table>

## Entradas

| Nome de entrada | Descrição |
| --- | --- |
| **Curvatura** em tons de cinza | Use o mapa de curvatura assado. |

## Parâmetros

<table>
  <tr>
    <th>Nome do parâmetro</th>
    <th>Descrição</th>
  </tr>
  <tr>
    <td><strong>Predefinição</strong></td>
    <td>Alternar entre as predefinições Inflado, Puxado a vácuo e Rígido.</td>
  </tr>
  <tr>
    <td><strong>Semente</strong></td>
    <td>Defina o valor de propagação usado para gerar a textura do dirt. <br><ul><li>Clique em Aleatório para alternar para outra semente aleatória.</li><li>Clique no lápis para ver o valor de semente atual e insira um valor específico, se desejar.</li></ul></td>
  </tr>
  <tr>
    <td><strong>Inflar ou encolher</strong></td>
    <td>Alterne entre os modos inflar e quebra automática.</td>
  </tr>
  <tr>
    <td><strong>Intensidade da costura</strong></td>
    <td>Ajuste a pronúncia das bordas.</td>
  </tr>
  <tr>
    <td><strong>Largura da borda elevada</strong></td>
    <td>Ajuste o quanto as bordas infladas esvaziam.</td>
  </tr>
  <tr>
    <td><strong>Intensidade de borda aumentada</strong></td>
    <td>Ajuste a força do efeito de borda elevada.</td>
  </tr>
  <tr>
    <td><strong>Densidade de enrugamento</strong></td>
    <td>Ajuste o número de rugas.</td>
  </tr>
  <tr>
    <td><strong>Rigidez das rugas</strong></td>
    <td>Ajuste como as rugas apertadas são puxadas juntas nas bordas UV.</td>
  </tr>
  <tr>
    <td><strong>Intervalo de rugas</strong></td>
    <td>Ajuste a distância que as rugas atingem das bordas UV.</td>
  </tr>
  <tr>
    <td><strong>Escala de rugas</strong></td>
    <td>Ajuste o tamanho das rugas.</td>
  </tr>
</table>

### Parâmetros técnicos

| Nome do parâmetro | Descrição |
| --- | --- |
| **Intervalo de Heights** | Defina o intervalo do height. |
| **Posição do Height** | Ajuste o height para preto (0) ou branco (1). |
| **Tamanho da superfície (cm)** | Defina o tamanho físico da superfície. |
| **Profundidade de superfície (cm)** | Defina a profundidade física da superfície. |
