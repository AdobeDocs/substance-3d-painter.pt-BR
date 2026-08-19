---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/release-notes/version-9-0.html"
breadcrumb-title: ''
description: Consulte as notas de versão do Substance 3D Painter versão 9.0 para saber mais sobre novos recursos, aprimoramentos e correções de erros.
helpx_creative_field: ""
helpx_description: Substance 3D Painter
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Versão 9.0
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '1447'
ht-degree: 0%

---


# Versão 9.0

O <b>Substance 3D Painter 9.0</b> apresenta uma nova maneira de pintar traçados com caminho reeditável no visor 3D, bem como conteúdo padrão atualizado.

Data de lançamento: *20 de junho de 2023*

## Principais recursos

### Nova pintura ao longo do caminho na viewport 3D

![Feche um sapato de couro com um caminho desenhado por cima com sua interface auxiliar](../assets/v90_banner_path.jpg)

A ferramenta <b>Pintar ao longo do caminho</b> é uma nova maneira de pintar traçados no visor 3D. Semelhante a outros aplicativos, você pode criar curvas baseadas em Bézier orientadas por pontos na superfície do objeto 3D para desenhar padrões. Combinado com materiais de Substance, essa nova ferramenta pode abrir muitas novas possibilidades.

* <b>Nova ferramenta para criar traçados de tinta orientados por um caminho com pontos</b>\
  Dentro da barra de ferramentas da ferramenta há um novo ícone dedicado à ferramenta Caminho. Essa nova ferramenta permite desenhar curvas na superfície do modelo 3D para criar traçados de tinta. Esses traçados sempre podem ser reeditados. Quando a ferramenta estiver ativa, basta clicar na superfície da malha para adicionar um ponto. Clique em um ponto existente e pressione Delete para removê-lo.

  ![Captura de tela da interface da barra de ferramentas mostrando os três tipos de ferramentas de caminho.](../assets/v90_path_toolbar.png)

  ![Gif mostrando adição e remoção de pontos em um caminho](../assets/v90_path_add_remove_points.gif)
* <b>Arraste e mova pontos na superfície da malha</b>\
  Para editar a forma de um caminho, basta clicar e arrastar um ponto para mover ao longo da superfície do modelo 3D.

  ![Gif mostrando como mover pontos](../assets/v90_path_move_points.gif)
* <b>Feche o caminho para criar padrões perfeitos</b>\
  O caminho também pode ser fechado para criar loops, que podem ser úteis para criar padrões repetidos em torno de áreas específicas, por exemplo.

  ![Gif mostrando um caminho aberto ou fechado](../assets/v90_path_open_close.gif)

  ![Gif mostrando um caminho fechado para desenhar rebites em uma superfície mecânica](../assets/v90_path_closed_loop_demo.gif)
* <b>Reeditar caminhos (e suas propriedades) com o painel Caminho</b>\
  Quando a ferramenta Caminho estiver selecionada, o caminho criado na camada de pintura atual será listado no painel Caminho dedicado na parte superior da janela de visualização 3D. Este painel permite selecionar, excluir ou renomear o caminho para

  ![Gif mostrando o painel de caminho em ação](../assets/v90_path_panel_demo.gif)

  ![Grade mostrando as propriedades do caminho que estão sendo modificadas](../assets/v90_path_edit_properties.gif)
* <b>Compatível com outros recursos de pintura, como simetria, máscara de geometria, traçados dinâmicos etc.</b>\
  Muitas configurações de traçados de tinta regulares podem ser usadas com a ferramenta de caminho:

  * Ativar a simetria permite desenhar um caminho várias vezes, enquanto gerencia apenas um.
  * Os caminhos que estão em uma camada com uma máscara de geometria ativada podem pintar em geometria oculta

  ![Gif mostrando um caminho sendo afogado duas vezes com a ajuda da propriedade de simetria](../assets/v90_path_symmetry.gif)
* <b>Pinte com outras ferramentas, como Borracha ou Borrar</b>\
  A ferramenta Caminho também é compatível com a ferramenta Borracha e a ferramenta Borrar, desbloqueando maneiras mais avançadas de pintar e combinando traçados com a maneira fácil e reeditável de manipular pontos do caminho.

  ![Grade mostrando um ponto de caminho sendo movido e atualizando o efeito de borrão](../assets/v90_path_smudge.gif)

* <b>Salvar e reutilizar propriedades de caminho com predefinições</b>\
  Ao usar a ferramenta Caminho, você também pode salvar as propriedades do pincel como predefinições. Isso permite salvar predefinições de ferramenta que alternarão automaticamente para a ferramenta Caminho quando selecionada na janela Ativos.

>[!NOTE]
>
> Para obter mais informações, consulte a [documentação dedicada](../painting/tool-list/path.md).

### Novo conteúdo a ser usado com o recurso pintar ao longo do caminho

![Imagem mostrando um capuz com diferentes tipos de pinceladas de ponto usadas.](../assets/v90_banner_content_path.jpg)

Algumas novas predefinições de ferramenta foram incluídas nesta versão para aproveitar o novo recurso de pintura ao longo do caminho:

* Ficção científica para rack de tubos
* Enrolação
* Costura
* Topstiching
* Metal de soldadura
* Fita com zíper

![Imagem da janela Ativos mostrando as novas predefinições de ferramenta](../assets/v90_path_presets_list.png)

![Imagem mostrando um exemplo da nova predefinição de solda](../assets/v90_path_welding_demo.jpg)

### Traçados dinâmicos aprimorados para o recurso de pintura ao longo do caminho

![Imagem mostrando um traçado de caminho parecido com uma seta com uma forma redonda como o início e a ponta da seta como o final.](../assets/v90_banner_dyn_strokes.jpg)

Aproveitamos a oportunidade da nova ferramenta de caminho para adicionar novas propriedades ao sistema de traçado dinâmico. Essas novas propriedades desbloqueiam novos tipos de traçados que não eram possíveis antes, como a seta na imagem acima que apresenta um visual diferente de início e fim.

* <b>Nova propriedade Início/Meio/Fim</b>\
  Uma nova propriedade pode ser definida para especificar ao gráfico de Substance se um carimbo dentro de um traçado é o primeiro, o último ou qualquer um no meio. Isso permite criar pontos de início e fim, que podem ser muito úteis, por exemplo, para criar zíperes. (<b>Observação</b>: o estado final só está disponível com a ferramenta de caminho.)
* <b>Nova propriedade de Tamanho e Espaçamento</b>\
  A propriedade de tamanho e espaçamento permite ajustar a saída de um gráfico de Substance com base no estado atual do carimbo.
* <b>Novas propriedades de comprimento de traçado</b>\
  Ter a distância ao longo do caminho e a distância máxima de um caminho permite melhor controle quando alguns efeitos se repetem, em vez de fornecer um valor normalizado diretamente.\
  Permite criar um traçado crescente, por exemplo, mas também um traçado com um padrão de repetição baseado na distância desenhada (e não no número total de carimbos desenhados).

![Gif mostrando um caminho com um traçado dinâmico](../assets/v90_path_dyn_stroke_wave_demo.gif)

>[!NOTE]
>
> Para obter mais informações, consulte a [documentação dedicada](../painting/dynamic-strokes/creating-custom-dynamic-strokes.md).

### Materiais padrão atualizados

![Uma lista de esferas exibindo lado a lado, mostrando os diferentes novos materiais](../assets/v90_banner_materials.jpg)

Com esta versão, decidimos fazer um pouco de limpeza em nossa biblioteca e, portanto, alteramos nossos materiais de base padrão para torná-los mais úteis a todos. Estes materiais foram criados pela mesma equipe que fornece conteúdo em [Substance 3D Assets](https://substance3d.adobe.com/assets).

>[!NOTE]
>
> O conteúdo que foi removido está disponível nos [ativos da comunidade do Substance 3D](https://substance3d.adobe.com/community-assets?q=painter23update&u=painter23update).

## Tutorials

Para descobrir e aprender sobre a nova ferramenta de caminho, confira nosso tutorial mais recente:

## Notas de versão

### 9.0.0

Data de lançamento: <b>2023/06/20</b>\
Resumo: <b>Versão principal com pintura ao longo de um caminho que permite Curvas 3D, novos materiais de base e limpeza de materiais legados e novas predefinições para Curvas 3D</b>

<b>Adicionado:</b>

* [Caminho] Adiciona nova ferramenta Pintura ao longo do caminho
* [Caminho] Adiciona um atalho vazio para a ferramenta de caminho
* [Caminho] Permite adicionar novos pontos a um caminho existente
* [Caminho] Adiciona um atalho para sair da criação do caminho atual
* [Caminho] Permite editar as propriedades do pincel para caminhos
* [Caminho] Ajustar tangentes automaticamente ao inserir um ponto
* [Caminho] Recalcular tangentes quando um ponto for movido
* [Caminho] Ajustar pontos recém-criados à superfície de uma malha
* [Caminho] Permitir a edição da pressão por vértice
* [Caminho] Ajuste a pressão do ponto recém-criado a partir de pontos vizinhos
* [Caminho] Permite converter pontos em suaves/de vértice (quebra tangente)
* [Caminho] Permite mover um ponto recém-adicionado imediatamente
* [Caminho] Permite remover pontos do caminho existente
* [Caminho] Permite inverter a direção de um caminho
* [Caminho] Permite selecionar um caminho na viewport
* [Caminho] Permite selecionar pontos de caminho com seleção de letreiro
* [Caminho] Introduza atalhos de CTRL-A para selecionar todos os pontos de um caminho
* [Caminho] Permite fechar o caminho
* [Caminho] Permite especificar o caminho acima do eixo em Propriedades
* [Caminho] Adiciona um menu de controle de vértice à barra de ferramentas contextual
* [Caminho] Introduza modos de pintura/apagamento/borrar na ferramenta de caminho
* [Caminho] Criar feedback visual para caminhos no visor
* [Caminho] Adiciona um indicador visual para a direção do caminho
* [Caminho] Adiciona thickness de linha às configurações de exibição de caminho
* [Caminho] Permitir ocultar a interface do usuário de caminhos
* [Caminho] Adiciona o painel Caminho para listar os caminhos da camada atualmente selecionada
* [Caminho] Adicionar feedback visual ao passar o mouse sobre um caminho no painel Caminho
* [Caminho] Exibe o painel de caminho sempre que a ferramenta Caminho é selecionada
* [Caminho] Permite renomear, excluir, copiar, recortar, duplicar o caminho no painel Caminho
* [Caminho] Exibe a mensagem ao tentar interagir na viewport 2D com a ferramenta Caminho
* [Biblioteca] Integrar novo conteúdo (ferramentas e materiais de base de caminho)
* [Traçados dinâmicos] Adicionar propriedade de distância para traçados dinâmicos
* [Traçados dinâmicos] Adicionar propriedades de tamanho e espaçamento aos traçados dinâmicos
* [Traçados dinâmicos] Adicionar propriedade início/meio/fim para traçados dinâmicos
* [Python]&#x200B;[USD] Expor parâmetros de configuração de projeto para o formato USD
* [Python]&#x200B;[USD] Expor os parâmetros de criação de projetos para o formato USD
* [Export]&#x200B;[USD] Adicionar informações do caminho do projeto no arquivo USD exportado
* [GLTF] Atualizar texturas na biblioteca ao recarregar um arquivo GLTF
* [Shader] Reduzir artefatos de costura para Ilhas UV com orientação diferente
* [Engine] Atualização para o mecanismo de Substance versão 9.0

<b>Corrigido:</b>

* [Importar] Algumas GLB com texturas não obtêm texturas no Painter
* [AMD] Artefatos em bordas para todos os preenchimentos de projeção 3D
* [Engine] As texturas se quebram ao alternar a visibilidade da camada
* [Engine] As texturas ficam vazias em alguns locais ao alterar o modo de mesclagem
* [Engine] A Textura/Projeção é o modo de distorção vazio em alguns casos
* [Iray] A iteração é redefinida para 0 ao salvar a renderização
* [Log] Mensagem de erro do USD ao executar File > New

<b>Problemas Conhecidos:</b>

* [Gerenciamento de cores] As conversões do espaço de cores HDR com ACE no Linux produzem cores vivas
* [Pilha de camadas] Fonte de entrada não salva por camada
