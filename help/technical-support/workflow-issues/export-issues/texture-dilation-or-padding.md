---
helpx_url: "https://helpx.adobe.com/br/substance-3d-painter/technical-support/workflow-issues/export-issues/texture-dilation-or-padding.html"
breadcrumb-title: ''
description: Saiba como usar a dilatação e o preenchimento de texturas no Substance 3D Painter para impedir artefatos de borda em texturas exportadas.
helpx_creative_field: ""
helpx_description: Painter > Technical support > Workflow Issues > Export Issues > Texture dilation or Padding
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Dilatação ou preenchimento da textura
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '332'
ht-degree: 0%

---


# Dilatação ou preenchimento da textura

O **Preenchimento** (às vezes, também chamado de **dilatação**) é um processo que ocorre após a geração de uma textura. Sua finalidade é dilatar as bordas das Ilhas UV para preencher áreas vazias com pixels semelhantes.

Gerar um preenchimento de boa qualidade é importante para garantir uma boa geração de [mipmaps](../../../getting-started/glossary.md) posteriormente por mecanismos de jogo ou renderizadores offline.\
O Substance 3D Painter pode gerar um preenchimento infinito: isso significa que um pixel será esticado até alcançar outra Ilha UV ou as bordas da textura.

## Geração de preenchimento infinita

Aqui está um exemplo de como o preenchimento infinito funciona:

<table>
<tr style="border: 0;">
<td style="border: 0;" valign="top">

![](../../../assets/padding.gif){width="512px"}

</td>
<td style="border: 0;" valign="top">

![](../../../assets/padding-zoom.gif)

</td>
</tr>
</table>

## MipMaps

Em gráficos 3D do computador, os **mipmaps** são sequências de texturas otimizadas pré-calculadas, cada uma das quais é uma representação de resolução progressivamente mais baixa da mesma imagem. O objetivo é aumentar a velocidade de renderização e reduzir os artefatos de suavização. Uma imagem mipmap de alta resolução é usada para objetos próximos à câmera. Imagens de resolução mais baixa são usadas à medida que o objeto fica mais distante. Essa é uma maneira eficiente de renderizar ou ler todos os pixels da textura original. Os mipmaps (cada nível) são incorporados dentro da própria textura (quando suportado pelo formato de arquivo).

O preenchimento é muito importante para mipmaps, pois evita que cores incorretas sangrem dentro dos UVs da malha ao diminuir as resoluções de textura.

<table>
<tr style="border: 0;">
<td style="border: 0;" valign="top">

![](../../../assets/mipmap-padding.gif){width="400px"}

</td>
<td style="border: 0;" valign="top">

![](../../../assets/mipmap-nopadding.gif){width="400px"}

</td>
</tr>
</table>

No exemplo acima, o fundo cinza sangra para os UVs (imagem à direita), enquanto com o preenchimento mantém a cor limpa (imagem à esquerda).

Em um aplicativo 3D, este é o resultado:

![](../../../assets/padding-toggle.gif)

## Controles de preenchimento

O Substance 3D Painter permite alterar o comportamento da geração de preenchimento (como desativá-la) em diferentes locais:

* **Ao assar** : consulte a [documentação de cozimento](../../../baking/baking.md) para obter mais informações.
* **Ao gerar texturas para um Conjunto de Texturas**: consulte a documentação [Configurações do Conjunto de Texturas](../../../interface/texture-set/texture-set-settings.md) para obter mais informações.
* **Ao exportar texturas** : consulte a seção “Configurações de preenchimento” da documentação de [configurações de exportação](../../../export/export-window/export-window.md) para obter mais informações.
