---
title: Bakers de mapa de malha
description: Saiba como usar o painel Padeiros de mapas de malha para controlar quais mapas de malha são cozidos em conjuntos de textura.
source-git-commit: 987b94e15c1dbe4ddf392ea7878126ecdf989423
workflow-type: tm+mt
source-wordcount: '716'
ht-degree: 0%

---


# Painel padeiros de mapa de malha

<table>
  <tr style="border: 0;">
    <td style="border: 0;" valign="top"><img src="../../assets/baking/mesh-map-bakers-panel.png" alt=""/></td>
    <td style="border: 0;" valign="top">O <strong>painel Preparadores de mapas de malha</strong> permite selecionar quais mapas preparar e acessar as configurações de cada tipo de mapa.</td>
  </tr>
</table>

## Controles por mapa

Cada mapa na lista de mapas de malha tem uma série de controles disponíveis:

![](../../assets/baking/mesh-map-controls.png)

1. **Verifique** ou **desmarque** a preparação do mapa.
1. **Visualize** o mapa no visor.
1. **Preparação rápida** somente este mapa.
1. Ative o **Recozimento automático** para o mapa de malha selecionado. Mapas **com refração automática** serão redefinidos automaticamente quando forem feitas alterações nos parâmetros de retificação ou na correção de inclinação.
1. **Sincronizar** configurações para este tipo de mapa em conjuntos de texturas. Desative essa opção para personalizar as configurações de cozimento de mapas individuais.

## Gerenciar configurações de mapa de malha

Há várias maneiras de gerenciar seu projeto para que as configurações de cozimento sejam compartilhadas entre mapas de malha ou conjuntos de texturas. Para projetos complexos, entender como compartilhar configurações pode ajudar a simplificar o processo de cozimento.

Há dois tipos de configurações que você pode compartilhar entre conjuntos de texturas:

* Configurações de cozimento: parâmetros que podem ser alterados nos **Painéis Configurações comuns** e **Configurações de mapa de malha**.
* Verificar status: use-os para ativar ou desativar a cozedura de mapas de malha específicos.

### Sincronizar configurações de cozimento em conjuntos de textura

Quando o projeto tiver vários conjuntos de textura, as opções para Sincronizar entre conjuntos de textura aparecerão no **painel Preparadores de mapas de malha**.

![](../../assets/baking/synchronize-texture-sets.png)

Selecionar o **botão Sincronizar configurações** na parte superior do **painel Preparadores de mapa de malha** abre a **janela Sincronização de configurações comuns**.

![](../../assets/baking/synchronize-common-settings.png)

Nessa janela, é possível selecionar os conjuntos de texturas pelos quais sincronizar as configurações comuns. Com todos os conjuntos de texturas selecionados, a alteração de configurações comuns em qualquer conjunto de texturas as alterará para todos os outros conjuntos de texturas.

Da mesma forma, se você usar o **botão Sincronizar configurações** ao lado de um mapa de malha individual, poderá selecionar conjuntos de textura para compartilhar as configurações específicas do mapa de malha.

![](../../assets/baking/synchronize-ao-settings.png)

#### Compartilhar configurações em conjuntos de textura não sincronizados

Às vezes, você pode querer manter os mapas de malha não sincronizados entre os conjuntos de textura, mas ainda querer copiar as configurações de cozimento de um conjunto de textura para outro.

Para copiar configurações comuns para conjuntos de textura específicos sem sincronização, selecione **Sincronizar todas as configurações com mais conjuntos de Textura...** no **Menu suspenso de preparadores de mapas de malha**.

Você também pode usar **Sincronizar todas as configurações com todos os Conjuntos de Textura** para copiar as configurações para todos os conjuntos de textura no projeto.

![](../../assets/baking/copy-common-baking-settings.png)

Como alternativa, se você deseja copiar as configurações de um único mapa de malha para conjuntos de texturas específicos:

1. Clique com o botão direito do mouse no mapa de malha.
1. Selecione **Aplicar configurações de &lt;mapa de malha> a mais conjuntos de Textura...**

![](../../assets/baking/copy-ao-settings.gif)

*No exemplo acima, cada conjunto de textura começa com configurações diferentes para o AO. Sem definir o mapa de malha do AO a ser sincronizado, usamos **Aplicar configurações de oclusão de ambiente a mais conjuntos de textura...**&#x200B;para começarmos a modificar as configurações do AO para o novo conjunto de textura da mesma linha de base.*

### Gerenciar status de verificação de mapas de malha

A verificação do status determina se determinado mapa é incluído quando você prepara os mapas de malha. Há muitas maneiras de gerenciar o status de verificação para o conjunto de texturas atual:

* Marque ou desmarque mapas individuais.
* Use **Marcar tudo** ou **Desmarcar tudo** para marcar ou desmarcar todos os mapas de malha.
* Use **Inverter mapas de malha verificados** da **lista suspensa Preparadores de mapas de malha** para alternar o status de verificação de todos os mapas.

![](../../assets/baking/click-drag-check.gif)

>[!TIP]
>
> Você pode clicar e arrastar de uma caixa de seleção para marcar ou desmarcar vários mapas rapidamente (consulte a animação acima).

![](../../assets/baking/invert-checked.gif)

*No exemplo acima, usamos **Inverter mapas de malha marcados**&#x200B;para alternar rapidamente a seleção e, em seguida, preparar mapas de malha que ainda não foram cozidos.*

Ao trabalhar com vários conjuntos de texturas, você também pode copiar o status marcado dos mapas para outros conjuntos de texturas selecionando **Aplicar marcado a mais conjuntos de texturas...**, ou copiar o status marcado para todos os conjuntos de texturas com **Aplicar marcado a todos os conjuntos de texturas**.

![](../../assets/baking/copy-checked-status.gif)

*No exemplo acima, ainda não cozinhamos o Height, os normais curvados ou a opacidade no conjunto de texturas **Material.001**. Já temos esses mapas de malha selecionados no conjunto de textura **Material**, então usamos **Aplicar verificado a mais conjuntos de textura...**&#x200B;e selecionamos **Material.001**&#x200B;para copiar o status verificado. Em seguida, assamos os mapas - observe que a visualização circula pelos mapas de malha duas vezes enquanto os mapas são assados. Isso ocorre porque eles estão sendo assados para ambos os conjuntos de texturas.*