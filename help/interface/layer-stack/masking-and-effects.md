---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/interface/layer-stack/masking-and-effects.html"
breadcrumb-title: ''
description: Saiba como usar máscaras e efeitos na pilha de camadas do Substance 3D Painter para controlar a visibilidade e aplicar efeitos de camada.
helpx_creative_field: ""
helpx_description: Painter > Interface > Layer stack > Masking and effects
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Mascaramento e efeitos
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '473'
ht-degree: 5%

---


# Mascaramento e efeitos

## Mascaramento

As camadas podem ser mascaradas para exibir/aplicar seu conteúdo apenas em partes específicas da textura. A máscara funciona como um parâmetro de intensidade no conteúdo da camada. Uma máscara em uma camada está sempre em tons de cinza, independentemente do conteúdo usado para pintar sobre ela (portanto, qualquer cor será convertida em um valor de tons de cinza antes de ser pintada).

Você pode adicionar uma máscara usando o menu de clique com o botão direito ou usando o botão dedicado :

![](../../assets/layer-mask.gif)

Possíveis operações em máscaras:

* Você pode visualizar a própria máscara **pressionando ALT + clicando com o botão esquerdo do mouse** em sua miniatura. Essa camada alternará a viewport para uma visualização isolada da máscara. Essa operação também está disponível nas configurações do visualizador.
* Você pode desabilitar temporariamente uma máscara fazendo **SHIFT + clique com o botão esquerdo do mouse** em sua miniatura. Refaça a mesma operação para ativá-la novamente. Essa operação também está disponível por meio do menu do botão direito do mouse (&quot;alternar máscara&quot;).
* Você pode copiar o conteúdo de uma máscara para outra máscara executando o **Clique com o botão direito do mouse > Copiar conteúdo da máscara** sobre a miniatura e executando o **Clique com o botão direito do mouse > Colar na máscara** na miniatura da segunda máscara.
* Você pode inverter o plano de fundo da máscara executando **Clique com o botão direito do mouse > Inverter plano de fundo da máscara**. Isso é útil se você quiser evitar a destruição dos efeitos anexados a uma máscara.

>[!WARNING]
>
> Adicionar ou remover uma máscara novamente destruirá a máscara e todos os efeitos anexados a ela.

É possível criar imediatamente uma máscara ao criar uma camada de preenchimento (arrastando e soltando) se a tecla **CTRL** for pressionada:

![](../../assets/mask-material-optimized.gif)

## Efeitos

Os efeitos são operações especiais que podem ser editadas a qualquer momento. Os efeitos podem ser colocados em uma máscara ou no conteúdo de uma camada.\
No entanto, os efeitos são mais adequados para um para o outro. Por exemplo, os “geradores” são apropriados para as máscaras.

A linha abaixo de cada miniatura em uma camada indica se há efeitos. Cinza é igual a nenhum efeito, vermelho é igual a pelo menos um efeito. Há uma pilha de efeitos por máscara e por conteúdo.

![](../../assets/effect.gif)

Para obter mais informações, [veja a página dedicada](../../features/effects/effects.md).

## Máscaras inteligentes

As máscaras inteligentes são uma maneira de salvar uma máscara e seu efeito para reutilizá-las facilmente em outras camadas ou outros projetos. Para criar uma máscara inteligente, basta clicar com o botão direito do mouse sobre uma máscara e escolher “**Criar máscara inteligente**”.\
Ao arrastar e soltar uma máscara inteligente em uma camada, uma máscara preta será criada se ainda não existir, caso contrário, a lista de efeitos será mesclada com a existente. É possível substituir completamente a lista de efeitos mantendo pressionada a tecla “**CTRL**” ao soltar a máscara inteligente.

![](../../assets/smart-mask-new-optimized.gif)

<table>
<tr style="border: 0;">
<td style="border: 0;" valign="top">

![](../../assets/smart-mask-add-optimized.gif)

</td>
<td style="border: 0;" valign="top">

![](../../assets/smart-mask-overwrite-optimized.gif)

</td>
</tr>
</table>
