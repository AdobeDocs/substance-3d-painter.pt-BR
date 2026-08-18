---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/release-notes/old-versions/version-7-3.html"
breadcrumb-title: ''
description: Consulte as notas de versão do Substance 3D Painter versão 7.3 para saber mais sobre novos recursos, aprimoramentos e correções de erros.
helpx_creative_field: ""
helpx_description: Painter > Release notes > Old versions > Version 7.3
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Versão 7.3
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '1822'
ht-degree: 0%

---


# Versão 7.3

O **Substance 3D Painter 7.3** traz novas maneiras de texturizar malhas com as novas projeções de distorção e cilindro para camadas de preenchimento.

Data de lançamento: *13 de outubro de 2021*

## Principais recursos

### Nova projeção de distorção

![](../../assets/proj-warp.jpg)

Esta versão apresenta a nova projeção de distorção 3D para camadas de preenchimento e efeitos de preenchimento. Essa projeção permite distorcer uma textura ou uma imagem com a ajuda de uma grade de deformação e pontos controláveis.

* **Configuração rápida via arrastar e soltar** Escolha um material, uma alfa, uma textura ou um procedimento na biblioteca Ativos, arraste e solte na parte desejada da malha (atalho **ALT** necessário para Materiais). Se o seu ativo não for um material, um pop-up com indagação de qual canal você gostaria de atribuí-lo.\
  Depois que a camada for criada, você verá que a nova *Projeção de distorção* é selecionada automaticamente. A camada tem controles de modo de projeção 3D padrão, mas também um novo parâmetro *Profundidade de projeção* que permite definir a profundidade da projeção de distorção (representada por setas verdes como uma fila visual).\
  Você também pode selecionar esse modo de projeção manualmente em qualquer camada de preenchimento ou efeito sem ter que arrastar e soltar um ativo na viewport.

  ![](../../assets/drop-viewport-warp.gif)

* **Posicionamento automático com a ferramenta Superfície** Quando a nova camada de Distorção for criada, você verá que a ferramenta Superfície está selecionada automaticamente. Isso permite que você mova a imagem para que ela permaneça na superfície da malha o tempo todo. No entanto, você sempre pode alternar para qualquer um dos outros manipuladores e ajustar sua conversão (atalho **W**), rotação (atalho **E**) ou escala (atalho **R**). Para retornar à ferramenta Superfície, use o atalho **SHIFT + W**. Ao alternar para o modo *Editar vértices*, a ferramenta Superfície também é a seleção padrão e ajusta o movimento do vértice à superfície da sua malha. No entanto, você pode substituir temporária e rapidamente a ferramenta de superfície **mantendo a tecla CTRL**, o que permite mover o ponto selecionado em qualquer direção, não apenas na superfície.

* **Grade de distorção facilmente editável** Depois que o posicionamento global da imagem for concluído, também será possível editar a própria grade de distorção para maior precisão e flexibilidade. Para entrar no modo de edição de grade, use o menu de distorção recém-adicionado ou o atalho **SHIFT + V**. Isso permitirá editar os vértices existentes da grade.\
  Você pode subdividir uniformemente a grade como um todo, mas tenha em mente que, se você tiver movido anteriormente os vértices, eles serão redefinidos para suas posições originais. A subdivisão de grade pode ser feita por meio do novo menu de opções de distorção.\
  Alternativamente, é possível adicionar divisões colocadas individualmente, o que permitiria ter mais detalhes apenas onde necessário. Para adicionar divisões, selecione qualquer uma das três opções no menu Distorcer - transversal, horizontal ou verticalmente. Quando um deles é selecionado, passar o cursor sobre a projeção Distorcer e clicar em qualquer lugar dentro dela adicionará uma nova divisão. Isso não alterará a posição dos pontos existentes.

  ![](../../assets/warp-split.gif)
* **Ajuste automático da orientação do vértice** Por padrão, as tangentes de vértices individuais são ajustadas à superfície da malha, o que significa que elas sempre estarão corretamente orientadas em relação à malha, independentemente de onde sejam arrastadas. Esta opção de tangente automática pode ser desativada por meio de um novo botão na barra de ferramentas contextual, caso em que a orientação permanecerá fixa em todos os momentos.

  ![](../../assets/warp-tangent-adjustment.gif)

Para obter mais informações sobre as configurações e propriedades da projeção de Distorção, consulte a [página de documentação dedicada](../../painting/fill-projections/warp-projection.md).

### Nova projeção de cilindro

![](../../assets/cylinder-proj.jpg)

Esta versão adiciona um método de projeção cilíndrica para camadas de preenchimento e efeitos de preenchimento. A nova projeção permite ajustar uma imagem ou textura ao redor de objetos, como colunas, pilares ou formas mais orgânicas, como os braços de um personagem.

* **Quebrar uma imagem em torno de uma malha**\
  Você pode quebrar uma imagem facilmente ao redor de uma superfície cilíndrica usando uma camada de preenchimento ou um efeito de preenchimento e selecionando *Projeção cilíndrica* no menu suspenso Projeção. Se a imagem não precisar ser repetida fora do gizmo de projeção, você precisará selecionar *Nenhum* para o *Empacotamento UV* e *Cortado na forma* no *Corte de forma* para garantir que a imagem não saia dos limites. Então você só precisa usar o manipulador para ajustar a projeção para a posição desejada.

* **Ajustar o ângulo de projeção**\
  Quando a imagem é inserida, há uma nova configuração de Ângulo disponível. Essa configuração pode ser usada para ajustar se a imagem é projetada ao redor da forma cilíndrica ou se é restrita a um certo ângulo. Ela não corta a imagem, mas reduz sua largura.

  ![](../../assets/cylindrical-angle.gif)

Para obter mais informações, consulte a [página de documentação dedicada](../../painting/fill-projections/cylindrical-projection.md).

### Seletor de cores aprimorado

![](../../assets/colorpicker-banner.jpg)

Esta versão traz várias melhorias de qualidade de vida para o seletor de cores.

* **Novo layout de janela**\
  A janela do seletor de cores aprimorada foi reformulada para acomodar um layout mais vertical, semelhante à versão mais recente do Sampler. Ele está dividido em três seções: o campo de cores principal, que inclui a seleção atual e a última, o campo hexadecimal, o conta-gotas e o controle deslizante de matiz; a seção de controles deslizantes RGB/HSV manuais; e as amostras.\
  ![](../../assets/colorpicker.jpg)

* **Novos valores de RGB 0 a 255**\
  Além de portar as maneiras existentes de inserir o valor da cor, o seletor de cores aprimorado também permite trabalhar em valores de RGB 0 a 255. Esta opção está disponível quando a opção *Valores de ponto flutuante* está desmarcada no menu suspenso da seção de controles deslizantes.

  ![](../../assets/colorpicker-floatingpoints.jpg)
* **Salvando amostras de cores**\
  As amostras de cores agora podem ser salvas no Painter. Depois que a cor desejada for selecionada, é possível pressionar o botão de adição na seção Amostras do seletor de cores, e a cor será armazenada em sessões e projetos. Uma amostra pode ser removida clicando com o botão direito do mouse nela ou, como alternativa, é possível excluir todas as amostras em massa de uma vez por meio do menu suspenso desta seção. Não há limite para o número de amostras que podem ser salvas.

  ![](../../assets/colorpicker-swatches.gif)
* **A janela do seletor de cores permanece aberta**\
  A janela do seletor de cores agora pode ser movida e colocada em qualquer lugar, mesmo em uma tela diferente, e permanecerá aberta desde que não haja nenhuma alteração de contexto, o que significa que, ao alternar entre camadas de tinta ao pintar texturas à mão, você pode manter a janela do seletor de cores aberta para facilitar o acesso.

  ![](../../assets/picker-persistent.gif)

* **Conta-gotas mais acessível**\
  O conta-gotas de seleção de cores pode ser encontrado diretamente ao lado do campo de cores, mas também é possível encontrá-lo no seletor de cores. O conta-gotas mais acessível mantém todas as funcionalidades anteriores - você ainda pode clicar e manter pressionado para escolher uma cor em qualquer lugar da tela. Esse conta-gotas exposto pode ser encontrado ao lado de todos os campos de cores no Painter, não apenas dos canais de camada.

  ![](../../assets/eyedropper-5.jpg)

Para obter mais informações, consulte a [página de documentação dedicada](../../interface/color-picker.md).

### Outros recursos e melhorias

* **Melhorias ao arrastar e soltar ativos**\
  Com a introdução da Distorção, o recurso de decalque, onde os ativos podem ser arrastados e soltos da biblioteca para a viewport enquanto mantêm o ALT, viu algum retrabalho. Agora, quando um decalque é criado dessa maneira, ele não usa mais a projeção Planar, mas a projeção Distorcer. A seleção automática da projeção de distorção deve melhorar a velocidade e a eficiência dos ajustes de decalque na malha.\
  Além disso, agora é possível arrastar e soltar não apenas materiais, mas ativos de tipo de imagem na viewport. Ao selecionar um alfa, uma textura ou um procedimento, não há necessidade de usar o modificador ALT. Ela pode ser solta na malha - isso acionaria um menu com a opção de selecionar se essa imagem deve ser usada dentro de uma máscara ou de qualquer um dos canais da camada.

  ![](../../assets/improved-decal.gif)

* **Aprimoramento do plug-in de salvamento automático**\
  O salvamento automático não será mais acionado durante operações mais longas ou mais pesadas, como recarregamento de malha, cozimento ou exportação.

* **Melhorias de desempenho**\
  Algumas operações de manutenção e otimização foram realizadas para manipulação de controles deslizantes e desempenho de pintura.

* **Novas funções na API Python**\
  A API Python tinha visto algumas adições recentes, que permitem recarregar malha, atualizar recursos, bem como definir e consultar a resolução de blocos UV via script.

* **atualização do mecanismo de Substance 8.3.0**\
  Juntamente com algumas correções e melhorias gerais, esta atualização do mecanismo Substance agora leva em consideração novos tipos de gráficos. Também é possível verificar a versão do arquivo .sbsar, o que deve melhorar o uso e o download das versões apropriadas do Substance 3D Assets.

* **Recebendo Substance 3D Assets da CC para desktop**\
  Agora é possível acessar Substance 3D Assets, como Materiais, Atlas e Decalques, pelo aplicativo de desktop da CC. Além disso, eles podem ser enviados diretamente para a biblioteca da Painter.

## Notas de versão

### 7.3.0

*(Lançado Em 13 De agosto De 2021)*\
Resumo: **Versão principal. Contém uma nova projeção de distorção 3D, uma nova projeção cilíndrica, melhorias no seletor de cores, novas funções na API Python e correções de erros**

**Adicionado:**

* [Projeção][Distorcer] Expor distorção 3D como um novo modo de projeção
* [Projeção][Distorcer] Permitir modo de decalque para Alpha, Texturas e Procedimentos com arrastar e soltar no visor
* [Projeção][Distorcer] Usar projeção de distorção com atalho de decalque (ALT)
* [Projeção][Distorcer][Barra de ferramentas] Transformar distorção como um todo ou por vértices
* [Projeção][Distorcer][Barra de ferramentas] Adicionar pontos de grade com opções dividir distorção cruzada, horizontal ou verticalmente
* [Projeção][Distorção][Barra de ferramentas] Menu dedicado para ações de redefinição
* [Projeção][Distorção][Barra de ferramentas] Opção para ajustar automaticamente as tangentes ao mover os pontos
* [Projection][Warp][Toolbar] Menu dedicado para edição de grade (tamanho, redefinição, cor e tamanho da alça)
* [Projeção][Distorcer] Novo atalho de teclado para alternar o modo de edição de distorção de vértices inteiros (SHIFT+V)
* [Projeção][Distorcer] Clicar + Ctrl permite alternar entre a ferramenta de superfície e outras ferramentas
* [Projeção][Cilíndrica] Expor o modo de projeção cilíndrica
* [Projeção][Barra de ferramentas] Configurações do manipulador de grupo (tamanho, etapas da grade, etapas do ângulo)
* [Seletor de cores] Nova interface do seletor de cores
* [Seletor de cores] Usar valores sRGB nos widgets do seletor de cores
* [Seletor de cores] Permite salvar e excluir amostras de cores
* [Seletor de cores] Conta-gotas acessível por meio de cores e slots normais
* [Seletor de cores] Permite editar cores dinâmicas entre 0 e 255 valores
* [Seletor de cores] Tornar o estado HSV/RGB comum no aplicativo
* [Seletor de cores] A janela do Seletor de cores é semipersistente
* [Seletor de cores] Pressionar Esc fecha a janela do seletor de cores
* Melhoria de desempenho para interação de interface e ao pintar
* [Engine] Atualização para a nova versão do mecanismo de Substance (8.3.0)
* [Scripting][Python] Permite recarregar a malha do projeto atual
* [Scripting][Python] Permitir atualização de recursos em projetos
* [Scripting][Python] Permite definir e consultar a resolução de blocos UV
* [Interoperabilidade] Não disponível para as edições Steam e Substance
* [Interoperabilidade] Receber vários recursos do Bridge

**Corrigido:**

* O seletor de cores não exibe a cor correta
* [Preparação] A lista de conjuntos de texturas não está ordenada corretamente
* [Importação de FBX] As transformações de tabela dinâmica de grupo 3ds Max não são levadas em consideração
* [Substance Engine] Falha com importação de SBSAR corrompido
* [MacOS] A opção de configuração do projeto em idiomas diferentes não está presente
* Os salvamentos automáticos podem congelar o Painter durante processos longos

**Problemas Conhecidos:**

* [Projeção][Distorcer] A opção Dividir permanece selecionada após a conclusão da divisão
* [Projeção][Distorcer] O recurso Inverter não funciona quando a transformação está definida como espaço global
* [Projeção][Distorção] Linhas de artefato entre correções em alguns casos raros
* [Projeção][UV] O ponto dinâmico é redefinido ao inverter a projeção
* [Mac M1] Os materiais inteligentes não são exibidos corretamente
* [M1][Regressão] Camadas de material não funcionando
