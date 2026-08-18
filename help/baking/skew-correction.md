---
title: Correção de distorção
description: Saiba como usar a correção de inclinação para corrigir artefatos de cozimento ao usar um fluxo de trabalho de alto a baixo poli no Substance 3D Painter.
source-git-commit: db1c8daa33389f21699c53b0d6555c153fbc66d6
workflow-type: tm+mt
source-wordcount: '1027'
ht-degree: 0%

---


# Correção de distorção

<table>
  <tr style="border: 0;">
    <td style="border: 0; width: 35%" valign="top"><img src="../assets/baking/skew-correction-example.png" alt=""/></td>
    <td style="border: 0; width: 65%" valign="top">Às vezes, ao assar para baixo-poli de um modelo de alto-poli, é possível que os detalhes pareçam distorcidos ou distorcidos. Isso geralmente acontece quando os normais da gaiola e os normais da superfície não se alinham bem. A cozedura automática projeta o polígono alto no polígono baixo com base nesses valores normais; portanto, se eles estiverem incorretos, a cozedura produzirá resultados ruins.<br>Felizmente, a correção de Inclinação (ou o mapeamento de Inclinação) está disponível para ajudar a corrigir esse tipo de artefato.<br>A correção de inclinação permite pintar valores diretamente na malha de baixo polímero para redirecionar a projeção usada durante a cozedura sem a necessidade de criar uma caixa personalizada.</td>
  </tr>
</table>

>[!NOTE]
>
> A correção de inclinação é pintada dentro do **Modo de cozimento** e é armazenada por conjunto de texturas.

## Pintar correções de inclinação

A pintura de correção de inclinação permite ajustar manualmente os normais de superfície da malha especificamente para cozimento. Embora você possa pintar correções de inclinação sem assar, isso pode ajudar a [preparar seus mapas de malha primeiro](how-to-bake-mesh-maps.md).

![](../assets/baking/mode_select_buttons.png)

*Alterne para o modo de suspensão para acessar as configurações de correção de inclinação.*

>[!IMPORTANT]
>
> A pintura de correção de inclinação requer as seguintes configurações:
>
> * Uma cena Poli superior precisa ser selecionada. A pintura de inclinação só está disponível ao passar do alto para o baixo poli; se a opção **Usar malha baixa do poli como malha alta do poli** estiver marcada, a pintura de correção de inclinação **não** estará disponível.
> * **Gaiola** deve ser definido como **Com base na distância**.
> * **Média normal** deve ser verificada.

Com as configurações acima, você pode clicar em **Correção de inclinação de pintura** no **painel Configurações comuns** para começar a pintar. Ao entrar pela primeira vez no modo de pintura de correção de inclinação, o **Recozimento automático** será ativado automaticamente para o canal normal. Se preferir, você pode desativar o **Recozimento automático** ou alterar o canal selecionado no [**painel Preparadores de mapas de malha**](../interface/baking-panels/mesh-map-bakers.md).

![](../assets/baking/skew-correction-menu.png)

### Ferramentas de pintura

Ao pintar correções de inclinação, você pode usar muitas das ferramentas e atalhos usados no modo de Pintura, incluindo as ferramentas **Borracha** e **Preenchimento de polígono**.

* Você pode alternar entre o **Pincel**, a **Borracha** e o **Preenchimento de polígono** da barra de ferramentas ou usar o [atalho de teclado](../interface/settings/shortcuts.md) padrão do modo de Pintura.
* Ao usar as ferramentas Pincel ou Borracha, você pode ajustar o tamanho, o fluxo, a opacidade e o espaçamento do pincel com os parâmetros na parte superior da **Janela de visualização**. Você também pode usar o [atalho de teclado](../interface/settings/shortcuts.md) relevante, quando disponível.

### Proteção de borda

A proteção de aresta ignora a correção de inclinação pintada perto das arestas para manter um gradiente suave de normais de superfície. Você pode alternar a **Proteção de borda** na seção **Correção de inclinação**. Quando a **Correção de borda** está habilitada, você pode ajustar a distância da borda e o contraste da borda para obter resultados ideais.

* Distância da borda: controla a distância da borda em que a proteção de borda entra em vigor.
* Contraste da borda: controle o gradiente da proteção de borda. O baixo contraste produz um degradê mais suave.

>[!TIP]
>
> Os valores para **Distância da borda** e **Contraste da borda** são baseados no tamanho da malha. Para malhas com detalhes muito pequenos em comparação ao tamanho da malha, pode ser mais fácil inserir manualmente valores pequenos, em vez de usar os controles deslizantes.

>[!NOTE]
>
> A proteção de borda é baseada no mapa de malha **Bordas sólidas**, que está vinculado à geometria da malha, não às bordas UV.

### Visualização do vetor de inclinação

Por padrão, quando você começa a pintar correções de inclinação, os normais de superfície da malha são visualizados na **Janela de visualização** como linhas vermelhas, amarelas e verdes. Você pode modificar a aparência dessas linhas ou desativá-las completamente na seção **Inclinar vetores** do **menu Visualizações** que aparece no **Viewport.**

![](../assets/baking/visualizations_menu.png)

* **Comprimento dos vetores**: ajuste o comprimento das linhas no visor. Linhas mais longas podem facilitar a compreensão da direção do vetor.
* **Densidade UV de vetores**: altere o número de linhas na superfície da malha. Vetores são colocados no espaço UV, portanto, se a malha tiver densidade de texel inconsistente, o número de vetores por unidade de área de superfície variará com o tamanho do polígono no mapa UV.
* **Opacidade dos vetores**: torne os vetores mais ou menos transparentes.

A cor dos vetores indica a correção de inclinação aplicada a cada posição de vetor.

* Vetores vermelhos indicam que não há correção de inclinação. Os normais de superfície padrão estão sendo usados.
* Vetores verdes indicam que os normais da superfície estão totalmente corrigidos e diretamente perpendiculares à superfície.

![](../assets/baking/skew-correction-painting.gif)*Pintar com um valor de fluxo baixo fornece um controle preciso sobre a intensidade da correção de inclinação.*

## Otimizar desempenho

### Organizar UVs

O **Recozimento automático** foi otimizado para tentar limitar o recozimento na área afetada por cada traçado de pincel ao pintar correções de inclinação. Quando você pinta um traçado, o **Recozimento automático** desenha uma caixa delimitadora ao redor do traçado no espaço UV e refaz tudo dentro da caixa. Isso significa que se o seu traço cobrir apenas uma pequena seção do espaço UV, apenas uma pequena área será rebaked, tornando a operação muito eficiente.

No entanto, se o traçado cruzar duas Ilhas UV em lados opostos do espaço UV, mesmo um traçado pequeno pode exigir a recalibragem de toda a textura, negando a otimização.

Como resultado, recomendamos organizar os UVs de malha para que as Ilhas UV próximas umas das outras no espaço 3D também fiquem próximas umas das outras no espaço UV. Isso melhora o desempenho do **Recozimento automático**.

### Definir Alinhamento como UV

Em geral, pintar correções de inclinação com **Projeção > Alinhamento** definido como UV é mais eficiente. Para alterar o **Alinhamento**:

1. Selecione **Correção de inclinação de pintura** e equipe o **Pincel** ou a **Borracha**.
1. Clique com o botão direito do mouse no **Viewport** para abrir o **painel de configurações do pincel**.
1. Role para baixo até **Projeção**.
1. Definir **Alinhamento** para **UV**.

Com o **Alinhamento** definido como **UV**, é mais difícil pintar traçados suaves em emendas de Ilha UV, no entanto, isso geralmente é menos importante ao pintar correções de inclinação do que ao texturizar sua malha.

>[!NOTE]
>
> Os parâmetros do **Pincel** e da **Borracha** são armazenados separadamente. Para maximizar o desempenho de ambas as ferramentas, você precisará definir o **Alinhamento** para cada uma individualmente.

## Inclinar correções e desfazer pilha

Cozimento e pintura compartilham um único histórico de desfazer. Alternar entre o Modo de cozimento e o modo de pintura é, em si, uma etapa que pode ser desfeita, e ativar ou desativar a correção de inclinação também pode ser desfeito. Ao desfazer uma ação de cozimento enquanto estiver no modo de pintura, o Modo de cozimento é reaberto automaticamente antes que essas etapas sejam desfeitas, portanto, uma ação nunca é desfeita fora do modo em que aconteceu.