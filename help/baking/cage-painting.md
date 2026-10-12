---
title: Pintura em gaiola
description: Saiba como evitar artefatos e personalizar a gaiola durante o processo de fça bake com a pintura em gaiola no Substance 3D Painter.
hold: true
source-git-commit: eb0b1c111b0c96a87283785cf702def7305f0aa9
workflow-type: tm+mt
source-wordcount: '1040'
ht-degree: 0%
---

# Pintura em gaiola

A **pintura em gaiola** permite tinta áreas para afastar a gaiola que está fazendo bake ou aproximá-la da superfície de baixo polígono. A pintura em gaiola ajuda a evitar artefatos durante o fça bake e, ao mesmo tempo, captura todos os detalhes de alto polígono da malha.

## Configurar pintura de gaiola

Para que a **Pintura em gaiola** esteja disponível, o projeto deve ter pelo menos um arquivo de cena de polígono alto a partir do qual fazer bake, e o tipo de Gaiola deve ser definido como **Com base na distância**.

>[!NOTE]
>
> O suporte para **Pintura em gaiola** será adicionado para o **tipo de Gaiola Automática** em uma versão futura.

Ajustar os parâmetros de **Gaiola** após a pintura Gaiola pode alterar as áreas pintadas, o que pode exigir retrabalho ou até mesmo a reinicialização do processo de pintura Gaiola, por isso é melhor ajustar esses parâmetros primeiro.

A **distância frontal máxima** e a **distância traseira máxima** controlam a distância de base entre o compartimento e a superfície de malha de baixo polígono. A pintura em gaiola usa esses valores como limites para determinar o quanto modificar o gaiola. Fazer grandes ajustes nesses valores após pintar a gaiola pode causar interseções inesperadas.

**Em relação à caixa delimitadora**, controla as unidades usadas para definir o tamanho do compartimento. Alternar esse parâmetro pode alterar drasticamente o tamanho do compartimento, portanto, é provável que todas as áreas pintadas precisem ser repintadas para corrigir os novos valores.

>[!TIP]
>
> Se quiser reiniciar a pintura em gaiola do zero, redefina os parâmetros de pintura em gaiola, os traçados de pintura em gaiola ou todas as configurações de fça bake.
>
> ![](../assets/baking/cage-painting/resetcage.png)

## Iniciar pintura de gaiola

Para iniciar a pintura em gaiola:

1. Alternar para [**modo de Fça bake**](baking.md).
1. Verifique se você selecionou pelo menos um arquivo de **Cena de polígono alto** do qual fazer bake.
1. No **painel** Configurações comuns **&#x200B;**, navegue até a **seção Gaiola**.
1. Defina o **Tipo de caixa** como **com base na distância**.
1. Clique em **Tinta compartimento**.

>[!NOTE]
>
> Por padrão, o **faço bake Rápido** está ativado para o canal normal quando você entra pela primeira vez na **Gaiola de pintura**. Isso significa que o mapa normal será recuperado automaticamente sempre que você modificar a gaiola. Se preferir, você pode desativar o **faço bake rápido** no [**painel baker do mapa de malha**](../interface/baking-panels/mesh-map-bakers.md).

Depois de entrar no modo de pintura de gaiola, a visualização padrão no **Visor** mostra:

* A gaiola ao redor da malha em bege transparente.
* Áreas onde o alto poli cruza a gaiola em vermelho vivo.
* Cage pintou áreas em verde na superfície de malha de baixo-poli.

No modo de pintura em Gaiola, você pode usar o [**menu de visualização Feita bake**](baking-visualization-settings.md) no **Visor** para modificar a cor e a opacidade da visualização de cada elemento, ou ativar ou desativar a visualização para elementos específicos.

>[!NOTE]
>
> A visualização em vermelho vivo das interseções de alto índice com a gaiola é uma visualização aproximada e não corresponde exatamente aos resultados finais do faço bake. Na maioria dos casos, a visualização é bastante precisa, mas, para malhas de baixo polígono com polígonos longos e finos, ela pode ser imprecisa e é melhor visualizar o resultado feito bake.

## Ferramentas de pintura de gaiola

Ao pintar a caixa, você pode usar muitas das ferramentas e atalhos que está acostumado a partir do **Modo de pintura**, incluindo as ferramentas **Pincel**, **Borracha** e **Preenchimento de polígono**.

* Você pode alternar entre o **Pincel**, a **Borracha** e o **Preenchimento de polígono** da barra de ferramentas ou usar os [atalhos de teclado](../interface/settings/shortcuts.md) padrão do modo de Pintura.
* Ao usar as ferramentas **Pincel** ou **Borracha**, você pode ajustar o tamanho, o fluxo, a opacidade e o espaçamento da ferramenta usando os parâmetros na parte superior do **Visor**. Você também pode usar os [atalhos de teclado](../interface/settings/shortcuts.md) relevantes onde estiverem disponíveis.

### Pincel

Usar o **Pincel** na **Força** total, o **Fluxo** e a **Opacidade** terá um impacto enorme na superfície da gaiola. Recomendamos definir um valor muito baixo de **Intensidade** e usar os parâmetros Fluxo e Opacidade para controlar a intensidade do pincel.

TODO: Animação/vídeo mostrando a diferença no efeito de força

>[!NOTE]
>
> Por padrão, na pintura em Gaiola, a ferramenta Pincel usa o modo de mesclagem **Subexposição linear (Adicionar)**. Esse modo de mesclagem faz com que os traçados subsequentes na mesma área aumentem consistentemente a intensidade do efeito, para que seja possível esculpir a superfície do compartimento com resultados consistentes. Os modos de mesclagem padrão **Máximo (clarear)** e **Normal** ainda estão disponíveis:
>
> 1. Clique com o botão direito para abrir as propriedades do pincel.
> 1. Role para baixo até **Alpha > Mesclagem avançada**.
> 1. Selecione o modo de **mesclagem de carimbos**.

### Borracha

A ferramenta Borracha permite remover a tinta da caixa, revertendo efetivamente as áreas apagadas para o tamanho de caixa padrão.

### Preenchimento de polígono

Na **pintura em gaiola** no **modo**, a ferramenta de preenchimento Polígono tem um recurso adicional. Depois de selecionar polígonos, um **controle deslizante de Intensidade** aparece na viewport, permitindo ajustar a intensidade dos polígonos selecionados. Isso pode facilitar o ajuste da intensidade do efeito sem a necessidade de selecionar os polígonos novamente constantemente.

>[!NOTE]
>
> Este recurso funciona refazendo a última operação (aplicando o preenchimento de polígono) com um valor de intensidade diferente. Como resultado, a execução de uma operação diferente ou a alteração de ferramentas fará com que o controle deslizante desapareça.

Geralmente, pode ser útil aplicar o mesmo valor de preenchimento de polígono a várias áreas da malha. Para fazer isso:

1. Selecione o primeiro conjunto de polígonos.
1. Use o controle deslizante de **Intensidade da gaiola** para ajustar a intensidade do efeito.
1. Copie o valor de **Intensidade da caixa** do controle deslizante temporário na **Janela de visualização**.
1. Cole o valor no controle deslizante **Intensidade** na parte superior da **Janela de visualização**.
1. Selecione os conjuntos subsequentes de polígonos para o mesmo valor de intensidade a ser aplicado a cada um deles.

O vídeo abaixo mostra este fluxo de trabalho em ação, usando a **ferramenta de** Preenchimento de polígono **&#x200B;**&#x200B;com o **Preenchimento de malha** selecionado.

TODO: VÍDEO

### modos Combinar

Por padrão, as ferramentas Pincel e Preenchimento de Polígono assumem o **modo de mesclagem (adição)** como padrão, mas você também pode usar os modos de mesclagem **Normal** e **Clarear (máx.)**.

* **Subexposição linear (adicionar)**: cada traço/carimbo adiciona ou subtrai o valor de intensidade especificado do valor existente. Esse modo de mesclagem funciona de maneira semelhante aos aplicativos de escultura 3D, em que cada traçado adicionado à superfície da malha é tinta.
* **Normal**: cada traçado/carimbo define o valor para a intensidade especificada, substituindo o valor existente. Esse modo de mesclagem se comporta como o pincel padrão no modo de pintura, permitindo cobrir a superfície existente com um valor diferente.
* **Clarear (Máx)**: cada traço/carimbo escolhe o valor máximo entre a intensidade e o valor existente. Com esse modo de mesclagem, as bordas do pincel demoram mais para se basear nos traçados subsequentes, ajudando a criar uma transição mais gradual.