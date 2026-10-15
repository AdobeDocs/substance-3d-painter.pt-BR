---
title: Pintura em gaiola
description: Saiba como evitar artefatos e personalizar a gaiola durante o processo de fça bake com a pintura em gaiola no Substance 3D Painter.
hold: true
source-git-commit: 8e09732a300f321ad8fc04883db7a338b8c6a5a7
workflow-type: tm+mt
source-wordcount: '1016'
ht-degree: 0%
---

# Pintura em gaiola

A **pintura em gaiola** permite tinta áreas para afastar a gaiola que está fazendo bake ou aproximá-la da superfície de baixo polígono. A pintura em gaiola ajuda a evitar artefatos durante o fça bake e, ao mesmo tempo, captura todos os detalhes de alto polígono da malha.

![](../assets/baking/cage-painting/splash_example.png)

*A luva esquerda, feita bake com uma gaiola à distância e uma distância frontal baixa do Max, mostra artefatos feitos bake, incluindo distorção e áreas onde a gaiola cruza a malha de alto polígono, perdendo detalhes. A luva direita foi feita bake usando as mesmas configurações, mas com pintura em gaiola para controlar o tamanho da gaiola.*

>[!NOTE]
>
> A pintura em gaiola subdivide automaticamente a malha da gaiola, o que significa que, mesmo com malhas de baixa resolução, a gaiola pode ser empurrada e puxada o suficiente para cobrir todos os detalhes.

## Configurar pintura de gaiola

Para que a **Pintura em gaiola** esteja disponível, o projeto deve ter pelo menos um arquivo de cena de polígono alto a partir do qual fazer bake, e o tipo de Gaiola deve ser definido como **Com base na distância**.

>[!NOTE]
>
> O suporte para **Pintura em gaiola** será adicionado para o **tipo de Gaiola Automática** em uma versão futura.

Recomendamos definir os valores de **Distância frontal máxima** e **Em relação à caixa delimitadora** antes de começar a tinta a gaiola, pois alterar esses valores após a pintura pode exigir retoques ou até mesmo repintar a gaiola do zero.

>[!TIP]
>
> Se desejar iniciar novamente a pintura em gaiola do zero, redefina os parâmetros da pintura em gaiola, os traçados de pintura em gaiola ou todas as configurações de fça bake.
>
> ![](../assets/baking/cage-painting/resetcage.png)

## Iniciar pintura de gaiola

Para iniciar a pintura em gaiola:

1. Alternar para [**modo de Fça bake**](baking.md).
1. Verifique se você selecionou pelo menos um arquivo de **Cena de polígono alto** do qual fazer bake.
1. No **painel** Configurações comuns ****, navegue até a **seção Gaiola**.
1. Defina o **Tipo de caixa** como **com base na distância**.
1. Clique em **Tinta compartimento**.

>[!VIDEO](https://video.tv.adobe.com/v/3504611?learn=on)

*Este vídeo mostra um novo projeto que está sendo configurado para pintura em gaiola. Primeiro, mudamos para o modo de fça bake e, em seguida, selecionamos uma cena de alta polivalência. O tipo de Gaiola baseada em Distância é selecionado por padrão, por isso podemos iniciar a pintura de gaiola imediatamente.*

>[!NOTE]
>
> Por padrão, o **Recozimento automático** está ativado para o canal normal quando você entra pela primeira vez na **Gaiola de pintura**. Isso significa que o mapa normal é recuperado automaticamente toda vez que você modifica a gaiola. Ative ou desative o **Recozimento automático** no [**painel baker do mapa de malha**](../interface/baking-panels/mesh-map-bakers.md).
>
> ![](../assets/baking/cage-painting/auto-rebake.png)

Depois de entrar no modo de pintura de gaiola, a visualização padrão no **Visor** mostra:

* A gaiola ao redor da malha em bege transparente.
* Áreas onde o alto poli cruza a gaiola em vermelho vivo.
* Jaula pintada áreas em verde (positivo) e azul (negativo) na superfície de malha de baixo-poli.

No modo de pintura em caixa, use o [**menu de visualização Feita bake**](baking-visualization-settings.md) no **Viewport** para personalizar a visualização de cada elemento.

>[!NOTE]
>
> A visualização em vermelho vivo das interseções de alto índice com a gaiola é uma visualização aproximada e não corresponde exatamente aos resultados finais do faço bake. Na maioria dos casos, a visualização é bastante precisa, mas para malhas de baixo polígono com polígonos longos e finos, ela pode ser imprecisa. Para essas malhas, é melhor usar o **Faço bake rápido** ou o **Recozimento automático** para verificar o resultado final.

## Ferramentas de pintura de gaiola

Ao pintar a caixa, você pode usar muitas das ferramentas e atalhos que está acostumado a partir do **Modo de pintura**, incluindo as ferramentas **Pincel**, **Borracha** e **Preenchimento de polígono**.

* Você pode alternar entre o **Pincel**, a **Borracha** e o **Preenchimento de polígono** da barra de ferramentas ou usar os [atalhos de teclado](../interface/settings/shortcuts.md) padrão do modo de Pintura.
* Ao usar as ferramentas **Pincel** ou **Borracha**, você pode ajustar o tamanho, o fluxo, a opacidade e o espaçamento da ferramenta usando os parâmetros na parte superior do **Visor**. Você também pode usar os [atalhos de teclado](../interface/settings/shortcuts.md) relevantes onde estiverem disponíveis.

### Pincel

Usar o **Pincel** na **Força** total, o **Fluxo** e a **Opacidade** tem um impacto enorme na superfície da gaiola. Recomendamos definir um valor muito baixo de **Intensidade** e usar os parâmetros Fluxo e Opacidade para controlar a intensidade do pincel.

![](../assets/baking/cage-painting/brush-strength.gif)

*Neste exemplo, o primeiro traçado de pincel é muito forte, mesmo com um valor de Intensidade de 0,05. Depois de diminuir a Intensidade, o Fluxo e a Opacidade do traçado, temos muito mais controle sobre o efeito.*

### Borracha

A ferramenta Borracha permite remover a tinta da caixa, revertendo efetivamente as áreas apagadas para o tamanho de caixa padrão.

### Preenchimento de polígono

Na **pintura em gaiola** no **modo**, a **ferramenta de preenchimento de polígono** tem um recurso adicional. Um **controle deslizante de Intensidade** aparece na **Janela de visualização** ao fazer alterações que você pode usar para ajustar o valor do último conjunto de polígonos selecionados.

Este recurso é particularmente útil para fazer ajustes por elemento usando o **Modo de preenchimento de malha** em cenas com várias malhas separadas.

>[!NOTE]
>
> Este recurso executa novamente a última operação (aplicando o preenchimento de polígono) com um valor de intensidade diferente. Como resultado, executar uma operação diferente ou alterar as ferramentas faz com que o controle deslizante desapareça.

Geralmente, é útil aplicar o mesmo valor de pintura da caixa a várias áreas da malha. Para fazer isso:

1. Selecione o primeiro conjunto de polígonos.
1. Use o controle deslizante de **Intensidade da gaiola** para ajustar a intensidade do efeito.
1. Copie o valor de **Intensidade da caixa** do controle deslizante temporário na **Janela de visualização**.
1. Cole o valor no controle deslizante **Intensidade** na parte superior da **Janela de visualização**.
1. Selecione os conjuntos subsequentes de polígonos para aplicar o mesmo valor de intensidade.

O vídeo abaixo mostra este fluxo de trabalho em ação, usando a **ferramenta de** Preenchimento de polígono **** com o **Preenchimento de malha** selecionado.

>[!VIDEO](https://video.tv.adobe.com/v/3504621?learn=on)

>[!NOTE]
>
> Ao seguir estas etapas, pode ser útil selecionar o **Modo de mesclagem normal** para que a ferramenta de preenchimento de Polígono substitua os valores pintados existentes, em vez de adicioná-los.

### modos Combinar

Por padrão, as ferramentas **Pincel** e **Preenchimento de polígono** usam o **modo de mesclagem (adição)** como padrão, mas você também pode usar os modos de mesclagem **Normal** e **Clarear (Máx)**.

* **Subexposição linear (adicionar)**
  * Cada traçado/carimbo adiciona ou subtrai o valor de intensidade especificado do valor existente.
  * Esse modo de mesclagem funciona de maneira semelhante aos aplicativos de escultura 3D, em que cada traçado adicionado à superfície da malha é tinta.
* **Normal**
  * Cada traçado/carimbo define o valor com a intensidade especificada, substituindo o valor existente.
  * Esse modo de mesclagem se comporta como o pincel padrão no modo de pintura, permitindo cobrir a superfície existente com um valor diferente.
* **Clarear (Máx.)**:
  * Cada traçado/carimbo escolhe o valor máximo entre a intensidade e o valor existente.
  * Com esse modo de mesclagem, as bordas do pincel demoram mais para se basear nos traçados subsequentes, ajudando a criar uma transição mais gradual.