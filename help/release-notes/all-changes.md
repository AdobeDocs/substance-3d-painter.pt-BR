---
helpx_url: 'https://helpx.adobe.com/substance-3d-painter/release-notes/all-changes.html'
breadcrumb-title: ''
description: Revise todas as alterações e atualizações nas versões do Substance 3D Painter para acompanhar a evolução e as melhorias de recursos ao longo do tempo.
helpx_creative_field: ''
helpx_description: Painter > Release notes > All Changes
helpx_experience_level: ''
helpx_learn_topic: ''
helpx_tags: ''
title: Todas as alterações
user-guide-description: ''
user-guide-title: ''
hold: false
source-git-commit: 77c68a586777b200c4d814928c5e93a752e1d355
workflow-type: tm+mt
source-wordcount: '33932'
ht-degree: 0%

---


# Todas as alterações

Esta página contém notas de versão de todas as versões anteriores do Substance 3D Painter, classificadas da mais recente para a mais antiga.

>[!NOTE]
>
> Para exibir os problemas conhecidos que podem afetar o Painter, consulte a [página de documentação dedicada](known-issues.md).

## Versão 12

### 12.1.2

Data de lançamento: **08/2026/03**

Resumo: **Versão secundária**

**Corrigido:**

* \[Falha\] Alguns Substance podem levar a uma falha quando renderizados
* \[Falha\] Reimportar malha enquanto estiver no modo de cozimento
* \&lbrack;Falha ao inicializar a exibição de gráficos pode levar a uma falha
* \[Falha\] A exportação de texturas pode falhar em alguns casos ao atualizar o registro
* \[Falha\] Falha no modo de cozimento em alguns casos ao carregar/atualizar o mapa do ambiente
* \[Preparação\] Reiniciar o bake após modificar o arquivo poli alto pode levar a um congelamento
* \[Enviar para o Photoshop\] Falha ao exportar a máscara da camada
* O resultado do ponto de ancoragem do \[Mecanismo\] não é renderizado entre uma máscara e um canal de cor

### 12.1.1

Data de lançamento: <b>07/2026/09</b>

Resumo: versão secundária

Adicionado:

* [Cozimento de inclinação] Expor o modo normal da base de inclinação: malha ou por triângulo
* [Propriedades] Faça com que as cores uniformes sejam sempre redefinidas para o valor padrão do canal
* [OpenPBR] Reagrupe canais por categorias na janela Exportar Texturas para criação de modelos de saída
* Atualize o mecanismo de Substance para a versão 9.4.5

Corrigido:

* [Projeto] Abrir e salvar alguns projetos pode demorar mais do que o normal
* [Falha] Recarregar várias malhas pode levar a uma falha
* [Falha] ao excluir um canal durante o modo de exibição de máscara, o que leva a uma falha
* [Falha] Alguns Substance podem levar a uma falha quando renderizados
* [Inclinação de pintura] A ferramenta selecionada na inclinação de pintura permanece selecionada após alternar para o Modo de Pintura
* [Preparando Configurações Comuns] As configurações de Distância da Gaiola não atualizam a visualização do wireframe e do sombreador da gaiola
* [O ] preenchimento UV do modo “Vizinho do Espaço 3D” não funciona bem em triângulos finos
* O resultado do ponto de ancoragem do [Mecanismo] não é renderizado entre uma máscara e um canal de cor

### 12.1.0

Data de lançamento: <b>2026/06/23</b>

Resumo: <b>Esta atualização é uma versão principal. Ela contém melhorias para PANELAS com Novo estado de interface de usuário padrão de cozimento, mapa de inclinação da pintura, retoque automático, nova opção de desencapsulamento automático UV para malhas de superfície dura e OpenPBR. Para obter mais detalhes, consulte as notas de versão completas.</b>

<b>Adicionado</b>:

* [Mastigar cozimento] Ferramentas de pintura de inclinação
* [Assoalho de inclinação] Adicionar sombreador de visualização de inclinação e visuais de vetor de direção de inclinação ao pintar mapa de inclinação
* [Mascarar cozimento] Opção Adicionar proteção de borda
* [Assobiar] Recozimento automático
* [Assoalho de inclinação] Interface do usuário de lista do mapa de malha de retrabalho
* [Assoalho de inclinação] Dividir as configurações do Mapa de malha/Preparação comum + Mover as configurações comuns para fora da lista de mapas de malha apenas com cor base ou máscara
* [Inclinar cozimento] Alterar botões da barra de ferramentas da viewport
* [Cozimento de inclinação] Mostrar alternância de simetria para o pincel na barra de ferramentas superior
* [Assoalho de inclinação] Opções de renomeação no menu de sincronização de lista do mapa de malha
* [Inclinação da montagem] Caixas de diálogo de sincronização de atualização e estado verificado
* [Assoalho de inclinação] Criar variante do seletor de cores em tons de cinza
* [Inclinar cozimento] Ícone Atualizar modo de cozimento
* [Desenvolver automaticamente] Opção Integrar superfície rígida
* [OpenPBR] Adicionar suporte para OpenPBR 1.1
* [OpenPBR] Tornar o OpenPBR o fluxo de trabalho e o sombreador padrão
* [OpenPBR] Importar materiais e texturas do OpenPBR via USD
* [OpenPBR] Exportar materiais e texturas do OpenPBR via USD
* [OpenPBR] Janela Atualizar Texturas de Exportação para mostrar a convenção de nomeação do OpenPBR
* [OpenPBR] Adicionar documentação sobre alterações para suportar o OpenPBR
* [OpenPBR][Iray] Adicione o novo MDL para suportar o OpenPBR 1.1 no Iray
* Várias pequenas melhorias nas exportações em USD
* [UI] Adicionar aviso no visor ao tentar pintar em outro conjunto de texturas
* [Nivelar] Permite nivelar todas as camadas da instância nos Conjuntos de textura
* [Configurações do conjunto de texturas] Permite selecionar vários canais de uma vez por meio de uma nova janela
* [History] Atualizar “valor” Desfazer a entrada de texto para refletir o nome do parâmetro
* [Pilha de camadas] Tornar efeitos de preenchimento em máscaras padrão em branco (1.0)
* [Substance] Adicionar nova entrada de mapa do mecanismo “mesh_hard_edges_triangle”
* [Substance] Adicionar nova entrada de mapa do mecanismo “mesh_hard_edges”
* [Shader] Impedir que instâncias de sombreador compartilhem os mesmos nomes
* [Shader] Use o sombreador do modelo do projeto ao importar um arquivo USD ou GLTF
* Atualize o Adobe Color Engine para a versão 7.0
* Atualização mínima da versão do MacOSX para a versão 13.0 (Ventura)
* [Conteúdo] Novos modelos de projeto para OpenPBR
* [Conteúdo] Atualizar projetos de amostra para usar o novo sombreador de OpenPBR
* [Python] Expandir a API da Máscara de geometria para permitir modos de inclusão e exclusão, como na interface do usuário

<b>Corrigido</b>:

* [Falha][Configurações de mapas de malha] Aplicar configurações a outros conjuntos de textura
* [Crash] Ao assar a curvatura do mapa sem espaço mundial normal
* [Falha][Preparação] Cozimento com caixa personalizada ativada, mas nenhum arquivo selecionado falha
* [Falha] Cancelando cozimento de AO
* [Caixa automática] Carga infinita quando o caminho de arquivo poli alto é inválido
* [Linux][Windows] O seletor de cores às vezes pode ser totalmente preto ou não aparecer
* [Ferramenta Preenchimento de polígono] A ferramenta não funciona com fontes não PBR
* &lbrack;[Paint] Excluir canal de cor base não exclui a cor pintada anteriormente
* [USD] Nem todas as instâncias do sombreador foram detectadas corretamente
* [Substance] Somente o primeiro uso de um nó de entrada/saída é levado em consideração
* [Shader] A Oclusão ambiente é aplicada duas vezes com conjuntos de texturas usando diferentes métodos de mistura
* [Engine] Texturas normais com canal azul vazio (preto) podem levar a resultados incorretos de mesclagem
* [Importação de GLTF] a mesclagem de Alpha está ativada em todos os conjuntos de texturas
* [Exportação GLTF] A mesclagem de Alpha é sempre ativada na exportação
* [Exportar] A geometria de dupla face é sempre desativada ao importar um arquivo GLTF
* [Javascript] A modificação das configurações de sombreadores não contribui para o histórico de desfazer
* [Amostras] A dispersão da subsuperfície não está ativada nas configurações de exibição do fosco de reunião

### 12.0.3

Data de lançamento: **5/2026**

Resumo: **Versão secundária**

**Adicionado:**

* Atualize os padeiros para a versão 3.22.2
* Atualize o mecanismo de Substance para a versão 9.4.3
* \[Python\] Salvar um material inteligente em um local específico

**Corrigido:**

* \[Ubuntu\] Falha ao selecionar o material
* \[Mac\] A janela pop-up recorrente aparece para solicitar acesso a dados de outros aplicativos
* \[Preparação\] Artefatos podem aparecer no mapa de curvatura
* \[Preparação\] Preparação é mais lenta em alguns casos
* \[Distorcer para geometria\] Distorcer para geometria é desativado em alguns casos
* \[Bloco UV\] Alfa extraído do ponto de ancoragem ignorado por outros blocos
* \[Python\]\[Mac\] Exceções no console Python com SSL
* \[Python\] Painter falha ao sair com widgets Qt restantes

### 12.0.2

Data de lançamento: **04/2026/07**

Resumo: **Versão secundária**

**Adicionado:**

* [Gerenciamento de cores] Adicione novo OCIO para especificar o espaço de cores padrão do seletor de cores
* [Python] Expor configurações de desajuste automático na API Python

**Corrigido:**

* [Falha] Salvar com espaço em disco insuficiente pode travar ou corromper projetos
* [Falha] [Faixa de opções] O uso da faixa de opções pode causar falhas para alguns projetos
* [Falha] [Backup] falha quando o arquivo .assbin não pode ser gravado na pasta
* [Importar] Malhas OBJ do Stager podem falhar na criação do projeto
* [Importar] O OBJ está sem rosto em alguns casos
* [Import] A malha do USD sem nenhum material atribuído pode falhar na importação
* [Caminho preenchido] Não afetado pela simetria
* A visualização [Estêncil] tem resolução menor do que o resultado pintado
* [UI] “ilha uv” ainda é mencionada na dica de ferramenta de origem de cores do mapa de ID
* [Tela] As sombras aparecem invertidas
* [Visor] A transformação da projeção de distorção permanece após alternar para o modo de cozimento
* [Distorcer] A grade desaparece quando a escala é definida como 0 no eixo Z com a opção Distorcer para geometria ativada
* [Python] Erro inesperado ao adicionar um canal com modificação no escopo

### 12.0.1

Data de lançamento: **03/2026/18**

Resumo: **Versão secundária**

**Corrigido:**

* \[Falha\]\[Congelar\] Exportar de projetos específicos

### 12.0.0

Data de lançamento: <b>03/2026/09</b>
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

## Versão 11

### 11.1.3

Data de lançamento: <b>2026/02/12</b>
Resumo: <b>Versão secundária</b>

<b>Corrigido</b>:

* [Pintura] O estêncil e a simetria não funcionam em alguns casos
* [Caminho] Nenhuma atualização ao alterar o controle deslizante de opacidade do traçado de borrar
* [Projeto] Não é possível pintar em alguma geometria
* [Ribbon] O caminho instanciado desaparece ao alterar a resolução do Conjunto de Texturas
* [IU] O seletor de cores pode diminuir e desaparecer em alguns casos

### 11.1.2

Data de lançamento: <b>1/2026/13</b>
Resumo: <b>Versão secundária</b>

<b>Adicionado</b>:

* [Preparação] Melhorar o tempo de cozimento para projetos de blocos UV com salvamento assíncrono
* [Shaders] Menção nas alterações do API de sombreamentoLog após a migração Vulkan
* Atualizar OpenEXR para a versão 3.4.4

<b>Corrigido</b>:

* [Falha] Falha durante a inicialização na série Nvidia GTX 10xx
* [Falha] Usar o seletor de cores em diferentes conjuntos de texturas pode resultar em uma falha ao sair do aplicativo
* [Desempenho] Problema de desempenho ao pintar em um projeto com muitas camadas
* [Desempenho] Atraso ao pintar com caneta eletrônica gráfica
* [UI] As configurações da câmera permanecem desativadas no modo de renderização (Iray)
* [Ribbon] O caminho pode se sobrepor inesperadamente após um canto em alguns casos
* [Ribbon] Problema de desempenho com blocos UV
* [Substance][IU] As entradas de imagem desaparecem quando recolhidas
* [Substance][IU] Os grupos aninhados podem permanecer mesmo se visíveis, se forem ocultados
* [Cozimento][IU] Não é possível definir o raio de amostragem da curvatura além de 0,01
* [Preparação][IU] Não é possível definir a Distância máxima do oclusor além de 1
* [Preparação] A configuração “Auto-oclusão” do AO é ignorada com vários conjuntos de textura e baixa como cozimento alto
* [Preparação] O mapa de IDs não cria cores de vértice do FBX no modo Baixo como Alto
* [Content] O filtro Highpass resulta em cores desbotadas em canais com gerenciamento de cores

### 11.1.1

Data de lançamento: <b>2025/12/09</b>
Resumo: <b>Versão secundária</b>

<b>Adicionado</b>:

* [Desempenho] Melhorar o desempenho dos blocos UV ao calcular texturas parciais
* [Padarias] Atualização para a versão 3.15.4

<b>Corrigido</b>:

* [Falha][MacOS] Salvar projeto de versões anteriores sempre falha
* [Falha] Fechar um projeto às vezes pode resultar em uma falha
* [Project] Erro “incompatibilidade de contagem de membros” ao abrir projeto feito em versão anterior
* [Preparação] Os ladrilhos UV não são combinados com resultados anteriores de cozimento, se presentes
* [Preparação] Dispositivo perdido mesmo com o rastreamento de raios desativado na série Nvidia GTX 10XX
* [Preparação] O AO com normal tem artefatos nas bordas porque não há preenchimento
* [Preparação] A configuração “Auto-oclusão” do AO é ignorada com vários conjuntos de texturas e “corresponder pelo nome” na
* [Cozimento] O mapa de ID será totalmente preto se alguma malha de alto polígono não tiver cores de vértice
* [Ribbon] A dica de ferramenta para o modo de mesclagem Alpha menciona o modo de mesclagem de tela em vez do Subexposição Linear
* [Path] As tangentes criam um loop inesperado quando o ponto é movido próximo das extremidades do caminho
* [Ferramenta] A visualização de material não funciona quando a projeção é usada em uma máscara
* [Engine] Pintar traçados pequenos pode resultar em artefatos de blocos
* [Shader] Desfazer a criação da instância do sombreador não a remove corretamente
* [Export] O modo Alpha para exportação de GLTF é sempre definido como MASK
* [Python] Erro inesperado ao editar a pilha de camadas fora do bloco de modificação com escopo

<b>Problemas Conhecidos</b>:

* [Ribbon] Problema de desempenho com blocos UV
* [Ribbon] O caminho pode se sobrepor inesperadamente após um canto em alguns casos
* [Falha][Faixa de opções] Criar textos muito longos na Faixa de opções pode falhar
* [Gerenciamento de cores] As conversões do espaço de cores HDR com ACE no Linux produzem cores vivas
* [Regression][UI] O menu do botão direito do mouse é muito pequeno em telas HD
* [Crash][Python] Exportação de USD acionada por TextureStateEvent
* [Engine] Pintar com a ferramenta Clonar em cores normais de deslocamento de canal incorretamente
* [Python] O widget fantasma aparece excluído pelo script ainda em funcionamento

### 11.1.0

Data de lançamento: <b>2025/11/18</b>
Resumo: <b>Esta atualização é uma versão importante. Ela contém a nova ferramenta Ribbon com novo conteúdo dedicado, suporte de simetria para camadas de preenchimento, parâmetro de tamanho físico para deslocamento, desempenho aprimorado por meio de padarias atualizadas, suporte completo a Vulkan para Windows e Linux e outras melhorias.</b>

<b>Adicionado</b>:

* Nova ferramenta da faixa de opções
* [Ferramenta] Adicionar nova ferramenta Faixa de opções para criar caminhos perfeitos
* [Faixa de opções] Adicionar atalhos predefinidos da Faixa de opções na janela Propriedades
* [Ribbon] Permite alterar a opacidade da Faixa de Opções por vértice no caminho
* [Ribbon] Permite alterar o tamanho da Faixa de Opções por vértice no caminho
* [Ribbon] Remover o início/fim definido em um Substance quando os caminhos são fechados
* [Ribbon] Remover visualização Caminho/Material na janela de propriedades das ferramentas Pintar/Borracha/Borrar caminho
* [Faixa de opções] Adicione modos de mesclagem para o alfa e alguns canais quando houver autosobreposição
* Simetria de preenchimento
* [Preenchimento] Adicionar suporte para simetria em camadas e efeitos de preenchimento
* [Fill][UI] Expor configurações de simetria na janela de propriedades para camada de preenchimento e efeitos
* [Fill] Reprocessar a interface de configurações de simetria no menu do visor e na janela de propriedades
* [Fill] Reorientar adequadamente texturas normais ao projetar no modo de distorção
* deslocamento do tamanho físico
* [Deslocamento] Usar o tamanho físico como unidade de deslocamento
* Melhoria de desempenho
* [Desempenho] Melhorar a renderização de pequenos traçados de pincel em triângulos grandes
* [Desempenho] Melhorar o tempo de compilação do Sombreador
* [Performance] Suporte completo à Vulkan para Windows e Linux
* [Desempenho] Padeiros atualizados com renderização mais rápida de GPU e suporte a rastreamento de raios AMD
* [UI] Reorganizar propriedades de ferramentas em grupos e recolher algumas por padrão
* [Engine] Atualização do Substance Engine para a versão 9.2.5
* [Substance] Expor a substituição de resolução para recursos Substance em Ferramentas e Preenchimentos
* [Exportar] Atualizar predefinição de exportação de Mapas de malha para exportar texturas em tons de cinza
* Python
* [Panificação][Python] Indicar em changelog mudanças de quebra após atualização de padeiros
* [Python] Expor as configurações de simetria de preenchimento no Python
* Conteúdo e novo conteúdo
* [Conteúdo] Adicione 75 novas predefinições de ferramenta para a ferramenta Faixa de opções
* [Conteúdo] Atualize o recurso construtor de gradientes para que seja compatível com a Faixa de opções

<b>Corrigido</b>:

* [Falha] Carregar outro projeto enquanto o encaixe de caminho está ativado pode falhar
* [Falha] Clicar com o botão direito do mouse no painel Caminho com informações de outra sessão na área de transferência pode travar
* [UI] A interface rola para cima nas propriedades da ferramenta ao criar um caminho
* [UI] O cursor do mouse desaparece quando a visualização do visor do caminho está oculta
* [Caminho] Copiar/colar diferentes propriedades da ferramenta no painel Caminho leva a propriedades instáveis
* [Ferramenta] As predefinições da ferramenta Borrar nem sempre atualizam a seleção de canal
* [Ferramenta] O valor pintado é cinza, mas a interface do usuário mostra branco após carregar a predefinição de ferramenta colorida na máscara
* [Ferramenta] A predefinição criada a partir da máscara mantém os valores de canais carregados de outra predefinição
* [Substance] A substituição do espaço da cor normal definida no gráfico não é levada em consideração
* [Content] O recurso de forma de pincel padrão usa um Substance desatualizado

<b>Problemas Conhecidos</b>:

* O histórico da instância do sombreador não foi rastreado corretamente
* [Ribbon] Problema de desempenho com blocos UV
* [Ribbon] O caminho pode se sobrepor inesperadamente após um canto em alguns casos
* [Ribbon] As tangentes criam um loop indesejado quando o ponto é movido próximo das extremidades do caminho
* [Falha][Faixa de opções] Criar textos muito longos na Faixa de opções pode falhar
* [Ferramenta] A visualização de material não funciona quando a projeção é usada em uma máscara
* [Preparação] A configuração “Auto-oclusão” do AO é ignorada com vários conjuntos de texturas e a opção “corresponder pelo nome” ativada
* [Cozimento] O AO com normal tem artefatos nas bordas devido à falta de preenchimento
* [Gerenciamento de cores] As conversões do espaço de cores HDR com ACE no Linux produzem cores vivas
* [Regression][UI] O menu do botão direito do mouse é muito pequeno em telas HD
* [Crash][Python] Exportação de USD acionada por TextureStateEvent
* [Engine] Pintar com a ferramenta Clonar em cores normais de deslocamento de canal incorretamente
* [Python] O widget fantasma aparece excluído pelo script ainda em funcionamento

### 11.0.3

Data de lançamento: <b>08/2025/05</b>
Resumo: <b>Versão secundária</b>

<b>Adicionado</b>:

* [Substance 3D Assets] Adicionar um ponto de notificação ao painel Ativos 3D
* [VFX Platform 2025] Adicionar a configuração do ACES 2.0 nas configurações de gerenciamento de cores
* [VFX Platform 2025] Atualize o OCIO para a versão 2.4.2
* Atualize o Iray para a versão 2024.10
* [Engine] Atualização para o Substance Engine v.9.2.3
* [Nvidia] Aumente a versão mínima dos drivers Nvidia para 572.60 (Win) e 570.169 (Linux)

<b>Corrigido</b>:

* [Python] A modificação com escopo não aparece na janela Histórico

<b>Problemas Conhecidos</b>:

* [Gerenciamento de cores] As conversões do espaço de cores HDR com ACE no Linux produzem cores vivas
* [Regression][UI] O menu do botão direito do mouse é muito pequeno em telas HD
* [Crash][Python] Exportação de USD acionada por TextureStateEvent
* [Engine] Pintar com a ferramenta Clonar em cores normais de deslocamento de canal incorretamente
* [Python] O widget fantasma aparece excluído pelo script ainda em funcionamento

### 11.0.2

Data de lançamento: <b>6/2025/10</b>
Resumo: <b>Versão secundária</b>

<b>Adicionado</b>:

* [Mac] Adicionar aviso sobre a versão específica do sistema operacional levando a artefatos
* [Atualização automática] Pequenas melhorias de UX no log de erros de Ativos
* [Desempacotamento automático] Atualize para a versão 1.3.2 com melhorias de costura
* [USD][FBX] Adicionar suporte para vários conjuntos UV com dados esparsos
* [Exportar] Malhas exportadas como FBX não têm seus conjuntos UV adicionais se algum estava presente na importação

<b>Corrigido</b>:

* [MacOS][Linux] Falha ao salvar na unidade de rede
* [Win][Tablet] Cintilação ao deslocar
* [SpaceMouse] Problema ao trabalhar com a ferramenta Caminho
* [Caixa automática] Não é possível assar após um recarregamento de malha
* [Atualização automática] A sequência de imagens não é recarregada quando o primeiro bloco está ausente
* [Caminho] A tangente personalizada pode afetar outra tangente
* [Caminho] O caminho não aparecerá no Conjunto de textura se o primeiro ponto estiver em outro Conjunto de textura
* [IU] Alguns menus são sempre desativados após a abertura de um projeto (por exemplo, simetria)
* [Propriedades] Não é possível usar/carregar predefinições de ferramenta com a ferramenta Caminho preenchido
* [USD] Vários conjuntos UV não são reconhecidos no sombreador personalizado ao usar arquivos USD
* [USD] Câmeras com os mesmos nomes são substituídas
* [Exportar] Enviar para o Photoshop resulta em espaço de cor incorreto para resultados em cores e em tons de cinza
* [Exportar] Os canais em tons de cinza com alfa são exportados como cores em vez de tons de cinza com formato PNG
* [Exportar] Exportar canal em tons de cinza como PSD em arquivo inválido/truncado
* [Conteúdo] O filtro de distorção no modo multidirecional não funciona
* [Python] Não é possível alocar o erro de lista ao rastrear nós de pilha de camadas

<b>Problemas Conhecidos</b>:

* [Gerenciamento de cores] As conversões do espaço de cores HDR com ACE no Linux produzem cores vivas
* [Regression][UI] O menu do botão direito do mouse é muito pequeno em telas HD
* [Crash][Python] Exportação de USD acionada por TextureStateEvent
* [Engine] Pintar com a ferramenta Clonar em cores normais de deslocamento de canal incorretamente
* [Python] O widget fantasma aparece excluído pelo script ainda em funcionamento

### 11.0.1

Data de lançamento: <b>4/2025/10</b>
Resumo: <b>Versão secundária</b>

Observação: a versão do CCD do <b>Linux será adiada até 29 de abril</b>

<b>Adicionado:</b>

* Atualize para Qt 6.5.8
* [Substance] Adicionar mensagem de log para filtros quando várias entradas de imagem compartilham o mesmo uso
* [Nvidia] Adicionar aviso sobre os drivers Nvidia mais recentes (572.47)

<b>Corrigido:</b>

* [Falha] Ao arrastar e soltar um sbsar com uso em slots de canal único
* [Falha][Caminho] A opção Alterar tipo de caminho não fica acinzentada quando você não clica em um caminho específico
* [Preencher caminho] Não deve ser capaz de selecionar o material do substance
* [Engine] Artefatos ao longo de pinceladas
* [Engine] Os caminhos podem ser quebrados com configurações específicas
* Problema com o menu suspenso para o espaço da cor do conta-gotas
* [Atualização automática] [Python] Mensagem de erro incorreta ao usar ResourceID sem versão
* [Shader] Falha ao abrir alguns projetos

<b>Problemas Conhecidos:</b>

* [SpaceMouse] Problema ao trabalhar com a ferramenta Caminho
* [Gerenciamento de cores] As conversões do espaço de cores HDR com ACE no Linux produzem cores vivas
* [Regression][UI] O menu do botão direito do mouse é muito pequeno em telas HD
* [Crash][Python] Exportação de USD acionada por TextureStateEvent
* [Engine] Pintar com a ferramenta Clonar em cores normais de deslocamento de canal incorretamente
* [Python] O widget fantasma aparece excluído pelo script ainda em funcionamento

### 11.0.0

Data de lançamento: <b>3/2025/11</b>
Resumo: <b>Versão principal, novo recurso de atualização automática, ferramenta de caminho preenchido e outras melhorias de caminho, bem como novos filtros e uma geração experimental de gaiola automática para cozimento</b>

<b>Adicionado</b>:

* Atualização automática
* [Atualização automática] Atualizar automaticamente os ativos modificados no painel Ativos
* [Atualização automática] Atualizar automaticamente os ativos modificados em todo o projeto
* [Atualização automática] Manter a atualização automática desativada por padrão
* [Atualização automática] Tornar a atualização opcional se os parâmetros de recurso não corresponderem (.sbsar, .glsl, .ai, .svg)
* [Atualização automática] Adicionar variável de ambiente para desativar o recurso de atualização automática
* [Atualização automática][SBSAR] Tornar a atualização opcional se os parâmetros de recurso não corresponderem
* Caminho preenchido
* [Caminho][Preenchimento] Adiciona nova ferramenta para criar caminhos preenchidos
* Melhorias de caminho
* [Caminho] Criar um caminho que se ajusta aos polígonos
* [Caminho] Permite alternar tipos de caminho
* [Caminho] Permite copiar e colar dados de vértice de caminho entre conteúdo e máscara
* [Caminho] Permite restringir o ângulo ao criar um novo ponto
* [Caminho] Permite restringir a criação de pontos a uma linha
* [Caminho] Feche a forma com um único clique
* [Caminho] Exibir informações de caminho
* [Caminho] Permite dimensionar e girar vértices de caminho
* [Path][UX] Facilitar o acesso aos gizmos de transformação
* [Caminho] Adicionar visualização de caminho
* [Caminho] Desativar a visualização do caminho com Shift + P
* [Caminho] Melhorar a edição da tangente da vista lateral
* [Caminho] Permitir foco em um caminho 3D
* [Caminho] Os vértices devem manter o status da seleção ao ativar e desativar a interface novamente
* [Caminho] Permite excluir o caminho usando Backspace
* [Caminho] Mantém a lista de caminhos aberta se o usuário a expandir
* [Caminho][Pilha de camadas] Renomear duplicatas corretamente ao copiar/colar
* Melhorias na interface do usuário [Caminho] e nas dicas de ferramenta
* Desempenho
* [Desempenho] Aprimorar o desempenho do visor ao usar um alto nível de mosaico
* [Desempenho] Habilita somente o primeiro canal em novas camadas/efeitos de preenchimento
* [Desempenho] Paralelizar o cálculo do traçado do pincel
* Baking
* [Cozimento] Adicione uma nova opção de geração de gaiola totalmente automática para assar com malhas de alto polietileno (experimental)
* Conteúdo
* [Conteúdo] Adicione 6 novos filtros: estilização, quantize, kuwahara anisotrópico, suavização de chanfro, distância direcional, conversão em tons de cinza
* [Conteúdo] Atualize Noises and Grunges para a versão mais recente do Designer (com o novo 2D Voronoi)
* [Content] Adicione 3 novos geradores de textura (Tile Random, Triangle Grid, Scratches Generator)
* [Conteúdo] Renomear modelo do Unreal Engine e exportar predefinições
* Python
* [Shelf][Python] Salvar material inteligente ou máscara inteligente em disco do Python
* [Python] Adicionar gaiola automática de cozimento à API do Python
* [Python] Permitir a edição de nomes e descrições de Conjuntos de texturas/Blocos UV
* [Python] Compartilhar configurações de resolução em fontes vetoriais e de fonte
* [Atualização automática][Python] Expor as funcionalidades de atualização automática do projeto no Python
* Diversos
* [Exportar] Facilite o acesso às opções de Enviar para com um novo painel
* [Nvidia] Adicionar aviso sobre os drivers Nvidia mais recentes (572.16)
* O encaixe de ângulo deve ser afetado pela seleção de espaço Objeto/Mundo
* [Lista de conjuntos de texturas] Permite adicionar um nome personalizado aos blocos UV e usá-los na exportação
* Mac
* [Mac] Usar Metal em vez de OpenGL para renderização de gráficos
* [Mac] Soltar o suporte ao Mac Intel

<b>Corrigido</b>:

* [Falha] Excluir entrada de imagem
* Não é possível adicionar o Smart Mat pelo botão de pilha de camadas
* [Python] Efeitos no GroupLayerNode não podem ser encontrados

<b>Problemas Conhecidos</b>:

* [Gerenciamento de cores] As conversões do espaço de cores HDR com ACE no Linux produzem cores vivas
* [Regression][UI] O menu do botão direito do mouse é muito pequeno em telas HD
* [Crash][Python] Exportação de USD acionada por TextureStateEvent
* [MacOS Intel] Falha ao importar algumas predefinições
* [Engine] Pintar com a ferramenta Clonar em cores normais de deslocamento de canal incorretamente
* [Python] O widget fantasma aparece excluído pelo script ainda em funcionamento
* [RedHat] Problemas no seletor de cores

## Versão 10

### 10.1.2

Data de lançamento: <b>2024/12/3</b>
Resumo: <b>Versão secundária, correções de erros</b>

<b>Corrigido</b>:

* [Falha] Excluir entrada de imagem
* Não é possível adicionar o Smart Mat pelo botão de pilha de camadas
* [Python] Efeitos no GroupLayerNode não podem ser encontrados

<b>Problemas Conhecidos</b>:

* [Gerenciamento de cores] As conversões do espaço de cores HDR com ACE no Linux produzem cores vivas
* [Regression][UI] O menu do botão direito do mouse é muito pequeno em telas HD
* [Crash][Python] Exportação de USD acionada por TextureStateEvent
* [MacOS Intel] Falha ao importar algumas predefinições
* [Engine] Pintar com a ferramenta Clonar em cores normais de deslocamento de canal incorretamente
* [Python] O widget fantasma aparece excluído pelo script ainda em funcionamento
* [RedHat] Problemas no seletor de cores

### 10.1.1

Data de lançamento: <b>2024/11/5</b>
Resumo: <b>Versão secundária, correções de erros</b>

<b>Adicionado</b>:

* [Project] Mantém o projeto atual aberto até que a seleção do novo projeto seja validada
* [Quebra automática] A densidade do texel permite dividir melhor as Ilhas UV em UDIMs
* [Preparação] Corrigir cópia ambígua no menu contextual de Mapas de malha
* [Distorcer] Remover dimensionamento na viewport para o eixo Z (profundidade)
* [Importação/exportação] Remova o suporte a formatos de arquivo de imagem não utilizados
* Atualizar Substance Engine para 9.1.4

<b>Corrigido</b>:

* [Falha] Depois de realocar o recurso no Assets e salvar o projeto
* [Falha] Problemas com a biblioteca do servidor
* [Falha] Falha no servidor Illustrator em alguns casos raros
* [Falha] Ao sair do aplicativo em alguns casos raros
* Não é possível enviar relatórios de falhas em alguns computadores
* [Preparação] A cor do vértice não é lida corretamente
* [IU] O local do Windows e das novidades na inicialização foi alterado
* [Assimp] A superfície padrão do Maya não é reconhecida no assamento de ID
* [Python] A biblioteca SSL ausente gera um erro
* [Python][Win] Erro ao chamar QColorConstants.Transparent
* [Python] As miniaturas de camadas criadas por meio do Python não são atualizadas até clicar dentro da pilha de camadas
* [Shader] Link quebrado no API de sombreamento changelog
* [Ativos 3D] Use as configurações de proxy do sistema operacional ao acessar Ativos 3D

<b>Problemas Conhecidos</b>:

* [Gerenciamento de cores] As conversões do espaço de cores HDR com ACE no Linux produzem cores vivas
* [Regressão][IU] O menu do botão direito do mouse é muito pequeno em telas HD
* [Crash][Python] Exportação de USD acionada por TextureStateEvent
* [MacOS Intel] Falha ao importar algumas predefinições
* [Engine] Pintar com a ferramenta Clonar em cores normais de deslocamento de canal incorretamente
* [Python] O widget que parece ser excluído por meio do script ainda está funcionando
* [RedHat] Problemas no seletor de cores

### 10.1.0

Data de lançamento: <b>9/2024/17</b>
Resumo: <b>Versão principal, conteúdo novo: máscara de área de preenchimento/filtro de cores, filtro de decalque de bordado e seis filtros de Substance genéricos, importação de USD com propriedades de material e sombreador, melhoria de desempenho, compatibilidade com a plataforma VFX 2024 e migração para Linux RedHat</b>

<b>Adicionado</b>:

* [Conteúdo] Adicionar novo filtro de máscara/cor da área de preenchimento
* [Conteúdo] Adicionar novo filtro de decalque de bordado
* [Conteúdo] Adicione 6 novos filtros de Substance genéricos (FXAA, pixelate, highpass, posterize, smoothstep, threshold)
* [USD] Exportar camada USD com um material ASM definido
* [USD] Importar USD com propriedades de material e sombreador
* [Desempenho] Ativar miniaturas otimizadas de pilha de camadas por padrão
* [Desempenho] Reduzir o tempo de abertura do arquivo de projeto e o consumo de memória (decodificação de dados)
* Compatível com a plataforma VFX 2024
* [VFX Platform 2024] Atualização para Python 3.11
* [VFX Platform 2024] Atualização para OpenEXR 3.2
* [VFX Platform 2024] [USD] Atualização do OpenSubdiv 3.6.0
* [VFX Platform 2024][Gerenciamento de cores] Atualização para OCIO 2.3.2
* [Linux] Migração para o Linux RedHat
* [Linux] Atualize a versão mínima do driver Nvidia para 535.171.04
* [Importar] Adicionar uma opção para inverter o mapa normal ao importar uma malha GLTF
* [UI] Usar o valor padrão do sistema operacional para a distância de detecção de eventos de arrastar
* [Substance Engine] Adicionar função de faixa de chamada para remover os símbolos do executável
* [Tela inicial] Atualização para o novo formato de tela inicial
* Atualize o Substance Engine para a versão 9.1.3
* [Python] Mostrar link para exemplos no menu de documentação da pilha de camadas
* [JavaScript] Mover plug-ins Javascript para a subpasta javascript/plugins

<b>Corrigido</b>:

* [Illustrator] Falha ao exportar um bloco UV com gráfico .ai em casos específicos
* [Traçados dinâmicos][Caminho] O aleatório por traçado não funciona em um caminho
* [UI][Propriedades] O bloqueio é habilitado quando a divisão em blocos gráficos não é uniforme
* O arquivo TXT de depuração é criado ao clicar duas vezes no projeto do Painter
* [USD][Export] Algumas texturas podem estar ausentes
* [ASM] O canal de dispersão de cores ignora metais
* [Conteúdo] O filtro de desfoque não funciona no espaço de cores “trabalho”
* [Conteúdo] O filtro Ajustar Height também modifica o alfa da camada

<b>Problemas Conhecidos</b>:

* [Gerenciamento de cores] As conversões do espaço de cores HDR com ACE no Linux produzem cores vivas
* [Win][Crash] [ACE] Não usar espaço da cor sRGB ICE para transformação de exibição
* [Regression][UI] O menu do botão direito do mouse é muito pequeno em telas HD
* [Crash][Python] Exportação de USD acionada por TextureStateEvent
* [MacOS Intel] Falha ao importar algumas predefinições
* [Falha] Realocar recurso e salvar projeto
* [Engine] Pintar com a ferramenta Clonar em cores normais de deslocamento de canal incorretamente
* [Python] O widget fantasma aparece excluído pelo script ainda em funcionamento
* [RedHat] Problemas no seletor de cores

### 10.0.1

Data de lançamento: <b>6/2024/11</b>
Resumo: <b>Versão secundária, correções de erros</b>

<b>Adicionado:</b>

* [Biblioteca] Converter fontes de Substance em arquivos de fonte comuns
* [Illustrator][SVG] Dá às miniaturas na seleção de escopo um fundo cinza claro
* [Python] Adicionar função na origem do bitmap para listar os espaços de cores disponíveis

<b>Corrigido</b>:

* [Pilha de camadas] Pasta sempre fechada quando movida para dentro ou para fora de outras pastas
* [Salvar] O arquivo de projeto é perdido ao “salvar como cópia” ou o salvamento automático falha em casos específicos
* [Import] Ativos com o mesmo nome, mas extensões diferentes, são substituídos
* [Propriedades] Configurações ausentes ao usar o ponto de ancoragem nas entradas da imagem
* [Illustrator] Não é possível importar arquivos do Illustrator após falha do servidor sem reiniciar o Painter
* [Python] O pai da instância não pode ser definido com o tipo “properties”
* [Python] Configurar o alto poli como um parâmetro de cozimento não carrega o alto poli
* [Python] A mensagem de erro para set\_color\_space() é muito genérica
* [Python] As fontes de referência permitem criar ciclos

<b>Problemas Conhecidos</b>:

* [Gerenciamento de cores] As conversões do espaço de cores HDR com ACE no Linux produzem cores vivas
* [Regression][UI] O menu do botão direito do mouse é muito pequeno em telas HD
* [Crash][Python] Exportação de USD acionada por TextureStateEvent
* [MacOS Intel] Falha ao importar algumas predefinições
* [Illustrator] Falha ao exportar um bloco UV com gráfico .ai em casos específicos
* [Traçados dinâmicos][Caminho] O aleatório por traçado não funciona em um caminho

### 10.0.0

Data de lançamento: <b>5/2024/16</b>
Resumo: <b>Versão principal, edição da pilha de camadas com a API Python, leitura de arquivos nativos do Illustrator, integração de ativos 3D e novo recurso de texto</b>

<b>Adicionado</b>:

* [Illustrator] Usar arquivos do Illustrator com painéis de arte no Painter
* [Illustrator][SVG] Adicionar visualizações na seleção de escopo
* [Substance 3D Assets] Procure, selecione e baixe ativos 3D diretamente no Painter
* [Substance 3D Assets][IU] Novo painel
* [Substance 3D Assets] Mapas e materiais do ambiente de suporte
* [Substance 3D Assets] Permitir recarregamento e navegar e abrir a pasta de local em novo painel do Substance 3D Assets
* [Substance 3D Assets] Adição de um gerenciador de downloads
* [Recurso de texto] Permitir o uso de fontes incorporáveis
* [Recurso de texto] Permite renderizar uma fonte/texto em uma malha
* [Recurso de texto] Exibir fontes do usuário e outros caminhos compartilhados no painel Ativos com uma nova categoria
* [Recurso de texto][Propriedades] Adicionar suporte para propriedades avançadas de fonte
* [Recurso de texto] Permitir pesquisar/exibir fontes em miniprateleiras
* [Recurso de texto] Adicionar mensagem/caixa de diálogo de erro ao importar uma fonte incompatível
* Diversos
* [Preencher projeção] Melhorar o comportamento do manipulador de escala ao usar valores pequenos
* [Manipuladores] Adicionar novo modo preciso ao pressionar o atalho CTRL
* [Manipuladores] Melhoram a estabilidade do manipulador de superfície ao traduzir
* [Exportar] Adicionar o nome do espaço de cores nas saídas SBSAR
* [Desempenho] Melhorar o tempo de descoberta da biblioteca de ativos em disco
* [Substance] Atualização do mecanismo de Substance versão 9.1.2
* [Arrastar e soltar] Alinhar a rotação do decalque na câmera ao soltar no visor
* [Python] Edição da pilha de camadas
* [Python] Permitir selecionar camada, efeito, máscara, máscara geográfica na interface do usuário
* [Python] Permitir modos de mesclagem de camada get/set
* [Python] Permitir obter/definir configurações de projeção da camada de preenchimento
* [Python] Permitir consultar a cor do material de Substance de uma camada de preenchimento
* [Python] Permitir consultar e definir cores e recursos uniformes em camadas e efeitos
* [Python] Permitir a criação e edição de recursos de texto na pilha de camadas
* [Python] Permitir a edição de canais ativos em camadas e efeitos
* [Python] Permitir que ações em lote tenham uma única operação de desfazer/refazer
* [Python] Permitir carregar/editar parâmetros de origem vetorial
* [Python] Permitir a edição de propriedades de cores de camadas e efeitos com o gerenciamento de cores
* [Python] Permitir consultar e criar camadas instanciadas
* [Python] Permitir a adição do efeito de seleção de cor
* [Python] Permitir o controle do gerenciamento de cores de imagens de bitmap
* [Python] Permitir pausa/cancelamento de pausa no mecanismo
* [Python] Permitir a navegação para nós irmãos e pai
* [Python] Permitir a criação do efeito filtro/gerador
* [Python] Permitir a adição de efeito de nível
* [Python] Permitir a adição de máscara inteligente em uma camada
* [Python] Permitir a criação/edição de pontos de ancoragem
* [Python] Permitir obter/definir máscara em camadas
* [Python] Permitir a criação do efeito de máscara de comparação
* [Python] Permitir consultar e usar predefinições de recursos Substance
* [Python] Permitir listar predefinições e seus valores por meio da função internal\_properties para recursos Substance
* [Python] Permitir listar predefinições de exportação predefinidas
* [Python] Permitir listar predefinições de exportação disponíveis na biblioteca
* [Python] Permite recuperar o conteúdo das predefinições de exportação

<b>Corrigido</b>:

* [Falha] Desfazer “Remover instância do sombreador” com Ctrl-Z
* [Falha] Criar uma camada em uma pilha vazia se a última seleção tiver sido um efeito
* [SVG] Problema com o valor personalizado da área cortada
* [Desembaçamento automático] Recomputar apenas a embalagem sem qualquer alteração na orientação UV resulta em falha
* [Arrastar e soltar] Atraso devido a recursos externos pré-carregados várias vezes
* [UI] Arrastar e soltar a miniatura de recurso pode ocultar a mensagem de aviso na pilha de camadas
* [Desempenho] Os blocos UV mascarados ainda são computados
* [USD] Destaque incorreto para seleção de escopo
* [Recurso] A imagem de bitmap é corrompida após pintar no canal normal e salvar o projeto
* [USD] Suporte a ordenação de malha de vértice com a mão esquerda
* [Substance] Redefinir para o padrão sempre voltar a zero para o widget de ângulo
* [Engine] Pintar com um SVG em um estêncil não funciona
* [Engine] Os traçados de pincel de mapa normais se quebram após uma ação de desfazer
* [Conteúdo] O filtro Gráfico para material tem mesclagem alfa e espaço de cores incorretos
* [Conteúdo] Os modos de mesclagem no Tile Generator não estão funcionando
* [Conteúdo] O filtro de exame de histograma produz faixas em alguns casos
* [Conteúdo] Iluminação cozida estilizada não leva em conta height pintado
* [Python] Erro inesperado ao recuperar informações de camada instanciadas após alteração do sombreador
* [Salvar] O arquivo de projeto é perdido quando o “salvar como” falha em casos específicos

<b>Problemas Conhecidos</b>:

* [Gerenciamento de cores] As conversões do espaço de cores HDR com ACE no Linux produzem cores vivas
* [Crash][Linux][AMD] Arrastar e soltar recursos na pilha de camadas no sistema operacional Wayland
* [Regression][UI] O menu do clique com o botão direito é muito pequeno em telas HD
* [Crash][Python] Exportação de USD acionada por TextureStateEvent
* [Salvar] O arquivo de projeto Spp é perdido quando a opção “salvar como cópia” falha em casos específicos
* [MacOS Intel] Falha ao importar algumas predefinições
* [Illustrator] Não é possível importar arquivos Ai após o travamento do servidor sem reiniciar o Painter
* [Import] Ativos com o mesmo nome, mas extensões diferentes, são substituídos

## Versão 9

### 9.1.2

Data de lançamento: <b>1/2024/30</b>
Resumo: <b>Versão secundária, correções de erros</b>

<b>Adicionado</b>:

* [Desempenho] Melhorar o tempo de criação da primeira camada de preenchimento em novos projetos
* [Desempenho] Reduzir o tempo de carregamento de mapas de ambiente pesado
* [Substance] Permitir salvar/fechar projetos mesmo quando as miniaturas estiverem sendo geradas

<b>Corrigido</b>:

* A gravação falha em projetos de versões anteriores quando o visor é modificado
* [Falha] Reimportar malha ao usar o AO personalizado e o gerenciamento de cores
* [Preencher projeção] Clicar no manipulador de escala exibe a mensagem “não é possível pintar”
* [Pincel] Pintar com alinhamento UV causa artefatos
* [Pilha de camadas] Renomear a camada é lento quando a pilha é muito longa
* [Pilha de camadas] Mensagem de erro incorreta ao usar filtro incompatível na máscara
* [Pilha de camadas] A seleção volta para a camada superior após a exclusão
* [Exportar] A textura normal gerada está sempre no modo de preenchimento Vizinho do Espaço 3D
* [Exportar] A textura alfa não é gerada com a predefinição de exportação Exibição 2D
* [Exportar] A exportação SBSAR tem usos incorretos com mapas convertidos
* [Shader] O log de alterações do API de sombreamento não está atualizado com as alterações mais recentes do ASM

<b>Problemas Conhecidos</b>:

* [Gerenciamento de cores] As conversões do espaço de cores HDR com ACE no Linux produzem cores vivas
* [Crash][Linux][AMD] Arrastar e soltar recursos na pilha de camadas no sistema operacional Wayland
* [Regression][UI] O menu do clique com o botão direito é muito pequeno em telas HD
* [Crash][Python] Exportação de USD acionada por TextureStateEvent

### 9.1.1

Data de lançamento: <b>2023/12/05</b>
Resumo: <b>Versão secundária, correções de erros e envio para a funcionalidade do After Effects</b>

<b>Adicionado:</b>

* [Interop] Permitir o envio de uma malha texturizada para o After Effects (Ae 24.1)

<b>Corrigido:</b>

* [Preenchimento] UV definido para projeção de conjunto UV não lê mais do que 2 conjuntos UV
* [Falha] Usar o mapa de ambiente de 16K
* [Falha] Exr usado como entrada de imagem
* [Falha] Copiar e colar caminhos entre projetos
* [QoL] Arrastar e soltar o recurso Alpha no modo de decalque cria Projeção UV na máscara
* [Caminho] Copiar vértices de caminho também renomeia o caminho de destino ao reabrir o projeto
* [Linux] A escolha de cores pode ser interrompida com várias telas
* [Desbobinar automaticamente] Problema de interface do usuário para controle de densidade de texel
* [Gerenciamento de cores] O feedback da interface é razoável, mas o mecanismo não
* [Gerenciamento de cores] Seleção incorreta de espaço de cores na máscara com substituição de dados do usuário

<b>Problemas Conhecidos:</b>

* [Gerenciamento de cores] As conversões do espaço de cores HDR com ACE no Linux produzem cores vivas
* [Crash][Linux] com Linux Wayland no AMD ao arrastar e soltar recursos na pilha de camadas
* [Crash][Mac] Alterar o valor da filtragem anisotrópica no sistema operacional Monterey
* [Regression][UI] O menu do clique com o botão direito é muito pequeno na tela hd
* [Python] Falha ao exportar USD acionada por TextureStateEvent

### 9.1.0

Data de lançamento: <b>2023/11/07</b>
Resumo: <b>Versão principal que apresenta suporte a SVG e transparência, bem como melhorias na ferramenta de arrastar e soltar e no caminho</b>

<b>Adicionado:</b>

* [SVG] Permitir a importação de arquivos vetoriais (SVG)
* [SVG][UI] Adicionar suporte para propriedades específicas de SVG
* [SVG] Adicione uma opção para preservar facilmente as proporções da imagem original
* [SVG] Permite usar automaticamente alfa de SVG com transparência
* [Interop] Permitir o envio de uma malha texturizada para o After Effects (Ae 24.1 beta)
* [Interoperabilidade] Adicionar configurações de Envio ao After Effects
* [QoL][Assets][UI] Importar ativo automaticamente ao arrastar e soltar no slot da interface
* [QoL] Permitir arrastar e soltar ativos externos na pilha de camadas
* [QoL][Pilha de camadas] Arrastar e soltar texturas do painel Ativos na Pilha de camadas
* [QoL][Janela de visualização] Permite arrastar e soltar o gerador, filtros na malha
* [QoL][Visor] Permitir soltar ativos externos na malha
* [QoL][Projeção] Adicionar novo conjunto UV ao modo de projeção do conjunto UV
* [QoL] Arrastar e soltar Máscaras inteligentes como novas camadas no visor e na Pilha de camadas
* [QoL] Adicionar seletor para Geradores com várias saídas quando usado em máscara
* [QoL] Permitir arrastar e soltar imagens de canal único sobre um efeito de preenchimento
* [QoL][Pilha de camadas] Use modificadores CTRL/ALT com arrastar e soltar para especificar onde/como criar efeitos/camada
* [Caminho] Alterna a visibilidade dos caminhos individualmente no painel Caminho
* [Caminho] Permitir o uso de manipuladores de transformação para pontos de caminho
* [Caminho] Permite controlar manualmente as tangentes por vértice
* [Caminho] Copiar/colar propriedades do caminho
* [Path] Introduzir um atalho vazio para o botão Quebrar tangente
* [Shader] Adicionar suporte para Opacidade e Translucidez no sombreador ASM
* [Shader] Adicionar suporte para canal de Cor de absorção com sombreador ASM
* [Shader] Melhorar dicas de ferramentas de parâmetros de sombreador ASM
* [Shader] Alterar a cor padrão do canal de transparência para preto
* [Configurações de exibição] Ativar Suavização temporal por padrão
* [Configurações de exibição] Ativar configuração de dispersão abaixo da superfície por padrão
* [Substance] Adicionar suporte para a propriedade ColorSpace a partir da entrada/saída do gráfico
* [Substance] Atualize o mecanismo de Substance para a versão 9.0.3
* [IU] Tornar acessível o botão contextual da barra de ferramentas, mesmo se a janela do aplicativo for pequena
* [Auto Unwrap] Controlar o número de ladrilhos UV com densidade de texel
* [Preparação] Desativar Rastreamento de raios do GPU em GPUs AMD por padrão
* [Desempenho] Aplique compactação sem perdas em imagens de 16 bits para reduzir o espaço ocupado pelo projeto
* [Python] Permitir manipular a câmera padrão na visualização 3D
* [Python] Expor a capacidade de exportar malha por meio de scripts
* [Conteúdo][Amostras] Adicionar novo projeto de amostra “Mesa de restaurante francês”
* [Content] Atualize o logotipo do Substance para a nova versão
* [Conteúdo] Adicione três filtros de material focados em SVG (adesivo personalizado, spray personalizado e gráfico para o material)

<b>Corrigido:</b>

* [Falha] Alterar o tamanho do manipulador quando não estiver usando a ferramenta de simetria
* [Falha] [Pilha de camadas] Criando camada quando nada está selecionado
* [Projeto] Mapas de malha podem ser corrompidos após a remoção de recursos não utilizados
* [Project] Corrupção de recursos após importar ou colocar novamente a imagem no forno
* [Assets] Recarregar um ativo o remove de Favoritos
* [Importar] Não é possível importar recursos quando “Nenhum resultado encontrado” no painel de ativos
* [UI] A seta da barra de ferramentas contextual não aparece em alguns casos
* [Substance] Botão lado a lado para valores booleanos não suportado
* [Level] Rótulo de canal incorreto quando usado na máscara
* [Export][glTF] Os arquivos glTF/GLB exportados do Painter não têm uma unidade de tamanho físico
* [Conteúdo] A intensidade do filtro de desfoque é fixada em 16
* [Conteúdo] A entrada da imagem de “cor de destino” do filtro Correspondência de Cores não está visível

<b>Problemas conhecidos:</b>

* [Gerenciamento de cores] As conversões do espaço de cores HDR com ACE no Linux produzem cores vivas
* [Crash][Linux] com Linux Wayland no AMD ao arrastar e soltar recursos na pilha de camadas
* [Crash][Mac] Alterar o valor da filtragem anisotrópica no sistema operacional Monterey
* [Falha] Exr usado como entrada de imagem
* [Falha] Usar o mapa de ambiente de 16K
* [Desbobinar automaticamente] Problema de interface do usuário para controle de densidade de texel
* [Regression][UI] O menu do clique com o botão direito é muito pequeno na tela hd
* [Python] Falha ao exportar USD acionada por TextureStateEvent
* [QoL] Arrastar e soltar o recurso Alpha no modo de decalque cria Projeção UV na máscara

### 9.0.1

Data de lançamento: <b>9/2023/19</b>
Resumo: <b>Versão de correção de erro secundária com várias melhorias</b>

<b>Adicionado:</b>

* [Importar] Definir local de importação padrão na janela de importação
* [Modo de Preparação] Permite redefinir parâmetros para seus valores padrão
* [Preparação] Defina a preparação para pintar a resolução ao criar um projeto
* [Simetria] Desvincular manipulador específico de simetria do atalho Q
* [Menu] Adicionar a opção “mostrar registro” no menu Ajuda
* [Visor] Melhorar a velocidade de renderização de sombra
* [Substance] Atualizar mecanismo para a versão 9.0.1
* [Gerenciamento de cores] O arquivo de configuração OCIO pode ter qualquer tipo de extensão
* [Assets] O recurso Sbsar com uso de “decalque” deve ser definido automaticamente para distorcer a projeção
* [Caminho] Exibe uma mensagem ao tentar interagir com a ferramenta Caminho enquanto a interface do usuário e os Gizmos estão ocultos

<b>Corrigido:</b>

* [Falha] Alt + Arrastar no painel Caminho
* [Importar Recursos] Falha aleatória ao remover recursos para importar
* Falha ao importar um arquivo GLB compactado
* Problema ao pintar em malhas que compartilham UVs
* Flash de malha preto ao recalcular ou carregar cache
* [Propriedades] O menu do botão direito do mouse para redefinir parâmetros não aparece nas listas suspensas
* [Nível] Controles deslizantes de entrada bloqueados pelo nível anterior
* [AMD][Esparsa] A opção SVT, se ativada, gera artefatos
* [Projeção][Distorcer] Falha ao clicar duas vezes nos vértices
* Interface do usuário do [Caminho] e caminho visível no modo de cozimento
* [AMD] Textura perdida ao brincar com a visibilidade
* [Esparso] Resolução muito baixa ao girar a malha

<b>Problemas Conhecidos:</b>

* [Gerenciamento de cores] As conversões do espaço de cores HDR com ACE no Linux produzem cores vivas

### 9.0.0

Data de lançamento: <b>06/2023/20</b>
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
* [Python][USD] Expor parâmetros de configuração de projeto para o formato USD
* [Python][USD] Expor os parâmetros de criação de projetos para o formato USD
* [Export][USD] Adicionar informações do caminho do projeto no arquivo USD exportado
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

## Versão 8

### 8.3.1

Data de lançamento: <b>2023/04/27</b>

<b>Adicionado:</b>

* [Modo de preparo] Adicionar atalho (vazio) para mostrar/ocultar a visualização do visor
* [Modo de cozimento] Sempre mostrar Low Poly ao usar o botão “Ocultar malhas de cozimento”
* [Modo de Preparação] Mostrar sufixo para Correspondência por Nome com base no Conjunto de Textura atual
* [Importar] Adicionar suporte para arquivos binários GLTF (glb)
* [Lista de conjuntos de texturas] Adicionar menu para selecionar ou criar ocorrências de sombreador
* [Lista de conjuntos de textura] Permite alterar rapidamente o conjunto de textura e a resolução de blocos UV
* [Tamanho físico] Melhorar o comportamento do manipulador ao usar tamanho físico no Projeção UV
* [UI] Trazer de volta “Salvar como” para o menu Arquivo principal
* [UI] Salvar seleção de exibição (somente 2D, somente 3D, ambos) no layout da interface do usuário
* [USD] Mensagem de erro menos vaga na criação do projeto com formas de USD não compatíveis
* [Python] Adicionar eventos de cozimento para seguir o progresso da cozedura
* [Python] Permitir o cancelamento de um bolo
* [Python] Expor “Com base no modelo de saída” para o tipo de arquivo e a profundidade de bits na exportação
* [Python] Expor tempo de atualização para TextureStateEvent.Update

<b>Corrigido:</b>

* [Falha] Falha rara ao fechar um projeto
* [Falha] [Preparação] Ativar a sincronização do mapa de malha com Height ou curvatura em um projeto específico
* [Falha][Script] Falha ao adicionar um material após a criação da instância do sombreador
* [Modo de cozedura] A intensidade do AO em material neutro não tem efeito
* [Modo de cozimento] Falha ao alternar para o modo de cozimento antes do modelo ser carregado
* [Modo de preparo] Mensagem de erro ausente na guia Processo de preparo
* [Modo de cozimento] As configurações de material neutro não têm efeito após a reimportação de uma malha
* [Modo de Preparação] O separador de visor é salvo globalmente, e não por modo
* [Modo de cozimento] Problema de visualização: o normal médio não altera a superfície da gaiola
* [Gerenciamento de cores] A configuração de detecção automática de espaço de cores é desativada quando a variável de ambiente OCIO está presente
* [Conteúdo] O filtro Contorno de máscara tem artefato com entrada de height
* [Conteúdo] O controle deslizante de intensidade do filtro de desfoque de Inclinação é apertado em 1.0
* [Interop] Não é possível criar projeto com GLTF a partir do Sampler
* [Pilha de camadas] O valor de divisão em blocos gráficos de projeção não é atualizado corretamente com o manipulador
* [Linux] Deslocamento entre a caneta eletrônica gráfica e o cursor com HDPI maior que 100%
* [Python] Falha ao reimportar uma malha após criar um projeto
* [Substance] Ruídos 3D são quebrados após a reimportação de uma malha
* [Blocos UV] O deslocamento da Projeção UV é fixado em 1
* [Visor] O feedback visual em linhas retas não está mais visível
* [WhatsNew] Retorno de linha incorreto em títulos de recursos

<b>Problemas Conhecidos:</b>

* [Importar] Algumas GLB com texturas não obtêm texturas no Painter

### 8.3.0

*(Lançado: 10 De Janeiro De 2023)*
Resumo: <b>Versão principal com novo modo de preparo, nova importação e exportação de arquivos USD e suporte de tamanho físico para Projeção UV</b>

<b>Adicionado:</b>

* [Modo de cozedura] Novo modo de cozedura dedicado ao processo de cozedura
* [Modo de cozimento] Defina o atalho para alternar para o modo de cozimento para F8
* [Modo de cozimento] Botão Adicionar início e Cancelar cozimento no visor
* [Modo de cozimento] Adicionar seleção de cozimento na lista Conjunto de textura
* [Modo de cozimento] Adicionar nova janela de padeiros de mapa de malha para selecionar padeiros
* [Modo de cozimento] Adicionar nova janela Configurações do mapa de malha para editar as configurações de cozimento
* [Modo de cozimento] Adicionar nova janela de registro de cozimento para seguir o processo de cozimento
* [Modo de cozimento] Adicionar parâmetros de cozimento e desfazer ações na janela Histórico
* [Modo Preparação] Adicionar trilhas nas Configurações do mapa de malha
* [Modo de cozimento] Adicione miniaturas de mapas de malha na janela Preparadores de mapas de malha
* [Modo de cozimento] Adicionar menu recolhível de configurações de visualização em uma janela de visualização 3D
* [Modo de cozimento] Adicionar configuração de visualização para mostrar/ocultar a malha de alto polímero
* [Modo de cozimento] Adicionar configuração de visualização para mostrar/ocultar a malha da gaiola e o wireframe
* [Modo de cozimento] Adicionar configuração de visualização para mostrar/ocultar a malha de baixo polímero
* [Modo de cozimento] Adicionar configuração de visualização para mostrar as bordas sólidas sem emendas UV como erros
* [Modo de cozimento] Informar na viewport sobre erros de malha e cozimento se o Registro de cozimento não estiver visível
* [Modo Preparação] Adicionar ação para sincronizar as configurações do padeiro em todos os Conjuntos de Textura

  Na janela Panificadores de mapa de malha, cada panificação (bem como as configurações comuns) pode ser sincronizada entre os conjuntos de textura clicando no ícone de link ao lado de seu nome. Esta ação abrirá uma janela que permite selecionar quais conjuntos de texturas compartilharão os mesmos parâmetros.

* [Modo de cozimento] Adicionar ações para copiar e colar configurações do padeiro

  Na janela Panificadores de mapa de malha estão disponíveis ações para copiar e colar cada configuração de panificação nos Conjuntos de textura por meio do menu dedicado na parte superior da janela ou do menu contextual do botão direito do mouse.

* [Modo de cozimento] Adicione o botão no Log de cozimento para pular do erro para as configurações corretas

  Quando um padeiro falha ou uma malha não é carregada corretamente, uma mensagem de erro aparece no registro de cozimento. Um botão ao lado da mensagem permite alterar a janela Configurações de pás e mapas de malha para mostrar as configurações relacionadas. Isso ajuda a isolar com mais facilidade a origem de um problema para corrigi-lo.

* [Modo Preparação] Adicionar menus para gerenciar conjuntos de texturas e seleções de pincéis

  Tanto na “lista de conjuntos de texturas” quanto na “PANELAS DE MAPA DE MALHA”, foi adicionado um pequeno menu de ação para ajudar a copiar e inverter as seleções.

* [Modo de cozimento] Dividir a lista de seleção do padeiro por conjunto de textura
* [Modo de cozimento] Dividir configurações comuns por conjunto de textura
* [Modo de cozedura] Carregue malhas de alto-poli e gaiola sem congelar a interface
* [Modo de cozimento] Use a barra de progresso do visor para mostrar a carga da malha
* [Modo de cozimento] Adicionar estado de carregamento de malha no Log de cozimento
* [Modo de cozedura] Permite girar a malha no visor durante a cozedura
* [Modo de cozedura] Definir a ordem de cozedura com base na visibilidade atual da janela de malha
* [Modo de cozimento] Exibir gaiola de cozimento implícita no visor

  Se não estiver usando um arquivo de malha de gaiola personalizado, uma malha de gaiola automática será gerada e exibida na janela de visualização. Seu tamanho será baseado no parâmetro Distância frontal máxima das configurações comuns de cozimento. A malha de gaiola é usada para indicar até onde a correspondência entre o poli baixo e alto irá.

* [Modo de cozimento] Mostrar lista correspondente de nomes de malha para correspondência por nome no Log de cozimento
* [Modo de cozimento] Usar material neutro para exibir o modelo 3D na viewport
* [Modo de cozimento] Desativa o cálculo do motor em modo de cozimento
* [Modo de cozimento] Exibir um aviso ao sair do aplicativo enquanto uma torta está em andamento
* [Padeiros] Atualizar rótulos de configuração de suavização de borda

  Os valores de configuração de suavização de borda foram renomeados para “Sobreamostragem” e com um número multiplicador explícito para esclarecer seu comportamento.

* [Padarias] Atualize as padarias para a versão 2.5.7.
* [USD] Importar e exportar arquivos do Universal Scene Description (USD)
* [USD] Adicione opções USD à janela Novo projeto ao selecionar um arquivo USD
* [USD] Adicionar nova janela de seleção de escopo e variantes

  Ao importar um arquivo USD, clicar no botão de alteração na janela Novo projeto ou Configuração de projeto permite selecionar qual parte e variantes de um arquivo USD importar.

* [USD] Opção Adicionar níveis de subdivisão

  Ao criar um novo projeto com um arquivo de malha do USD que contém subdivisões, é possível selecionar o nível de subdivisões usando um controle deslizante. O projeto será criado com a malha subdividida. O nível pode ser modificador por meio da Configuração do projeto.

* [USD] Importar malhas com pele em USD em um quadro específico

  Ao criar um novo projeto com um arquivo de malha USD que contém animação, é possível selecionar o quadro usando um controle deslizante que reflete a sequência de linha do tempo incorporada. O quadro pode ser modificador por meio da Configuração do projeto.

* [USD][Exportar] Adicione uma opção para exportar arquivos USD

  Nova caixa de seleção Exportar USD adicionada à janela Exportar texturas. Quando marcada, permite exportar arquivos USD, bem como mapas de textura usando qualquer modelo.

* [USD][Exportar] Adicionar formato de arquivo USD à exportação de malha
* [USD] Renomeie a predefinição de exportação “USD PBR Metal Roughness” existente para mais explícita

  O modelo de exportação para USD anteriormente conhecido como “USD PBR Metal Roughness” ainda é acessível por meio de Exportar texturas > Modelo de saída > USDz (Apple AR).

* [Abrir automaticamente] Adicionar orientação Bloquear para embalagem

  Nova opção para configurações de abertura automática que permitem preservar a orientação de Ilhas UV existentes ao usar o recurso de embalagem. Ele pode ser acessado em Novo projeto > Opções de quebra automática > Orientação da Ilha UV.

* [Tamanho físico] Adicionar configuração para usar Tamanho físico automaticamente no efeito/camada de preenchimento

  Foi adicionada uma nova opção para alternar automaticamente para a escala de tamanho físico ao usar um material com tamanho físico incorporado. Ele pode ser ativado por projeto por meio de Novo projeto ou de Editar > Configuração do projeto > Tamanho físico > Alternar o dimensionamento da camada de preenchimento para Tamanho físico ao atribuir materiais.

* [Tamanho físico] Expor tamanho físico para Projeção UV

  O dimensionamento de tamanhos físicos agora está disponível para Projeção UV. Ele ativa o redimensionamento automático de um material com base no tamanho físico de uma malha. Pode ser selecionado por meio de Escala > Tamanho físico na janela Propriedades da camada de preenchimento ou do efeito.

* [Scripting][Python] Permite consultar a versão do aplicativo
* [Script][JavaScript] Atualizar API para corresponder aos novos parâmetros de criação
* [Scripting][Python] Módulo de cozimento: editar parâmetros de cozimento
* [Scripting][Python] Módulo de cozimento: iniciar/cancelar cozimento
* [Scripting][Python] Módulo de preparo: selecionar o método de curvatura
* [Scripting][Python] Módulo de cozedura: seleção de padeiros / azulejos uv
* [Scripting][Python] Módulo de preparo: sincronizar as configurações do padeiro em todos os conjuntos de texturas
* [SVT] Habilitar suporte a hardware esparso em GPUs AMD

  A aceleração de hardware para o sistema de texturas virtuais esparsas agora pode ser ativada com as GPUs da AMD. Essa configuração é ativada automaticamente nas preferências gerais.

* [Projection] Renomear os parâmetros de projeção cilíndrica

  O parâmetro “Cylinder Cap Culling” foi renomeado para “Backface Culling” para melhor representar sua ação. A dica de ferramenta associada foi ajustada de acordo.

* [Project] Salvar a versão do aplicativo no projeto e recuperá-la por meio de scripts

  Desde a versão 8.2, a versão do aplicativo agora é armazenada dentro do arquivo spp ao salvar.
  Esse número de versão pode ser recuperado com a função last\_saved\_substance\_painter\_version() no módulo do projeto da API Python.
  Para projetos feitos antes de 8.2, o valor retornado será nulo.

* [Importar] Melhorar o tempo de importação geral de modelos 3D

  Melhoramos o tempo geral de importação das malhas. Por exemplo, reduzir o tempo de espera ao carregar malhas de alto-poli para cozimento. Essa otimização aplica-se em particular ao carregamento de arquivos OBJ.

<b>Corrigido:</b>

* [Falha] Alterar canais no filtro com pilha específica
* [Mac][M1] Falha ao criar uma camada de preenchimento e sair da pilha de camadas

  Esse problema pode ser corrigido atualizando para o Mac OS 13 (Ventura).

* [Scripting][Python] Falha ao usar ui.add\_dock\_widget() com tipo errado
* [Preparação] Mensagem de erro incompleta no log quando um bake falha
* [Preparação] A memória não é liberada quando a cozedura é concluída
* [Engine] O cache de textura não é atualizado ao alterar a visibilidade do efeito
* [Exportar] Mapa uniforme de exportações em 2D aleatoriamente
* [Project] Erro de alocação de memória ao salvar projeto com malha grande
* [Visor] O TAA causa artefatos ao pintar em alguns casos

<b>Problemas Conhecidos:</b>

* [Gerenciamento de cores] As conversões do espaço de cores HDR com ACE no Linux produzem cores vivas
* [Pilha de camadas] Fonte de entrada não salva por camada

### 8.2.0

*(Lançado: 06 De outubro De 2022)*
Resumo: **Versão principal com novos painéis de integração (novo painel de boas-vindas e painel de novidades), exportação para SBSAR, efeitos para pasta, várias melhorias na qualidade de vida e correções de erros.**

**Adicionado:**

* [Integração] Painel de integração para acolher novos usuários

  Adicionada uma nova tela de boas-vindas quando novos usuários da CC abrem o Painter pela primeira vez.

* [Integração] Painel de novidades para aprimorar a descoberta de novos recursos

  Adicionada uma nova tela Novidades que exibe os novos recursos principais. Ele é exibido automaticamente na primeira vez que o Painter é aberto após uma atualização importante e pode ser acessado novamente em Ajuda > Novidades.

* [Integração] Renomear antigo Bem-vindo à “Tela inicial”

  A tela de boas-vindas antiga foi renomeada para Tela inicial para evitar confusões com a nova tela de boas-vindas.

* [UI] Resolver problemas de dimensionamento para telas de alto DPI

  Adaptação aprimorada da interface do Painter em telas de alta definição com dimensionamento de exibição personalizado.

* [UI] Evitar mensagens de erro persistentes na interface do usuário

  As mensagens de erro de projetos anteriores agora são removidas da barra de status inferior.

* [UI] Menu de salvamento de retrabalho

  Opções adicionais de salvamento agora estão agrupadas em um submenu e algumas são renomeadas para fins de consistência.

* [UI] Salvar e exportar/compartilhar layouts de interface do usuário

  Dentro do menu Janela existem novas ações para salvar o layout da interface em arquivos e recarregá-los. Os layouts de Pintura e Renderização são salvos separadamente.
  Várias funções foram adicionadas a “substance\_painter.ui” para salvar, redefinir e carregar os layouts de interface também.

* Adicionar ações de copiar/colar para modos de mesclagem/opacidade de uma camada

  Adicionada uma nova entrada “Opções de mesclagem” no menu de contexto camadas. Permite copiar e colar o modo de mesclagem e a opacidade de todos os canais de uma camada para outra.

* Aplicar modo de mesclagem/opacidade a todos os canais de uma camada

  Adicionada a funcionalidade de clicar com o botão direito do mouse ao modo de mesclagem de camadas e à opacidade, que permite aplicar a configuração atualmente clicada a todos os canais.

* Recarregar malha com um atalho de teclado (CTRL+SHIFT+R)

  Foi adicionado um atalho editável para recarregar o arquivo de malha com as últimas configurações disponíveis. Também pode ser acessada em Editar > Reimportar malha.

* Redefinir parâmetros de Substance para padrão

  Adicionado um novo botão em Propriedades na parte inferior dos recursos .sbsar que permite redefinir o recurso para padrão.

* Redefinir pincel para padrão

  Adicionado um novo menu à seção Pincel em Propriedades, o que permite redefinir para o pincel básico padrão.

* Clique com o botão direito do mouse para redefinir os parâmetros de Substance individuais como padrão

  Foi adicionada a possibilidade de redefinir parâmetros individuais em um recurso .sbsar com o botão direito do mouse.

* [Painel Ativos] “Fixe” ativos favoritos para aparecerem sobre o painel Ativos

  Adicionada a nova opção de clicar com o botão direito em ativos da biblioteca que permite fixá-los como favoritos na parte superior do painel. Você também pode exibir todos os seus ativos favoritos em Pesquisas salvas.

* [Painel Ativos] Excluir, recarregar e renomear ativos

  Adicionadas as opções do menu de contexto para excluir, recarregar e renomear ativos na biblioteca do usuário. Eles são excluídos diretamente do local da biblioteca no disco e recarregados do local original. Os ativos que fazem parte de um pacote como .abr ou .sbsar não podem ser editados individualmente.

* [Seleção de cores] Adicionar modos de mesclagem ao efeito Seleção de cores
* [Pilha de camadas] Adicionar modo de mesclagem e opacidade em filtros
* [Pilha de camadas] Permitir valores de divisão em blocos maiores que 128 para camada/efeitos de preenchimento
* [Pilha de camadas] Tampas de cilindro para projeção cilíndrica na camada/efeito de preenchimento

  A projeção cilíndrica nas propriedades da camada de preenchimento agora tem a opção de remover as tampas dos cilindros.

* [Log] Mostra uma mensagem de erro se as partes da malha estiverem em espaço negativo ao tentar criar um projeto de Bloco UV

  Adicionada uma mensagem de erro mais clara ao falhar ao criar um projeto de Bloco UV porque as partes UV são encontradas em espaços negativos.

* [Project] Indica a versão na mensagem de erro “dados muito recentes” ao abrir um projeto

  Ao abrir um projeto que é muito recente para o aplicativo, a mensagem de erro agora indicará a versão do projeto para facilitar a identificação da versão correta do aplicativo.

* [Janela de visualização] Permitir a iluminação da malha por baixo

  Foi adicionado um novo parâmetro de Alinhamento de ambiente em Configurações de exibição > Câmera > Configurações de ambiente para alinhar a iluminação do mapa de ambiente à câmera quando definida como “Local”.

* [Visor] Visualize R, G, B e Alpha no visor (modo de exibição individual)

  Em Configurações de exibição > Configurações do visor > Exibição de canal, há uma nova configuração de Canais de cores que permite exibir apenas o componente R, G, B ou Alpha de um canal quando estiver no modo de exibição única.

* [Shader] Permite definir canais do usuário como RGBA em sombreadores de camada de material

  Ao definir a configuração de canais do Conjunto de texturas dentro de um sombreador para camadas de material, agora é possível especificar o formato do canal para se desviar do valor padrão. Isso permite solicitar canais de usuário coloridos em vez de somente tons de cinza.

* [Exportar] Permite exportar texturas como SBSAR

  Ao exportar texturas por meio da janela Arquivo > Exportar texturas, o formato de arquivo SBSAR (Substance Archive) pode ser escolhido para reagrupá-los. O conteúdo do SBSAR é orientado pelo modelo de saída usado.
  O formato de arquivo SBSAR também pode ser definido nas predefinições de exportação. Ao usar texturas de configuração híbrida (SBSAR + Outro formato) que se destinam a um SBSAR são agrupadas enquanto o restante é exportado junto.

* [Exportar] Opção Expor 16 bits para o formato de arquivo EXR

  Ao exportar arquivos de textura EXR, agora é possível escolher bit 16f (Half-Float) ou bit 32f (Float) na janela Exportar texturas (para configurações de exportação e predefinições de exportação). Projetos antigos e predefinições de exportação antigas terão o bit 16f como padrão para refletir o comportamento antigo.

* [Python] Adicionar evento para saber quando os conjuntos de texturas são modificados

  O novo “substance\_painter.event.TextureStateEvent” permite saber quando um conjunto de texturas foi modificado por causa de um traçado de tinta, um novo canal adicionado ou um canal removido.

* [Python] Permitir obter e definir recursos de Mapa de malha nas configurações de conjunto de textura

  Novas funções foram adicionadas ao módulo “substance\_painter.project” para obter e definir recursos de mapas de malha. Essas funções podem ser usadas para atualizar os mapas de malha referenciados pelas configurações do Conjunto de texturas.

* [Plugins] Remover a opção para obter outros plug-ins JS

  Remoção da opção para obter plug-ins JavaScript, pois eles estavam hospedados no site de compartilhamento obsoleto.

* [Content] Adicionar novo modelo Roblox e exportar predefinição

  Um novo modelo de projeto e predefinição de exportação Roblox “Material Variant” e “Surface Appearance” foram adicionados para facilitar a exportação de texturas PBR para Roblox. O modelo pode ser acessado pela janela Arquivo > Novo projeto.

* Atualize o Substance Engine para a última versão (8.6.3)
* [Steam] Compilação otimizada para o chipset Apple Silicon (Apple M1 / M2)

**Corrigido:**

* Falha ao usar exr 16k
* [Falha] Ctrl Z Após excluir uma instância de sombreador
* [Iray] IoR bloqueada em 1 para alguns sombreadores
* [Win][Cozimento] Falha ao carregar alguns itens de alto polígono
* [Gerenciamento de cores] Nome do espaço de cores incorreto na interface do usuário com filtros
* [Python] Os objetos de recurso retornados pela função de importação não têm um tipo

  Ao importar um pacote Substance em Python, a função estava retornando o pacote em vez de seu(s) gráfico(s). O módulo de recursos agora fornece funções e parâmetros para recuperar o(s) gráfico(s) de um pacote de Substance.

**Problemas Conhecidos:**

* [Gerenciamento de cores] As conversões do espaço de cores HDR com ACE no Linux produzem cores vivas
* [Pilha de camadas] Fonte de entrada não salva por camada
* [Pintura] A suavização temporal causa artefatos ao pintar em alguns casos
* [Exportar] Mapa uniforme de exportações em 2D aleatoriamente

### 8.1.3

*(Lançado: 25 de agosto de 2022)*
Resumo: **Versão de correção de erro secundária**

**Adicionado:**

* Atualização para o Iray SDK 1.6

**Corrigido:**

* [Shader] Falha com o antigo sombreador defeituoso
* [Camada de material] Os materiais podem desaparecer ao reabrir um projeto

**Problemas Conhecidos:**

* [Gerenciamento de cores] As conversões do espaço de cores HDR com ACE no Linux produzem cores vivas
* [Pilha de camadas] Fonte de entrada não salva por camada
* [Falha] Ctrl Z Após excluir uma instância de sombreador
* [Iray] IoR bloqueada em 1 para alguns sombreadores

### 8.1.2

*(Lançado: 19 De julho De 2022)*
Resumo: **Versão de correção de erro secundária**

**Adicionado:**

* [Auto Unwrap] Nova opção “Otimizar para malhas orgânicas” para selecionar o algoritmo de segmentação
* [Tamanho físico] Exponha as opções de unidade em Novo projeto e Configuração de projeto
* [Gerenciamento de cores] Use a exibição de monitor por padrão ao usar o ACE
* [Gerenciamento de cores][Python] Leve em consideração o arquivo de predefinição env-var do ACE ao criar projetos
* [Gerenciamento de cores] Redefinir as configurações de Gerenciamento de cores na janela Novo projeto quando a configuração for alterada
* [Gerenciamento de cores] Desativar o acesso às configurações OCIO quando env-var estiver presente
* [Gerenciamento de cores] Atualizar com segurança as configurações de ACE quando um parâmetro não existir mais
* Atualize o Substance Engine para a versão 8.6.0
* [Exportar] Adicionar nova predefinição de exportação de GLTF com suporte ao Deslocamento
* [Scripting][Python] Recuperar informações de recursos (incluindo metadados personalizados)
* [Scripting][Python] Adicionar função à lista de consulta de nomes de malha por conjunto de textura
* [Conteúdo] Adicionar novo modelo do Blender e exportar predefinição

**Corrigido:**

* [MacOS] Falha ao iniciar o Iray em alguns casos
* [Miniaturas] As miniaturas de prateleira não são carregadas corretamente
* Vários canais UV são ignorados
* [Desempacotar automaticamente] Cálculo desnecessário ao dividir ilhas longas
* [Auto Unwrap] Opção para evitar ilhas alongadas não considerada
* [Desembaçamento automático] Perda de dados extras (cores de vértice) ao recompactar UVs
* [UI] Barra de rolagem horizontal na janela de propriedades quando o Gerenciamento de cores está ativado
* [Gerenciamento de cores] As configurações OCIO não têm a função substance\_3d\_painter\_standard\_srgb
* [Gerador] Uso incorreto de dados do usuário “desativado”
* [Gerenciamento de cores] A lista suspensa Espaço de cor “Não compatível” não deve ser clicável
* [Gerenciamento de cores][Shader] A definição de substituição sRGB não funciona mais
* [Gerador] Uso incorreto de dados do usuário “disable”
* [Pilha de camadas] Visualizações quebradas com projetos de blocos UV
* [Shader] A documentação da API não está totalmente atualizada com os normais tortos
* [Exportar][Interoperabilidade] Não é possível enviar para o Stager com caracteres especiais
* [Conteúdo] Algumas miniaturas de predefinições de pincel estão vazias ou muito escuras

**Problemas Conhecidos:**

* [Gerenciamento de cores] As conversões do espaço de cores HDR com ACE no Linux produzem cores vivas
* [Pilha de camadas] A fonte de entrada não é salva por camada
* [Falha] Ctrl Z Após excluir uma instância de sombreador
* [Iray] IoR bloqueada em 1 para alguns sombreadores
* [Shader] Falha com o antigo sombreador defeituoso

### 8.1.1

*(Lançado: 28 de junho de 2022)*
Resumo: **Hotfix de versão secundária**

**Adicionado:**

* [Pilha de camadas] Alt - clicar na máscara não desmarca mais os efeitos

**Corrigido:**

* [Falha] Abrir projeto antigo salvo no modo de exibição solo
* [Falha] Excluir um gerador nas propriedades
* [Configurações do conjunto de textura] A mistura de Oclusão Normal/Ambiente e o height para os métodos normais estão quebrados
* [Exportar] Exportar texturas usando o preenchimento de difusão renderiza mapas em preto

**Problemas Conhecidos:**

* [MacOS] Falha ao lançar Iray em Monterey
* [Visualizar miniatura] As miniaturas simplificadas não são atualizadas quando uma âncora é usada
* [Gerenciamento de cores] As conversões do espaço de cores HDR com ACE no Linux produzem cores vivas

### 8.1.0

*(Lançado: 07 De junho De 2022)*
Resumo: **Versão principal com suporte ICC, dimensionamento de material com base em dados de tamanho físico, novos panificadores, melhorias de conta-gotas de cores e uma variedade de conteúdos adicionais**

**Adicionado:**

* [Gerenciamento de cores] Adicione suporte para perfis ICC com Adobe Color Engine (ACE)
* [Gerenciamento de cores] Adicione suporte para “Adobe 98 RGB” como espaço de cores de trabalho para ICC
* [Gerenciamento de cores] Permita definir as configurações de ACE/ICC por meio de um arquivo de configuração
* [Gerenciamento de cores] Permitir a entrada de valores de cor linear no Seletor de cores com o modo Legado
* [Gerenciamento de cores] Permite especificar o perfil de cores usado para escolher a cor fora da interface do usuário
* [Gerenciamento de cores] Lembrar o último valor de exibição escolhido na viewport
* [Gerenciamento de cores][Substance] Faça com que os geradores/filtros funcionem corretamente com o Gerenciamento de cores
* [Gerenciamento de cores][Substance] Adicionar novas palavras-chave de substituição colorspace $working e $standardsrgb
* [Tamanho físico][Mecanismo] Extrair informações de tamanho físico da malha
* Cálculo do Tamanho físico [Tamanho físico][Mecanismo]
* [Tamanho físico] Expor as opções para usar o tamanho físico na interface do usuário
* [Tamanho físico] Adicionar auxiliares visuais na viewport
* [Preparação] Adicionar Height
* [Cozimento] Adicionar padeiro de normais curvados
* [Preparação] Adicionar padeiro de opacidade
* [Conta-gotas] Nova visualização de conta-gotas de cor ao lado do mouse e gerenciamento de cores
* [Conta-gotas] O painel Seletor de cores reaparece em sua última posição quando reaberto
* [Conta-gotas] Um novo ícone para o Seletor de materiais
* [Conta-gotas] Gerenciamento de cores da visualização do canal do seletor de cores
* [Conta-gotas] Adicionar a funcionalidade de clicar para selecionar ao conta-gotas
* [Conta-gotas] O seletor de material não ativa mais canais não ativos
* [Conta-gotas] Permitir o uso do conta-gotas com um atalho
* [Conta-gotas] O conta-gotas seleciona o canal relevante, quando aplicável
* [Conta-gotas] Entrar no modo de seletor de cores desativa todos os atalhos
* [Conta-gotas] Remove a seleção automática do campo hexadecimal
* [Conta-gotas] Não fechar o painel ao usar o seletor de material
* [Conta-gotas] Novo estado desativado quando o canal não está disponível para seleção
* [Exportar] Adicionar o atributo tangente à exportação de glTF
* Atualize o Substance Engine para v8.4
* Atualizar a quebra automática para 0. 9. 0
* Atualize para Qt 5.15.8
* Atualização para o Python 3.9
* [Shader] Adicionar suporte para sombreamento Bent Normals
* [MacOS] Suporte a 3DConnection SpaceMouse
* [Python] Documentar a versão Python usada na API
* [Conteúdo] Adicione 6 novos ruídos 3D com 105 predefinições
* [Content] 20 novos mapas de desgaste e 2 padrões de dobras de pano
* [Content] Atualizar a predefinição de exportação “Mapas de malha” para usar novos padeiros
* [Conteúdo] A Inclinação de desfoque e o filtro de distorção dependem da resolução do conjunto de texturas
* [Conteúdo] Atualize projetos de amostra para usar os 3 novos padeiros

**Corrigido:**

* [glTF] Não é possível abrir glTF com caractere especial
* [Engine] Artefatos com anisotropia e SVT desativados
* [MacOS][M1] Os materiais inteligentes não são exibidos corretamente
* [Processamento de malha] Não é possível importar malhas do Modeler
* [UI] Barra de rolagem horizontal na janela do novo projeto com o Gerenciamento de cores ativado
* [Gerenciamento de cores] Valor do espaço de trabalho ausente no seletor de cores com algumas configurações OCIO
* [Gerenciamento de cores] A visualização do pincel na janela de visualização não é gerenciada por cores
* [SpaceMouse] A tabela dinâmica não é atualizada imediatamente com alteração de foco e às vezes fora do modelo
* [Export][USD] Os arquivos USD exportados têm uma estrutura incorreta
* [USD] Problema de Oclusão ambiente ao exportar
* [Conteúdo] Atualizar a malha da miniatura para corresponder ao projeto de amostra da esfera de visualização

**Problemas Conhecidos:**

* Exportar texturas usando o preenchimento de difusão renderiza mapas em preto
* A mistura de Oclusão normal/ambiente está quebrada
* [MacOS] Falha ao iniciar o Iray em alguns casos raros
* [Visualizar miniatura] As miniaturas simplificadas não são atualizadas quando uma âncora é usada
* [Gerenciamento de cores] As conversões do espaço de cores HDR com ACE no Linux produzem cores vivas

## Versão 7

### 7.4.3

*(Lançado: 11 De abril De 2022)*
Resumo: **Correção de erro com suporte a SpaceMouse 3Dconnection em Visor 2D**

**Adicionado:**

* [SpaceMouse] Suporte a 3DConnection SpaceMouse em Visor 2D

**Corrigido:**

* [Seletor de cores] Não é possível gravar em campo hexadecimal
* [Gerenciamento de cores] Os recursos usados no modo de projeção não são gerenciados por cores na sobreposição
* [Gerenciamento de cores] Os erros não são relatados no registro
* [SpaceMouse] Remove a mensagem de erro genérica se o usuário não tiver um SpaceMouse
* [SpaceMouse] Ao carregar um projeto, o ponto dinâmico é sempre oculto
* [Bakers] A configuração “Average normals” não tem efeito em projetos de blocos UV
* [Bloco UV] As sobreposições de blocos uv inativos desaparecem ao recarregar a malha com blocos diferentes
* [Scripting][Python] O script remoto está corrompido
* [Scripting][Python] Vários canais não podem ser consultados pela API e isso gera um erro
* [Scripting][Python] Falha ao usar o evento ProjectEditionEntered
* [Scripting][Python] Falha ao chamar get\_ative\_stack()

**Problemas Conhecidos:**

* Espaço de conexão 3Dsem suporte para mouse no MacOS
* [UI] Barra de rolagem horizontal com gerenciamento de cores exibida em alguns casos em uma nova janela do projeto
* [Mac M1] Os materiais inteligentes não são exibidos corretamente

### 7.4.2

*(Lançado: 08 De março De 2022)*
Resumo: **Correção de erros com suporte a melhorias no 3Dconnection SpaceMouse and color management (OCIO)**

**Adicionado:**

* [SpaceMouse][Windows] Suporte ao SpaceMouse 3Dconnection na Janela de Visualização 3D para navegação
* [SpaceMouse][Windows] Atalhos/teclas básicos para modelos Pro e Enterprise SpaceMouse no visor 3D
* [SpaceMouse][Windows] Ícone do centro de rotação dedicado no visor 3D
* [Gerenciamento de cores] Use funções da configuração OCIO para alterar as configurações padrão
* [Gerenciamento de cores] Gerenciamento de cores na janela de propriedades dos widgets de cores
* [Gerenciamento de cores] Gerenciamento de cores na janela de propriedades para visualização de material
* [Gerenciamento de cores] Amostras de gerenciamento de cores no seletor de cores
* [Gerenciamento de cores] Adicionar uma configuração para definir o espaço de cores sRGB padrão
* [Gerenciamento de cores] Adicionar o espaço de cores sRGB padrão da configuração OCIO no seletor de cores Lista de seletores de exibição
* [Gerenciamento de cores] Melhorias para o menu de substituição do espaço de cores
* [Gerenciamento de cores] Permitir substituição do espaço de cores do mapa de ambiente nas Configurações de exibição
* [Gerenciamento de cores] Desenhar gradientes do seletor de cores com base na exibição atual
* [Gerenciamento de cores] Valores HDR do suporte por padrão no editor de cores
* [Gerenciamento de cores] Usar passagem (sem espaço de cores) para filtros no modo Legado
* [Gerenciamento de cores] Limitar a exibição de gradientes no editor de cores para corresponder ao intervalo [0-1]
* [Gerenciamento de cores] Ocultar seletor de exibição no seletor de cores no modo Legado
* [Gerenciamento de cores] Tornar o seletor de cores hexadecimal sempre no espaço de cores sRGB
* [Gerenciamento de cores] Desativar menu suspenso Exibição do seletor de cores para canais de dados
* [Otimização] A grade de distorção recalcula apenas blocos UV cobertos
* [Exportar] Permitir a exportação de projetos de Bloco UV para Sketchfab, USD e glTF
* [Scripting][Python] Permitir a alteração da função de mapeamento de tom

**Corrigido:**

* [Sketchfab] A atualização do modelo existente acaba criando um novo modelo
* [Sketchfab] Falha ao procurar modelo atualizado anteriormente
* Falha ao exportar para USD
* Falha ao criar uma nova ocorrência de sombreador na Máscara de geometria ou quando a geometria está oculta
* [Janela Importar ativo] Falha ao alterar o tipo de recursos importados
* Os mapas de malha normal são invertidos quando usados em uma pilha de camadas
* [Substance] O modo de mesclagem de dados do usuário não é levado em consideração
* [Gerenciamento de cores] Bitmaps com espaço de cor no nome do arquivo são importados como sequências de Bloco UV
* [Gerenciamento de cores] As saídas gerenciadas por cores do gráfico de Substance estão no espaço de cores incorreto
* [Gerenciamento de cores] A ferramenta Preenchimento de polígono exibe a cor errada
* [Gerenciamento de cores] O mapeador de tons ACES é aplicado a canais no modo solo
* [Gerenciamento de cores] A visualização da ferramenta de iluminação da esfera não é gerenciada por cores
* [Gerenciamento de cores][Exportar] Mapas convertidos aplicam uma conversão incorreta
* [Scripting][Python][Color Management] Os projetos criados com o modelo e a variável de ambiente OCIO estão no modo Legado
* [Scripting][Python] Não é possível usar a função de avaliação JavaScript na inicialização
* [Oferta de Adobe 3D] Não é possível iniciar o Painter ao usar configurações regionais com idiomas não compatíveis por padrão

**Problemas Conhecidos:**

* Espaço de conexão 3Dsem suporte para mouse no MacOS
* [UI] Barra de rolagem horizontal com gerenciamento de cores exibida em alguns casos em uma nova janela do projeto
* [Bakers] A configuração “Average normals” não tem efeito em projetos de blocos UV
* [Mac M1] Os materiais inteligentes não são exibidos corretamente
* [Gerenciamento de cores] Os recursos usados no modo de projeção não são gerenciados por cores na sobreposição
* [Seletor de cores] Não é possível gravar em campo hexadecimal

### 7.4.1

*(Lançado: 14 De dezembro De 2021)*
Resumo: **Correção de erros com melhorias no gerenciamento de cores**

**Adicionado:**

* [Gerenciamento de cores] Usar função de dados em nomes de arquivos exportados
* [Gerenciamento de cores] Expanda a seção Gerenciamento de cores, por padrão, quando o OCIO for selecionado nas novas janelas de configurações do projeto e do projeto
* [Gerenciamento de cores] Adicionar o mapeador de tons ACES no modo herdado
* [Gerenciamento de cores] Ajuste as configurações padrão
* [Gerenciamento de cores][Exportar] Preencher $colorSpace nos nomes de arquivos para canais de dados
* [Exportar] Exportar projeto de Bloco UV para o Stager
* [Interoperabilidade] Não disponível para as edições Steam e Substance
* [Interoperabilidade] Permitir o envio de um projeto de Bloco UV para o Stager

**Corrigido:**

* [MacOS][Falha] O Painter não começa com o Catalina
* [Gerenciamento de cores][Falha] Falha aleatória ao reproduzir o tipo de dados/gerenciamento de cores no canal do usuário
* [Gerenciamento de cores] Recursos usados como tons de cinza no novo menu Espaço de cores de exibição de máscara
* [Gerenciamento de cores] O canal do usuário é mais escuro na viewport no modo legado + visualização individual
* [Gerenciamento de cores] O mapa de ambiente é sempre linear quando usado no iRay
* [Gerenciamento de cores] O seletor de cores não seleciona o valor correto para o canal de dados no modo herdado
* [Gerenciamento de cores] O seletor de cores está quebrado dentro de um Substance no modo herdado
* [Gerenciamento de cores] Alternar entre exibições de canal solo na viewport não é exibido com o espaço de cor certo ao usar o menu suspenso
* [Gerenciamento de cores] Exportar aplica a conversão incorreta em canais de usuário com gerenciamento de cores no modo herdado
* Os traçados feitos na máscara de exibição individual não são exibidos ao voltar para a exibição de material
* [Exportar] Mapas convertidos não são exportados como canais com gerenciamento de cores
* [Texture Set] A dica de ferramenta com o nome original está ausente em canais de usuário renomeados
* [Steam] Arquivos ausentes ao verificar a integridade do arquivo com o Steam

**Problemas Conhecidos:**

* [Mac M1] Os materiais inteligentes não são exibidos corretamente

### 7.4.0

*(Lançado: 24 De novembro De 2021)*
Resumo: **Versão principal. Introdução da 1ª versão de gerenciamento de cores, desencaixe da exibição 2D ou 3D, nova opção de desencapsulamento automático UV para evitar ilhas alongadas, chame funções JavaScript da API Python e novo conteúdo**

**Adicionado:**

* [Gerenciamento de cores] Suporte ao gerenciamento de cores OpenColorIO versão 2
* [Gerenciamento de cores] Adicionar configurações de gerenciamento de cores às configurações do projeto
* [Gerenciamento de cores] Janela de aviso sobre as alterações de configuração do Gerenciamento de cores ao abrir um projeto
* [Gerenciamento de cores] Exibe uma mensagem de erro se um arquivo de configuração OCIO inválido for selecionado
* [Gerenciamento de cores] Permite substituir a configuração pela variável de ambiente OCIO
* [Gerenciamento de cores] Várias configurações OCIO integradas por padrão ao aplicativo
* [Gerenciamento de cores] Extrair o nome do espaço de cores do nome de arquivo bitmap importado
* [Gerenciamento de cores] Permite substituir o espaço de cores por um espaço de cores da configuração na janela Propriedades
* [Gerenciamento de cores] Adicione opções de gerenciamento de cores nas Configurações do conjunto de texturas
* [Gerenciamento de cores][Janela de visualização] Permita o gerenciamento de cores de exibições 2D e 3D separadamente
* [Gerenciamento de cores] Carregue e converta o mapa de ambiente para o espaço de cores de trabalho
* [Gerenciamento de cores] Ajustar o seletor e editor de cores com o espaço de cores atual
* [Gerenciamento de cores] Permite selecionar o espaço da cor de transformação de vídeo no visor com um novo menu suspenso
* [Gerenciamento de cores] Aplicar transformação de exibição com resultados de renderização de matriz
* [Gerenciamento de cores] Exportar texturas com espaços de cores diferentes
* [Gerenciamento de cores][Python] Aplicar configurações de gerenciamento de cores da variável de ambiente (OCIO) aos novos projetos
* [Visor] Permite desencaixar o visor 2D ou 3D
* [Desempacotamento automático] Nova opção para evitar ilhas alongadas
* [Scripting Python] Chamar funções JavaScript da API Python
* [Janela Novo projeto] Tornar a seção de mapas importados flexível
* [Projeção][Distorcer] Permite ocultar normais como uma opção nas configurações de Distorção
* [Conteúdo] 11 novos mapas de desgaste
* [Conteúdo] 8 novas predefinições de ferramenta (zíper, cabo de aperto, brilho)
* [Conteúdo] 8 novos materiais (cicatriz, bolso, ...)
* [Conteúdo] 1 novo gerador (inflar deformação)

**Problemas Conhecidos:**

* [Mac M1] Os materiais inteligentes não são exibidos corretamente
* [Gerenciamento de cores][Falha] Falha aleatória ao reproduzir o tipo de dados/gerenciamento de cores no canal do usuário
* [Gerenciamento de cores] O seletor de cores não seleciona o valor correto para o canal de dados no modo herdado
* [Gerenciamento de cores][Iray] Salvar a renderização em EXR ou TIFF enquanto o Gerenciamento de cores está ativado na janela de visualização sempre será salvo em linear
* [Gerenciamento de cores] Os recursos usados como tons de cinza na máscara exibem o menu Espaço de cores errado
* [Color Management][Iray] O mapa de ambiente é sempre linear quando usado em Iray
* [Gerenciamento de cores][Exportar] Os mapas convertidos não são exportados como canais gerenciados por cores
* [Gerenciamento de cores][Exportar] A exportação ignora se o canal do usuário é gerenciado por cores ou não com o modo legado

### 7.3.1

*(Lançado: 24 De novembro De 2021)*
Resumo: **Correção de erros**

**Adicionado:**

* [Projeção] O dimensionamento deve funcionar somente no Espaço do objeto

**Corrigido:**

* [Mac M1] Camadas de material não funcionam
* [Mac M1][Projeção] A distorção não funciona
* Os microdetalhes não são exibidos corretamente
* [Projeção][Falha] Alternar para o modo de distorção com uma camada criada com uma versão anterior
* [Projeção][Distorcer] O recurso Inverter não funciona quando a transformação está definida como espaço global
* [Projeção][Distorcer] A opção Dividir permanece selecionada após a conclusão da divisão
* [Projeção][UV] O ponto dinâmico é redefinido ao inverter a projeção
* [Filtro] O ambiente de Iluminação do forno está mudando ao recarregar ou alterar um parâmetro
* [Interoperabilidade] Não disponível para as edições Steam e Substance
* [Interoperabilidade] O botão “Pesquisar ativos 3D no Marketplace” sempre deve abrir o CCD na guia Stock e Marketplace 3D

**Problemas Conhecidos:**

* [Mac M1] Os materiais inteligentes não são exibidos corretamente

### 7.3.0

*(Lançado: 13 De outubro De 2021)*
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

### 7.2.3

*(Lançado: 24 De agosto De 2021)*
Resumo: **versão secundária, correção de erro**

**Adicionado:**

* [Bibliotecas] Adicionar uma maneira de impedir que arquivos indesejados sejam rastreados

**Corrigido:**

* [Win] Problemas de suspensão e várias telas
* [MacOS][Falha] Alternar sombreador ao usar efeitos
* [Visor] O modo de visualização completa não mostra mais o cursor do pincel sem alfa
* [IU] O widget Ângulo gira na direção errada
* [Pilha de camadas] Muitas subpastas criam um congelamento muito longo
* [Iray] Visualizações diferentes em Iray e OpenGL: Visível se não estiver funcionando
* [Iray] Índice de refração não levado em conta e não aparece nas propriedades mdl
* [JavaScript] ShowExportDialog() nunca retorna true
* Não é possível ler o mtl do Adobe Stock

### 7.2.2

*(Lançado: 27 de julho de 2021)*
Resumo: **versão secundária, correção de erro**

**Adicionado:**

* Atualizar versão de requisitos de driver AMD

**Corrigido:**

* [Mac M1] Detecção de memória incorreta
* [Exportar] Caminhos muito longos não são exibidos corretamente

**Problemas Conhecidos:**

* [Conteúdo] Sombreadores desatualizados das amostras

### 7.2.1

*(Lançado em: 2 de julho de 2021)*
Resumo: **Versão secundária, Hotfix**

**Adicionado:**

* [Interop] Adicione uma dica de ferramenta para informar que ainda não há suporte ao envio de projetos de Bloco UV para o Stager
* [Plug-in][IU] Atualização do ícone do Livelink

**Corrigido:**

* [Nvidia] A versão do driver começando com 30 é considerada desatualizada
* [Bibliotecas] O estado do painel Ativos não é salvo, a menos que um projeto esteja aberto
* [Bibliotecas] A nova pesquisa salva mantém a palavra-chave da pesquisa salva antiga
* [Bakers][UVTiles] Mapas de ID por meshID também levam os blocos UV em consideração
* [Exportar] Arquivos gLTF não importam a cor do vértice
* [Iray] Algumas dicas de ferramentas estão ausentes
* [Interop] Enviar para o Stager nem sempre é desativado quando o Stager não é detectado
* [Resource Updater] O criador do pincel Photoshop não pode ser atualizado
* [Conteúdo] O gerador de desgaste de borda de vidro de fibra está quebrado

### 7.2.0

*(Lançado: 23 de junho de 2021)*
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
* [Abrir Automaticamente]
* [Desencapsulamento automático] Melhorias no desempenho da Embalagem
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

### 7.1.1 (2021.1.1)

*(Lançado: 23 De março De 2021)*
Resumo: **Versão secundária, correção de erro com possibilidade de inserir valores hexadecimais no seletor de cores**

**Adicionado:**

* [Log] Avisa os usuários sobre drivers de GPU AMD incompatíveis
* [Seletor de cores] Permite digitar valores hexadecimais

**Corrigido:**

* [Baker] Queda no desempenho
* [Máscara de geometria] Clicar com a tecla Alt pressionada no nome da malha pode levar a um travamento
* [Mecanismo] A pintura não atualiza toda a exibição quando necessário
* [Pilha de camadas] A seleção trava após alterar o sombreador
* [MacOS][Seletor de cores] A cor é um pouco diferente da selecionada
* [Exportar] O uso do formato de arquivo PSD não gera um arquivo por Bloco UV
* [Scripting][Javascript] alg.mapexport.getPathsExportDocumentMaps() não retorna todos os valores
* [Scripting][Python] Os plug-ins desativados são ativados novamente ao reabrir o Painter

### 7.1.0 (2021.1.0)

*(Lançado: 28 De Janeiro De 2021)*
Resumo: **Versão principal, nova Máscara de geometria que permite selecionar e pintar partes da geometria, efeitos de cópia/colagem na pilha de camadas, melhoria do fluxo de trabalho de Bloco UV, atualização do Iray, Padeiros, Substance Engine e novo conteúdo**

**Adicionado:**

* Nova máscara de geometria e pintar partes selecionadas da geometria
* [Máscara de geometria] Permite pintar partes selecionadas da geometria por nomes de malha
* [Máscara de geometria] Seleção retangular em ambas as viewports
* [Máscara de geometria] Permite ocultar/ignorar a geometria excluída em qualquer camada
* [Máscara de geometria][Propriedades] Seleção rápida de caixas de seleção com clicar e arrastar
* [Máscara de geometria][Propriedades][IU] Incluir/Excluir tudo com um menu suspenso na janela Propriedades
* [Máscara de geometria][Propriedades] Permite selecionar rapidamente um item em uma lista com ALT+CLIQUE ESQUERDO
* [Máscara de geometria][Propriedades] Sobreposição em viewports ao passar o mouse sobre nomes de malha/blocos UV na janela Propriedades
* [Máscara de geometria][Pilha de camadas] Adicionar opções de copiar/colar à máscara de geometria
* [Máscara de geometria] Novo ícone do botão Ocultar/ignorar geometria excluída
* [Máscara de geometria] Nova dica de ferramenta para Ocultar/ignorar geometria excluída
* [Máscara de geometria] Atalho de teclado ALT+H para ativar/desativar o botão “ocultar ignorar geometria excluída”
* [Blocos UV][Pilha de camadas] Nova miniatura de visualização da esfera da camada de preenchimento para blocos UV e modo simplificado
* [Blocos UV][Pilha de camadas] Permitir sair facilmente da máscara de bloco UV
* [Blocos UV][Lista de conjuntos de texturas] Permite dar uma descrição por Bloco UV
* [Blocos UV][Configurações do conjunto de textura][IU] Dois novos títulos de seção no menu suspenso para alterar a resolução do bloco UV
* [Blocos UV][Visor] Sair da Máscara de bloco UV ao arrastar um material para o visor
* [Pilha de camadas] Adicionar opções de copiar/colar para efeitos
* [Pilha de camadas] Permitir copiar/colar efeitos de um conjunto de texturas para outro
* [Pilha de camadas] Permitir várias seleções de efeitos
* [Pilha de camadas] Adicionar opções de copiar/colar como atalhos para efeitos de camada
* [Pilha de camadas] Alternar automaticamente entre máscara e conteúdo ao arrastar efeitos para outra camada
* [Pilha de camadas] Criar automaticamente uma máscara ao colar uma máscara de outra camada
* [Pilha de camadas] Adicionar ações de efeito de movimento dentro do menu contextual de clique com o botão direito do mouse dos efeitos
* [Pilha de camadas] Permite arrastar e soltar efeitos de uma camada para outra
* [Pilha de camadas] Arrastar itens para uma pasta os coloca na parte superior da pasta
* Atualize o Iray para a versão 2020.1.0
* [Padeiros] Atualize os Padeiros para a versão 2.5.4
* [Padeiros] Exibir blocos UV individuais na janela de progresso da cozedura
* [Padeiros][IU] Permita preparar rapidamente o conjunto de textura atual com um novo botão
* [Padeiros] Permite ao usuário selecionar rapidamente um dos padeiros com ALT + CLIQUE ESQUERDO
* Atualize o Substance Engine para a versão 8.0.8
* [Substance Engine] Suporte à cor padrão em novos arquivos .sbsar
* [Desempacotamento automático] Melhoria de desempenho
* [Exportar] Adicionar feedback visual para indicar qual resolução do bloco UV difere do padrão do projeto
* [Exportar] Adicionar o fator de tamanho da cena no arquivo shader json exportado
* [Idioma] Adicionar tradução para japonês
* [UI] Janela Atualizar sobre com controle de versão de dependências internas
* [Scripting][Python] Permitir gerenciar recursos de prateleira
* [Scripting][Python] Permitir saber quando um projeto está pronto para assar e exportar
* [Scripting][Python] Permitir saber quando uma prateleira terminou de rastrear recursos no disco
* [Scripting][Python] Permite consultar a lista de blocos UV por conjuntos de textura
* [Scripting][Python] Permitir a atribuição de visualização personalizada aos recursos de prateleira
* [Scripting][Python] Permitir gerenciar prateleiras personalizadas
* [Scripting][Python] Adicionar um índice de método em cada submódulo na documentação
* [Scripting][Python] Novo estilo para a documentação
* [Scripting][Python] Aprimoramento de recursos e documentação de prateleira
* [Conteúdo] Três novas predefinições de ferramenta para fazer pontos
* [Prateleira] Remova temporariamente a opção “Exportar para Substance share” durante a transição para a nova plataforma de Substance share

**Corrigido:**

* Falha ao usar monitores com diferentes resoluções
* Falha no Substance Engine com alguns projetos raros
* A atualização do visor falha com a opção Ocultar/Ignorar geometria excluída ao alternar as camadas
* [Visualização 2D] A viewport 2D pode estar ausente em alguns projetos
* [Preparação] “Corresponder pelo nome da malha” ignora partes do objeto
* [Pilha de camadas] Clicar em um efeito de camada abre a pasta
* [Máscara de geometria] O bloco UV ainda é contado na máscara mesmo ao reimportar a malha sem ele
* [Máscara de geometria] O menu do botão direito no visor não fornece as ferramentas corretas
* [Motor] Grandes atrasos em projetos específicos
* [Scripting] Alta latência com solicitações remotas de POST JSON no Windows
* [Linux] A quantidade de Vram não é detectada corretamente com GPUs integradas específicas
* [Desfazer quebra automática] Falha ou desquebra longa em alguns projetos

## Versão 6

### 6.2.2 (2020.2.2)

*(Lançado: 28 De setembro De 2020)*
Resumo: **Versão secundária, correção de erro com algumas funções na API Python**

**Adicionado:**

* [Desempenho] Não calcula todos os blocos UV ao usar a seleção de ID de cor
* [Padeiros][IU] Exibir descrições de conjuntos de texturas
* [Padeiros] Permitir salvar configurações de cozimento
* [Preparadores] Adicionar todas as opções de recolher/expandir todas à guia Seleção
* [Lista de conjuntos de texturas] Ocultar descrição quando vazia
* [Blocos UV][Texture Set List] Clicar em Bloco UV deve expandir/recolher a lista
* [Exportar][IU] Permite redimensionar o painel Lista de conjuntos de texturas horizontalmente
* [Exportar][IU] Texto de dica de ferramenta consistente para Blocos UV e para o fluxo de trabalho Conjunto de texturas com texturas não selecionadas
* [Scripting][Python] Permitir o uso de predefinições de exportação para exportar texturas
* [Scripting][Python] Adicionar um changelog na documentação
* [Scripting][Python] Permite consultar todos os canais disponíveis em uma determinada pilha
* Melhorias na interface do console do [Scripting][Python]

**Corrigido:**

* [AMD] Detecção incorreta de versão de driver desatualizada
* Falha ao reimportar uma malha com um layout de blocos UV diferente em alguns casos
* Falha ao usar partículas com UDIMs em malhas muito pesadas
* [Blocos UV] Falha ao exportar uma malha com informações de deslocamento em alguns casos
* [Exportar][Falha] Exportar exibição 2D em formato psd pode causar uma falha
* Importar imagens como sequências ao criar um projeto não funciona
* Mecanismo travado em um loop infinito
* [Atalho] A câmera gira sempre no modo de ajuste ao alterar os atalhos do modo de ajuste
* As malhas são sempre desempacotadas automaticamente quando reimportadas, mesmo que a opção esteja desativada
* [Texture Set List] O campo de texto de descrição às vezes não é totalmente visível durante a edição
* [Lista de conjuntos de texturas] O menu suspenso para ocultar/reexibir conjuntos de texturas não está totalmente visível
* [Lista de conjuntos de texturas] Clicar no ícone de olho não deve inserir o “Editar nome do conjunto de texturas”
* [Configurações do conjunto de texturas] A remoção de um canal também remove o canal abaixo
* [Exportar] Incluir tudo e Redefinir tudo não leva em consideração os Blocos UV
* [Panificadores] Os panificadores não selecionados aparecem durante a cozedura
* A atualização de resolução não é levada em consideração para mapas baked usados como entrada
* [Blocos UV][Visor] O Visor 3D congela ao adicionar Material inteligente após a pasta com a Máscara de bloco UV selecionada
* [Blocos UV][Visor] O Wireframe ainda está visível para blocos ocultos com o modo Pintar através de
* [Export][Sketchfab] Problemas com o tipo de assinatura “plus”
* [Sketchfab] A caixa de seleção “Este ativo é privado” não é exibida após alternar a conta
* [Exportar][Conteúdo] Predefinições de pincel “onduladas” podem levar a problemas de desempenho
* [Plugin Photoshop] Mensagem no registro: não compatível com o fluxo de trabalho de Bloco UV
* [Scripting][Python] PYTHONPATH env var impede que o aplicativo seja iniciado
* [Scripting][Python] Erro de digitação na documentação do Python

### 6.2.1 (2020.2.1)

*(Lançado: 29 de julho de 2020)*
Resumo: **Versão secundária, Hotfix**

**Adicionado:**

* Adicione a variável de ambiente “SUBSTANCE\_PAINTER\_VRAM\_BUDGET” para substituir a quantidade de VRam da GPU
* [Blocos UV][Desempenho] Não calcula todos os blocos UV ao usar a ferramenta Preenchimento de polígono

**Corrigido:**

* [Iray] Salvar renderização retorna um erro e resulta em uma imagem em preto
* [Linux] Falha após a tela inicial no CentOS 7.3
* [Linux] A quantidade de Vram não é detectada corretamente com configurações específicas
* [Falha] Abrir um projeto com o nome do conjunto de texturas duplicado
* [Engine] Problema de invalidação de cache ao modificar uma máscara
* [Lista de conjuntos de texturas] Efeito de fonte incorreto quando o conjunto de texturas está desativado

**Problemas Conhecidos:**

* [Lista de Conjuntos de Texturas] Não é possível ocultar a descrição
* Problemas de interface do [Texture Set List]
* A renderização do PSD [Iray] não abre
* [Plug-in Photoshop] Não compatível com o fluxo de trabalho de blocos UV

### 6.2.0 (2020.2.0)

*(Lançado: 23 de julho de 2020)*
Resumo: **Versão principal com novo fluxo de trabalho de Blocos UV, pintura em Blocos UV e melhoria de desempenho**

**Adicionado:**

* Blocos UV (UDIMs)
* [Blocos UV] Pintar em blocos UV
* [Blocos UV] Permitir a escolha entre o fluxo de trabalho novo e herdado para Blocos UV
* [Blocos UV] Importar sequências de imagem de blocos UDIMs/UV como um recurso
* [Blocos UV] Adicionar lista de blocos UV por conjunto de textura na janela Lista de conjuntos de textura
* [Blocos UV] Permitir a edição da resolução de vários blocos UV de uma só vez nas Configurações do conjunto de textura
* [Blocos UV][Exibição 2D] Exibir Blocos UV como uma grade
* [UV Tiles][2D View] Novo botão de visor para exibir ou ocultar informações de UV Tiles
* [Ladrilhos UV] Alternar a ferramenta de pintura para canal único por padrão para projetos de Ladrilho UV
* [Blocos UV] Novo botão na barra de ferramentas contextual para ignorar blocos UV mascarados ao pintar
* [Blocos UV][Pilha de camadas] Novos ícones de pilha de camadas para melhorar o desempenho
* [Blocos UV][Pilha de camadas] Aprimorar ícones de pintura e preenchimento na barra de ferramentas
* [Máscara de bloco UV][Visualização 2D] Permite incluir ou excluir vários blocos UV de uma vez (clique com o botão esquerdo, CTRL+clique com o botão esquerdo)
* [Máscara de bloco UV] Nova máscara de bloco UV para incluir, excluir blocos por camada com um novo ícone
* [Máscara de bloco UV][Pilha de camadas] Exibir o número de blocos UV no ícone de máscara de blocos UV quando nem todos estiverem incluídos
* [Máscara de bloco UV][Visualização 2D/3D] Adicionar efeito hover para visualizar blocos UV sob o cursor
* [Blocos UV][Padeiros] Permitir selecionar e assar blocos UV específicos
* [Blocos UV][Padeiros] Adicionar opções de seleção para Conjuntos de textura/Blocos UV
* [Blocos UV][Padeiros] Clique com o botão direito do mouse na opção de menu para selecionar Blocos UV em um conjunto de textura
* [Blocos UV][Padeiros] Permitem a seleção rápida no Conjunto de textura/Blocos UV arrastando
* [Blocos UV][Padeiros] Substituir os botões “Todos” e “Nenhum” nos Mapas de malha por opções de seleção mais explícitas
* [Blocos UV][Padeiros] Exibir o número de texturas a serem assadas
* [Blocos UV][Exportar] Permite selecionar e exportar blocos UV específicos
* [Blocos UV][Exportar] Permitir a seleção rápida de blocos UV arrastando
* [Blocos UV][Exportar] Adicionar opções do menu suspenso para Blocos UV
* [Blocos UV][Exportar] Torne algumas predefinições de exportação indisponíveis se não funcionarem com Blocos UV (Adobe Dimension, Sketchfab, glTF, USD)
* [Blocos UV][Conteúdo] Atualizar predefinições de exportação para usar a nova tag $udim
* [Blocos UV] Aprimorar o relatório de erros ao importar malhas com Ilhas UV sobrepostas
* [UV Tiles] Telhas UV compatíveis em Iray
* [UV Tiles][Scripting] Adicionar documentação de exportação de UV Tile ao documento Python
* Desempenho
* [Desempenho] Botão Novo na barra de ferramentas contextual para pausar o cálculo do mecanismo ao trabalhar (SHIFT+ESC)
* [Desempenho] Abertura mais rápida do projeto com o atraso do cálculo do cache do Conjunto de texturas
* [Desempenho] Não espere os mapas de malha serem carregados ao abrir o projeto
* [Desempenho][Exibição 2D/3D] Não calcular o canal da Máscara no visor quando não estiver em uso
* [Desempenho] Não bloqueia o aplicativo ao carregar mapas de malha exibidos nas viewports
* [Desempenho] Melhorar a velocidade de salvamento incremental ao salvar um projeto
* [Performance][Bakers] Alterar as configurações de dilatação padrão para melhorar a economia de tempo e tamanho do projeto
* [Performance][Bakers] Migre para tons de cinza em padeiros específicos para melhorar a economia de tempo e tamanho do projeto
* [Desempenho][Exportar] Aprimorar o desempenho do mecanismo para exportar texturas mais rapidamente
* [Desempenho][Exportar] Melhore a capacidade de resposta ao abrir a caixa de diálogo de exportação com muitos conjuntos de texturas
* [Desempenho][Exportar] Melhorar o desempenho ao mudar para a guia “Lista de exportações”
* [Performance][Iray] Reduzir o tempo de inicialização do Iray
* Outro
* [Padeiros] Adicionar opções de seleção para Conjuntos de textura
* Mover gerenciamento de instância de sombreador para Configurações de Conjunto de Textura
* [Exibição 2D/3D] Adiciona uma mensagem na parte inferior da viewport para indicar qual tipo de máscara está editado
* [Pilha de camadas] Nova opção nas configurações para alternar entre miniaturas antigas e novas
* [Pilha de camadas] Adicionar feedback visual para indicar o estado de carregamento das miniaturas
* [Proj] Novo modo de projeção “Fill (Match Per UV-Tile)” para carregar sequências de imagens
* [Proj] Altere o modo de projeção das camadas de preenchimento para “Preencher (corresponder por bloco UV)” em casos específicos
* [Conteúdo] Otimizar as predefinições do pincel a carvão para melhorar o desempenho
* Atualize o Iray para a versão 2020.0.0
* [Exportar] Desative a guia Lista de exportações quando nada estiver selecionado
* Desempacotar automaticamente
* [Desfazer quebra automática] Melhorar a taxa de sucesso do processo de desquebra automática
* [Desempacotamento automático] Parametrização aprimorada para aumentar a velocidade e estabilidade

**Corrigido:**

* [Alembic] Os facesets são ignorados ao importar arquivos
* [Alembic] Tempo de carregamento infinito com arquivos específicos
* [Importar] A sequência de imagens UDIM incorreta é importada quando apenas a extensão do arquivo é diferente
* [Falha] A tentativa de abrir um projeto bloqueado por outro processo leva a uma falha
* [Projeção] Artefatos em malha duplicada ao usar projeção triplanar
* [Exportar] O canal emissivo não é exportado com o formato USD
* [Content] Material inteligente “Carvão” contém traçados de tinta

**Problemas Conhecidos:**

* [Lista de Conjuntos de Texturas] Não é possível ocultar a descrição
* Problemas de interface do [Texture Set List]

### 6.1.3 (2020.1.3)

*(Lançado: 16 De junho De 2020)*
Resumo: **Correção de erros**

**Adicionado:**

* [Exportar] Adicionar configurações de deslocamento no arquivo json de parâmetros do Sombreador

**Corrigido:**

* [Falha][Mecanismo] Falha ao tentar apagar e substituir canais existentes
* [Falha] Alterar o sombreador após pintar uma máscara em camadas de material
* [Falha][Mecanismo] Falha com alguns projetos pesados
* [Padeiros] A correspondência por nome não funciona com OBJs exportados do zBrush
* [Deslocamento][SVT] As texturas não são exibidas na abertura do projeto quando o deslocamento está ativado
* [Exportar] Algumas texturas são exportadas com cinza uniforme
* [Exportar] Os conjuntos de textura desativados não devem ser exportados para predefinições de exportação de Dimension e Sketchfab
* [Scripting][JavaScript] Falha ao usar a API JavaScript para acessar a configuração de exportação no evento onProjectOpened
* [Scripting][Javascript] onExportFinished() não é chamado após uma exportação

### 6.1.2 (2020.1.2)

*(Lançado: 28 de maio de 2020)*
Resumo: **Correção de erro com atualização de Substance Engine e Padeiros**

**Adicionado:**

* [Padeiros] Atualização para a versão mais recente
* [Padarias] Novo método de amostragem em Oclusão ambiente, curvatura, panificação de Thickness
* Atualize para a versão mais recente do Substance Engine
* [Scripting][Python] Permitir a criação de ResourceID para recursos do projeto
* [Scripting][Python] Permitir consulta de informações de canal
* [Scripting][Python] Adicione funções dryrun e callback para simular a exportação de textura

**Corrigido:**

* [Bakers] Normais incorretos no padeiro World Space Normals usando um mapa normal tangente em casos específicos
* [Bakers] Erro ao assar Oclusão ambiente com Optix quando não há alta poli
* [Traçados dinâmicos] Atraso ao carregar um conjunto de texturas específico
* [Exportar] Não deve exportar os conjuntos de texturas desativados para USD, glTF
* [Script][JavaScript] Não é possível editar novas configurações do Criador de curvatura
* [Scripting][JavaScript] alg.texturesets.addChannel() não retorna um erro em alguns casos
* [Scripting][JavaScript] Erro de digitação na documentação da API Javascript para setProjectExportOptions()
* [Scripts][JavaScript] Sempre exporta todos os conjuntos de texturas
* [Scripting][Python] sys.executable retorna um caminho para python.exe em vez de Substance Painter
* Cache de textura não compatível com o sistema operacional Mac e Windows/Linux
* [Livelink UE4] Somente o último material é usado para todos os conjuntos de texturas em uma malha combinada

**Problemas Conhecidos:**

* [Export][Dimension][Skecthfab] Não deve exportar os conjuntos de textura desativados
* [Falha] Alterar sombreador depois de pintar uma máscara em camadas de material

### 6.1.1 (2020.1.1)

*(Lançado: 05 de maio de 2020)*
Resumo: **Hotfix**

**Adicionado:**

* [Exportar] Feedback visual de estado substituído no TextureSet

**Corrigido:**

* [Export] Tamanho da janela do exportador muito grande no monitor de resolução especial e não pode ser redimensionado
* [Exportar] As opções não são salvas após a exportação
* [Exportar] Falha ou não é possível exportar com a predefinição de exportação “do cache”
* [Exportar] O cancelamento da exportação gera um mapa vazio adicional inesperado
* [Exportar] Corrigir configurações de predefinição de exportação virtual
* [Python] A variável env PYTHONPATH não é levada em conta
* [Python][Exportar] O cancelamento da exportação via Python retorna um erro de exceção
* [Python][Exportar] exportar\_projeto\_texturas resultado incorreto com formato de arquivo psd
* [Bakers] Falha no Linux com Rastreamento de raios do GPU

**Problemas Conhecidos:**

* [JavaScript] Não é possível editar as novas configurações do criador de curvatura
* [JavaScript][Exportar] Sempre exporta todos os conjuntos de texturas
* [Export][USD] Não deve exportar os conjuntos de textura desativados
* [Falha] Alterar sombreador depois de pintar uma máscara em camadas de material

### 6.1.0 (2020.1.0)

*(Lançado: 22 De abril De 2020)*
Resumo: **Versão principal com Novo exportador de textura e malha (com deslocamento e mosaico), desempacotamento UV atualizado com mais controles, novos padeiros, nova API python de script, melhor UX para projeção de decalques e novo conteúdo**

**Adicionado:**

* Novo exportador de textura e malha
* [Exportar] Interface de novo exportador
* [Exportar][guia Exportar] Permite a seleção dos canais de mapas que são exportados por conjunto de textura
* [Exportar][Guia Exportar] Permite a modificação do tamanho do Conjunto de texturas para todos os Conjuntos de texturas em uma ação
* [Exportar][guia Exportar] Permite um modelo diferente por conjunto de textura (exceto USD, glTF, Sketchfab e Dimension)
* [Exportar][guia Exportar] Ativação e desativação rápidas de mapas e conjuntos de texturas
* [Exportar][Guia Exportar] A resolução de exportação 8192 x 8192 não é mais experimental
* [Exportar][guia Exportar] Permite a modificação do formato de arquivo e a profundidade de bits por mapa
* [Exportar][guia Exportar] Permite redefinir os valores dos parâmetros padrão
* [Exportar][guia Exportar] Permite que as configurações sejam salvas sem exportar
* [Exportar][guia Modelos de saída] Renomeie a guia “Configuração” para a guia “Modelos de saída”
* [Exportar][guia Modelos de saída] Permite a definição de formato de arquivo e a profundidade de bits por mapa predefinido
* [Exportar][Guia Lista de exportações] Nova guia de visualização para resumir e visualizar o processo de exportação
* [Malha de importação/exportação] Otimização de desempenho de tempo de importação/exportação
* [Exportar malha] Exportar malha em FBX
* [Exportar malha] Exportar malha com deslocamento e mosaico
* [Exportar malha][IU] Novas configurações para recalcular vértice normal, aplicar triangulação
* [Exportar malha] Exporte a topologia de malha original com novos UVs gerados pelo desencapsulamento automático
* Desencapsulamento automático UV atualizado com mais controles
* [Desempacotamento UV][IU] Adicionar configuração para ativar o desempacotamento UV automático na nova janela do projeto
* [UV Unwrapping][UI] Novas opções para controlar os passos de abertura (costuras, abertura, embalagem)
* [UV Unwrapping][UI] Permitir a conservação de emendas de abertura/desembrulho/embalagem existentes
* [UV Unwrapping][UI] Novas opções para recalcular totalmente as etapas de desencapsulamento
* [UV Unwrapping][UI] Nova opção para controlar o tamanho da margem (nenhum, pequeno, médio e grande)
* Novos Panificadores
* [Padarias] Substituir a curvatura antiga pela nova curvatura da malha
* [Padeiros] Adicione a opção de correspondência por nome para ignorar a face traseira no padeiro “Oclusão ambiente”
* [Padeiros] Adicionar opção de plano de chão no padeiro “Oclusão ambiente”
* Nova API de script do Python (3.7.6)
* [Python][UI] Novo menu de scripts para o Python
* [Python][UI] Nova documentação do Python no menu Ajuda
* [Python] Expor módulos Substance Painter python: substance\_painter, alg, display, project.setting, project, texturesets, ui
* [Python] Expor novo módulo Python “substance\_painter”
* [Python] Expor novo submódulo Python: alg, display, log, project, resource, texturesets, ui
* [Python] Ouvinte para alterações de projeto
* [Python] Novos exemplos na documentação do Python
* [JavaScript][UI] Menu de plug-ins substituído pelo JavaScript
* [Visor] Permite a criação de uma projeção de decalque “arrastando/soltando + ALT” um recurso da prateleira
* Novo conteúdo
* [Content] 5 novos materiais de decalque do Substance Source
* [Content] Adicionar novos modelos de projeto e predefinições de exportação para o renderizador Maxwell
* [Content] Adicionar modelo de projeto para exportação do Keyshot 9
* [Content] Atualize a predefinição de exportação Keyshot 9 para oferecer suporte a deslocamento e emissivo
* [Conteúdo][Exportador] Atualização de todas as predefinições de exportação para corresponder às versões mais recentes de mecanismos e renderizadores de jogos
* [Conteúdo][Exportador] Atualizar arquivos de predefinições de exportação para usar o novo formato e configurações de pontilhamento
* [Content] Novos modelos e sombreadores para suportar material VRay (VRayMtl)
* [Pilha de camadas] Permitir exclusão de efeitos de camada usando o ícone de lixeira ou o atalho de teclado Excluir
* Remover o Substance Source de plug-in (use o iniciador com a funcionalidade “enviar para”)
* [Windows] Não exibir aviso de TDR em GPUs de alta capacidade

**Corrigido:**

* Problemas de tradução na caixa de diálogo Novo arquivo de projeto
* [Padeiros] A configuração “Salvar arquivo de cena pré-processado” não funciona mais
* [Projeção planar] A projeção não funciona em malhas com UVs repetidos
* [Decalque] Diferença de comportamento no canal normal ao usar diferentes modos de projeção de camada de preenchimento
* [Borrar][Clonar] O artefato pode aparecer ao pintar em uma máscara
* [Engine] Falha com conteúdo de camada específico
* [Engine] Falha aleatória ao pintar em alguns casos
* [Ponto de ancoragem] A referência a uma máscara vazia sempre retorna branco
* [Exportar] Camada não considerada em algumas configurações de pilha específicas
* [Exportar malha] Não é possível exportar com caminho que contém caracteres especiais
* [Exportar malha] Não é possível ler arquivos glTF quando exportado do Linux ou MacOS
* [Importar malha] A reimportação do DAE, PLY ou glTF não funciona conforme o esperado

**Problemas Conhecidos:**

* [Script][JavaScript] Não é possível editar novas configurações do Criador de curvatura
* [Bakers] Falha no Linux com Rastreamento de raios do GPU
* [Export][USD] Não deve exportar os conjuntos de textura desativados
* [Falha] Alterar sombreador depois de pintar uma máscara em camadas de material

## Versão 5

### 5.3.3 (2019.3.3)

*(Lançado: 06 De fevereiro De 2020)*
Resumo: **Correção de erro com a atualização para o Iray 2019.3**

**Adicionado:**

* Atualização para o Iray 2019.3
* [Log] Indica bios desatualizado para CPU Ryzen levando a falha durante a cozedura
* [ABR] Extrair alfa ABR para prateleira

**Corrigido:**

* [Baker] Falha na cozedura se a malha de alto-poli não tiver UVs
* [Linux] Os atalhos de mouse personalizados não são salvos
* [Pincel] O contorno desaparece com algumas formas alfa
* [Tablet] Detecção incorreta ao mover controles deslizantes
* [Atalhos] Não é possível configurar nenhum atalho com “Ctrl+Alt+Clique do Mouse”
* [Prateleira] Não é possível ver a dica de ferramenta do recurso ao usar um tablet com caneta
* [2D View][Export] A predefinição de exibição 2D não leva em consideração as informações normais
* Congela ao pintar em alinhamento UV com determinados pincéis
* Pintar sob um filtro cria artefatos no traçado em andamento
* [Visor] Cache de textura incorreto no visor após a reimportação de uma malha
* [Falha] Erro ao salvar após exportar para o Photoshop
* [Falha] Gravar símbolos especiais no prefixo ao importar recursos
* [Falha] Clique na referência em Propriedades de ponto de ancoragem
* [Pontos de ancoragem] O canal não é atualizado quando há um filtro entre o ponto de ancoragem e a referência
* O link de URL do Iray no menu Ajuda não funciona

**Problemas Conhecidos:**

* [Desempacotamento UV] O processamento de malhas de alta polarização pode demorar muito tempo
* [Desempacotamento UV] Os vértices exatamente nas mesmas coordenadas são mesclados
* [UV Unwrapping] A geração de UV pode falhar em algumas partes da malha em alguns casos raros
* [Desempacotamento UV] Proporção de texel não uniforme ou altamente distorcida em uma única Ilha UV em alguns casos
* [Desempacotamento UV] Relação de texel não uniforme entre conjuntos de textura
* [UV Unwrapping] A Ilha UV gerada pode ser muito alongada e não se encaixar no espaço UV em alguns casos
* [Desempacotamento por UV] Faces degeneradas ou faces de malha não triangulares com bordas pequenas ou sobrepostas podem não ter o UV desempacotado

### 5.3.2 (2019.3.2)

*(Lançado: 21 De Janeiro De 2020)*
Resumo: **Correção de erros**

**Corrigido:**

* Abrir um projeto que foi salvo no modo de canal individual não exibe a malha
* A janela de visualização nem sempre é atualizada ao pintar sob uma camada usando a ferramenta clone

**Problemas Conhecidos:**

* [Bakers] Falha relacionada a multi-threading em CPUs Ryzen
* [Desempacotamento UV] O processamento de malhas de alta polarização pode demorar muito tempo
* [Desempacotamento UV] Os vértices exatamente nas mesmas coordenadas são mesclados
* [UV Unwrapping] A geração de UV pode falhar em algumas partes da malha em alguns casos raros
* [Desempacotamento UV] Proporção de texel não uniforme ou altamente distorcida em uma única Ilha UV em alguns casos
* [Desempacotamento UV] Relação de texel não uniforme entre conjuntos de textura
* [UV Unwrapping] A Ilha UV gerada pode ser muito alongada e não se encaixar no espaço UV em alguns casos
* [Desempacotamento por UV] Faces degeneradas ou faces de malha não triangulares com bordas pequenas ou sobrepostas podem não ter o UV desempacotado

### 5.3.1 (2019.3.1)

*(Lançado: 20 de dezembro de 2019)*
Resumo: **Hotfix**

**Corrigido:**

* Falha ao trabalhar em malhas com Projeções UV específicas
* [ABR] Falha ao alternar entre predefinições Photoshop
* [Linux] Não é possível iniciar o Substance Painter no CentOS 7.4 devido a um problema de dependência do libGLX
* [Padeiros] Falha ao assar após usar Arquivo > Limpar
* [Padeiros] A caixa de diálogo de progresso da cozedura congela após o cancelamento
* [Padarias] A malha de cozimento após a exportação de texturas não funciona
* [Padarias] O uso da opção “Corresponder por nome” resulta em mapas de malha pretos
* [Padeiros] A gaiola não é tida em conta
* [Prateleira] Importar arquivos de PSD leva a imagens quebradas
* [Amostra] O projeto de amostra “Mat” possui câmeras quebradas e predefinição de exportação incorreta

**Problemas Conhecidos:**

* [Bakers] Falha relacionada a multi-threading em CPUs Ryzen
* [Desempacotamento UV] O processamento de malhas de alta polarização pode demorar muito tempo
* [Desempacotamento UV] Os vértices exatamente nas mesmas coordenadas são mesclados
* [UV Unwrapping] A geração de UV pode falhar em algumas partes da malha em alguns casos raros
* [Desempacotamento UV] Proporção de texel não uniforme ou altamente distorcida em uma única Ilha UV em alguns casos
* [Desempacotamento UV] Relação de texel não uniforme entre conjuntos de textura
* [UV Unwrapping] A Ilha UV gerada pode ser muito alongada e não se encaixar no espaço UV em alguns casos
* [Desempacotamento por UV] Faces degeneradas ou faces de malha não triangulares com bordas pequenas ou sobrepostas podem não ter o UV desempacotado

### 5.3.0 (2019.3.0)

*(Lançado: 17 de dezembro de 2019)*
Resumo: **Versão principal com melhoria na experiência do usuário de pintura manual, trabalho com tablets, desencapsulamento automático de UV em beta (0.3.0) e conteúdo novo diversificado para pintura manual**

**Adicionado:**

* Integrar a versão 0.3.0 de desenrolamento automático de UV no Substance Painter
* [Desencapsulamento UV] Desencapsulamento UV automático em Substance Painter quando nenhum UV presente ou UVs parciais
* [Desencapsulamento UV] Uma configuração global para ativá-lo e desativá-lo
* [Desencapsulamento UV] Versão relatada no arquivo de log
* [Desencapsulamento UV][IU] Indicar progresso do desencapsulamento UV
* [UI] Novas configurações na barra de ferramentas contextual para selecionar a visualização do pincel: visualização completa, contorno e mira
* [Ferramenta] Novo modo de mesclagem avançado na seção alfa: Clarear (máximo) além de Normal
* [Pilha de camadas] Opção de correção de gama por camada para alfa ou máscara (menu do botão direito do mouse)
* [Pilha de camadas][IU] Adicionar ícone &#39;i&#39; quando um alfa de camada for corrigido para a gama
* [Tablet][Ferramenta] Expor a pressão mínima para tamanho e fluxo
* [Tablet][IU] Nova configuração na barra de ferramentas contextual para selecionar a pressão da curva: linear, fácil de entrar, fácil de sair
* [Tablet][UX] Adicionar Ctrl+Alt+clique para rolar
* Importar predefinições de pincel do Photoshop (formato ABR)
* [ABR] Suporte a parâmetros de forma
* [ABR] Suporte a parâmetros de dinâmica de forma
* [ABR] Parâmetros de transferência de suporte
* [ABR] Parâmetros de dispersão de suporte
* [ABR][Traçados dinâmicos] Redondez e giro de suporte
* [ABR][Prateleira] Expor a estrutura de pastas de pincéis no Editor de filtros
* [ABR][Prateleira] Adicionar ícone do Photoshop em miniaturas
* [ABR][Prateleira] Adicionar lista de parâmetros não suportados na miniatura detalhada do ABR
* [Ferramenta][Traçados dinâmicos] Nova configuração de traçado dinâmico para controlar a quantidade de semente aleatória a ser gerada
* [Ferramenta][IU] Adicionar nova distribuição e configurações de eixo para dispersão de tremulação
* [Atalho] Adicione Ctrl+Shift+B para abrir a janela Cozimento
* [UI][Menu] Adicionar entrada no menu “Editar” para abrir a janela Cozimento
* [UI][Configurações] Aprimoramento do alinhamento da lista de atalhos
* [IU] Substituir ícones de controles de pressão (tamanho e fluxo) por botões de ligar/desligar
* [Janela de visualização] Permitir focalizar as portas de visualização 2D e 3D separadamente
* Atualize para QT 5.12.5
* [IU] Indicar progresso do carregamento de malha
* [Substance] Adicione suporte para faixa suave e não fixa com controles deslizantes
* [Substance] Aumente a precisão dos parâmetros de Substance até 6 decimais
* [Substance] Considere a etapa definida por um parâmetro
* [Substance] Otimizar a geração de traço dinâmico com suporte a condições nos dados do usuário
* [Substance] Permitir designar uma saída de gráfico como uma máscara para todos os canais via userdata
* [Content] Atualizar projeto de amostra &#39;Mat&#39; com topologia amigável ao deslocamento, novo mapa de ID e novas câmeras
* [Conteúdo] Integrar 3 novos filtros (MatFx): Quadrinhos, Aquarela, Pintura a óleo (inspirada no trabalho de Emrecan Cubukcu)
* [Conteúdo] Integrar 102 predefinições de pincel Photoshop dos pacotes de Kyle T. Webster
* [Content] Integrar 18 novas predefinições de pincel: Seta de rolo de pintura, Texto de aviso de rolo de pintura, Carvão fino e muito mais
* [Content] Integrar 9 novas alfas: rolo de pintura do criador de pincel, Photoshop do criador de pincel, padrões de pincel e muito mais
* [Content] Integrar 2 novas predefinições de ferramenta: Gouache Dense e Gouache Faded
* [Conteúdo] Integrar 1 novo gerador : verificador UV (destacar Ilhas UV e costuras)
* [Content] Integrar 2 novas predefinições de exportação: Keyshot 9+ e Spark AR Studio
* [Content] Integrar 1 novo modelo de projeto: Spark AR Studio (Facebook)

**Corrigido:**

* [Tablet] Desfazer traçados da caneta (Ctrl + Z) atrasa mais do que desfazer traçados do mouse
* [Tablet] A pressão inicial e final não é considerada ao desenhar uma linha reta
* [Tablet] O primeiro carimbo é desenhado duas vezes ao usar uma linha reta
* [Tablet] Aprimorar o suporte para atalhos de tablet Huion
* [Tablet] Aprimorar o suporte para botões de caneta Huion
* [Tablet] Deslocamento entre a visualização do pincel e o carimbo desenhado
* [Tablet] Os atalhos para modificar pincéis com caneta resultam em baixo desempenho em casos raros
* [Tablet] Atraso ao pintar em uma camada específica
* Texturas desfocadas podem ocorrer em casos raros ao alternar entre viewport
* [UI][Substance] As entradas de imagem nem sempre são exibidas
* Limpar não remove as predefinições da prateleira que foram importadas em um projeto
* [Tool][Dynamic Stroke] Problema de desempenho ao ajustar a contagem de ciclos de carimbo
* Problemas de atualização ao pintar no modo de visor 3D/2D em casos raros
* Pintar um traçado muito longo pode causar congelamento
* [Ferramenta] Problema de desempenho ao pintar com traçados dinâmicos específicos
* [UI] A barra de ferramentas contextual ainda exibe as propriedades do pincel ao selecionar uma pasta
* Os valores do eixo de simetria não são redefinidos
* A importação de texturas EXR com valores de ponto flutuante é totalmente preta
* Alt+clique em um canal para isolar não funciona para filtro e gerador
* [Export] Falha específica do projeto na exportação
* [Substance] Valor padrão incorreto no menu suspenso se o parâmetro estiver oculto por Visible If
* [Shader] Os canais definidos por meio da Camada de material não são classificados da mesma maneira na interface do usuário
* [Prateleira] Os metadados de predefinições não são salvos no disco

**Problemas Conhecidos:**

* [Desempacotamento UV] O processamento de malhas de alta polarização pode demorar muito tempo
* [Desempacotamento UV] Os vértices exatamente nas mesmas coordenadas são mesclados
* [UV Unwrapping] A geração de UV pode falhar em algumas partes da malha em alguns casos raros
* [Desempacotamento UV] Proporção de texel não uniforme ou altamente distorcida em uma única Ilha UV em alguns casos
* [Desempacotamento UV] Relação de texel não uniforme entre conjuntos de textura
* [UV Unwrapping] A Ilha UV gerada pode ser muito alongada e não se encaixar no espaço UV em alguns casos
* [Desempacotamento por UV] Faces degeneradas ou faces de malha não triangulares com bordas pequenas ou sobrepostas podem não ter o UV desempacotado
* A amostra do metamat tem alguns problemas com câmeras importadas

### 5.2.3 (2019.2.3)

*(Lançado: 23 de outubro de 2019)*
Resumo: **Versão de correção de erros**

**Adicionado:**

* [Texture Set List] Adicionar botão para ativar/desativar rapidamente o modo de foco
* [Log] Adiciona o número de versão do Windows 10 no arquivo de log
* Atualize para a versão mais recente do Substance Engine
* [MacOS] Autenticação do software para atender aos novos requisitos de distribuição do MacOS Catalina

**Corrigido:**

* [Plug-in] A origem do plug-in não funciona
* [MacOS][Shader] Mac OS 10.14.5 e AMD: a disposição em camadas de material não funciona conforme o esperado

**Problemas Conhecidos:**

* Arquivos Alembic com subdivisões não podem ser importados
* Falhas raras ao importar alguns arquivos Alembic
* A interface não responde temporariamente ao assar com DXR em GPUs Pascal

### 5.2.2 (2019.2.2)

*(Lançado: 20 De setembro De 2019)*
Resumo: **Versão de correção de erros**

**Corrigido:**

* A importação de recursos por scripts pode causar uma falha
* [Plug-in] Baixar material da origem pode levar a uma falha

**Problemas Conhecidos:**

* Arquivos Alembic com subdivisões não podem ser importados
* Falhas raras ao importar alguns arquivos Alembic
* A interface não responde temporariamente ao assar com DXR em GPUs Pascal

### 5.2.1 (2019.2.1)

*(Lançado: 17 de setembro de 2019)*
Resumo: **Versão de correção de erros**

**Corrigido:**

* [Mac][USD] Arquivos USDZ exportados do MacOS não podem ser abertos
* [Conjunto de texturas] Não é possível isolar um conjunto de texturas com o modificador ALT
* [Prateleira] Predefinições, Materiais inteligentes e Máscaras inteligentes são sempre modificados ao sair do aplicativo
* [Pilha de camadas] Não é possível selecionar o efeito após excluir outro efeito
* Cintilação ao usar um controle deslizante dentro do painel de propriedades da ferramenta
* Falha ao exportar predefinições para prateleira
* Falha ao exportar uma predefinição com espaço insuficiente
* Falha ao criar uma predefinição com espaço insuficiente

**Problemas Conhecidos:**

* Arquivos Alembic com subdivisões não podem ser importados
* Falhas raras ao importar alguns arquivos Alembic
* A interface não responde temporariamente ao assar com DXR em GPUs Pascal

### 5.2.0 (2019.2.0)

*(Lançado: 25 de julho de 2019)*
Resumo: **Lançamento principal com atualizações dos padeiros em termos de desempenho e um novo modo de pré-visualização + novo conteúdo**

**Adicionado:**

* [Padarias] Suporte adicionado para Rastreamento de raios do GPU com DXR e OptiX (Oclusão ambiente, Thickness)
* [Bakers] Otimizações e acelerações para o rastreamento de raio da CPU
* [Padeiros][Modo Vis][IU] Novo modo de visualização de cozimento no visor
* [Bakers][Preferences][UI] Nova opção de cozimento para ativar/desativar o Rastreamento de raios do GPU
* [Padeiros][IU] Retrabalho da caixa de diálogo da barra de progresso
* [Padeiros] Melhoria das mensagens de aviso e de erro
* [Padeiros] Permitem o cancelamento mais responsivo do processo de cozimento
* [Padeiros] Reabrir a janela do bolo após clicar em Cancelar
* [Proj][UX] Melhoria da usabilidade do manipulador de rotação
* [Settings] Opção para melhorar o desempenho reduzindo a resolução do visor para telas HDPI
* [Script] Alterar resolução do conjunto de texturas
* [Script] Obter conjunto de textura selecionado
* [Script] Permite que o usuário selecione um conjunto de texturas
* [Scripting] Função para saber quando a seleção do conjunto de texturas foi alterada
* [Prateleira] Adicionado 40 novos materiais inteligentes
* [Prateleira] Adicionado 20 novas máscaras inteligentes

**Corrigido:**

* [Pilha de camadas] Congelamento da interface do usuário ao selecionar várias camadas
* [Pilha de camadas] Agrupar muitas camadas congela a interface por mais tempo do que o normal
* [Pilha de camadas] Uma camada e um efeito podem ser selecionados ao mesmo tempo em alguns casos
* os gráficos de Substance usados nas ferramentas de pintura não são gerados na resolução correta
* [Baker] O botão “Cozinhar todos os conjuntos de textura” não é desativado quando nenhum padeiro está selecionado
* [MacOS] Desativar a mensagem de aviso sobre o mosaico
* A ferramenta de projeção não tem visualização quando usada com uma máscara
* Falha e projetos corrompidos ao tentar salvar com espaço em disco insuficiente
* [Shelf] Falha ao importar um recurso no disco via shelf com espaço insuficiente
* [Prateleira] Falha ao restaurar a predefinição de sessão
* [Prateleira] Importar uma predefinição com um nome que termina com um espaço leva a uma falha
* [Prateleira] Importar um recurso com um prefixo que termina com um espaço vazio leva a uma falha

**Problemas Conhecidos:**

* Arquivos Alembic com subdivisões não podem ser importados
* Falhas raras ao importar alguns arquivos Alembic
* A interface não responde temporariamente ao assar com DXR em GPUs Pascal

### 5.1.3 (2019.1.3)

*(Lançado em: 01 de julho de 2019)*
Resumo: **Correção de erro com 2 novos recursos**

**Adicionado:**

* Permite especificar o orçamento VRam com uma linha de comando (por exemplo, —vram-budget 4096)
* [QML] Expor as propriedades wrapMode e elide dos botões e caixas de seleção do QML

**Corrigido:**

* “Seguir caminho” não funciona o tempo todo
* O mapeamento de canal não funciona com SBSAR usado em slots de canal único
* [Pilha de camadas] Baixo desempenho ao rolar com camadas ocultas
* [TextureSet] Falha ao clicar entre máscaras
* [SVT] O Deslocamento não é exibido corretamente e pisca em alguns casos
* [Alembic] Falha com malha usando normais de ponto em vez de normais de vértice
* [Alembic][Log] Relata um erro no Log se o arquivo Alembic não for suportado durante a importação

**Problemas Conhecidos:**

* Arquivos Alembic com subdivisões não podem ser importados
* Falhas raras ao importar alguns arquivos Alembic

### 5.1.2 (2019.1.2)

*(Lançado: 21 de maio de 2019)*
Resumo: **Hotfix**

**Corrigido:**

* Falha ao selecionar dois recursos com uma entrada de imagem

### 5.1.1 (2019.1.1)

*(Lançado: 20 de maio de 2019)*
Resumo: **Hotfix**

**Adicionado:**

* Atualize para a versão mais recente do Substance Engine com a última versão do Substance Designer 2019.1

**Corrigido:**

* [Substance] Visível Se não for levado em consideração para Imagens de entrada
* [SVT][Mecanismo] Alterar a resolução do conjunto de texturas leva a uma falha em alguns casos
* [Engine] Texturas pretas aleatórias aparecem em alguns casos
* [Pilha de camadas][IU] Alternar uma máscara com SHIFT pode selecionar várias camadas ao mesmo tempo
* [Pilha de camadas] A opacidade não tem efeito no efeito Pintura com o modo de mistura Passagem
* [Pilha de camadas] A entrada do filtro Height para normal não é atualizada corretamente com o traçado do pincel de borracha
* [LayersStack] Falha ao desfazer o soltar de uma máscara inteligente
* Wireframe piscando com sombras e suavização de borda temporal ativada
* [Deslocamento] Atraso na AMD com algumas malhas pesadas
* [Windows] Falha ao abrir alguns projetos por meio do explorador de arquivos
* [Histograma] Falha ao remover a máscara com o ponto de ancoragem em alguns casos
* Falha na geração de visualização em alguns casos raros
* [Falha] Não é possível reabrir um projeto usando muitas ferramentas de clonar e borrar
* Nenhuma malha exibida no modo de material após salvar em alguns casos
* [Scripting] alg.mapexport.documentStructure() retorna valores incorretos para pastas

**Problemas Conhecidos:**

* Clicar duas vezes no nome do conjunto de texturas o selecionará antes de entrar no modo de renomeação

### 5.1.0 (2019.1.0)

*(Lançado: 23 de abril de 2019)*
Resumo: **Traçado dinâmico com novo conteúdo dedicado, Deslocamento e mosaico em tempo real e Iray, efeito Comparar máscara, simetria radial, Planar e Projeção esférica**

**Adicionado:**

* [Ferramenta] Traçado dinâmico: variação de Substance ao lado de um traçado de pincel
* [Traçado dinâmico] Expor novo parâmetro de índice de carimbo com opções
* [Traço dinâmico] Leve em consideração o parâmetro $time
* [Traço dinâmico] Gera novo parâmetro $randomseed por traço e por carimbo
* [Traçado dinâmico] Iniciar um índice de traçado dinâmico a partir de um número aleatório
* [Dynamic stroke][Prateleira] Ajuda a encontrar um recurso de traçado dinâmico com novo ícone dedicado
* Deslocamento e mosaico em viewport em tempo real
* Deslocamento e mosaico em Irlanda
* [Configurações do sombreador][IU] Nova guia para controlar deslocamento e mosaico
* [Pilha de camadas] Novo efeito CompareMask: gerar uma máscara comparando dois canais
* [Pilha de camadas][IU] Nova entrada no menu do botão direito do mouse “Adicionar máscara com combinação de height” para inserir um efeito CompareMask
* [Simetria] Novo modo de simetria: pintura radial
* [Configurações de simetria] Expande as duas seções “Configurações” e “Exibição”
* [Configurações de simetria][IU] Visualização para pintura radial
* Exponha dois novos modos de projeção: planar e esférico
* [Proj] Novo modo de corte de forma para todas as projeções
* [Proj] Modo planar com novo manipulador: ferramenta Superfície
* [Proj][Atalho] Atalho SHIFT+W para a ferramenta Superfície
* [Proj] Máscara de projeção planar com seleção de profundidade e abate de backface
* [Manipulador] Melhoria do manipulador de rotação nos três eixos para triplanar
* [Tool][UX] Clicar com a tecla Alt pressionada em um canal focaliza esse canal (ativa ou desativa todos os outros)
* [Engine] Atualização para a versão mais recente do Substance Engine
* [Conjunto de textura] Seleção múltipla e resolução de alteração
* [Conjunto de textura] Ativação e desativação rápidas dos conjuntos de textura
* [Conjunto de texturas] Combina solo e todas as opções em um novo menu
* [Conjunto de texturas][Pilha de camadas] Novo ícone para ativação e desativação
* [Pilha de camadas][UX] Inserir efeitos acima dos já selecionados
* [Pilha de camadas][IU] Retrabalhar o estilo de seleção da exibição da pilha de camadas
* [Pilha de camadas] O modo de mesclagem para camadas instanciadas agora está no modo de Passagem por padrão
* [Exportar] Opção para ativar e desativar o pontilhamento
* [Plug-in] Suporte ao modificador de precisão para controles deslizantes (SHIFT)
* [Plug-in][IU] Novo ícone para salvamento automático
* [Scripts] Lista o conteúdo de uma pasta
* [Script] Permitir exclusão de arquivos
* [Scripts] Ler todas as informações da pilha, inclusive os recursos usados
* [Conteúdo][Traçado dinâmico] Novas ferramentas e predefinições de pincel
* [Conteúdo][Traço dinâmico] Dois novos gradientes de procedimento: Matiz de gradiente e Construtor de gradiente
* [Content] 11 novos filtros: Pintura de descascamento MatFx, gotas de água MatFx e muito mais
* [Content] 7 novos geradores: Auto Stitcher, Cor aleatória UV, Densidade de texel UV e muito mais
* [Content] 93 novos alfas: novos textos, setas e várias outras formas
* [Conteúdo] 2 novos procedimentos: Matiz de gradiente, Construtor de gradiente e muito mais
* [Content] 21 novas predefinições de ferramenta e pincel para Traçados dinâmicos: Pebbles, Footprints, Spray e muito mais
* [Content] 2 Novos HDRis: Canopus Ground e Floresta de outono
* [Content] Atualizar conteúdo com curadoria de semente aleatória na prateleira
* [Content] Ícone novo com parâmetro semente aleatório exposto na prateleira

**Corrigido:**

* [Pilha de camadas] A pilha de camadas continua arrastando para sempre
* [Mac] “Mostrar no Finder” pode levar ao congelamento
* [Script] As configurações salvas por meio da interface do usuário personalizada são perdidas se o arquivo de sombreador for movido
* [Scripting] O número de versão da API está incorreto e não está atualizado
* [Efeito] O conteúdo do histograma não é exibido corretamente
* [Efeito] O efeito do histograma não é atualizado em alguns casos
* [Prateleira] Os pontos não estão corretamente alinhados no material “Pirâmide de tecido plástico”

**Problemas Conhecidos:**

* Clicar duas vezes no nome do conjunto de texturas o selecionará antes de entrar no modo de renomeação
* [Pilha de camadas][IU] Alternar uma máscara com SHIFT pode selecionar várias camadas ao mesmo tempo

## Versão 4

### 4.3.3 (2018.3.3)

*(Lançado em: 07 de março de 2019)*
Resumo: **correção de erros**

**Adicionado:**

* [Content] Integrar novo modelo de projeto: “PBR - Alpha de aspereza metálica”
* A ordem de pesquisa da biblioteca dinâmica Linux foi alterada para priorizar as bibliotecas no diretório de instalação antes do que está instalado no sistema

**Corrigido:**

* A malha às vezes desaparece da viewport 3D (pressione F para redefinir a câmera)
* Atualize o carregador do Substance Painter Sketchfab com os novos tipos de licença do Sketchfab
* [Import][glTF] Manipulação incorreta de modulação de textura de entrada conforme definido nos arquivos glTF
* [Import][glTF] O plano horizontal é exibido incorretamente com a importação de glTF em alguns casos
* [Export][USD] A opacidade não funciona no Arkit
* [Export][USD] A exportação de USDz falha em alguns casos
* [Export][USD] Exportar para USD sem salvar leva a falha
* [Export][USD] Modo de divisão incorreto para texturas, modo de subdivisão para malhas e tipos de saída para sombreadores
* [Export][USD] Exportações esparsas de apenas alguns conjuntos de textura com toda a geometria
* [Instância] Falha ao tentar excluir uma camada de instância quebrada
* [Regressão][Exportar] Alguns mapas não são exportados na profundidade de bits escolhida
* [Linux] Problema com a biblioteca libtbb.so.2

**Problemas Conhecidos:**

* O congelamento da computação em alguns casos em GPUs AMD VEGA
* Problema do tablet Huion com atalhos no sistema operacional Windows

### 4.3.2 (2018.3.2)

*(Lançado: 24 De Janeiro De 2019)*
Resumo: **Hotfix com novos recursos (exportação USDZ e filtragem de textura no visor)**

**Adicionado:**

* [Exportar] Permitir exportação para USDZ
* [Visor] Permite controlar a qualidade da textura nas Configurações de exibição
* [Visor] Configuração de polarização mip adicionada nas Configurações de exibição
* [Visor] Filtragem anisotrópica adicionada nas Configurações de Exibição
* [plugins] Atualize os plugins oficiais para usar o estilo do Substance Painter 2018
* [License] Instalar licença por padrão em uma pasta de usuário

**Corrigido:**

* Falha vinculada à descompactação
* Adicionar TAA em material solo
* Ruído com sombra, TAA e sombreador de teste alfa com pontilhamento
* Remover pontilhamento de specular para todos os sombreadores PBR clássicos
* Falha nas configurações do sombreador em alguns casos
* A ativação de dispersão não está sincronizada entre as renderizações OpenGL e Iray
* As ferramentas Borrar e Clonar não funcionam mais em malhas específicas
* Alguns conjuntos de texturas não podem aparecer na renderização Iray
* Os conjuntos de texturas renomeados não são salvos após o fechamento do projeto
* Artefatos de wireframe ao arrastar e soltar materiais em mapas de ID
* [Script] Criação de caminho de arquivo não forçada ao salvar um projeto
* [Scripting] O retorno de chamada “onProjectAboutToSave()” não funciona mais
* Links do fórum quebrados na janela de erro do relatório

**Problemas Conhecidos:**

* O congelamento da computação em alguns casos em GPUs AMD VEGA
* Problema do tablet Huion com atalhos no sistema operacional Windows

### 4.3.1 (2018.3.1)

*(Lançado em: 06 de dezembro de 2018)*
Resumo: **Hotfix**

**Adicionado:**

* [Simetria][Janela de visualização] A pintura de simetria na exibição 2D está de volta e agora apresenta uma visualização de pincel de clone corrigida

**Corrigido:**

* [Exportar] A exportação de exibição 2D gera uma textura preta em alguns casos
* [Iray] Informações normais se tornam incorretas em Iray após instanciar uma camada de material
* Conjuntos de textura não quadrada podem levar, em alguns casos, a falhas
* [Desfazer] Várias teclas Ctrl+Z podem levar aleatoriamente, em alguns casos, a falhas
* [QML] O AlgScrollView pode criar um aviso no registro em alguns casos (loops de ligação)

**Problemas Conhecidos:**

* O congelamento da computação em alguns casos em GPUs AMD VEGA
* Problema do tablet Huion com atalhos no sistema operacional Windows
* A suavização de borda e as sombras quando ativas em conjunto podem gerar resultados inesperados

### 4.3.0 (2018.3.0)

*(Lançado: 20 de novembro de 2018)*
Resumo: <b>Atualizações de viewport, exportação de visualização 2D adequada, novos auxiliares de interface, uma ferramenta de simetria aprimorada, novo conteúdo e um enorme aumento no desempenho</b>

<b>Adicionado:</b>

* [Suavização de borda][Janela de visualização] Nova filtragem de suavizações temporais para a janela de visualização 3D (através das Configurações de exibição)
* [Exportar] Exporta o conteúdo da viewport 2D como uma textura única
* [Exportar][Pontilhamento] Expor pontilhamento na exportação
* [Pilha de camadas] Cores em camadas e pastas
* [Pilha de camadas] Ativação e desativação rápidas de várias camadas e efeitos
* [Pilha de camadas] Navegação mais fácil para modos de mesclagem com teclas para cima e rolagem do mouse
* [Proj][UI] Manipulador de rotação adicional nos três eixos para triplanar
* [Proj][Atalhos] - e + para alterar o tamanho do manipulador de Projeção UV
* [Shader] Controle os parâmetros de camada com canais no sombreador revestido por PBR
* [Substance] Expor novas entradas de textura com base em malha para filtros e geradores
* [Simetria][Visor][IU] Controla o deslocamento de simetria com manipuladores
* [Simetria][Barra de ferramentas contextual][IU] Novo painel de simetria com opções
* [Simetria] Novo modo de interseção de linha de simetria
* [Simetria] Novo cursor de clone de simetria
* [Simetria][Atalhos] Q para ocultar e -, + para alterar o tamanho e shift para ajustar
* [Log] Aprimorar mensagens de erro quando não for possível exportar texturas
* [Script] Permitir a alteração ou atualização dos recursos em Configurações de exibição
* [Script] Permitir a criação ou a remoção de canais em Conjuntos de Textura
* [Content][Shaders] Adicionar suporte para anisotropia com um sombreador dedicado (pbr-metal-rough-anisotropia-angle)
* [Conteúdo] Atualização da esfera de visualização com anisotropia e ângulo modificado
* [Content] shutline matFx atualizado
* [Content] New Texturing.XYZ varredura de rosto sem emenda
* [Conteúdo] Novos procedimentos anisotrópicos
* [Content] Novo filtro: ambiente de iluminação baked
* [Content] Novo mapa ambiental: estúdio automotivo neutro
* [Content] Novo modelo de projeto: PBR - ângulo de Anisotropia de aspereza metálica (com canais de anisotropia)
* [Content] Novo modelo de projeto: PBR - aspereza metálica revestida
* [SVT][Engine] Texturas virtuais esparsas (SVT)
* [SVT][Preferências][IU] Opção de aceleração de suporte a hardware SVT
* [SVT][Log] Informações adicionais para o recurso Texturização Virtual Esparsa (por exemplo, tamanho do disco)
* [SVT][UI] Janela de mensagem na inicialização se o tamanho no disco for muito baixo para o cache
* Localização do cache global de Substance Painter [SVT][Preferências][UI]
* [SVT] Nova variável de ambiente para especificar o caminho do cache de Substance Painter
* [SVT] Nova variável de ambiente para ativar a aceleração de suporte de hardware SVT
* [SVT] Detectar suporte esparso por hardware
* [SVT][Dispersão de hardware] Aumentar a versão mínima do driver para a GPU Nvidia
* [SVT][Shader][Viewport][UI] Avisa o usuário se artefatos presentes com Texturização virtual esparsa na abertura do projeto

<b>Corrigido:</b>

* [Seletor de cores] Cursor de pintura que aparece ao tentar selecionar uma cor
* A falha ao selecionar ou cancelar a seleção de camadas em uma ordem específica pode causar falha
* Falha ao colar como uma ocorrência uma camada com uma máscara
* [User Channel][Regression] Falha ao renomear canal de usuário
* [User Channel] Visualização do pincel esmaecido
* [Alembic] Somente uma textura definida de vários materiais após a importação
* [Engine] A textura exportada é diferente da viewport para carimbos de pincel
* [Mecanismo] Inverter com um efeito de nível não afeta totalmente uma textura
* O seletor de material está aplicando um traçado de pincel ao separar
* Alternar a resolução para 128x128px leva a um travamento
* Os links de mapas de malha não são atualizados corretamente ao reorganizar ou instanciar camadas
* [Substance] O espaço de cor UserData não funciona no normal de malha cozida solicitado como entrada
* Incompatibilidade de associação MDL ao usar várias instâncias de sombreadores
* [Simetria][Camada de preenchimento] Plano de simetria e seu manipulador ativo na Camada de preenchimento
* [Visor] O ponto dinâmico para tradução nem sempre é atualizado após clicar
* [UI] Ícones corrigidos e remoção de espaços reservados para monitores HDPI

<b>Problemas Conhecidos:</b>

* O congelamento da computação em alguns casos em GPUs AMD VEGA
* Problema do tablet Huion com atalhos no sistema operacional Windows
* A suavização de borda e as sombras quando ativas em conjunto podem gerar resultados inesperados

### 4.2.3 (2018.2.3)

*(Lançado: 25 de setembro de 2018)*

**Corrigido:**

* [2D View] A visualização 2D é quebrada com algumas malhas ao criar um novo projeto
* [Falha] Alternar de Projeção UV para projeção triplanar leva a um travamento
* [RayCollider] Várias falhas devido ao “RayCollider”
* [Ferramenta] A alternância de camadas perde as propriedades modificadas do pincel
* As configurações do pincel são redefinidas ao alternar para a borracha

**Problemas Conhecidos:**

* Congelamento de computação em GPUs AMD VEGA
* Problema do tablet Huion com atalhos no sistema operacional Windows

### 4.2.2 (2018.2.2)

*(Lançado: 11 de setembro de 2018)*
Resumo: **Hotfix com atualização de conteúdo, novas funcionalidades de script e capacidade de desabilitar a atualização automática**

**Adicionado:**

* [Conteúdo][Prateleira] Adicionar uma predefinição de prateleira de pele
* [Content][shelf] Conversão de 19 normais de pele em materiais para dispersão subsuperficial
* [Script] Criar um modelo de projeto a partir de um projeto aberto
* [Script] Obter/Definir configurações de exportação de um projeto aberto
* [Atualizações] Desative o pop-up de atualização automática nas configurações e na variável de ambiente
* [Atualizações] Não exibir até a próxima versão do pop-up de manutenção desatualizada

**Corrigido:**

* [Câmera] Zoom incorreto ao alternar de ortográfico para perspectiva
* [Exibir] Alguns mapas são exibidos em linear em vez de sRGB
* [Visores] O foco da malha não se comporta corretamente
* [2D View] Projeto com câmera quebrada tem desaparecendo UVs Shells
* [SSS][Dica de ferramenta] as dicas de ferramentas de dispersão da subsuperfície aparecem no registro
* Alguns projetos não podem ser abertos em 2018.2 e a mensagem de erro não pode salvar um pacote nulo do substance
* [Máscara] A cor da ferramenta de pintura pode travar em alguns casos ao trabalhar em uma máscara
* [Material] Mapas que não aparecem em situações específicas
* [Proj][Ferramentas] Manipulador ativo com um gerador
* [Substance] Grupos de Substance de parâmetros ausentes
* [Scripting] Nome de software incorreto na documentação
* [UDIMs] Não há informações no log sobre shells UVs em vários blocos UVs

**Problemas Conhecidos:**

* Congelamento de computação em GPUs AMD VEGA
* Problema do tablet Huion com atalhos no sistema operacional Windows

### 4.2.1 (2018.2.1)

*(Lançado em: 3 de agosto de 2018)*

**Corrigido:**

* Parâmetros de sombreador de dispersão de subsuperfície ausentes em projetos de atualização

**Problemas Conhecidos:**

* Congelamento de computação em GPUs AMD VEGA
* Problema do tablet Huion com atalhos no sistema operacional Windows

### 4.2.0 (2018.2.0)

*(Lançado em: 2 de agosto de 2018)*
Resumo: **Versão de verão, suporte a dispersão de subsuperfície, melhorias de projeção e preenchimento, importação e seleção de câmera, suporte a Alembic e glTF, arrastar e soltar no mapa de ID, suporte aprimorado ao formato Substance e novo conteúdo**

**Adicionado:**

* [SSS][Viewport][Iray] Dispersão genérica de subsuperfície
* [SSS] Sincronizar parâmetros de dispersão da subsuperfície e MDL
* [SSS] Adicionado um novo canal em tons de cinza chamado Dispersão
* [SSS][Configurações do sombreador] Parâmetro de tipo de dispersão para dispersão subsuperficial (pele ou translúcida)
* [SSS][Configurações do sombreador] Parâmetro de escala de dispersão para dispersão subsuperficial
* [SSS][Configurações do sombreador] Parâmetro de cor de dispersão para dispersão subsuperficial
* [SSS][Configurações de exibição] Contagem de amostra de dispersão para dispersão subsuperfície
* [Shader][Iray] Integrar MDL de dispersão de subsuperfície para Iray
* [Shader] Atualização do sombreador por meio do atualizador de recursos
* [Shader] Atualizar a API e a documentação do log de alterações
* [Propriedades da ferramenta][Proj] Novos parâmetros para a projeção triplanar
* [Visor][Proj] Controlar as propriedades da Camada de preenchimento na exibição 3D diretamente com manipuladores (projeção triplanar)
* [Shortcuts][Proj] Novos atalhos Q, W, E, R, T para manipuladores de projeção triplanar
* [Viewport][Proj] Controlar as propriedades da Camada de preenchimento na exibição 2D diretamente com manipuladores (Projeção UV)
* [Shortcuts][Proj] Novo atalho Q para manipuladores de Projeção UV
* [Barra de ferramentas contextual][Proj] Controla os manipuladores de projeção triplanar
* [Barra de ferramentas contextual][Proj] Controlar manipuladores de Projeção UV
* [Propriedades da ferramenta] Desativar a divisão em blocos gráficos de textura com a ferramenta Projeção e Estêncil
* [Estêncil] Usar imagens não quadradas com a ferramenta de projeção/estêncil
* [Estêncil] Permitir o controle do modo de divisão em blocos gráficos na janela Propriedades
* [Estêncil] O zoom não está centralizado em um estêncil sem divisão em blocos gráficos
* [Câmeras] Importar câmeras do Maya, Max, Blender, Modo, DAE
* [Câmeras][Visor] Selecionar e controlar câmeras importadas no visor
* [Câmeras][Iray] Selecionar e controlar câmeras importadas no Iray
* [Câmeras][IU][Novo projeto][Configuração do projeto] Importar câmeras é verificado por padrão
* [Câmeras][Atalhos] Adicionar atalhos para alternar entre câmeras
* [Câmeras][Visor] Adicionar quadro no visor
* [Câmeras][Configurações do visor] Controle de opacidade de quadro
* [Câmeras][Configurações da câmera] distância focal máxima em 500 mm
* [Câmeras][Configurações da câmera] Taxa de exposição
* [Câmeras][Configurações da câmera] Adicionar uma opção de bloqueio
* [Câmeras][Configurações da câmera] Adicionar uma opção de restauração
* [Câmeras][Configurações de câmera] Adicionar atributo de distância de foco
* [glTF] Importação de um arquivo glTF
* [glTF] Importar mapa de oclusão do ambiente
* [Alembic] Importar quadro Alembic 1 com geometria estática
* [Prateleira] Arraste e solte materiais diretamente na malha usando mapas de ID com um modificador (CTRL/Command)
* [Pilha de camadas] Criação automática de máscara de ID com arrastar e soltar materiais na malha com mapas de ID
* [Pilha de camadas] Rolagem automática de camadas com arrastar e soltar na pilha de camadas
* [UI][Propriedades da ferramenta] Expor predefinição de Substance
* [UI][Menu Ajuda] Aprimoramento do menu Ajuda
* [UI][Novo projeto][Configuração do projeto] Reorganização da janela
* [UI][Novo projeto][Configuração de projeto] Substituir termo de malha por arquivo
* [UI][Substance] Exibir atributos de Substance na interface
* [Atalhos] F4 alterna entre as exibições 2D e 3D
* [Atalhos] Novos atalhos para alternar estêncil N e máscara rápida U
* [Integração Substance] Leve em consideração as instruções &#39;visible if&#39; nos parâmetros Substance
* [Janela de visualização] As sombras não são forçadas a serem computadas após a movimentação da câmera
* [Content] Atualizar o MeetMat com câmeras importadas
* [Content] Adicionar uma amostra com dispersão subsuperficial ativada - JadeToad
* [Content] Adicionar um novo modelo de projeto PBR com a dispersão subsuperficial ativada
* [Conteúdo] Predefinições de exportação atualizadas para adicionar um novo canal de Dispersão
* [Content][Prateleira] Adicionado suporte à dispersão de subsuperfície para: pbr-metal-rough, pbr-metal-rough-alpha-test, pbr-coated, pbr-spec-gloss
* [Content][Prateleira] Adicionado canal de dispersão para 5 materiais inteligentes (mármores e peles)
* [Content][Shelf] 1 novo material jade
* [Conteúdo][Prateleira] 1 novo material de cera

**Corrigido:**

* [CMD] Resultados diferentes usando a mesma linha de comando com versões diferentes
* [TDR] Se o TdrLevel estiver configurado, você não tem erros no seu registro
* [Baker] O mapa de oclusão do ambiente está invertido
* [Mapa de ID] Falha ao separar fora do intervalo 0-1
* [Iray] Falha ao alternar conjuntos de texturas e voltar para o modo de Pintura
* [Janela de visualização] Sincronizar áreas de soltar entre portas de visualização para arrastar e soltar
* [Engine] Artefato Moiré ao colocar camadas de preenchimento lado a lado ou pintar um pequeno pincel
* [License] Verificação de versão de software incorreta do serviço de licença
* [Licença] Reformular a maneira como lidamos com a autenticação
* [API] Chamar o evento de API de script onNewProjectCreated mesmo ao criar com um modelo
* [Shader] O sombreador compilado não é carregado do cache quando o arquivo de sombreador não é compilado
* [Prateleira] Exportar arquivo HDR da prateleira exibirá um arquivo com valores fixados
* [Exportar] A exportação de EXR mantém os valores de cor do RGB entre 0 e 1
* [Conteúdo] O fractal de ruído Perlin 3D de ruído de procedimento está pixelado

**Problemas Conhecidos:**

* Congelamento de computação em GPUs AMD VEGA
* Problema do tablet Huion com atalhos no sistema operacional Windows

### 4.1.3 (2018.1.3)

*(Lançado: 28 de junho de 2018)*

**Adicionado:**

* [Preferências] Proponha salvar o projeto quando o Painter for reiniciado

**Corrigido:**

* [Plug-in] O Substance Source de pesquisa não funciona
* [Materiais inteligentes] A importação de materiais inteligentes leva a uma falha em alguns casos
* [Materiais inteligentes] Excluir materiais inteligentes leva a uma falha em alguns casos
* [Salvar] Salvar leva a uma falha em alguns casos raros
* [Prateleira] Inverter não funciona no Células 2 e no Células 3
* [Prateleira] Erro de digitação em alguns Alpha
* [Prateleira] Alguns materiais da substância não renderizam corretamente

**Problemas Conhecidos:**

* Congelamento de computação em GPUs AMD VEGA

### 4.1.2 (2018.1.2)

*(Lançado: 12 de junho de 2018)*
Resumo: **Velocidade de cozimento aprimorada, Sistema de salvamento aprimorado, Controles deslizantes atualizados, API de plug-in atualizada, Tradução para chinês, Preenchimento aprimorado agora opcional**

**Adicionado:**

* [Padeiros] Melhoria de desempenho com nova versão de panificação
* Forçar caixa de diálogo de exibição com GPU incompatível
* [Salvar] Expor a nova funcionalidade de projeto compacto (modo de salvamento completo/compacto)
* [Salvar] Informar o usuário em caso de erro ao salvar
* [Clean] Próxima gravação no modo completo/compacto
* [Controles deslizantes] Aprimoramento da precisão das barras e dos controles deslizantes de cor/escala de cinza
* [Controles deslizantes] Adição de controles de seta para cima ou para baixo
* [Controles deslizantes] Mesma zona de detecção para controles deslizantes de barra colorida e de tons de cinza
* [Plug-in] Salvamento automático sempre em modo incremental
* [Plug-in] Opção para alternar plug-ins para o novo estilo de interface
* [Language] Adicionar tradução para chinês
* [Preenchimento] Opção para alternar entre o preenchimento UV e vizinho de espaço 3D por Textura Definida nas Configurações do conjunto de textura
* [Script] Modo de salvamento de exposição: completo/compacto ou incremental
* [Script] Atualizar script/documentação QML
* [Log] Indica o modo de salvamento no log (completo/compacto ou incremental)

**Corrigido:**

* [Ferramenta] O slot do canal se transforma em um slot de material em preenchimentos de canal único
* Falha ao carregar uma malha (FBX) com algumas faces não atribuídas por um material
* Falha na Iray com NVIDIA GRID 5.2 na máquina virtual
* Falha ao desfazer uma exclusão de predefinição de material
* Falha ao carregar alguns projetos
* [Linha de comando] Nova linha de comando para malhas UDIM divididas por udim
* [Barra de ferramentas] Redução da barra de ferramentas
* [Instanciação] Não é possível instanciar bitmaps em vários conjuntos de texturas
* [Janela de visualização] A atualização não é concluída ao pintar na malha com UVs lado a lado
* [Iray] O mapa normal é aplicado duas vezes para dielétricos
* [Prateleira] Erros de digitação em alguns parâmetros de Substance (alfas, procedimentos e matfx)
* [Shelf] Erro de ortografia no bitmap “Somente Pessoal Autorizado”
* [Script] A função alg.shaders.materials() não funciona mais

**Problemas Conhecidos:**

* Congelamento de computação em GPUs AMD VEGA

### 4.1.1 (2018.1.1)

*(Lançado em: 3 de abril de 2018)*

**Corrigido:**

* [Tablet] Problema ao alterar as opções de interação padrão
* [Bakers] Falha com a biblioteca Assimp
* [Bakers] Regressão no desempenho com mapa A.O.
* [Iray] A Distorção de lente não é aplicada ao canal de Alpha
* [Drivers] Atualização dos requisitos mínimos de drivers
* [3Dview] Normais não gerados corretamente em malhas UDIM sem informações normais
* [Intel] Falha com o Substance Painter 2018.1.0
* [Intel][Visor] Problema com preenchimento (artefatos pretos)

**Problemas Conhecidos:**

* Congelamento de computação em GPUs AMD VEGA

### 4.1.0 (2018.1.0)

*(Lançado: 15 de março de 2018)*

**Adicionado:**

* Novo estilo geral (ícones, cor, comportamento)
* Novo layout padrão
* [Tablet] Aprimoramento da experiência do usuário ao pintar
* [Menu principal] Classificar itens nativos em exibições e barras de ferramentas primeiro
* [Menu principal] Mover ações de máscara rápida na seção do visor
* [Menu principal] Mover as ações do botão direito do mouse para a seção do visor
* [Menu principal] Renomear o menu “Exibir” como “Janela”
* [Menu rápido] Novas propriedades de ferramenta clicando com o botão direito do mouse no visor
* [Widget de encaixe] Nova barra de ferramentas de encaixe para redução/recuperação rápida
* [Configurações de exibição] Janela de configurações da câmera e do visualizador mesclada
* [Pilha de camadas] Menu contextual de clique com o botão direito
* [Pilha de camadas] Arraste e solte para mover qualquer efeito dentro da mesma camada
* [Barra de ferramentas] Reorganização da barra de ferramentas e da nova barra de ferramentas contextual
* [Barra de ferramentas Ferramentas] Dividir a ferramenta Clonar em duas ferramentas separadas
* [Propriedades das ferramentas] Valor de tons de cinza do plano de fundo mais claro na visualização
* [Propriedades das ferramentas] Organização em guias (preenchimento e ferramentas)
* [Ferramenta] O resultado da pintura corresponde ao estêncil
* [Visor] Novo cursor para camada de preenchimento
* [Visor] Navegação e pintura mais suaves (maior taxa de quadros)
* [Janela de visualização] Caixa de combinação Material/Canal/Seleção de mapa no visor
* [Visor] Reduzir cintilação ao girar (sombra ativada)
* [Prateleira] Exibir materiais por padrão ao abrir o Painter
* [Prateleira] Melhoria do tempo de carregamento de texturas e materiais de Substance (2 a 6 vezes mais rápido)
* [Prateleira] Reorganizar pastas de materiais para se ajustar à estrutura de Substance Source
* [Prateleira] Arraste e solte materiais diretamente na malha no visor
* [Prateleira] Novos ruídos 3D (Perlin, Perlin Fractal, Simplex e Worley)
* [Prateleira] Novo gerador de máscara de 3D linear gradient usando a posição da malha
* [Shelf] Ruídos básicos atualizados para suportar o expansão não quadrada
* [Prateleira] Adicionado novo modelo e predefinição de exportação para o Lens Studio (aplicativo Snap)
* [Prateleira] Materiais inteligentes e Máscaras inteligentes atualizados para usar a versão mais recente do Editor de máscaras (microdetalhes)
* [Shelf] Novo projeto de amostra “TilingMaterial” para criar materiais de revestimento perfeitos
* [Prateleira] Novas predefinições de pincel (Caligrafia, Molhado, Hachura e assim por diante)
* [Controles deslizantes] Novos controles deslizantes e estilo e comportamento de barras de tons de cinza/cores
* [Padeiros] Permitir o uso de uma caixa delimitadora de cena inteira para calcular o mapa de posição
* [Shader] Remove o parâmetro de força de height dos parâmetros de sombreador padrão
* [Engine] Mecanismo de Substance atualizado
* [Engine] Nenhuma ou menos descontinuidades nos blocos UV
* [Plug-ins] Importar materiais baixados do Substance Source mais rapidamente
* [Plug-ins] Atualizar todos os plug-ins para corresponder ao novo estilo geral
* [Preferências] Visualizar alterações de cor de fundo automaticamente
* [Simples] Risco reduzido de corrupção do projeto
* [Aberto] Aperfeiçoamento do tempo do projeto de abertura
* [Novo projeto] Novo projeto - melhoria no tempo de atualização da malha
* [Salvar] Salvando a melhoria no tempo do projeto
* [Log] Tipo de licença relatado no log
* [TextureSet] Renomeie o botão “Bake Textures” como “Bake Mesh Maps”
* Renomear “Mapas adicionais” como “Mapas de malha”

**Corrigido:**

* [Visor] Maus desempenhos com malhas que contêm muitos subobjetos
* [Propriedades de ferramentas] Canal desativado ao arrastar e soltar uma imagem no slot de material
* [Propriedades das ferramentas] A visualização do pincel é interrompida com as ferramentas de borrar e clonar
* [Conjunto de texturas] A ordem dos canais está incorreta ao usar modelos
* [Prateleira] Ícone ausente para o gerador de conversão em tons de cinza
* [Prateleira] O Número de Círculo do Sinal alfa está quebrado (fonte ausente)
* Detecção incorreta de GPUs integradas na inicialização
* [Falha] Arrastar e soltar um recurso importado nomeado com um caractere #
* [Engine] Problema de detecção de Vram na GPU integrada
* [Engine] Corrigidas várias falhas no Substance Engine Linker
* [Engine] Artefatos quadrados ao alterar a resolução
* [Post Effects] O redimensionamento da interface fica lento quando os pós-efeitos estão ativados
* [Padeiros] A unidade de cena não é respeitada corretamente para valores de distância de raio
* [Bakers] A distância do Ocluder da malha é fixada em 1, independentemente do valor de entrada
* [Padeiros] Corresponder pelo nome ignora algumas malhas com nomes específicos
* [Padeiros] A cor da configuração de malha Poligrupo e ID de submalha sempre retorna uma imagem preta
* [Bakers] A cozedura de ID falha com malhas binárias FBX do Blender
* [Shader] Ruído na visualização 2D com dota-2 e brilho não pbr-spec
* [Linux] Somente um thread de CPU é usado ao assar
* [MacOS] Falha com o cursor do pincel se movendo sobre a janela de visualização

**Problemas Conhecidos:**

* Congelamento de computação em GPUs AMD VEGA
* Pós-processo de distorção não levado em conta ao exportar no IRay (alfa)

## Versão 3

### 3.4.2 (2017.4.2)

*(Lançado: 24 de janeiro de 2018)*

**Adicionado:**

* [Exportar] Obter o status de uma exportação com progresso de etapa
* [Exportar] Permitir o cancelamento de uma exportação
* [Exportar] Exportar texturas para o Sketchfab sem perder a qualidade normal do mapa
* [Exportar] Exportar no formato binário glTF (glb)
* [Exportar] Permitir o redimensionamento de colunas na guia Configuração da janela de exportação
* [Shader] Adicionar um registro de alterações para a API de sombreamento
* [Script] Adicionar funções de retorno de chamada Antes e Depois ao exportar texturas
* [Iray] Atualização para o SDK 2017.1 (suporte a Volta GPUs)

**Corrigido:**

* Falha ao sair do aplicativo antes que a janela principal seja exibida
* [MAC] Falha ao carregar mapas em tons de cinza com IRAY
* [MAC] A detecção de VRAM não está correta com o novo sistema operacional High Sierra
* [Plug-in] Baixar ativos do Substance Source não funciona mais
* [Script] Detecção de versão mínima incorreta do plug-in
* [Exportar] Falha ao salvar a predefinição de exportação após exportar as texturas
* [Instanciação] Problema em geradores instanciados em um TextureSet sem Mapas Adicionais
* [Visor] O pontilhamento não funciona com resolução acima de 4k
* [Visor] A exibição de material 2D é coberta por ruído
* [Prateleira] Melhorar o tempo de carregamento das predefinições de prateleira
* [Engine] Mesclagem incorreta ao pintar com seleção de cores

### 3.4.1 (2017.4.1)

*(Lançado: 15 de dezembro de 2017)*

**Adicionado:**

* [Script] Exportar malha por meio da API de script
* [Importação] Desativa a importação de formato de arquivo de malha não suportado (permitir somente obj, fbx, dae, ply)
* [Log] Indique com mais precisão o problema de TDR no arquivo de registro

**Corrigido:**

* Falha se o aplicativo for fechado antes da conclusão do rastreamento de recursos
* Falha ao abrir projetos com a ferramenta Borrar/Clonar
* Falha ao usar a ação de refazer após desfazer uma alteração de Sombreador nas Configurações do visualizador
* [Engine] A texturização difere entre o Painter 2017.2 e 2017.4
* [Visor] A separação em um mapa de ID de uma instância obtém a amostra da cor errada
* [Export] Falha ao exportar uma textura normal ou de oclusão inválida
* [Exportar] Os arquivos de PSD têm seus grupos bloqueados quando abertos no Photoshop CS6
* [Plug-in] O plug-in do Photoshop ignora a seleção de canal e sempre exporta tudo
* [Camadas] As âncoras são rompidas quando copiadas/coladas em conjuntos de texturas
* [Camadas] Algumas referências de âncora não podem ser restauradas se estiverem quebradas
* [Shader] O parâmetro de aspereza secundária revestido com pbr está danificado
* [Steam] O pop-up do verificador de versão não deve estar visível na inicialização

**Problemas Conhecidos:**

* [AMD] Falha/Congela ao tentar pintar em uma malha. Pode ser corrigido com uma atualização de driver de GPU.

### 3.4.0 (2017.4.0)

*(Lançado: 23 de novembro de 2017)*

**Adicionado:**

* [Instanciação] Permite criar instâncias de parâmetros em camadas
* [Instanciação] Permite saltar entre uma camada de origem e uma instância
* [Instanciação] Adicionar uma ação “instanciar em conjuntos de texturas”
* [Instanciação] Indique na pilha de camadas instâncias reentrantes (ciclos)
* [Instância] Excluir instâncias quando uma origem é removida
* [Instanciação] Não permitir referências de Âncora de fora de uma pasta de instância
* [UI] Mova a pilha Desfazer para sua própria janela chamada “History”
* [Plug-in] Plug-in de integração de link dinâmico DCC
* [Mecanismo] Aprimorar o desempenho da pintura com pintura Esparsa
* [Exportar] Adicionar opções de rascunho e reexportação ao exportador do Sketchfab
* [Prateleira] Adicionar controle “virar” para substâncias de fonte
* [Prateleira] Adicione 20 novos materiais de procedimento
* [Prateleira] Adicione 40 novos mapas grunges (bitmap baseado e procedimento)
* [Visor] Ativar colisões de visualização de pincel em outros conjuntos de texturas visíveis
* Atualizar os requisitos mínimos dos drivers de GPU AMD

**Corrigido:**

* Falha ao computar Substance em resoluções muito grandes
* Falha ao pintar fortemente com partículas
* [Visor] Reflexo de specular incorreto na exibição 2D com malhas específicas
* [UI] Algumas ações indesejadas são exibidas na janela Histórico

**Problemas Conhecidos:**

* [Camadas] Algumas referências de âncora não podem ser restauradas se estiverem quebradas
* Falha ao usar a ação de refazer após desfazer uma alteração de Sombreador nas Configurações do visualizador

### 3.3.3 (2017.3.3)

*(Lançado em: 01 de dezembro de 2017)*

**Corrigido:**

* [Steam] O pop-up do verificador de versão não deve estar visível na inicialização
* [Exportar] Os arquivos de PSD têm seus grupos bloqueados quando abertos no Photoshop CS6

### 3.3.2 (2017.3.2)

*(Lançado: 20 De novembro De 2017)*

**Adicionado:**

* [IU] Aprimorar a caixa de diálogo da nova versão e adicionar changelog
* [UI] Indica se a manutenção expirou na caixa de diálogo de nova versão
* [License] Atualizar o sistema de licenças para lidar com as Datas de manutenção
* [Exportar] Renomear material padrão da Adobe para Adobe Dimension

**Corrigido:**

* [Mac] A pintura leva a quadrados pretos e corrupções de textura
* [Engine] Às vezes, o cache pode desaparecer no visor
* [Engine] Artefatos de bloco aparecem quando o acionador de compactação de memória
* [Preparação] Mensagens de erro estranhas ao assar malhas específicas
* [Export] PSD são gravados incorretamente e não são reconhecidos corretamente pelo Photoshop
* [Camadas] Não deveria ser possível copiar/colar camadas em vários projetos
* [Substance] O espaço de cores UserData para a entrada Normal é invertido em alguns casos
* [Prateleira] Micro-normal em geradores produz curvatura invertida
* [Prateleira] O filtro HSL também afeta o canal alfa
* [Linux] A instalação em Centos falha devido a dependências ausentes
* O instalador não remove todos os recursos da instalação anterior em certos casos

### 3.3.1 (2017.3.1)

*(Lançado: 26 de outubro de 2017)*

**Adicionado:**

* [Exportar] Permite exportar a malha de um projeto
* [Prateleira] Remover “Sub-prateleira” dos títulos das guias
* Salvar configurações de pós-processamento em modelos
* Tornar a mensagem TDR mais compreensível
* Melhorar a janela Configurações para relatar erros

**Corrigido:**

* Falha ao excluir várias subprateleiras
* Falha ao alternar de um nível para algo diferente durante um cálculo do mecanismo
* [Mac] Falha na GPU Intel durante cálculos de mecanismo
* [Mac][Viewport] Desempenho insatisfatório quando o pontilhamento está habilitado
* [Mac] O MacOS 10.13 é reconhecido como “Versão desconhecida” no arquivo de log
* [Baker] Cozinhar com uma gaiola não funciona mais
* [Camadas] O atalho Ctrl + C (ação de cópia) não funciona mais
* [Camadas] Colar camadas não atualiza a interface com as referências da âncora
* [Âncora] Duplicar ou copiar/colar camada com referências quebra os links
* [Exportar] A exportação em 8K pode travar ou bloquear o aplicativo em alguns casos
* [Exportar] Vários problemas no formato de arquivo glTF gerado
* [Importar] A reimportação de uma malha com o mesmo nome de arquivo não funciona mais
* [Plug-in] A janela de salvamento automático sempre aparece acima de tudo
* [UI] Loop infinito ao pressionar “Escape” na caixa de diálogo TDR
* [UI] Redefinir interface exibe uma segunda barra de título na janela da prateleira

### 3.3.0 (2017.3.0)

*(Lançado: 28 de setembro de 2017)*

**Adicionado:**

* [Exportar] Permitir a exportação de malha e texturas para o Projeto Adobe Felix
* [Exportar] Permite exportar para o formato de arquivo glTF
* [Engine] Otimizar o tamanho das texturas em VRAM usando a compactação de bloco
* [Visor] Ser capaz de arrastar e soltar uma malha ou projeto no visor
* [UI] Melhorar a mensagem de aviso sobre o TDR
* [UI] O log deve ser exibido somente mediante solicitação
* [UI] Permitir limpar o conteúdo da janela de log
* [UI] Exibir avisos e erros na barra de status
* [IU] Exibir guias na parte superior como em navegadores da Web
* [UI] Melhorar contexto e mensagens “não pintáveis”
* [UI] Adicionar uma ação “salvar como cópia” no menu Arquivo
* [Camada] Definir a configuração padrão de divisão em blocos gráficos como 1 por padrão
* [Prateleira] Filtro de gradiente aprimorado para suporte a 10 cores dinâmicas
* [Prateleira] Adicionar um espaço na consulta padrão da prateleira
* [Prateleira] Adicionar uma ação “Abrir no explorador” para recursos locais na prateleira
* [Prateleira] Adicionar modelo e sombreador para Adobe Material Standard (Projeto Felix)
* [Prateleira] Aumentar a divisão em blocos gráficos máxima para 128 em sombreadores de camada de material
* [Prateleira] Adicionado curvatura sobel para microdetalhes de geradores de máscaras
* [Plug-in] Adicionar plug-in de salvamento automático com intervalo de tempo personalizável
* [Script] Adicionar uma função “salvar como cópia”

**Corrigido:**

* [IU] O layout é quebrado na primeira inicialização
* [Export] O PSD gerado na exportação tem erros de formato
* [Exportar] EXR sempre exporta mapa de heights de 8 bits
* [Export] Falha ao exportar mapas adicionais corrompidos
* [Importar] As bordas sólidas não são preservadas em malhas de poli baixo em alguns casos
* [Importar] Mensagens de erro aprimoradas ao importar malhas com problemas
* [Padeiros] Falha no cozimento do mapa de ID com a opção Corresponder pelo nome ativada
* [Visor] O espaço tangente não é sincronizado com padeiros
* [Efeito] Voltar uma camada não restaura a referência de uma âncora
* [Efeito] Problema de atualização ao criar um link entre duas máscaras com âncoras
* [Efeito] As âncoras de máscaras acima da máscara não devem ser listadas
* [Efeito] Extrair configuração de Alpha de Âncoras não funciona
* [Mecanismo] A máscara se inverte após o primeiro traçado do pincel
* [Engine] Falha ao alternar o Conjunto de texturas em um projeto específico
* [Prateleira] Falha ao excluir uma predefinição que está em um projeto
* [Prateleira] Erro de ortografia no filtro Triplanar avançado
* [Prateleira] MG Mask Builder AO Noise Scale não funciona corretamente
* [Prateleira] MG Mask Builder tem parâmetros de curvatura invertidos
* [Prateleira] Os alfa importados geram uma visualização de esfera de material em vez de uma simples

### 3.2.0 (2017.2.0)

*(Lançado: 27 de julho de 2017)*

**Adicionado:**

* Pontos de ancoragem - Sistema de referência de camada e máscara
* [Camadas] Capacidade de renomear efeitos de preenchimento e pintura
* [Plugin] Plug-in Substance Source atualizado
* [Scripting] Permitir consultar Resolução de Conjunto de Textura
* [Script] Permite obter o status do mecanismo de pintura
* [Desempenho] Otimizações aprimoradas de carregamento e carimbo de pincel no projeto

**Corrigido:**

* [Ferramenta] Problemas de desempenho ao ajustar parâmetros de material
* [Engine] Desaparecimento de pinceladas ao alterar a resolução (4K>2K)
* [Exibição 3D] O espaço tangente não é sincronizado com padeiros
* [Prateleira] O caminho de prateleira nos documentos do usuário não é criado automaticamente
* [Prateleira] Fazer predefinições compatíveis com versões anteriores após uma atualização
* [Shader] O sombreador não PBR não funciona mais
* [Padeiros] Falha no cozimento do mapa de ID com a opção Corresponder pelo nome ativada
* [Amostra] Os nomes dos conjuntos de texturas do projeto de amostra do Mat da reunião estão incorretos
* Salvar um projeto antes de criar um modelo retorna erros de permissão de gravação

### 3.1.0 (2017.1.0)

*(Lançado: 20 de junho de 2017)*

**Adicionado:**

* [Plug-in] Novo plug-in Substance Source (permite baixar ativos na prateleira)
* [Prateleira] 4 Novas Fontes (Japonês + Chinês Simplificado, Máquina De Escrever, Segmento)
* [Prateleira] 230 novos Alpha (mistura de padrões, pincéis e digitalizações de impressão digital)
* [Prateleira] 50 Novos Procedurals (Padrões de tecido de roupas medievais e contemporâneas)
* [Prateleira] 2 Novos mapas ambientais (Mondarrain e Villa Nova Street)
* [Prateleira] 9 Novos filtros (Edge Wear de detalhes MatFx, Suporte, HBAO, etc.)
* [Prateleira] Mapa de ambiente de panorama padrão aprimorado
* [Prateleira] Novas predefinições de exportação para Arnold 5
* [Scripting] Permitir a importação de recursos para a Prateleira

**Problemas Conhecidos:**

* [Exportar] A edição de uma predefinição de exportação é muito lenta

## Versão 2

### 2.6.2

*(Lançado: 20 de outubro de 2017)*

<b>Adicionado:</b>

* [Conjunto de texturas] Permite excluir conjuntos de texturas desativados
* [Prateleira] Permite que vários usuários gravem dentro da mesma pasta de prateleira
* [Script] Poder recarregar a pasta de plug-ins
* [Script] Adicione uma versão mínima necessária da API nos metadados do plug-in para garantir a compatibilidade
* [IRay] Melhorias na caixa de diálogo Exportar imagem

<b>Corrigido:</b>

* [Engine] Problema de desaparecimento de traços, ao alterar a resolução (4K>2K)
* [Padeiros] Falha no cozimento do mapa de ID com a opção Corresponder pelo nome ativada
* [Padeiros] As mensagens de erro não são suficientemente explícitas
* [Exibição 3D] O espaço tangente não é sincronizado com padeiros
* [Ferramenta] Artefatos pretos ao usar a ferramenta de borrar
* [Shader] O sombreador não PBR não funciona mais
* [Shader] “pbr-coated” está quebrado
* [Shader] A aspereza do revestimento do sombreador “revestido com pbr” não tem mais impacto
* [Shader] O sombreador de brilho de especificação não corresponde a Iray e SD
* [Prateleira] Falha ao carregar dois arquivos com o mesmo nome, mas com extensões diferentes
* [Prateleira] Não é mais possível editar a predefinição nas prateleiras
* [Prateleira] Não é possível definir uma visualização personalizada para ativos importados na prateleira
* Os recursos carregados do cache perdem seus usos
* Salvar um projeto antes de criar um modelo retorna erros de permissão de gravação
* Salvar projeto incorreto se o nome do arquivo contiver dois pontos
* Importação de arquivos com vários pontos (.) no nome do arquivo causa problemas

### 2.6.1

*(Lançado: 12 de maio de 2017)*

**Adicionado:**

* [TextureSet] Não permitir a reatribuição de materiais de malha a nada

**Corrigido:**

* Falha ao alternar o TextureSet após substituir o mapa baked
* Falha ao fazer “Desfazer e Refazer” após alterar o modo de mesclagem da camada
* Falha ou congelamento ao usar o efeito “seleção de cores” com um mapa de ID grande
* [Exportar] Os conjuntos de texturas renomeados não são classificados em ordem alfabética na janela de exportação
* [TextureSet] Redefinir para o nome padrão não verifica a unicidade
* [TextureSet] O conjunto de texturas renomeado é desativado após a reabertura do projeto
* [Prateleira] Conteúdo de modelos padrão ausente
* [Prateleira] As texturas não quadradas são exibidas como quadradas
* [Shader] Depois que um conjunto de textura é desativado, o sombreador associado é destruído
* [Scripting] alg.baking.setTextureSetBakingParameters() não funciona mais
* [Script] Erro de digitação no tutorial do websocket
* [Scripting] Vários problemas em AlgWidgets
* [Log] Detecção incorreta de memória virtual disponível em alguns casos

### 2.6.0

*(Lançado: 27 de abril de 2017)*

**Adicionado:**

* Adicionar novo projeto de amostra “Meet Mat”
* [Plug-in] Novo plug-in “Atualizador de recursos”
* [TextureSet] Permite renomear e adicionar uma descrição a conjuntos de textura
* [TextureSet] Permitir a reatribuição de materiais
* [TextureSet] Adiciona um botão de configuração na janela de lista do conjunto de textura
* [TextureSet] Mostra os conjuntos de texturas “desativados” na parte inferior da lista
* [Substance] Use mapas adicionais na resolução atual do conjunto de texturas para melhorar o desempenho
* [Script] Permite atualizar um recurso usado em um projeto (material, gerador etc.)
* [Script] Adicionar uma maneira de adicionar/remover uma prateleira
* [Scripts] Permitir a consulta de informações do recurso em projetos
* [Scripting] Permite recuperar uma lista de prateleiras disponíveis
* [Script] Tutorial de aprimoramento de miniatura do AlgWidget
* [Export] Desativar/ativar profundidade de bits com base no suporte ao formato de arquivo
* [Log] Adicionar nome de plug-in para imprimir no console
* [Log] Remover erro sobre conjuntos de texturas ocultos
* Atualizar “Tela de boas-vindas” com novos ícones e texto para amostras

**Corrigido:**

* Falha ao atualizar uma malha em projetos específicos
* [Janela de visualização] A cor interna do plano de simetria não está mais visível
* [Janela de visualização] Alguns efeitos de pós-processo são ativados ao usar a visualização individual
* [Shaders] A mesclagem “over\_premult” não funciona corretamente
* [Shaders] Aviso sobre o teste alfa com o sombreador padrão
* [Prateleira] Análise incorreta de marcas de Substance
* [Shelf] O Envolvimento de Ferrugem do MatFX não funciona corretamente
* [Prateleira] O filtro HSL está habilitado em canais incorretos por padrão
* [Prateleira] A nitidez está ativada no canal Height/Normal por padrão
* [Exportar] As predefinições de exportação do Vray não usam um mapa normal do OpenGL
* [Ferramenta] Problemas de imprecisão com a ferramenta clonar/borrar criam artefatos

### 2.5.3

*(Lançado: 15 de março de 2017)*

**Corrigido:**

* [Baker] Falha ao assar com malhas específicas

**Problemas Conhecidos:**

* [Mac] As partículas podem criar corrupção de textura em alguns casos

### 2.5.2

*(Lançado: 14 De março De 2017)*

**Corrigido:**

* [Ferramenta] Os tablets Wacom não funcionam no Linux
* [Ferramenta] Artefatos pretos ao usar a ferramenta de borrar
* [Padarias] A cozedura falha se a opção Coincidir pelo nome for usada com uma caixa
* [Pães] Oclusão ambiente quebrada ao assar apenas com mapa normal
* [Prateleira] Os filtros genéricos não tratam o alfa corretamente (Contraste/Luminosidade, Highpass etc.)
* [Viewport] Problema de desempenho ao carregar um projeto com sombras ativadas
* [Janela de visualização] Problema de pontilhamento na visualização 3D no MacOS
* [Janela de visualização] As visualizações de partículas são exibidas incorretamente quando o perfil de cores está ativado
* [Iray] Falha ao alternar o projeto de volta para OpenGL se o Iray não inicializar
* [IRay] A reluzência é ignorada ao renderizar o sombreador/mdl SpecGloss
* [Shader] O sombreador de espec/brilho não corresponde a Iray e SD
* [Shader] Conversão de sRGB diferente da conversão linear para sRGB LUT
* [Shader] Renderização incorreta ao carregar projeto com sombreadores desatualizados
* [Shader] O sombreador “pbr-coated” não funciona mais
* [Exportar] Alguns canais ainda são exportados, mesmo que não estejam presentes no conjunto de texturas
* [Camadas] O modo de mesclagem “detalhe inverso do mapa normal” não funciona em canais em tons de cinza
* [UI] Problema na “Janela de seleção de cores” com monitor HDPI e zoom de exibição em 150%

**Problemas Conhecidos:**

* [Mac] As partículas podem criar corrupção de textura em alguns casos

### 2.5.1

*(Lançado: 27 de fevereiro de 2017)*

**Corrigido:**

* [Mac] A entrada da mesa digitalizadora Wacom está interrompida na exibição 3D e 2D
* [Padeiros] A correspondência por nome não funciona mais
* [Bakers] A configuração “Average Normals” não funciona mais
* [Iray] Renderização incorreta com mapa normal cozido ausente
* [Iray] Os perfis de cores se comportam de maneira diferente em comparação ao renderizador OpenGL
* [Iray] Exportar renderização como bitmap não inclui correção de perfil de cores
* [Substance] Os filtros de material não funcionam mais
* [Ferramenta] A opacidade do traçado não é armazenada em predefinições de pincel
* [Ferramenta] O alinhamento UV do pincel do clone não funciona mais
* [Exportar] O canal de Deslocamento deve ser centralizado em 0,5 ao exportar em número inteiro
* [Modelo] O caminho absoluto é armazenado em Modelos
* [TextureSet] A textura do canal persiste após a remoção do canal

**Problemas Conhecidos:**

* [Linux] As entradas dos tablets Wacom não funcionam na exibição 3D e 2D
* [Mac] As partículas podem criar corrupção de textura em alguns casos
* [Exportar] Em casos muito raros, retângulos pretos podem aparecer em GPUs da AMD

### 2.5.0

*(Lançado em: 21 de fevereiro de 2017)*

**Adicionado:**

* Adicionar compatibilidade com as GPUs AMD Radeon Pro e AMD FirePro
* [Ferramenta] Adicionar suporte para opacidade de traçado
* [Ferramenta] Adiciona um modificador que permite continuar a última pincelada
* [Iray] Atualização para oferecer suporte a GPUs Pascal
* [Visor] Adicionar suporte para perfis de cores (LUT)
* [Substance] Integrar nova estrutura (mecanismo SD6)
* [UI] Aumentar a lista de tamanhos de “arquivo recente” no menu Arquivo
* [Importar] Use a categoria de substâncias para preencher o prefixo na caixa de diálogo Importar
* [Padeiros] Permitir assar texturas 8K
* [Padarias] Permitam assar resoluções não quadradas
* [Padarias] Melhorar o consumo de memória ao assar malhas pesadas de alta polarização
* [Prateleira] Bloqueie prateleiras (e projetos) para proibir a edição simultânea e evitar corrupções
* [Prateleira] Ler categoria e palavras-chave de substâncias para usá-las para filtragem
* [Prateleira] Permitir a exclusão de recursos do resultado de uma consulta de pesquisa
* [Prateleira] Cálculo de tempo de miniaturas aprimorado
* [Prateleira] Permite incorporar predefinições em projetos
* [Prateleira] Permite recolher/expandir rapidamente a exibição de árvore com SHIFT
* [Prateleira] Permite salvar miniaturas quando os ativos são somente leitura (cache local)
* [Prateleira] Novo conteúdo : novos filtros (transformação, espelho, triplano, etc.)
* [Prateleira] Novo conteúdo : novos perfis de LUTs (clássicos e artísticos, como Film Noir, Vintage etc.)
* [Prateleira] Novo conteúdo : 10 novas fontes Substance para gerar rapidamente textos personalizados
* [Prateleira] Novos modelos: Unity 5 e Unreal Engine 4
* [Shelf] Filtro HSL aprimorado para ser mais amigável com artistas
* [Shader] Adicionar suporte para canal de specular level em sombreadores PBR
* [Shader] Adicionar suporte para pontilhamento no sombreador de teste Alpha
* [Shader] Adicionar suporte para mapeamento de oclusão de paralaxe em sombreadores PBR
* [Shader] Permite definir interface personalizada para parâmetros de sombreador
* [MatLayering] Criar novo canal Máscara para fluxo de trabalho de camada de material
* [Script] Permitir a gravação de metadados em um projeto SP
* [Script] Permitir exportação com uma predefinição de exportação específica
* [Script] Permite recuperar parâmetros de sombreador como um JSON
* [Script] Adicionar suporte para conexões WebSocket
* [Script] Adicionar a possibilidade de carregar instâncias de sombreador
* [Script] Adicione a possibilidade de criar um novo projeto
* [Script] Permite recuperar a url da malha importada em um projeto
* [Script] Permitir cozimento não quadrado
* [Script] Relatar erros ao definir dados por meio da API de script
* [Substance] Adicionar tag de dados do usuário para especificar o formato de mapa normal

**Corrigido:**

* Falha ao selecionar cor com substâncias
* Falha ao carregar uma imagem não RGBA32f como mapa de ambiente
* Falha relacionada à pintura em GPUs AMD
* [Mesh] A importação de OBJ não reconhece materiais sem arquivo mtl
* [Mesh] A geração do nome do conjunto de textura UDIM pode estar incorreta em algumas malhas
* [UI] Botão Desfazer/Refazer na Configuração do visualizador roubar foco e parar a rolagem do mouse
* [UI] Alguns rótulos são cortados incorretamente em Hi-DPI
* [Camada] O modo de substituição do efeito de pintura tem um comportamento incorreto na máscara
* [Camada] O modo de mesclagem Subtrair tem um comportamento incorreto com alfa
* [Ferramenta] O tamanho do pincel se torna enorme na visualização 2D ao pintar nas bordas UV
* [Ferramenta] A linha reta encaixada apresenta um comportamento irregular com Hi-DPI
* [Tool] A resolução do estêncil às vezes está incorreta
* [Bakers] Os valores de “Distância Máxima do Ocultador” são bloqueados se “em relação à caixa delimitadora” for “Desativado”
* [Shader] As definições de canal Pilha e Parâmetro automático não correspondem
* [Visualização 3D] Exibição inconsistente do canal normal dependendo da configuração do projeto
* [Janela de visualização] Alguns mapas normais têm valores fixados que aparecem como artefatos
* [Janela de visualização] O pós-efeito é sempre desativado por padrão
* [Export] A configuração de mixagem normal está incorreta se o canal normal estiver ausente
* [Exportar] Geração de textura incorreta em alguns casos em GPUs AMD
* [Exportar] Os parâmetros de sombreador não são exportados corretamente se localizados dentro de um grupo
* [Exportar] Editar uma predefinição de exportação em uma prateleira personalizada gera um erro de log
* [Prateleira] A filtragem do modo de exibição de árvore não corresponde exatamente ao nome da pasta
* [Prateleira] Renomear uma predefinição de prateleira é difícil de ler
* [Prateleira] O recurso de sombreador importado na Prateleira não é preservado após a reinicialização
* [Prateleira] Conteúdo : Predefinição de ferramenta de solda ausente
* [Prateleira] Conteúdo : Tile Generator não funciona corretamente
* [Prateleira] Conteúdo: Máscara incorreta corrigida no material inteligente sujo de pneu de borracha
* [Shelf] Conteúdo: corrigido o nome incorreto do grupo no material da bolsa de couro
* [Iray] Metade das malhas está ausente em Iray
* [Linux] Falha ao arrastar um recurso acima da Visualização 3D
* [Mac] As preferências são redefinidas em cada lançamento no Sierra

**Problemas Conhecidos:**

* [Exportar] Em casos muito raros, retângulos pretos podem aparecer em GPUs da AMD
* [Iray] Os perfis de cores podem se comportar de maneiras ímpares às vezes

### 2.4.1

*(Lançado: 28 de outubro de 2016)*

**Corrigido:**

* Falha ao criar um projeto com um modelo
* Falha ao fechar a caixa de diálogo de exportação durante uma exportação
* [Mac] Erros ao salvar o projeto (falha ao salvar a predefinição de exportação)
* [Prateleira] Criar uma nova predefinição a exibirá duas vezes
* [Prateleira] As predefinições não podem ser carregadas no modo somente leitura sem direitos administrativos

### 2.4.0

*(Lançado: 27 de outubro de 2016)*

**Adicionado:**

* [Prateleira] Nova interface para procurar recursos (exibição de árvore, filtros e assim por diante)
* [Prateleira] Permite salvar uma pesquisa como predefinição
* [Prateleira] Permite criar uma nova janela a partir de uma predefinição
* [Prateleira] Nova interface para importar recursos
* [Prateleira] Não copiar a prateleira alegorítmica padrão na pasta Documentos
* [Prateleira] Novas predefinições de partículas: Circuito elétrico, Linhas elétricas, Rococó, Veias pequenas
* [Prateleira] Predefinições de partículas mais antigas aprimoradas para serem mais fáceis de usar (como “Chuva”)
* [Prateleira] Adicionar novas informações no menu contextual de recursos
* [Visor] Melhorar o desempenho ao carregar mapas de ambiente
* [Visor] Adicionar suporte a mapas de ambiente que não são potência de dois

**Corrigido:**

* Falha ao remover uma máscara
* Falha ao pintar após salvar uma predefinição
* Falha com desfoque de ambiente em algumas GPUs
* Falha ao atribuir um recurso errado com a miniprateleira
* [Prateleira] Limpar e salvar remove as marcas e metadados dos recursos no projeto
* [Prateleira] importar uma predefinição exibirá seus recursos na prateleira
* [Exportar] O mapa normal gerado a partir do canal de height tem uma intensidade baixa
* [Exportar] O normal da malha nem sempre está presente no mapa normal final
* [Exportar] Às vezes, a dilatação com transparência pode resultar sem transparência
* [Scripting] “alg.plugin\_root\_diretory” pode retornar um caminho de rede truncado
* [TextureSet] O botão Bloquear é ativado ao reabrir projetos não quadrados

### 2.3.1

*(Lançado em: 07 de outubro de 2016)*

**Adicionado:**

* [Plug-in][Photoshop] Permite especificar qual material/pilha/canais exportar
* [Scripting] Os nomes de função têm algumas inconsistências

**Corrigido:**

* [Exportar] o Alpha pode ser descartado nas predefinições de exportação personalizadas
* [Exportar] o Alpha obtém conversão gama incorreta em canais sRGB
* [Exportar] Documentos não quadrados são exportados como quadrados
* [Exportar] Não é possível exportar mapas adicionais se algum estiver ausente
* [Iray] Alguns parâmetros (como Intensidade de emissivo) não têm efeito
* [NVIDIA] Falha na inicialização com a NVIDIA Quadro K2200/GTX 750/760
* [AMD] Conjunto incorreto de cores para miniaturas e visualizações
* [AMD] Congela e falha de driver em Novo arquivo e Abrir arquivo
* [Log] “software-version” está ausente no arquivo de log

### 2.3.0

*(Lançado: 15 de setembro de 2016)*

**Adicionado:**

* [Plug-in] Novo plug-in “Exportar para o Photoshop” (exportar pilha de camadas completa)
* [Exportar] Permite especificar a largura do preenchimento (em pixels ou infinito)
* [Exportar] Permite definir o tipo de fundo fora dos UVs
* [Prateleira] Novo sombreador de camada de material para misturar 10 materiais
* [Prateleira] Novo sombreador de argila para ver detalhes com o canal height/normal
* [Prateleira] Novo filtro de iluminação cozido com entrada de ambiente
* [Prateleira] Alguns geradores de máscara atualizados para adicionar transformações não quadradas
* [Janela de visualização] Adiciona o mapa normal composto (normal+height+bake) ao modo solo
* [Script] Permitir a exportação de mapas adicionais
* [Scripts] Permitir consultar mapas adicionais disponíveis por conjunto de texturas
* [Script] Permitir recuperação de formato de canal
* [Roteiro] Adicione exemplos na documentação de cozimento
* [Script] Permitir consulta da visibilidade de uma camada
* [Script] Permitir consulta do modo de mesclagem e da opacidade da camada
* [Scripting] Permitir exportar mapas convertidos (mapas normais finais, AO misto, etc.)
* [Substance] Ler e conectar usos personalizados
* [Atalhos] Adicionar tecla modificadora (SHIFT) para percorrer o modo solo para trás
* [Exportar] Predefinição de exportação padrão atualizada para desativar alfa
* [IU] Agora, as miniaturas são calculadas somente se o mecanismo estiver disponível
* [IU] Exibir uma menção quando as miniaturas estiverem em processamento

**Corrigido:**

* Falha com alguns projetos antigos ao abri-los
* Falha com cache de canais de textura corrompido
* Falha ao mesclar mais de 4 materiais com o fluxo de trabalho de Camada de material
* [IU] Os atalhos de ferramenta não funcionam se a barra de ferramentas estiver oculta
* [UI] A barra de ferramentas do Iray está marcada como “Sem título” no menu Exibir
* [UI] As barras de ferramentas do plug-in são chamadas de “Não inclinadas” no menu Exibir
* [Baker] Pressionar Enter durante a edição de uma configuração de cozimento inicia o processo de cozimento
* [Baker] Intervalos incorretos para alguns parâmetros
* [Importar] Não é possível importar malhas OBJ devido a números muito grandes
* [Importar] Alguns arquivos OBJ são importados com muitos subobjetos
* [Exportar] o fundo do canal é preenchido com preto em vez da cor padrão na exportação
* [Ferramenta] As partículas não funcionam corretamente se o CDV for muito baixo
* [Ferramenta] A cor de visualização do pincel está incorreta com máscaras em subpilhas
* [Visor] Quando o pincel vai para áreas vazias na exibição 2D, ele se torna gigantesco
* [Visor] Visualização de pincel em branco ao pintar texturas Normais
* [Scripting] Documentação incorreta : “ao” listado em vez de “ambientocclusion”
* [Scripting] O processo iniciado com subprocess() é finalizado ao fechar o Painter
* [Prateleira] Filtro de iluminação assado usa entrada de AO incorreta
* [MacOS] Projeto de hidrante contra incêndio removido (incompatível)
* O projeto padrão é aberto ao carregar um arquivo \*.spt (em vez de \*.spp)

**Problemas Conhecidos:**

* [Plug-in] Por causa do Photoshop, o height e o canal normal não podem ser convertidos como estão

### 2.2.0

*(Lançado: 22 de julho de 2016)*

**Adicionado:**

* [Prateleira] Melhorar o sistema de pesquisa e as consultas
* [Prateleira] Adicionar campo de pesquisa para miniprateleiras
* [Shader] Permite definir a precisão da etapa para controles deslizantes
* [Shader] Adiciona um botão Desfazer/Refazer para parâmetros de sombreador
* [Shader] Recarregar um sombreador não deve redefinir seus parâmetros
* [MatLayering] Adicionar suporte para Camadas de material dinâmico e subpilhas
* [MatLayering] Permite importar arquivo json para definir as configurações do sombreador
* [MatLayering] Limite de desbloqueio de classificadores de textura (alternar para texturas sem associação)
* [Script] Permitir a definição de configurações de padeiros e iniciar seu cálculo
* [Substance] Usar “uso” para conexões de entradas/saídas, além de identificadores
* [Ferramenta] Permite selecionar o canal de visualização no visor para a Ferramenta de projeção

**Corrigido:**

* Falha durante a inicialização se as substâncias estiverem localizadas na pasta errada
* O relatório de falhas às vezes não funciona devido a um arquivo de log incorreto
* [Iray] Os pós-efeitos não são atualizados quando o Iray está pausado
* [Iray] O atalho de foco automático não funciona mais
* [Iray] O comportamento do controle deslizante de abertura muda dependendo do tamanho do ativo
* [Camadas] O primeiro canal de material não é ativado por padrão se estiver desativado
* [Shader] Nenhum erro será impresso se um “param auto” estiver incorreto

**Problemas Conhecidos:**

* [Mac] O limite de amostras de textura está bloqueado em 16 (problema do driver de GPU)

### 2.1.1

*(Lançado em: 01 de julho de 2016)*

**Adicionado:**

* [License] Não será possível alterar o local do arquivo de licença
* [Janela de visualização] Adicionar um atalho “B” para alternar entre mapas adicionais
* [Importar] Permita importar o FBX 2016/2017 corretamente
* [Ferramenta] Remover verificadores ao usar a máscara rápida
* [Iray] Adicionar informações de dimensões de cena
* [Iray] Permita aumentar o número máximo de amostras e o tempo de renderização
* [UI] Atualizar o resultado imediatamente ao usar o botão +/- nos controles deslizantes
* [UI] Permitir maior precisão para controles deslizantes de Tons de Cinza
* [Exportar] Não exporte um canal alfa para texturas que são apenas RGB
* [Exportar] Atualizar predefinição de exportação do Dota 2
* [Prateleira] Novo padrão “Ladrilhos de hexágono”
* [Prateleira] Nova ferramenta “Solda”
* [Prateleira] Filtros de acabamento atualizados para fornecer controles de direção

**Corrigido:**

* [Exportar] Impossível exportar arquivos de PSD em 8 bits
* [Exportar] A exportação em 8K não está disponível em algumas configurações de hardware
* [Export] A janela do Sketchfab foi cortada
* [Exportar] Mapa de aspereza incorreto na predefinição de exportação de Espec/Gloss
* [IU] A digitação em controles deslizantes de tons de cinza não funciona mais
* [IU] Impossibilidade de colocar filtros nas entradas de substância (como Geradores)
* [IU] Alguns controles deslizantes têm comportamentos estranhos
* [UI] A etapa DeltaTime +/- para partículas é muito grande
* [Iray] Alguns projetos bloqueiam o aplicativo ao mudar para o Iray
* [Iray] Falha ao detectar hardware
* [Ferramenta] A cor de visualização de pincel está incorreta no modo Máscara
* [Ferramenta] O seletor de material pode ser usado com ferramentas incompatíveis
* [Ferramenta] A visualização da projeção não alterna para Difusa com o fluxo de trabalho Especificação/Brilho
* [Prateleira] Alterar sombreador padrão quebra as visualizações de tapetes inteligentes/máscaras inteligentes
* [Prateleira] Alguns materiais inteligentes têm nomes incorretos
* [Prateleira] Formas alfa adicionais estão corrompidas e não serão carregadas
* [Viewport] Alternar para o modo “Mapa adicional” exibe “outro” primeiro
* [Viewport] A opção Viewport volta para “other” quando não existe um mapa adicional
* [Crash][Linux] O relatório de falha não funciona no Ubuntu (Steam)
* [Crash][Linux] Os links de URL da Web não funcionam no Ubuntu (Steam)
* [Crash][Windows] Remover o “crashwatcher” quando o Substance painter não estiver mais em execução
* [Falha][Mac] O sistema de relatório de falhas não funciona corretamente
* [Falha] A importação de uma malha durante a importação de uma malha leva a uma falha
* O atalho de separação do conjunto de textura não é redefinido para nada após uma reinicialização

### 2.1.0

*(Lançado em: 2 de junho de 2016)*

**Adicionado:**

* [UDIM] Importar ladrilhos UDIM de uma malha como conjuntos de texturas
* [Linux] Suporte adicionado para CentOS 6.6 e Ubuntu 12.4
* [Exportar] Adicionar resolução 8K (experimental)
* [Exportar] Permite escolher a profundidade de bits durante a exportação
* [Baker] Permitir assar vários conjuntos de textura de uma só vez
* Suporte a monitores de alta resolução (dimensionamento de DPI alto)
* [Script] Definir resolução personalizada e preenchimento por textura na exportação
* [Visor] Permite alternar entre o conjunto de textura clicando na malha (via Ctrl+Alt+Clique)
* [Visor] Ir para onde está o cursor do mouse ao aplicar zoom com a roda do mouse
* [UI] Atualizar a cor de fundo padrão e a exibição do mapa de ambiente
* [UI] Adicionar dicas de ferramentas com nomes originais para canais do usuário
* [UI] Alterar a cor do plano de fundo de canais que não podem ser renomeados
* [Ferramenta] Remover verificadores ao usar a máscara rápida
* [Sombreador] Permite definir grupos para parâmetros de sombreador e materiais/máscaras
* [Engine] Otimização de carimbo de tamanho pequeno
* [Estêncil] Adicionar “W” como atalho para alternar temporariamente a máscara
* [Prateleira] Adicionar um botão de cruz para limpar o campo de pesquisa
* [Prateleira] Carregue o Alpha com um único clique
* [Prateleira] Nova predefinição de exportação: Vray UDIM, Arnold UDIM, Spec/Gloss from Metal/Rough
* [Prateleira] Alfas novas : formas geométricas, veias e sinais
* Adicionar nome e versão nas propriedades do executável Substance Painter

**Corrigido:**

* [Substance] Impossível usar o canal normal e o mapa adicional ao mesmo tempo
* [Iray] A refração MDL e a configuração de absorção não funcionam
* [Iray] A escala da cena original não é preservada
* [Prateleira] O modelo de Specular/Textura reluzente usa um sombreador incorreto
* [Exportar] A predefinição de exportação padrão não exporta alguns mapas (como AO)
* [Janela de visualização] O ponto dinâmico não é atualizado ao clicar fora dos UVs na visualização 2D
* [UI] Os valores do controle deslizante são arredondados
* [UI] Às vezes, ao editar os valores dos controles deslizantes, há um espaço livre muito pequeno
* [Novo projeto] A lista suspensa do modelo não foi atualizada corretamente (de 1.x para 2.x)
* [Script] Comportamento “hover” corrigido nos botões personalizados
* [Mac] Desfazer em um projeto vazio bloqueia a câmera

**Problemas Conhecidos:**

* O relatório de falha não está disponível no Ubuntu
* Alguns botões de URL podem não funcionar. Consulte nossas Perguntas frequentes para obter uma solução alternativa

### 2.0.5

*(Lançado: 29 de abril de 2016)*

**Adicionado:**

* [Prateleira] Modelo não pbr adicionado/atualizado, sombreador e predefinição de exportação
* [Shelf] Predefinição de exportação UE4 atualizada para incluir Oclusão ambiente

**Corrigido:**

* Falha ao abrir e salvar alguns projetos com recursos corrompidos
* [Visor] O Wireframe aparece quebrado na exibição 2D
* [Prateleira] Desempenho aprimorado de alguns mapas de ambiente de estúdio
* [Prateleira] Alguns mapas de ambiente de estúdio estão duplicados
* [Shelf] “Baked Lighting Material” (Material de iluminação assado) ausente
* [Shelf] Gerador “conversão em tons de cinza” ausente

### 2.0.4

*(Lançado: 26 de abril de 2016)*

**Adicionado:**

* Melhorar colisões de malha e otimizar a renderização de wireframe
* Melhore o desempenho e o gerenciamento de memória com grandes projetos
* Melhorar a precisão e a revisão do controle deslizante
* [UI] Atualizar o mecanismo somente ao validar um controle deslizante (não ao inserir um valor)
* [IU] Mova a opção Iray para um botão dedicado na barra de ferramentas principal (e altere seu atalho)
* [Ferramenta] Adicionar configuração para o comportamento de local de origem da ferramenta Clonar
* [Shader] Permite ler cores de vértice de malha em sombreadores personalizados
* [Scripts] Permite recuperar a lista de conjuntos de texturas, canais e camadas
* [Script] Adicionar funções do auxiliar (URL para caminho, obter caminho de exportação do projeto)
* [Mac] Detectar a versão “El Capitan” do Mac Os no arquivo de registro

**Corrigido:**

* Falha após a segunda exportação para o Substance share
* Falha ao copiar uma camada entre conjuntos de texturas com dados de Máscara rápida.
* Alguns projetos têm um atualizador muito longo que consome muita memória
* [Ferramenta] Falha ao selecionar uma predefinição de partícula com a ferramenta clone/borrar
* [Baker] Carregar arquivos FBX leva muito tempo para malhas pesadas
* [Visor] Mapa de ambiente ampliado em alguns computadores
* [Visor] Conversão de gama incorreta do alfa do pincel
* [Exportar] o Alpha é armazenado como transparência em vez de um canal separado com arquivos Tiff.
* [Exportar] O canal normal é sempre exportado como OpenGL
* [Iray] Nomes de controles deslizantes ausentes para configurações de Iray
* [Iray] A renderização é feita em uma resolução incorreta em Retina/High DPI
* [Iray] Falha ao redimensionar a interface no modo Iray
* [Iray] Enorme redução de desempenho ao renderizar em algumas resoluções baixas
* [Iray] A pausa não funciona (Iray ainda calcula em segundo plano)
* O canal normal às vezes tem artefatos de quadrado preto
* O canal normal é invertido pelos filtros de tons de cinza
* O canal normal não é mesclado corretamente se a pilha tiver algum alfa
* O projeto é editado no disco ao abrir um projeto, mesmo que ele ainda não tenha sido salvo
* A reimportação de uma malha em alguns projetos fornece desempenhos de GPU muito ruins
* A orientação do pincel está incorreta quando não está tocando em uma malha
* O logotipo do substance share está ausente na tela de boas-vindas

### 2.0.2

*(Lançado: 25 de março de 2016)*

**Adicionado:**

* [Iray] Atualize o modelo e o sombreador de Spec/Gloss para serem compatíveis com o Iray
* [Exportar] Conseguir exportar capturas de tela para o ArtStation
* [Scripting] Suporte à execução a partir do diretório de plug-ins
* [Script] Permitir “Salvar como”
* [IU] Permitir que você clique duas vezes em um controle deslizante para editar seu valor
* Mover amostra do Vela para o Substance share
* Novo projeto de amostra: Visualização da esfera
* Avisar os usuários sobre conflito de extensão do shell

**Corrigido:**

* Instalação de substituição do instalador do Substance Painter 1.x
* [IU] O layout da lista de canais está quebrado com filtros
* [UI] Os parâmetros de sombreador não são exibidos
* [IU] Redimensionar a janela da camada corta incorretamente o conteúdo
* [Ferramenta] O canal de opacidade nem sempre é usado corretamente
* [Ferramenta] Borrar/Clonar não funciona com Simetria
* [Ferramenta] A opacidade da visualização do pincel está incorreta em alguns canais
* [Iray] Falha ao usar o Iray enquanto ele ainda não foi criado
* [Iray] Não é possível carregar dados de configurações de iray do projeto
* [Iray] O Iray não cuida da modificação de configurações após uma pausa
* [Prateleira] Importar um material para a prateleira não funciona
* O estêncil não funciona com o canal Normal
* Falha ao pintar em alguns projetos
* Falha ao pintar com partículas em alguns projetos
* Falha com o processador Pixel durante alguns cálculos

### 2.0.0

*(Lançado: 16 de março de 2016)*

**Adicionado:**

* Atalho para armazenamento em Substance na barra de ferramentas principal
* Renderizador Iray com modo de visualização e exportação de captura de tela
* Suporte para criação e uso de “Máscaras inteligentes”
* Suporte para o fluxo de trabalho PBR de Specular/Glossários (com o novo canal difuso)
* Substance de encadeamento (conecta substâncias nas entradas de imagem do substance)
* Suporte a scripts com plug-ins personalizados
* Melhorar a conversão de Height em Normal usando um filtro Sobel
* Alternar resolução de visualização de estêncil/projeção para 2K
* Adicionar canal normal por padrão para novos projetos
* Ler a tag de dados do usuário no nó de saída para ativar/desativar os canais de uma substância por padrão
* Expor mesclagem normal/AO nas configurações do TextureSet
* [Ferramenta] Nova ferramenta Borrar para mesclar e espalhar cores
* [Ferramenta] Nova ferramenta Clonar para copiar parte de texturas
* [Ferramenta] Permite selecionar canais para as ferramentas Borrar, Clonar e Borracha
* [Camada] Adicionar nome de Substance para o nome do efeito de preenchimento
* [Camada] Permitir exportação de máscara para a área de transferência
* [Janela de visualização] Alternar entre o modo de perspectiva e ortográfico
* [Janela de visualização] Permite controlar o campo de visualização no modo de perspectiva
* [Janela de visualização] Permitir a definição da distância da Profundidade do campo com CTRL+Clique no botão do meio
* [Janela de visualização] Permite arrastar e soltar mapas de ambiente na Visualização 3D.
* [Visor] Feedback aprimorado quando o mecanismo está realizando cálculos fortes
* [Exportar] Permite exportar parâmetros de sombreador em um arquivo json
* [UI] Atualizar interface com novos ícones, cores e layout
* [IU] Adicionar nomes de ativos às miniprateleiras
* [UI] Recolher “Mapeamento de canais” por padrão
* [Shader] Escolha uma cor personalizada para os parâmetros de textura do sombreador
* [Prateleira] Perguntar onde importar arquivos ao arrastar e soltar recursos
* [Shelf] Nova esfera de visualização para materiais e geradores inteligentes
* [Prateleira] Adicionar sombreador de textura reluzente de Specular
* [Prateleira] Novas formas de Superfície Dura
* [Prateleira] Novas texturas e formas de Alpha
* [Shelf] Novas texturas de pele
* [Prateleira] Novos materiais baseados em digitalização e materiais inteligentes
* [Prateleira] Novos materiais inteligentes e suporte a especificações/brilhos de antigos
* [Prateleira] Novos filtros de acabamento para simulação de superfície metálica
* [Prateleira] Novo poderoso gerador de máscara “Editor de máscara”
* [Prateleira] Materiais antigos retrabalhados e limpos
* Novo projeto de amostra “Vela”

**Corrigido:**

* [Configurações] A rotação e a velocidade de zoom da câmera são substituídas pelo projeto
* [Visor] Problema de precisão na textura normal padrão leva a reflexos incorretos
* [Visor] A vinheta fica ativada por padrão
* [Visor] Os artefatos aparecem nas bordas do mapa ambiental (GPUs Nvidia)
* [Visor] A miniatura no modo de projeção/estêncil é muito longa para carregar
* [Baker] Armazenar texturas assadas em inteiros de 16 bits em vez de 32 bits
* [Camada] Substâncias desatualizadas são exibidas incorretamente na pilha
* A cor padrão e a profundidade de bits de alguns canais estão incorretas (por exemplo: Specular, Textura reluzente)
* Corrigido o comportamento de borracha para desativar a mesclagem no modo de passagem

**Problemas Conhecidos:**

* A simetria não funciona com a ferramenta Borrar e clonar
* A exportação do ArtStation está ausente

## Versão 1

### 1.7.3

*(Lançado em: 01 de março de 2016)*

**Adicionado:**

* [Exportar] Adicione uma opção para desativar o preenchimento
* [Prateleira] Suporte a hierarquia de subprateleira dentro de uma pasta de prateleira

**Corrigido:**

* Falha ao salvar sobre arquivo somente leitura anterior
* Falha ao abrir um segundo projeto
* Falha ao carregar algumas miniaturas (prateleira, camadas ou dicas de ferramentas)
* A desativação da opção “Preservar posições de traçados na malha” não funciona
* [Exportar] A ampliação de bitmaps é feita com a filtragem mais próxima
* [Prateleira] A descoberta de recursos é muito lenta
* [Prateleira] Os filtros de desfoque não são compatíveis com 16 bits
* [Ferramenta] A simetria não funciona se você carregar uma predefinição de ferramenta antiga
* A caixa de diálogo de cor do canal de Specular não faz uma conversão do espaço de cor

### 1.7.2

*(Lançado: 13 de janeiro de 2016)*

**Adicionado:**

* [Camadas] Permite especificar a divisão em blocos gráficos padrão para camadas de preenchimento

**Corrigido:**

* [Exportar] A exportação do Sketchfab não funciona mais
* [Camada] A filtragem bilinear é aplicada mesmo no Preenchimento sem nenhuma transformação
* [Ferramenta] Desempenho insatisfatório ao usar o substance com entradas de imagem no modo de projeção
* [Ferramenta] O seletor de material está danificado

### 1.7.1

*(Lançado: 18 de dezembro de 2015)*

**Corrigido:**

* Falha ao alternar o conjunto de textura
* Desempenho lento ao pintar

### 1.7.0

*(Lançado: 17 de dezembro de 2015)*

**Adicionado:**

* [Desempenho] Calcular o conteúdo das camadas e suas miniaturas ao mesmo tempo
* [Exportar] Salvar o caminho de exportação como relativo ao lado do projeto
* [Camadas] Adicionado novo modo de mesclagem: subtrair e adicionar/sub
* [Camadas] Nova filtragem de matriz bilinear para camadas de preenchimento
* [Shader] Defina um sombreador padrão para geração de miniaturas nas preferências.
* [Sombreador] Permite especificar um sombreador por conjunto de textura
* [Shader] Permite obter amostras de texturas da prateleira
* [Ferramenta] Novo comportamento de pincel “em contorno” para pintura
* [Ferramenta] Filtragem aprimorada e suavização reduzida ao pintar
* [Ferramenta] Qualidade de pintura de subpixels aprimorada
* [Ferramenta] A exibição “básica” das configurações de pincel foi removida e o ícone de abrir/fechar quadro foi aprimorado
* [Menu] Adicionar ícones de efeito no menu do botão direito do mouse
* Criação de modelo a partir de projetos
* [Prateleira] Novos modelos: PBR, Dota 2
* [Prateleira] Nova predefinição de exportação: Dota 2
* [Prateleira] Novos sombreadores: Dota 2, PBR Car paint, PBR Coated, PBR Velvet
* [Prateleira] Novo material : ferrugem de aço e desgaste, iluminação estilizada
* [Prateleira] Novos filtros : Desfocar iluminação direcional, estilizada
* [Prateleira] Novo pincel : padrão suave e padrão rígido com um novo alfa para um melhor controle de dureza
* [Prateleira] Novos geradores: Distância 3D e luz
* [Prateleira] Pincéis atualizados com projeção de quebra e remoção de face de fundo (ativada por padrão)
* [Shelf] Ruído branco atualizado com versão de processador de pixel para computação mais rápida

**Corrigido:**

* [Tela de boas-vindas] link Tutorials enviar para vídeos antigos
* [Canais] Dizer “não” para preencher a criação de camada com o AO ainda cria a camada
* [Canais] Os nomes de canais UserX não se propagam na interface
* [Janela de visualização] A entrada da máscara está vazia na lista de canais individuais
* [Compartilhar] Exportar um alfa para Compartilhar do SP cria um arquivo .image ilegível
* [Licença] Corrigir ativação para nomes de usuário com caracteres não ASCII
* [Shader] A caixa de diálogo Parâmetro de cor desaparece ao escolher uma cor
* [Prateleira] As miniaturas não são descarregadas da memória quando não usadas
* [Prateleira] Filtro de gradiente fixo
* [Ferramenta] A simetria não funciona com estêncil/projeção
* [Ferramenta] Nome incorreto ao criar uma nova predefinição de pincel
* A configuração Preservar traçado permanece desativada mesmo ao reimportar uma malha
* Reinicialização do driver (TDR) ao calcular partículas com tamanho grande.

### 1.6.1

*(Lançado: 09 de novembro de 2015)*

**Corrigido:**

* Falha ao abrir projeto se a exibição 2D estiver visível
* Falha ao criar nova predefinição de exportação se a prateleira atual não existir
* [Ferramenta] O ícone do seletor de material pode permanecer exibido
* [Ferramenta] O seletor de materiais oculta o cursor do mouse ao pintar ao mesmo tempo
* [Prateleira] Os metadados são gravados no disco após cada saída

### 1.6.0

*(Lançado: 29 de outubro de 2015)*

**Adicionado:**

* Suporte oficial para Windows 10
* [Substance] Recolher grupos de parâmetros de substância por padrão
* [Substance] Adicionar nova estrutura (melhorar o desempenho do processador de pixels)
* [Janela de visualização] Permite desativar a exibição do plano de simetria quando em modo de simetria.
* [Visor] Aprimorar o desempenho e a renderização de sombras
* [Visor] Pausar o cálculo de sombra ao pintar
* [Visor] Aprimorar os desempenhos da renderização do wireframe
* [Engine] Melhorar o gerenciamento de memória Vram para reduzir seu espaço
* [Engine] Aprimorar a atualização de textura nas GPUs AMD para obter melhores desempenhos
* [Engine] Desativar a configuração de otimização por threads nas GPUs NVIDIA para um melhor desempenho
* [Efeito] Adicionar uma tag para solicitar entrada de imagem “preenchida”
* [Camada] Aumenta a precisão do Deslocamento UV/escala no preenchimento
* [Camada] Tornar o controle deslizante de escala exponencial no preenchimento
* [Camada] Permite arrastar e soltar materiais diretamente na pilha de camadas.
* [Camada] Permite arrastar e soltar filtros diretamente na pilha de camadas
* [Camada] Ajuste a cor do pincel da máscara para a cor de máscara recém-criada
* [Shader] Expor várias texcoords
* [Shader] Expor a função de mapeamento de gama/tons para permitir funções personalizadas
* [Padeiros] Alterar configurações padrão do padeiro de posição para uso TriPlanar
* [Ferramenta] Renomear “Decalque de geometria” como “Preenchimento de polígono”
* [Prateleira] Geradores de atualização para apoiar TriPlanar: MG Metal edge wear, MG Mask builder, MG Fiber glass, MG Dirt
* [Prateleira] Atualizar materiais com novas configurações e materiais não utilizados removidos
* [Prateleira] 22 Novos materiais inteligentes (Plástico, Ferro, Tecido, Aço e mais)
* [Prateleira] Atualize os filtros de Nitidez, Desfoque e Distorção com entrada de imagem preenchida para evitar emendas
* [Prateleira] Melhorar as configurações de Distorção para facilitar o uso
* [Prateleira] 2 Novos ruídos de procedimento: ruído 3D Perlin e ruído 3D Worley

**Corrigido:**

* [Engine] A detecção de quantidade de Vram para GPU dedicada está incorreta no Mac
* [Engine] As texturas se transformam na versão mais escura no visor
* [Engine] Mau desempenho ao pintar abaixo de várias camadas
* [Engine] As camadas computadas ao abrir o projeto são diferentes da versão em cache
* [Substance] Resultados incorretos em 4K no Mac
* [Substance] Os parâmetros estão na ordem errada
* [Shader] Sombreadores de tons e pixels são totalmente pretos
* [Shader] Parâmetros desaparecem após alterar env-map
* [Prateleira] Falha ao colocar arquivos png na pasta do gerador
* [Prateleira] As miniaturas são geradas com baixa aspereza
* [Ferramenta] Falha ao usar um bitmap na alfa do pincel no Windows
* [Export] A predefinição de exportação de mapa adicional agora exporta um mapa de RGB para a Posição

### 1.5.7

*(Lançado: 24 de setembro de 2015)*

**Corrigido:**

* O relatório de falha não funciona mais

### 1.5.6

*(Lançado: 21 de setembro de 2015)*

**Adicionado:**

* [Prateleira] Melhorar a qualidade da renderização de miniaturas (usar texturas de 1 K)

**Corrigido:**

* [Compartilhar] Não é possível assinar com outra conta
* [Prateleira] Miniaturas muito pesadas no disco
* [Prateleira] Materiais inteligentes são muito lentos de carregar
* [Windows] Corrigir a instalação do serviço de licença
* [Canais] O mapa transmissivo é criado como G8 por padrão

### 1.5.5

*(Lançado: 15 de setembro de 2015)*

**Adicionado:**

* [Prateleira] Exportar ativos para o Substance share
* [Prateleira] Adicionar nova visualização de esfera para Materiais
* [Prateleira] Use o mapa de ambiente “Pátio vidrado” para gerar miniaturas
* [Prateleira] Aumentar a resolução do tamanho da miniatura para 512 x 512 pixels
* [Exibição 3D] Expor o valor da rotação do ambiente
* [Windows] Assinar o aplicativo

**Corrigido:**

* [Padarias] Resultados incorretos ao preparar mapas ao mesmo tempo
* [Exibição 3D] O mapa de ambiente é exibido quando nenhum projeto está aberto
* [Camadas] Os geradores de máscaras não funcionam no conteúdo da camada
* [Camadas] Você pode pintar em camadas ocultas
* [Prateleira] Os ruídos de Dirt\_5 e Dirt\_6 são idênticos
* [Prateleira] Alguns geradores de máscara são pixelados ou de baixa qualidade
* [Ferramenta] Rotação incorreta do cursor em determinados ângulos.
* [Ferramenta] Muitos canais fazem com que os botões do canal sejam cortados
* [Ferramenta] O atalho Inverter máscara para Máscara rápida não funciona
* [Exportar] Sketchfab: o botão Cancelar não foi levado corretamente em consideração
* A ativação do [License] falhou quando a licença não pode ser copiada
* O limitador de taxa de quadros não funciona mais na interface do usuário

### 1.5.0

*(Lançado: 20 de agosto de 2015)*

<b>Adicionado:</b>

* [Shader] Adicionar número de linha nas mensagens de erro de compilação do Shader
* [Prateleira] Melhorar a qualidade das visualizações de miniaturas
* [Prateleira] Automatizar geração de miniaturas para materiais inteligentes
* [Ferramenta] Atalho para controlar a configuração de dureza no substance
* [Ferramenta] Usar o widget de tons de cinza para decalque geométrico quando estiver sobre uma máscara
* [Ferramenta] Atalho para inverter a cor da pintura ao pintar em um mapa em tons de cinza
* [Visor] Permite exibir o wireframe e alterar sua cor
* [Visor] Desfocar o fundo do ambiente
* [Controles] Adicionar rotação aos atalhos de mouse do pincel
* [Exportar] Exportar para o Sketchfab
* [Exportar] Criar predefinições de exportação para renderizadores
* [Exportar] Adicionar Reflexo de mapa convertido, F0 e 1/IOR
* [UI] Tela Adicionar boas-vindas
* [UI] Atualizar layout padrão
* [UI] Adicionar dicas de ferramentas ausentes e renomear alguma entrada de menu
* [Camadas] Exportar máscara selecionada atualmente como bitmap
* [Camadas] Adicionar a ação “inverter máscara” no menu do botão direito do mouse

<b>Corrigido:</b>

* [Projeto] Se os eixos das malhas forem diferentes no FBX, as malhas são explodidas na importação
* [Substance] Os Substance usados nas ferramentas de projeção estão bloqueados em 256\*256
* [Camadas] Falha ao usar limpar máscara
* [Exportar] Conversão de gama incorreta em texturas muito escuras
* [Exportar] O mapa de posição só pode ser usado em predefinições de exportação como um mapa em tons de cinza
* [Ferramenta] A cor inicial do decalque de geometria é preta quando usada em uma máscara
* [Ferramenta] O atalho de rotação não funciona se não houver dureza no alfa

### 1.4.2

*(Lançado: 15 de julho de 2015)*

**Corrigido:**

* [Ferramenta] Falha ao usar o decalque de geometria com máscara rápida
* A atualização do projeto da versão 1.4.0 para a 1.4.1 consome toda a memória do computador
* Importação incorreta do formato do projeto antigo
* Prateleiras personalizadas analisam toda a hierarquia e duplicam ativos em todos os lugares

### 1.4.1

*(Lançado: 23 de junho de 2015)*

**Adicionado:**

* [Visor] Permitir encaixe dos painéis lado a lado
* [Efeito] Adicionar um plano de fundo e uma régua para o efeito de nível
* [Efeito] Adicionar um efeito de pintura que permite trabalhar sobre outro efeito

**Corrigido:**

* [Prateleira] A geração de miniaturas é interrompida se nenhum projeto estiver aberto
* [Prateleira] Falha ao gerar a visualização de predefinição de material
* [Prateleira] As visualizações de material são geradas em uma malha com normais invertidos
* [Prateleira] As miniaturas sempre são recalculadas devido à função de hash incorreta
* [Prateleira] Clicar em um material do substance não conecta mapas adicionais
* [Ferramenta] Valor incorreto amostrado com seletor de material
* [Ferramenta] Cor do cursor do visor de seleção de cores
* [Exibição 2D] Taxa de quadros/desempenhos muito baixos
* [Exportar] Falha ao abrir a janela de exportação com predefinições de exportação muito recentes.
* [Exportar] O canal de Height para o Mapa normal é convertido no espaço errado
* [Mac] BaseColor dos efeitos de substância é exibido como Linear
* [Mac] O widget de linhas retas é desenhado incorretamente na Retina
* As linhas retas podem permanecer ativadas mesmo com o atalho liberado.
* O guizmo de linhas retas desaparece após girar o mapa ambiental
* As saídas de oclusão ambiente de substâncias não são conectadas ao canal AO automaticamente
* Corrigir problema de cópia de licença no Windows com caractere especial no nome de usuário

### 1.4.0

*(Lançado: 10 de junho de 2015)*

**Adicionado:**

* [Exportar] Adicionar mapas adicionais na lista de mapas de entrada disponíveis
* [Prateleira] Usar materiais sbsar como predefinições de material
* [Prateleira] Permitir o uso de caminhos de biblioteca personalizados
* [Prateleira] Alterar o tamanho mínimo
* [Prateleira] Novo conteúdo: 20 novos materiais inteligentes
* [Prateleira] Novo conteúdo : nova substância processual (tecelagem, malha)
* [Prateleira] Filtro Desfoque atualizado
* Desenhar linhas retas usando uma tecla modificadora
* Adicionar canal de Oclusão ambiente e retrabalhar o comportamento AO/Normal na pilha de camadas
* Ler a cor padrão da Entrada de imagem definida nos dados do usuário Substance
* Permitir a exportação do log a partir do menu Ajuda

**Corrigido:**

* [Baker][Mac] Falha com normal do padeiro de malha
* [Baker] Falha se não houver UVs no arquivo da caixa
* [Baker] A correspondência por nomes não funciona com OBJs exportados do zBrush
* [Baker] Cozimento com uma gaiola sobrescreve o cozimento se usar vários conjuntos de textura e UVs sobrepostos
* [Baker] Arquivos OBJ específicos resultam em texturas pretas
* [Prateleira] Não é possível ler recursos se definido como somente leitura
* [Prateleira] Os arquivos de ativos estão sendo gravados no Painter se tiverem sido usados no projeto.
* [Prateleira] Recarregamento de substâncias também atualizar a camada
* [Export] O Tiff exporta imagens de 32 bits que não podem ser lidas corretamente pelo Photoshop ou por mecanismos de jogo
* [Exportar] A predefinição de canais padrão sempre é exportar como RGB
* [Material] Canal difuso substitui o mapeamento de BaseColor com substâncias
* [Visualização 3D] Iluminação difusa incorreta com mapas de ambiente específicos
* [Ferramenta] Não é possível girar um pincel para um ângulo específico
* O visor obtém o foco quando o mouse é ativado ao digitar em um campo de texto
* Falha com predefinições muito recentes para a versão atual da prateleira
* Falha após substituir a malha
* Falha ao recarregar uma substância com um número diferente de entradas
* Malhas FBX da importação do Cinema4D com nomes de material incorretos

### 1.3.5

*(Lançado: 29 de maio de 2015)*

**Adicionado:**

* Problema de ativação do [License] quando há um arquivo de licença existente
* [Mac] Falha ao carregar arquivos FBX específicos
* [Mac][Exibição 3D] Reflexão incorreta para GPU integrada
* [Exibição 3D] A fonte da Máscara rápida está quebrada
* [Exibição 3D] O seletor de materiais torna a janela de visualização totalmente preta
* Falha após abrir projetos criados na versão 1.3.3
* A visualização do material fica vazia ao usar sombreadores com alfa
* Pintura para de funcionar em malhas específicas
* O desempenho diminui muito com malhas OBJ específicas
* Os canais do usuário não são mapeados ao usar efeitos
* As pastas temporárias não são limpas na inicialização

**Corrigido:**

* Melhorias no tempo de computação em projetos extremamente longos para carregar
* Altere a janela “Solução de problemas de GPU” para ser mais compreensível
* [Camadas] Salva o status do bloqueio de proporção para camadas de preenchimento e torna-o “Ativado” por padrão
* [Padeiros] A correspondência por nome agora usa o sufixo como separador

### 1.3.4

*(Lançado: 27 de abril de 2015)*

**Adicionado:**

* [Mac] Falha com o Mac OS X Yosemite (10.10)
* [Mac] Não é possível sair do modo de tela cheia
* [Panificadores] A opção Coincidir pelo nome não funciona
* [Bakers] O espaço tangente Mikk usado no SP não funciona com UE4
* [Padeiros] O padeiro de identidade não pode assar cores de ID de material
* [2D View] O Wireframe não aparece ao usar a ferramenta de decalque Geométrico
* [Ferramenta] O canal alfa do pincel é exibido como verificador em vez de transparência com materiais
* [Ferramenta] Falha com decalque de geometria
* [Camadas] O slot de material é recolhido por padrão na camada de preenchimento
* [Exportar] Falha ao exportar em tamanho maior do que a resolução do conjunto de textura
* O canal do specular não é reconhecido nos filtros.
* Limpar e salvar não remove os recursos do arquivo do spp corretamente
* Não armazenar transformação de baixo polígono em arquivo de alta poliuretagem do compartimento
* O arquivo FBX é importado com muitos conjuntos de textura

**Corrigido:**

* Efeitos: os níveis de fixação devem estar ativados por padrão para imitar os níveis “clássicos”
* Camadas: alterar a divisão mínima e máxima na ação Preencher
* Camadas: salvar e restaurar o status da pilha
* Padeiros: AO Baker levar o mapa normal em consideração se nenhum HP é especificado
* Panificadores: Dicas de ferramentas e informações adicionais adicionadas na janela de cozimento
* Criar um arquivo de backup ao salvar um projeto

### 1.3.3

*(Lançado em: 01 de abril de 2015)*

**Adicionado:**

* Adicionar versão de software e nome do projeto na barra de título
* Limpar nomes de TextureSet e nomes de materiais inteligentes
* Atualizar mecanismo de Substance para V5
* [Shelf] Adicionar novos mapas de ambiente: praia da Córsega, estúdio 05, estúdio de Tornoco e muito mais
* [Prateleira] Atualizar MG Mask Builder com novos parâmetros
* [Prateleira] Atualizar e calibrar mapas de ambiente antigos

**Corrigido:**

* Falha ao abrir a janela de exportação
* Não é possível arrastar e soltar no widget da interface do usuário quando desencaixado
* “Verificar atualizações” não está funcionando
* [Camadas] Não selecione a máscara ao pressionar ALT e clicar nela
* [Ferramenta] O tri-planar não funciona com o canal Normal
* [Visualização 3D] A iluminação difusa do mapa de ambiente está incorreta
* [Visualização 3D] O cálculo da exposição é diferente do Designer
* [Exibição 3D] As sombras não devem ser visíveis em uma superfície 100% metálica
* [Exibição 3D] A malha com UVs espelhados inverteu a tangente/binômios
* [Exibição 3D] As sombras produzem resultados incorretos em determinadas malhas
* [Bakers] Remove a pasta “.alg\_meta” criada por arquivos assbin
* [Padeiros] Falha ao assar se o Painter recalcular um TextureSet ao mesmo tempo
* [Mac] Falha na interface do usuário da caixa branca ao iniciar o aplicativo

### 1.3.2

*(Lançado: 06 de março de 2015)*

**Corrigido:**

* [Exibição 3D] Falha ao recarregar um mapa de ambiente salvo com o projeto

### 1.3.1

*(Lançado: 05 de março de 2015)*

**Adicionado:**

* [Padeiros] Adicione uma versão em cache de malhas de alto polígono para acelerar o cálculo
* [Padeiros] Adicionar um ícone de aviso se nenhuma malha de alto polígono estiver carregada
* [Padeiros] Se nenhuma malha de alto polígono estiver carregada, use a malha do projeto

**Corrigido:**

* [Bakers] Pressione “enter” ao editar o valor de um controle deslizante para fechar a janela
* [Padeiros] Ativar/desativar um padeiro também acionará o botão
* [Bakers] Impossível assar se você usar o botão “todos/nenhum”
* [Padeiros] A ordenação dos botões do padeiro não está na ordem correta
* [Padeiros] Caixa de seleção ignorada e todos os padeiros são sempre processados
* [Padeiros] Progresso da barra de progresso fixo

### 1.3.0

*(Lançado: 04 de março de 2015)*

**Adicionado:**

* [Padeiros][Visualização 3D] Usar computação de espaço tangente Mikkt se nenhuma tangente/binormal for encontrado
* [Pães] Adicionado novos padeiros: Normal, ID, Oclusão, Curvatura, Thickness, Posição
* [Efeitos] A pilha de efeitos agora é invertida e exibida de cima para baixo (como camadas)
* [Efeitos] Adicionar novos ícones na pilha de efeitos
* [Efeitos] Adicionar modo de mesclagem entre ações de preenchimento na pilha de efeitos
* [Efeitos] Renomear efeitos (efeito de substância = filtro, etc.)
* Adicionar um arquivo de “bloqueio” durante o processo de salvamento
* [Efeitos] Adicionar ação de preenchimento na pilha de efeitos
* Adicionado novo recurso: materiais inteligentes
* [Camadas] Permitir a reordenação de efeitos de camada
* [Tool] Adicionar projeção triplanar
* [Exibição 3D] Adicionar suporte para sombras
* [Visualização 3D] Capacidade de definir estados OpenGL necessários em sombreadores personalizados
* [Visualização 3D] Suporte para alfa por meio de novos sombreadores
* [Exibição 3D] Os sombreadores agora têm versão e foram salvos completamente em um projeto
* [Exibição 3D] Avisa o usuário se o sombreador não compilar mais

**Corrigido:**

* [Camadas] corrigir soltar em uma pasta recolhida
* [Prateleira] Corrigir filtragem de conteúdo em miniprateleiras
* [Prateleira] Renomear categorias e reorganizar guias

### 1.2.1

*(Lançado em: 12 de fevereiro de 2015)*

**Adicionado:**

* Os arquivos \*.spp agora podem ser abertos com um clique duplo no explorador
* [Exportar] Nova tag “$project” para predefinições de exportação
* [Exportar] Adicionar a lista de mapas (com nomenclatura) abaixo de cada conjunto de textura
* [Exportar] Adicionar um botão Todos/Nenhum para selecionar os conjuntos de texturas
* [Exportar] Mapas vazios são descartados durante a exportação

**Corrigido:**

* [Export] As predefinições do Unity5 têm mapas invertidos
* [Exportar] Adicionar uma barra em um nome predefinido criará uma pasta corrompida
* [Exportar] O canal de Height exportado em formatos de 32 bits está incorretamente compactado
* [Exportar] A lista de conjuntos de texturas não é classificada como no projeto
* [Ferramenta] A remoção de fundo não funciona mais
* Salvar não funciona com caracteres especiais no caminho

### 1.2.0

*(Lançado: 28 de janeiro de 2015)*

**Adicionado:**

* Novo canal Normal permitindo pintar os dados normais do mapa e combinar os resultados
* [Exportar] Nova janela de exportação com a capacidade de criar uma embalagem personalizada e definir nomes personalizados
* O formato de arquivo do projeto agora é um único arquivo em vez de pastas
* [Exportar] Suporte a diferentes formatos Normais (DirectX, OpenGL)
* [Exportar] Criar um arquivo temporário de “bloqueio” durante a exportação
* [Camadas] Shift+Clique com o botão esquerdo do mouse pode ser usado para alternar uma máscara
* [Parâmetros] Expor o espaço de cores na parte inferior de uma entrada de imagem
* [Prateleira] O efeito “MG Mask Builder” agora tem novas configurações
* [Exibição 3D] O mapa de Oclusão ambiente agora oclui a contribuição difusa, não o specular

**Corrigido:**

* A visualização do material de projeção/estêncil não é exibida corretamente no visor
* [Exibição 3D] Dica de ferramenta de atalho não exibida ao usar o atalho “S” (estêncil)
* [Shelf] O efeito “Escala de pele MatFx” agora tem melhores desempenhos em baixa resolução
* [Exportar] As texturas da exportação são ampliadas ao especificar um tamanho de documento maior

### 1.1.2

*(Lançado: 15 de janeiro de 2015)*

**Adicionado:**

* Adicionado: novas configurações de Traduzir, Girar e Dimensionar na camada Preenchimento
* Filtragem aprimorada para camadas de Pincéis e Preenchimento
* A versão de teste agora está completa em recursos (pode exportar), mas é limitada no tempo.

**Corrigido:**

* Impossível importar malhas OBJ com precisão muito pequena
* Problema ao ativar uma licença no Windows 7 e 8
* Falha durante um “Salvar como” de um projeto
* Falha ao excluir o último canal de um conjunto de textura
* Falha ao excluir uma camada em um contexto específico

### 1.1.1

*(Lançado: 25 de dezembro de 2014)*

**Adicionado:**

* [Camada] Selecione a camada na parte superior ao abrir um conjunto de texturas de projeto/alternância
* Velocidade aprimorada de “Salvar” e “Salvar como” com o novo algoritmo de compactação
* Exibir um erro ao abrir um projeto muito recente para o Painter

**Corrigido:**

* [Ferramenta] O decalque geométrico produz corrupções na memória
* [Pincel] Impossível inserir manualmente valores de flutuação abaixo de 1 para o tamanho do pincel
* [Camada] Criar um efeito de seleção de cor não o adiciona à pilha de camadas
* [Camada] Mover o mouse sobre as camadas faz com que o Painter passe rapidamente na barra de tarefas
* [Camada] Adicionar um bitmap como máscara pode levar a uma falha
* A interface gráfica para o modo solo com o canal de Height está incorreta
* “Salvar projeto” pode falhar e corromper um projeto
* Falha ao abrir um projeto após carregar outro com um sombreador desatualizado

### 1.1.0

*(Lançado: 16 de dezembro de 2014)*

**Adicionado:**

* [Efeito] Novo criador de máscara de ID de material
* Nova linha branca/preta pontilhada para o cursor do pincel
* Novo parâmetro de sequência de ângulo
* Novo parâmetro de remoção de tela de fundo
* Novo parâmetro de mouse lento
* [Camadas] Suporte para várias seleções e gerenciamento
* [Camadas] Copiar e colar de um conjunto de texturas para outro
* [Exportar] Formato PSD do Adobe Photoshop
* [Prateleira] Nova ferramenta : pele, pontos de metal e zíper
* [Prateleira] Novo pincel : molde, lápis, linha afiada e ponto
* [Prateleira] Novo alfa : ruído gaussiano, linha afiada, molde, caneta, respingo, ponto, zíper
* O desempenho da pintura melhorou atualizando apenas partes das texturas necessárias

**Corrigido:**

* [Prateleira] Impossível carregar uma substância com gráfico com rótulos idênticos
* [Camadas] O modo de mistura Passagem não funciona com máscaras
* A escala de [Estêncil] está quebrada na exibição 2D
* Problemas e falha no Mac OS Yosemite

### 1.0.2

*(Lançado: 09 de novembro de 2014)*

**Adicionado:**

* Desempenho aprimorado na visualização de material com substâncias
* Desempenho aprimorado com visualização de traçado de pincel ao atualizar o documento
* Desempenho aprimorado no visor com menor taxa de atualização para a área não funcional
* [Post Effects] Interface do usuário aprimorada para gerenciar configurações
* [Post Effects] Redefinir para valores padrão
* efeitos de Substance e operações de camadas no menu do botão direito do mouse
* Apoio a entradas/saídas pré-multiplicadas em substâncias

**Corrigido:**

* [Exibição 3D] Os parâmetros de sombreador personalizados são separados por um espaço grande
* [Exportar] Conversão sRGB para predefinição Unity4 ausente
* Possível falha ao carregar malhas fbx
* Falha às vezes ao carregar malhas obj simples
* A barra de computação permanece bloqueada até 100% no carregamento
* Recarregar uma substância a coloca em todas as categorias
* Chave de DirectX/OpenGL quebrada

### 1.0.1

*(Lançado: 27 de outubro de 2014)*

**Adicionado:**

* [Ferramenta] Uso aprimorado de parâmetros de material
* Novo atalho para o site do UserVoice no menu Ajuda
* Várias melhorias de desempenho no motor

**Corrigido:**

* Os valores dos parâmetros são limitados a 2 decimais para Partículas
* Os Substance carregados do cache não são exibidos na interface como desatualizados
* Falha ao carregar uma malha de uma url de rede
* O Painter agora é reconhecido como assinado no Mac OS X

### 1.0.0

*(Lançado: 15 de outubro de 2014)*

**Adicionado:**

* Suporte a shader personalizado
* Suporte para resolução 4k
* Projetos de personagem de amostra
* Exibir barra de progresso para longos tempos de computação
* [Exportar] Adicionar uma passagem de dilatação antes do pós-processo de difusão
* Argumentos de linha de comando no SP para operações simples
* Novos materiais e efeitos
* Visualização da ferramenta (visualização de material em tempo real separado e área de teste de traçado)
* Não criar um documento padrão quando o Painter for iniciado
* [Ferramenta] Adicionar a possibilidade de editar manualmente um valor em tons de cinza
* Várias melhorias para os estênceis (Ajustar, Redefinir)
* As partículas agora são subferramentas das ferramentas Pincel, Borracha e Projeção
* [Exibição 3D] Usar AO cozido na renderização do visor
* Dividir os controles de estênceis entre a exibição 2D e 3D
* Ajuste pequeno do tamanho do polegar na biblioteca
* Os campos de pesquisa são específicos para cada janela
* Ajustes da interface

**Corrigido:**

* [Substância] O switch não funciona
* [Caixa de diálogo Cor] Degradê de matiz não atualizado
* Não é possível atualizar uma malha se o nome do arquivo é idêntico
* A ferramenta não fica visível nas exibições quando muito pequena
* A ferramenta de decalque na tela Retina não funciona corretamente
* [Substance] Int1 são exibidos como float1
* [Substance] A entrada/saída basecolor não é reconhecida
* Não é possível recarregar os filtros [Substance]
* O widget de tons de cinza [Ferramenta] sempre é recolhido

## Beta

### &#x200B;0. 12. 1- beta

*(Lançado: 18 de setembro de 2014)*

**Adicionado:**

* Predefinição de exportação do Unity 5

**Corrigido:**

* PBR Shader, a qualidade da renderização deve melhorar muito
* A função de foco está quebrada e as malhas são cortadas por padrão

### &#x200B;0. 12. 0- beta

*(Lançado: 17 de setembro de 2014)*

**Adicionado:**

* Ferramenta Conta-gotas
* A opção “Preservar posição de traçado” foi adicionada à reimportação de malha para quando a caixa delimitadora for alterada.
* Mapa normal para a malha padrão de Cymourai
* Aprimorar a interface de exibição da ferramenta (as cores são wip)
* Mova o menu “Ajuda->Configurações” para “Editar->Configurações”
* Salve o caminho de exportação na janela “Exportar todos os canais”
* Novos níveis de GUI com exibição de histograma
* Melhor gerenciamento de ativos (arrastar e soltar, recarregar recursos, excluir não usados)
* Alternar de “difusa” para “basecolor”
* Controles deslizantes que editam ajustes - permitem pontos além de vírgulas
* Camada de preenchimento: aumentar o valor máximo de divisão em blocos gráficos
* Mapa de ambiente padrão

**Corrigido:**

* Artefatos de reflexo inválidos em ângulos extremos
* Exportação de specular/brilho quebrado
* Links na janela “sobre” do pintor não funcionam
* Falha com o OSX Yosemite
* A malha é salva triangulada
* O atalho de cor da janela Ferramenta envia para o emissor em vez da escala de cinza
* O seletor de cores permanece aberto ao alternar de camada para máscara
* Não é possível salvar o material de uma camada de preenchimento
* Habilitar o redimensionamento das três regiões da prateleira

### &#x200B;0. 11. 0- beta

*(Lançado em: 4 de setembro de 2014)*

**Adicionado:**

* Adicionar um divisor entre as visualizações 3D e 2D
* Usar um plano de fundo gradiente nas visualizações 2D/3D
* Interface para o histograma de Níveis
* Mesclar prateleira e biblioteca
* Nenhuma ação de salvamento é necessária ao criar ou atualizar uma predefinição
* Importar ativos de prateleira por meio da funcionalidade de arrastar e soltar

**Corrigido:**

* O nome dos botões é exibido acima na barra de ferramentas principal

### &#x200B;0. 10. 2- beta

*(Lançado: 28 de agosto de 2014)*

**Corrigido:**

* Exportar todos os canais produz resultados incorretos

### &#x200B;0. 10. 1- beta

*(Lançado: 26 de agosto de 2014)*

**Corrigido:**

* O sombreador dá resultado preto com baixa aspereza
* Verificação da GPU: use placas “Quadro”, detecte todos os dispositivos e adapte as mensagens do usuário de acordo
* A maioria dos materiais do Substance está limitada a 256 na versão Beta 9
* O height é bloqueado quando exportado como bitmap
* A visualização do pincel é diferente da sobreposição da projeção no Mac
* O uso da ferramenta Geometria para criar máscaras não é exibido em viewports
* A máscara rápida está quebrada
* Corrigir problema de mesclagem no mac pro antigo

### &#x200B;0. 10. 0- beta

*(Lançado em: 07 de agosto de 2014)*

**Adicionado:**

* Máscaras de estêncil

**Corrigido:**

* Suporte a placas Quadro
* O sombreador dá resultado preto com baixa aspereza
* Os materiais do Substance estão limitados a 256
* A exportação normal de mapa exclui o canal verde

### &#x200B;0. 9. 0- beta

*(Lançado: 17 de julho de 2014)*

**Adicionado:**

* Pós-processamento do Yebis 2
* O assistente para Novo projeto permite importar mapas de entrada (AO, Curvatura, etc.)
* Conectar automaticamente mapas de entrada (AO, curvatura etc.) para Efeitos de Substance
* Controle da escala sobre os materiais aplicados às camadas de preenchimento

### &#x200B;0. 8. 2- beta

*(Lançado: 11 de julho de 2014)*

**Corrigido:**

* O controle deslizante Matiz assume branco como padrão
* Projeto será redefinido se o Nome do material contiver caracteres especiais
* A alteração do nome do material em um único objeto de material não deve invalidar o projeto.
* Os UVs ficam confusos depois de salvar o projeto e reabri-lo

### 0.8.1-beta

*(Lançado em: 4 de julho de 2014)*

**Corrigido:**

* Várias falhas de GPU
* Falha ao exportar canais

### &#x200B;0. 8. 0- beta

*(Lançado: 28 de junho de 2014)*

**Adicionado:**

* Vários materiais - agora você pode pintar em vários materiais no mesmo documento
* Pintura de simetria
* Todos os modos de mesclagem agora estão disponíveis

**Corrigido:**

* Várias falhas de GPU
* Projeto será redefinido se o Nome do material contiver caracteres especiais
* Os UVs ficam confusos depois de salvar o projeto e reabrem com vários UVs

### &#x200B;0. 7. 0- beta

*(Lançado: 18 de junho de 2014)*

**Adicionado:**

* Efeitos de camada
* Novos materiais de estêncil de Substance
* Limpar máscara
* Permitir copiar/colar camada/máscara
* Permitir Duplicar Camada
* Alterar ferramenta ao editar máscara de camada
* Os Substance agora são ativados por GPU

**Corrigido:**

* A pintura do mapa de heights não pinta valores negativos.
* A exibição do Seletor de materiais não deve levar em conta o mapa normal amostrado
* Determinismo de partículas quebrado
* Matriz de estêncil na exibição 2D
* Ngons em arquivos obj
* Várias falhas

### &#x200B;0. 6. 0- beta

*(Lançado em: 04 de junho de 2014)*

**Adicionado:**

* Nova opção de exportação para exportar um mapa de Specular de um composto de aspereza e canais metálicos

**Corrigido:**

* Compatibilidade com o Windows Vista
* O mapa de heights não pintará valores negativos

### &#x200B;0. 5. 0- beta

*(Lançado em: 07 de maio de 2014)*

**Adicionado:**

* Opções de exibição 3D/2D
* Ferramenta Seleção de partes UV
* A ferramenta muda automaticamente ao pintar em máscaras.
* A resolução dos Substance depende da

**Corrigido:**

* Falha na inicialização
* Falha com malhas ASCII
* Matriz de estêncil fixa na exibição 2D
* Falha com Borracha

### &#x200B;0. 4. 0- beta

*(Lançado: 17 de abril de 2014)*

**Adicionado:**

* Visualização 2D contínua
* Máscaras de camada de bitmap
* Controle de exposição do ambiente
* Preencher camadas agora usa a janela Ferramentas para definir suas propriedades
* Os materiais podem ser aplicados a camadas de preenchimento
* Adicionou mais estênceis à biblioteca de estênceis
* Predefinições de partículas atualizadas para uma computação mais rápida
* Otimização de sombreador PBR e melhoria de qualidade para configurações de qualidade inferior

**Corrigido:**

* As miniaturas de camadas são vinculadas ao canal atualmente selecionado
* Muitas falhas

### &#x200B;0. 3. 0- beta

*(Lançado: 04 de abril de 2014)*

**Adicionado:**

* Permitir valores negativos no seletor de cores para pintura de mapa de height
* Mostrar visualização do material/cor separado
* Adicionar atalhos para as Ferramentas na Barra de Ferramentas (1, 2, 3, 4)
* Alternar o formato normal (OpenGL versus DirectX) globalmente em um projeto
* Assistente para Novo projeto
* O controle deslizante de espaçamento não está mais apertado
* Estilo atualizado dos controles deslizantes
* Tornar o seletor de cores não modal
* Selecionar um material na biblioteca define o tipo de ferramenta adequadamente

**Corrigido:**

* Corrigido: o caminho da malha de importação não é preservado
* Correção: geração de texturas incorreta
* Corrigido: falha na inicialização

### &#x200B;0. 2. 0- beta

*(Lançado: 17 de março de 2014)*

**Adicionado:**

* Conta-gotas de material (atalho P)
* Miniaturas na visualização da ferramenta 3D
* Sistema de licenciamento para versões autônomas
* Atalhos [ e ] para Tamanho do pincel
* Preenchimento em mapas exportados
* Estilo de Janela de Ferramenta Atualizado
* Estilo atualizado dos controles deslizantes
* Ambiente HDR padrão atualizado

**Corrigido:**

* Estêncil: alterar o valor do fluxo na exibição 3D para em 52
* Loop infinito no motor ao adicionar teclas de pressão 0 ao traço é fixo
* Ferramenta: a tremulação de ângulo não retorna valores acima de +/- 90%
* A exibição 3D muda quando uma máscara de camada é selecionada
* Zoom invertido

### 0.1.0-beta

*(Lançado: 02 de março de 2014)*

**Adicionado:**

* Novo gerenciamento de biblioteca
* Novo conteúdo de pincéis e partículas
* Visualização do pincel 3D
* Estilo de Janela de Ferramenta Atualizado
* Estilo atualizado dos controles deslizantes
* Desempenho atualizado do cache

**Corrigido:**

* Controles de câmera
* Rotação do pincel
