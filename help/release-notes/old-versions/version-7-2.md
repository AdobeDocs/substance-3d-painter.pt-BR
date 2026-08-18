---
helpx_url: "https://helpx.adobe.com/br/substance-3d-painter/release-notes/old-versions/version-7-2.html"
breadcrumb-title: ''
description: Consulte as notas de versão do Substance 3D Painter versão 7.2 para saber mais sobre novos recursos, aprimoramentos e correções de erros.
helpx_creative_field: ""
helpx_description: Painter > Release notes > Old versions > Version 7.2
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Versão 7.2
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '2333'
ht-degree: 1%

---


# Versão 7.2

O **Substance 3D Painter 7.2** traz novos recursos de renderização com o fluxo de trabalho de Material Padrão da Adobe, novas maneiras de compartilhar conteúdo em [aplicativos da Substance 3D](https://www.adobe.com/br/products/substance3d/3d-augmented-reality.html) e uma janela de Ativos revisada.

Data de lançamento: *23 de junho de 2021*

## Principais recursos

### Janela Novos Ativos

![](../../assets/banner-assets.jpg)

A antiga janela Prateleira foi aprimorada e renomeada como janela Ativos. Esse novo design visa tornar o conteúdo mais rapidamente acessível e mais fácil de filtrar com os novos ícones dedicados. Ele também vem com um sistema de navegação mais fácil com as trilhas de navegação. Esse novo design também visa tornar a experiência semelhante a outros softwares da Substance 3D, para facilitar o gerenciamento de conteúdo entre aplicativos.

>[!NOTE]
>
> Esta versão introduz alterações na forma como gerenciamos as preferências do aplicativo e o conteúdo de Prateleira/Ativos. Para saber como migrar seus dados, dê uma olhada na [página dedicada](../../pipeline-and-integration/resource-management/preferences-and-content-migration.md).

* **Novo design e layout**\
  O novo design se concentra na simplicidade, mas também em uma organização mais fácil da janela. A janela agora pode ser encaixada verticalmente sem perder espaço. Um novo modo de exibição de “lista” permite pesquisar ativos por nome com muito mais facilidade.

  ![](../../assets/assets-vertical.png)

* **Nova navegação de navegação estrutural**\
  Às vezes, o recurso de navegação pode ser difícil em uma interface de usuário pequena. Com a navegação estrutural, não é mais fácil alternar entre pastas sem exibir toda a hierarquia de pastas.

  ![](../../assets/breadcrumbs-2.png)

* **Novos filtros de uso**\
  Há muitos conteúdos diferentes na janela Ativos, e os usos são uma boa maneira de filtrar conteúdo e isolar recursos específicos. Para selecionar um uso específico, basta clicar no botão dedicado. Para adicionar ou remover vários usos, pressione e mantenha a tecla CTRL enquanto clica em um botão.

  ![](../../assets/demo-filters.gif)

* **Renderização de miniatura aprimorada**\
  Aproveitamos o tempo para retrabalhar nosso sistema de geração de miniaturas para melhorar a qualidade e torná-los mais consistentes em todo o ecossistema do Substance 3D. Também adicionamos o suporte ao deslocamento.

  ![](../../assets/cropped-icons-before-after.jpg){width="500px"}

* **Carregando miniaturas de arquivos de Substance (sbsar)**\
  Miniaturas personalizadas incorporadas em arquivos Substance não são carregadas e exibidas na janela Ativos. Compartilhar recursos personalizados agora ficou mais fácil, pois não há necessidade de incluir os metadados de recursos para ícones personalizados.

* **Desempenho aprimorado** O carregamento e o tempo de geração das miniaturas foram aprimorados em vários aspectos e agora devem ser muito mais rápidos.

* **Aumentar o orçamento de memória de visualização para carregar mais miniaturas**\
  Por padrão, uma quantidade limitada de memória é alocada para a exibição de miniaturas para economizar em desempenhos. Ter uma biblioteca com muitos recursos, no entanto, pode levar a carregar e descarregar miniaturas constantemente, o que dificulta a navegação e a pesquisa de recursos. Agora há uma nova [variável de ambiente](../../pipeline-and-integration/configuration/environment-variables.md) para substituir o valor de orçamento padrão.

### Novo fluxo de trabalho de materiais padrão da Adobe

![](../../assets/banner-asm.jpg)

Um novo sombreador foi adicionado, denominado **Material Padrão da Adobe** (ASM), que oferece suporte a vários recursos de uma só vez, permitindo criar materiais mais complexos e precisos em um único Conjunto de Texturas. Com este novo sombreador também aproveitamos a oportunidade para adicionar novos canais para tornar a criação de materiais mais fácil também.

* **Novo sombreador de materiais padrão da Adobe**\
  O novo sombreador ASM é um sombreador que reagrupa várias funcionalidades, bem como uma evolução da renderização do PBR. Ele suporta ao mesmo tempo:
  * **Anisotropia**
  * **Revestimento claro**
  * **Brilho**
  * **Specular edge color**
  * **Métodos adicionais de dispersão da subsuperfície**
  * E, claro, os outros recursos existentes, como Oclusão de Parralax, Deslocamento, etc.

* **Novos canais e canais de usuário**\
  Para suportar o novo sombreador ASM, novos canais foram adicionados. Também dobramos o número de usuários e canais para expandir as possibilidades de informações personalizadas e shaders personalizados.
  * Cor do revestimento
  * Rugosidade do revestimento
  * Normal do Revestimento
  * Opacidade do revestimento
  * Nível da Especular do Revestimento
  * Cor de dispersão
  * Cor do brilho
  * Rugosidade do brilho
  * Opacidade do brilho
  * Cor da aresta da especular
  * Canais de usuário de 8 a 15

* **Configurações de conjunto de textura aprimoradas**\
  O menu de lista de canais nas configurações do Conjunto de texturas agora agrupa os canais com base em sua compatibilidade com o sombreador atual. Isso ajuda a identificar quais canais terão um efeito na viewport.

  ![](../../assets/channel-list-grouping.png)

* **Novos recursos do API de sombreamento com if visível e recompilação**\
  Com o desenvolvimento do sombreador ASM, algumas alterações na API foram feitas com dois recursos notáveis:
  * **Visível If**: os parâmetros de sombreador podem ser mostrados ou ocultados com base na condição, facilitando a leitura da interface do usuário do sombreador.
  * **Recompilação**: declarando parâmetros de uma maneira específica, agora é possível desabilitar parte de um sombreador e recompilá-lo para otimizá-lo quando o parâmetro for alterado. Isso permite descartar funcionalidades não utilizadas.

### Novo intercâmbio de ecossistemas do Substance 3D

![](../../assets/banner-send-to.jpg)

Enviar recursos e ativos entre aplicativos da Substance 3D agora é muito mais fácil e acessível com um clique usando esse novo fluxo de trabalho. Agora é possível receber arquivos de Substance do Substance 3D Designer ou do Substance 3D Sampler ou enviar um projeto para o Substance 3D Stager com muita facilidade para iterar rapidamente no conteúdo.

>[!WARNING]
>
> Essas funcionalidades de envio e recebimento só estão disponíveis por meio da versão Creative Cloud para desktop do aplicativo, pois ele depende de tecnologias específicas para torná-lo possível. Isso significa que a versão Steam ou Substance 3D autônoma não suporta esses recursos.

* **Painter para Stager**\
  Exporte do Painter para o Stager com a predefinição de exportação atualizada ou use a ação **Enviar para o Substance 3D Stager** para exportar e importar automaticamente o projeto atual no Stager. Nenhuma configuração manual necessária.

* **Stager para Painter**\
  Receba modelos do Stager para texturizar com uma ação semelhante de um clique diretamente do Stager.

* **Do Designer ou do Sampler para o Painter**\
  Receba materiais de Substance, filtros e muito mais do Designer ou Sampler diretamente na janela Ativos com um clique.

* **Substance 3D Assets para Painter**\
  Receba conteúdo como material de Substance da área de trabalho do Creative Cloud diretamente na janela Ativos do Painter.

* **Mostrar no Bridge**\
  Os recursos da janela Ativos localizados em uma biblioteca gerenciada pelo Adobe Bridge podem ser abertos no Bridge diretamente usando o menu do botão direito sobre um recurso específico.

### Novo conteúdo

![](../../assets/banner-content-5.jpg)

Um novo conteúdo foi adicionado nesta versão:

* **Novos modelos de projeto para Adobe Stand Material (ASM)**\
  Para facilitar o uso do novo sombreador do ASM, novos modelos de projeto foram criados para acelerar a criação do projeto:
  * ASM - aspereza metálica de PBR
  * ASM - Ângulo de Anisotropia de aspereza metálica de PBR
  * ASM - Revestimento de aspereza metálica PBR
  * ASM - PBR Metallic Roughness SSS
  * ASM - Brilho de aspereza metálica PBR

* **Novos mapas de ambiente**\
  Vários novos mapas de ambiente foram adicionados para iluminar seus projetos, incluindo o Studio 06 usado para renderizar as novas miniaturas de ativos:
  * Interior:
    * Atelier
  * Studio:
    * Studio 06
    * Studio 80s Horror Flick A
    * Estúdio preto suave
    * Estúdio branco suave
    * Guarda-chuva branco de estúdio

### Desencapsulamento Automático UV Aprimorado

![](../../assets/banner-uv.jpg)

Uma nova atualização do desempacotamento automático de UV foi adicionada, que traz o suporte de blocos UV e controle adicional sobre a geração de UV:

* **Quantidade de Blocos UV**\
  Ao gerar UVs, agora é possível especificar o número máximo de blocos UV desejados a serem criados. Isso permite usar a geração UV com o fluxo de trabalho UV Tile também.

* **Orientação da Ilha UV**\
  Um novo parâmetro foi adicionado para adicionar uma restrição na orientação da Ilha UV quando empacotado. Isso permite fazer Ilhas UV um pouco mais alinhadas, permitindo texturizar alguns objetos com mais facilidade (por exemplo: uma porta de madeira para alinhar o padrão da madeira).

* **Desempenho de embalagem aprimorado**\
  A função de embalagem foi melhorada, bem como para oferecer bom desempenho com o novo suporte UV Tile.

### Melhorias gerais

![](../../assets/banner-misc-2.jpg)

Esta nova versão adiciona várias melhorias na qualidade de vida:

* **Desempenho aprimorado dos controles deslizantes com a caneta do tablet gráfico**\
  Arrastar pelos controles deslizantes com uma caneta agora deve ser muito mais responsivo. Os controles deslizantes não devem mais se sentir pegajosos.

* **Desempenho aprimorado com camadas já pintadas**\
  Pintar em uma camada com muitos traçados de pincel existentes agora deve ser muito mais rápido e não deve mais levar à lentidão.

* **Pintura mais rápida após abrir um projeto**\
  Agora é imediato pintar uma camada no topo da pilha de camadas logo após abrir um projeto. O cálculo do cache do mecanismo foi adiado para depois, tornando a reedição de projetos antigos um pouco mais rápida neste contexto.

* **Método normal nítido**\
  Há um novo parâmetro de método Height para Normal nas configurações do Conjunto de texturas que permite controlar como o canal de Height é convertido em um mapa normal. Esse novo parâmetro é útil para melhorar a qualidade das superfícies com muitos detalhes variáveis, como materiais de tecido.

  ![](../../assets/normal-mode.jpg){width="450px"}

* **Novo estilo de interface**\
  A interface geral foi ligeiramente ajustada para se alinhar melhor ao ecossistema geral do Substance 3D. Isso torna o salto de um aplicativo para outro menos surpreendente e mais fácil de navegar.

* **Novas traduções**\
  Três novos idiomas foram adicionados para traduzir a interface do programa:
  * Francês
  * Alemão
  * Chinês simplificado

## Notas de versão

### 7.2.0

*(Lançado Em 23 De junho De 2021)*\
Resumo: **Versão principal, fornece uma atualização para o painel de ativos, um novo sombreador com acesso a novos canais e parâmetros, uma atualização geral da interface do usuário, algumas melhorias de desempenho muito solicitadas, suporte a idiomas expandido e muito mais!**

**Adicionado:**

* [Bibliotecas] Novo painel Ativo para substituir a prateleira
* [Libraries][UI] Novo layout do painel Ativos
* [Bibliotecas][IU] Alterar a orientação padrão do painel Ativos e a interface do usuário
* [Bibliotecas][IU] Introduzir uma opção de exibição de lista na biblioteca
* [Bibliotecas][IU] Nova navegação de trilha no Painel de ativos
* [Bibliotecas][IU] Selecione “Todas as bibliotecas” ao selecionar uma pesquisa salva
* [Bibliotecas][IU] Selecione “Todas as bibliotecas” quando todas as pastas estiverem desmarcadas
* [Libraries][UI] Nova marca para pincéis de partícula
* [Bibliotecas][IU] Substituído “prateleira” por “Todas as bibliotecas” no aplicativo
* [Bibliotecas][IU] Permitir ocultar pastas vazias
* [Libraries][UI] A biblioteca de usuário padrão deve estar visível mesmo que vazia
* [Bibliotecas][IU] Novo método de filtragem por meio de ícones de tipo de ativo
* [Bibliotecas] Atalho “CTRL” para selecionar vários tipos de ativos
* [Bibliotecas] Nova variável de ambiente para controlar o orçamento de memória de visualização do ativo
* [Bibliotecas][Conteúdo] Novos mapas de ambiente
* [Libraries][Content][UI] Renderizar deslocamento em materiais padrão
* [Bibliotecas][Conteúdo] Definir sombreador de Material Padrão da Adobe (ASM) como padrão para a geração de visualizações
* [Bibliotecas][Conteúdo][ASM] Novos modelos de projeto para o novo sombreador ASM
* [Bibliotecas][Miniatura] Usar o novo mapa de ambiente do Studio 6
* [Bibliotecas][Miniatura] Ler miniatura no recurso em vez de gerá-lo
* [Bibliotecas][Miniatura] Adicionar deslocamento à geração de miniaturas
* [Configurações do conjunto de texturas]
* [Configurações do conjunto de texturas][IU] Expor novo height ao método de conversão normal
* [Configurações de conjunto de textura][IU] Retrabalho da organização da interface do usuário dos canais
* [Configurações do conjunto de textura] Limite de canais do usuário aumentado para 16 canais
* [Configurações do conjunto de texturas][IU] Indicar quais canais são compatíveis com o sombreador selecionado no momento
* [Shader][ASM] Novo sombreador de material padrão da Adobe
* [Shader][ASM] Suporte adicionado para Anisotropia, Revestimento transparente, Dispersão subsuperficial, Specular edge color e Brilho
* [Shader][ASM] Alterar valores de cor dos canais padrão
* [Shader][ASM][Export] Modelo de exportação atualizado do Adobe Dimension para o Adobe Substance 3D Stager
* [Shader][ASM] Rótulos e dicas de ferramentas adicionados para os parâmetros de sombreador e MDL
* [Shader][ASM] Tornar a Cor da Dispersão visível na Exibição 2D mesmo se o SSS não for suportado
* [Shader][ASM][Iray] Suporte ao sombreador ASM no Iray com o novo MDL
* [Shader][ASM][Iray] Espalhamento de subsuperfície atualizado no brilho e na superfície revestida das especificações de PBR legadas
* [Shader][ASM][Content] Alterou o tipo de SSS padrão para amostras
* [Shader][ASM] Documentação adicionada para a API do ASM
* [Shader][ASM] Otimizar sombreadores para ignorar canais não usados
* [Shader] Expor novos canais de conjunto de textura
* [Shader] Dispersão de subsuperfície aprimorada
* [Shader] Novos parâmetros de sombreador ocultos para alguns sombreadores
* [Sombreador] Visível se for para parâmetros de sombreador
* [Desempenho]
* [Bibliotecas] Melhorias no tempo de carregamento da visualização de recursos e no desempenho do cálculo
* [Engine] Melhorias no desempenho da pintura
* [Desencapsulamento automático] Melhorias no desempenho da Embalagem
* [Abrir Automaticamente]
* [Auto Unwrap] Auto unwrap compatível com o fluxo de trabalho de bloco UV
* [Desenvolver automaticamente] Nova opção para posicionar UVs de acordo com a orientação da malha
* [Outro]
* [Configurações] Direção de zoom padrão alterada
* [UI] Atualização geral da interface do usuário
* [UI] Retrabalho do menu Ajuda
* [IU] Ícone Substituir inversão
* [UI][Plug-in] Ícone de substituição do link dcc do plug-in
* [UI][AMD] Atualizar a versão mínima necessária e a mensagem pop-up
* [Pilha de camadas] Cria nova camada dentro da pasta vazia selecionada
* Atualizar Documentação do Python
* [Marca]
* [Branding][UI] Atualização do nome do aplicativo para Adobe Substance 3D Painter
* [Branding][UI] Versão autônoma atualizada para &#39;Substance edition&#39;
* [Branding][UI] Nome executável atualizado do aplicativo, caminho de instalação, pacote e ícones
* [Branding][UI] Biblioteca e caminho padrão renomeados
* [Branding][UI] Atualizado Sobre o Windows
* [Branding][UI] Tela de boas-vindas atualizada
* [Branding][UI] Número de versão anual removido
* [Localização] Novas traduções para alemão, francês e chinês simplificado
* [Interoperabilidade] Não disponível para as edições Steam e Substance
* [Interoperabilidade] Interoperabilidade com o ecossistema Adobe: Designer, Sampler, Stager e Bridge
* [Interoperabilidade][IU] Receber e atualizar ativos do Designer
* [Interoperabilidade][IU] Receber ativo do Sampler
* [Interoperabilidade][IU] Enviar ativo para o Stager
* [Interoperabilidade][IU] Mostrar no Adobe Bridge
* [Interoperabilidade][IU] Permitir acesso rápido a ativos Adobe 3D
* [Interoperabilidade] Novas tags de uso do sbsar
* [Interoperabilidade] Gerenciar tipos de ativos recebidos
* [Interoperabilidade] Os ativos recebidos do Adobe Substance 3D Designer ou do Adobe Substance 3D Sampler são armazenados na biblioteca padrão escolhida pelo usuário
* [Interoperabilidade][IU] Novo ícone na barra de ferramentas à esquerda para enviar ao Stager ou Photoshop

**Corrigido:**

* [Tablet] Baixo desempenho ao pintar com pressão
* [Tablet] Problema em tablets com controles deslizantes
* [Falha] Incompatibilidade de nome entre a lista do conjunto de texturas e o exportador
* [Falha][Bibliotecas] Clique duas vezes em uma subbiblioteca
* [Bibliotecas] Problema ao Rastrear diretórios de bibliotecas
* [Bibliotecas] A linha de comando para forçar geração de visualização não funciona conforme o esperado
* [Bibliotecas][Conteúdo] O filtro Ambiente de luz assada está preto por padrão
* [Linux][MacOS][Export Mesh] Não é possível importar glTF criado no Linux/MacOS
* [Linux] Arrastar e soltar um arquivo no painel Ativos pode causar uma falha
* [Desfazer quebra automática] O ajuste automático está disponível mesmo se uma malha não tiver sido selecionada para recarregamento
* [Partículas] Comportamento de partícula incorreto com a gravidade
* [Pilha de camadas] O histograma de nível só pode usar a Luminância com alguns canais
* [Máscara de geometria] O menu do botão direito do mouse em uma pasta quando a edição da máscara de geometria não funciona
* [Projeção] Costura com projeção esférica e filtragem bilinear
* [UV Tiles] Exportar máscara para arquivo exporta somente bloco 0, 0
* [Exportar malha] A exportação de malha FBX está vazia
* [Iray] O mapa normal não é levado em consideração em novos projetos ao renderizar
* [Salvar] Problemas ao salvar em unidades compartilhadas
* [Preparação] Reassentar uma malha com parâmetros modificados exibe um aviso
* [Cozimento][Regressão] Resultado incorreto quando a caixa delimitadora global de grandes malhas polidas não inclui a origem da cena
* [Python] Bibliotecas de usuários personalizadas não são levadas em consideração

**Problemas Conhecidos:**

* [Bibliotecas] As pesquisas salvas não são salvas se nenhum projeto for aberto
* [NVIDIA] Mensagem para driver desatualizado mesmo se o driver estiver atualizado
