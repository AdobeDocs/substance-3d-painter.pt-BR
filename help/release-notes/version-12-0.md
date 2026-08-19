---
title: Versão 12.0
description: ''
helpx_description: "Substance 3D Painter"
helpx_url: "https://helpx.adobe.com/substance-3d-painter/release-notes/version-12-0.html"
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '1138'
ht-degree: 0%

---


# Versão 12.0

O <b>Substance 3D Painter 12.0</b> oferece nivelamento de textura diretamente na pilha de camadas, um novo modo automático para projeção de distorção, um conjunto renovado de efeitos de pós-processamento e um fluxo de trabalho de criação e configurações de projeto aprimorado.

Data de lançamento: <b>9 de março de 2026</b>

>[!NOTE]
>
> Nesta versão, o suporte de <b>GPUs integradas</b> com <b>memória unificada/compartilhada</b> foi aprimorado. Pode-se esperar uma melhor detecção da memória de vídeo, o que deve levar a melhor desempenho e menos problemas gráficos.

## Principais recursos

### Novo nivelamento de CAMADAS

![](../assets/v12_banner_flatten.jpg)

Uma nova ação <b>Achatar</b> agora está disponível no menu de contexto do botão direito do mouse da pilha de camadas. É possível mesclar várias camadas rapidamente agrupando-as (<b>Ctrl/Cmd + G</b>) e criando uma cópia achatada (<b>Ctrl/Cmd + M</b>). O grupo de origem é desabilitado automaticamente, deixando a opção de excluí-lo ou salvá-lo como um <b>Material Inteligente</b> para edição posterior.

Os elementos achatados da pilha de camadas também podem ser exportados diretamente para o disco para iterações rápidas em outros aplicativos. Grupos, camadas ou máscaras podem ser exportados individualmente ou em lote por meio do menu de contexto da pilha de camadas.

* <b>Achatar texturas diretamente na pilha de camadas</b>\
  Para nivelar qualquer grupo, pressione <b>Ctrl/Cmd + M</b> ou selecione a entrada <b>Nivelar grupo</b> no menu contextual do botão direito do mouse. Isso gera uma cópia mesclada do conteúdo selecionado e desativa automaticamente o grupo de origem, mantendo as camadas originais intactas até que seja tomada a decisão de removê-las ou restaurá-las.

  ![](../assets/v12_flatten_menu.jpg)
* <b>Nivelar e exportar texturas para o disco</b>\
  Uma ação de exportação dedicada no menu do botão direito do mouse salva o resultado nivelado de uma camada, máscara ou grupo e o salva diretamente no disco. Isso é útil para transferir conteúdo preparado para outros aplicativos sem passar pelo pipeline de exportação de textura completa.
* <b>Operações em lote</b>\
  Várias camadas, grupos ou máscaras podem ser selecionados de uma só vez e nivelados ou exportados individualmente em uma única operação, tornando mais eficiente o processamento de grandes partes de uma pilha de camadas em uma só etapa.

  ![](../assets/v12_flatten_batch.jpg)

>[!NOTE]
>
> Mais informações sobre o nivelamento de camadas estão disponíveis na [página de documentação dedicada](../interface/layer-stack/flatten-layers.md).

### Novo modo Distorcer para geometria para projeções

![](../assets/v12_banner_warp_auto.jpg)

Decalques agora podem se adaptar automaticamente a superfícies complexas, reduzindo a necessidade de ajustes manuais. A alternância <b>Distorcer para geometria</b> está disponível na barra de ferramentas contextual enquanto a projeção Distorcer está ativa.

* <b>Novo parâmetro na barra de ferramentas contextual</b>\
  Um novo botão de alternância <b>Distorcer para geometria</b> estará disponível na barra de ferramentas contextual sempre que o modo de projeção Distorcer estiver ativo. Ele pode ser desativado a qualquer momento sem redefinir a configuração de projeção atual.

  ![](../assets/v12_warp_toolbar.png)
* <b>Disposição automática na superfície da malha</b>\
  Quando ativada, a projeção de distorção segue automaticamente a curvatura e a topologia da malha subjacente. Arrastar a projeção pela superfície fará com que ela esteja em conformidade com a geometria, reduzindo significativamente a quantidade de ajuste fino manual necessário ao inserir decalques em formas complexas ou curvas.

  ![](../assets/v12_warp_to_geometry.gif)
* <b>Preservação de deformações locais</b>\
  Ao editar os vértices da grade de projeção de distorção, o modo de distorção para geometria tentará manter a deformação predefinida para garantir que a mesma forma seja sempre projetada.

  ![](../assets/v12_warp_to_geometry_deformed.gif)

>[!NOTE]
>
> Para obter mais informações sobre a projeção de distorção, confira a [página de documentação dedicada](../painting/fill-projections/warp-projection.md).

### Novos efeitos de postagem

![](../assets/v12_banner_post_effects2.jpg)

As renderizações no Painter agora podem ser aprimoradas com um novo conjunto de efeitos de pós-processamento disponível na janela <b>Configurações de Exibição</b>. Novas adições, como <b>Reflexo de lente</b> e <b>Granulação do filme</b>, já estão disponíveis, junto com os efeitos de <b>Profundidade de campo</b> e <b>Reflexo</b> aprimorados, entre muitos outros.

Veja um exemplo do que você pode alcançar com os novos efeitos:

![](../assets/v12_render_withpost.jpg)

* <b>Novos efeitos de pós-processamento</b>\
  Todos os efeitos de pós-processamento podem ser habilitados e configurados individualmente na janela <b>Configurações de Exibição</b>. Os efeitos são aplicados em ordem de pilha e cada um pode ser ativado ou desativado independentemente, facilitando a combinação e a experiência com diferentes resultados.

  ![](../assets/v12_display_settings_post_effects.png)
* <b>Nova lista de efeitos:</b>

  * <b>Profundidade de campo</b>: desfoca objetos fora do intervalo focal para simular o foco da lente da câmera.
  * <b>Inchar</b>: adiciona um brilho suave proveniente de áreas brilhantes da imagem.
  * <b>Reflexo</b>: cria listras de luz ao redor das fontes de luz.
  * <b>Clarão da lente</b>: simula reflexos ópticos da lente quando uma luz brilhante brilha na câmera.
  * <b>Aberração lateral</b>: simula dispersão cromática nas bordas da imagem causada por imperfeições da lente.
  * <b>Vinheta</b>: escurece os cantos e bordas do quadro para chamar a atenção para o centro.
  * <b>Nitidez</b>: aumenta o contraste da borda para tornar a imagem renderizada mais nítida.
  * <b>Granulação do filme</b>: sobrepõe um ruído sutil para replicar a textura de um filme analógico.
  * <b>Mapeamento de tons</b>: remapeia valores de luminância HDR para um intervalo exibível para uma aparência mais cinematográfica.
  * <b>Correção de cores</b>: ajusta o contraste, a saturação, o brilho e a temperatura para ajustar o equilíbrio geral de cores.

>[!NOTE]
>
> Para obter mais informações sobre os novos efeitos, consulte a [documentação dedicada](../features/post-processing/post-processing.md).

### Aprimoramento do novo projeto e da janela de configurações

![](../assets/v12_banner_project_window.jpg)

A janela do novo projeto e a caixa de diálogo de configurações do projeto foram reprojetadas para facilitar a navegação. Os parâmetros foram reordenados e agrupados para melhor legibilidade, e o fluxo de trabalho de reimportação de malha foi aprimorado para reduzir etapas repetitivas ao iterar em um projeto.

* <b>Janela de novo projeto aprimorada</b>\
  Os parâmetros na janela do novo projeto foram reorganizados e reordenados para que as configurações mais usadas sejam posicionadas com mais destaque. O layout geral agora é mais fácil de examinar, reduzindo o tempo necessário para configurar um novo projeto.
* <b>Novo fluxo de trabalho para reimportar malhas nas configurações do projeto</b>\
  Uma nova caixa de seleção <b>Reimportar malha</b> nas configurações do projeto permite reimportar a malha do projeto com mais facilidade, graças ao caminho do arquivo carregado anteriormente, que agora está sendo salvo e pré-preenchido automaticamente.

  ![](../assets/v12_project_settings.png)

## Notas de versão

## Versão 12

### 12.0.0

Data de lançamento: <b>03/2026/09</b>\
Resumo: <b>Esta é uma versão principal. Esta versão contém os recursos de camadas achatadas, distorção na geometria, novos pós-efeitos, melhoria na janela do novo projeto e outras melhorias.</b>

<b>Adicionado</b>:

* [Achatar camadas] Achatar camadas dentro da pilha de camadas
* [Achatar camadas] Exportar camadas achatadas para disco
* [Distorcer para geometria] Adicionar nova funcionalidade de distorção automática a Projeções de distorção
* [Pós-efeitos] Substituir pós-efeitos pela adição de novos
* [Pós-efeitos] Atualizar mapeador de tom
* [Pós-efeitos] Adicionar novo uso para ativos de Pós-efeitos
* [Conteúdo][Pós-efeitos] Integrar ativos de pós-efeitos padrão na biblioteca
* [Novo projeto] Aprimorar a interface do usuário para criação de projetos
* [Novo projeto] Alterações na funcionalidade de malha de reimportação
* [Novo projeto] Permitir que arquivos \*.geo.usd sejam abertos
* [Configuração do projeto] Melhorar a interface do usuário para a configuração do projeto
* Atualize a biblioteca do USD para a versão 25.05
* Atualize o Substance Engine para a versão 9.3.4
* Aumente o mínimo de drivers para 25.3.1/25.Q2 para GPUs AMD
* Atualize o Qt para 6. 8. 6
* [Script] Atualize a API JavaScript para a versão 1.1.20
* Atualizar Python para a versão 3.13

<b>Corrigido:</b>

* [Falha] Alterar uma saída de canal de material em uma máscara pode falhar
* [Import] As texturas EXR são forçadas para sRGB em vez de lineares ao importar arquivos USD
* [Blocos UV] A sequência de imagens com uma única imagem também preenche outros blocos UV
* [Preparação] O AO é diferente entre a CPU e a preparação de GPU
* [Gerenciamento de cores][MacOS] Viewport BaseColor não corresponde ao selecionador de cores
* [USD] Valores uniformes não são importados em alguns casos
