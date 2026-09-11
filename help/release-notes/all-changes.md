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
source-git-commit: fc154cd38e23b0e598c15bfbfee8a263d5770592
workflow-type: tm+mt
source-wordcount: '34015'
ht-degree: 0%

---


# Todas as alterações

Esta página contém notas de versão de todas as versões anteriores do Substance 3D Painter, classificadas da mais recente para a mais antiga.

>[!NOTE]
>
> Para exibir os problemas conhecidos que podem afetar o Painter, consulte a [página de documentação dedicada](known-issues.md).

## Versão 12

### 12.1.4

Data de lançamento: **9/2026/04**

Resumo: **Versão secundária**

**Corrigido:**

- \[Falha\] Falha ao importar ou exportar arquivos cujos nomes de arquivo contenham caracteres não-ASCII

### 12.1.3

Data de lançamento: **2026/08/26**

Resumo: **Versão secundária**

**Adicionado:**

&#x200B;* Atualize o mecanismo de Substance para a versão 9.4.6

**Corrigido:**

&#x200B;* O seletor [Escala de cinza] permanece aberto após a alteração da ferramenta
&#x200B;* [Inclinar Fazendo bake] Inclinar as interrupções da correção ao pintar e desfazer
&#x200B;* [A interação Janela de Projeção] foi bloqueada pela ferramenta de projeção
&#x200B;* [Traço dinâmico] Parâmetros de traço dinâmico ausentes nas propriedades do pincel
&#x200B;* Exportar para uma rede não funciona mais

### 12.1.2

Data de lançamento: **08/2026/03**

Resumo: **Versão secundária**

**Corrigido:**

&#x200B;* \[Falha\] Alguns Substance podem levar a uma falha quando renderizados
&#x200B;* \[Falha\] Reimportar malha enquanto estiver no modo de fça bake
&#x200B;* \&lbrack;Falha ao inicializar a exibição de gráficos pode levar a uma falha
&#x200B;* \[Falha\] A exportação de texturas pode falhar em alguns casos ao atualizar o registro
&#x200B;* \[Falha\] Falha no modo de cozimento em alguns casos ao carregar/atualizar o mapa do ambiente
&#x200B;* \[Preparação\] Reiniciar o bake após modificar o arquivo poli alto pode levar a um congelamento
&#x200B;* \[Enviar para o Photoshop\] Falha ao exportar a máscara da camada
&#x200B;* O resultado do ponto de ancoragem do \[Mecanismo\] não é renderizado entre uma máscara e um canal de cor

### 12.1.1

Data de lançamento: <b>07/2026/09</b>

Resumo: versão secundária

Adicionado:

&#x200B;* [Cozimento de inclinação] Expor o modo normal da base de inclinação: malha ou por triângulo
&#x200B;* [Propriedades] Faça com que as cores uniformes sejam sempre redefinidas para o valor padrão do canal
&#x200B;* [OpenPBR] Reagrupe canais por categorias na janela Exportar Texturas para criação de modelos de saída
&#x200B;* Atualize o mecanismo de Substance para a versão 9.4.5

Corrigido:

&#x200B;* [Projeto] Abrir e salvar alguns projetos pode demorar mais do que o normal
&#x200B;* [Falha] Recarregar várias malhas pode levar a uma falha
&#x200B;* [Falha] ao excluir um canal durante o modo de exibição de máscara, o que leva a uma falha
&#x200B;* [Falha] Alguns Substance podem levar a uma falha quando renderizados
&#x200B;* [Inclinação de pintura] A ferramenta selecionada na inclinação de pintura permanece selecionada após alternar para o Modo de Pintura
&#x200B;* [Preparando Configurações Comuns] As configurações de Distância da Gaiola não atualizam a visualização do wireframe e do sombreador da gaiola
&#x200B;* [O ] preenchimento UV do modo “Vizinho do Espaço 3D” não funciona bem em triângulos finos
&#x200B;* O resultado do ponto de ancoragem do [Mecanismo] não é renderizado entre uma máscara e um canal de cor

### 12.1.0

Data de lançamento: <b>2026/06/23</b>

Resumo: <b>Esta atualização é uma versão principal. Ela contém melhorias para PANELAS com Novo estado de interface de usuário padrão de cozimento, mapa de inclinação da pintura, retoque automático, nova opção de desencapsulamento automático UV para malhas de superfície dura e OpenPBR. Para obter mais detalhes, consulte as notas de versão completas.</b>

<b>Adicionado</b>:

&#x200B;* [Mastigar cozimento] Ferramentas de pintura de inclinação
&#x200B;* [Assoalho de inclinação] Adicionar sombreador de visualização de inclinação e visuais de vetor de direção de inclinação ao pintar mapa de inclinação
&#x200B;* [Mascarar cozimento] Opção Adicionar proteção de borda
&#x200B;* [Assobiar] Recozimento automático
&#x200B;* [Assoalho de inclinação] Interface do usuário de lista do mapa de malha de retrabalho
&#x200B;* [Assoalho de inclinação] Dividir as configurações do Mapa de malha/Preparação comum + Mover as configurações comuns para fora da lista de mapas de malha apenas com cor base ou máscara
&#x200B;* [Inclinar cozimento] Alterar botões da barra de ferramentas da viewport
&#x200B;* [Cozimento de inclinação] Mostrar alternância de simetria para o pincel na barra de ferramentas superior
&#x200B;* [Assoalho de inclinação] Opções de renomeação no menu de sincronização de lista do mapa de malha
&#x200B;* [Inclinação da montagem] Caixas de diálogo de sincronização de atualização e estado verificado
&#x200B;* [Assoalho de inclinação] Criar variante do seletor de cores em tons de cinza
&#x200B;* [Inclinar cozimento] Ícone Atualizar modo de cozimento
&#x200B;* [Desenvolver automaticamente] Opção Integrar superfície rígida
&#x200B;* [OpenPBR] Adicionar suporte para OpenPBR 1.1
&#x200B;* [OpenPBR] Tornar o OpenPBR o fluxo de trabalho e o sombreador padrão
&#x200B;* [OpenPBR] Importar materiais e texturas do OpenPBR via USD
&#x200B;* [OpenPBR] Exportar materiais e texturas do OpenPBR via USD
&#x200B;* [OpenPBR] Janela Atualizar Texturas de Exportação para mostrar a convenção de nomeação do OpenPBR
&#x200B;* [OpenPBR] Adicionar documentação sobre alterações para suportar o OpenPBR
&#x200B;* [OpenPBR]&#x200B;[Iray] Adicione o novo MDL para suportar o OpenPBR 1.1 no Iray
&#x200B;* Várias pequenas melhorias nas exportações em USD
&#x200B;* [UI] Adicionar aviso no visor ao tentar pintar em outro conjunto de texturas
&#x200B;* [Nivelar] Permite nivelar todas as camadas da instância nos Conjuntos de textura
&#x200B;* [Configurações do conjunto de texturas] Permite selecionar vários canais de uma vez por meio de uma nova janela
&#x200B;* [History] Atualizar “valor” Desfazer a entrada de texto para refletir o nome do parâmetro
&#x200B;* [Pilha de camadas] Tornar efeitos de preenchimento em máscaras padrão em branco (1.0)
&#x200B;* [Substance] Adicionar nova entrada de mapa do mecanismo “mesh_hard_edges_triangle”
&#x200B;* [Substance] Adicionar nova entrada de mapa do mecanismo “mesh_hard_edges”
&#x200B;* [Shader] Impedir que instâncias de sombreador compartilhem os mesmos nomes
&#x200B;* [Shader] Use o sombreador do modelo do projeto ao importar um arquivo USD ou GLTF
&#x200B;* Atualize o Adobe Color Engine para a versão 7.0
&#x200B;* Atualização mínima da versão do MacOSX para a versão 13.0 (Ventura)
&#x200B;* [Conteúdo] Novos modelos de projeto para OpenPBR
&#x200B;* [Conteúdo] Atualizar projetos de amostra para usar o novo sombreador de OpenPBR
&#x200B;* [Python] Expandir a API da Máscara de geometria para permitir modos de inclusão e exclusão, como na interface do usuário

<b>Corrigido</b>:

&#x200B;* [Falha]&#x200B;[Configurações de mapas de malha] Aplicar configurações a outros conjuntos de textura
&#x200B;* [Crash] Ao assar a curvatura do mapa sem espaço mundial normal
&#x200B;* [Falha]&#x200B;[Preparação] Cozimento com caixa personalizada ativada, mas nenhum arquivo selecionado falha
&#x200B;* [Falha] Cancelando cozimento de AO
&#x200B;* [Caixa automática] Carga infinita quando o caminho de arquivo poli alto é inválido
&#x200B;* [Linux]&#x200B;[Windows] O seletor de cores às vezes pode ser totalmente preto ou não aparecer
&#x200B;* [Ferramenta Preenchimento de polígono] A ferramenta não funciona com fontes não PBR
&#x200B;* &lbrack;[Paint] Excluir canal de cor base não exclui a cor pintada anteriormente
&#x200B;* [USD] Nem todas as instâncias do sombreador foram detectadas corretamente
&#x200B;* [Substance] Somente o primeiro uso de um nó de entrada/saída é levado em consideração
&#x200B;* [Shader] A Oclusão ambiente é aplicada duas vezes com conjuntos de texturas usando diferentes métodos de mistura
&#x200B;* [Engine] Texturas normais com canal azul vazio (preto) podem levar a resultados incorretos de mesclagem
&#x200B;* [Importação de GLTF] a mesclagem de Alpha está ativada em todos os conjuntos de texturas
&#x200B;* [Exportação GLTF] A mesclagem de Alpha é sempre ativada na exportação
&#x200B;* [Exportar] A geometria de dupla face é sempre desativada ao importar um arquivo GLTF
&#x200B;* [Javascript] A modificação das configurações de sombreadores não contribui para o histórico de desfazer
&#x200B;* [Amostras] A dispersão da subsuperfície não está ativada nas configurações de exibição do fosco de reunião

### 12.0.3

Data de lançamento: **5/2026**

Resumo: **Versão secundária**

**Adicionado:**

&#x200B;* Atualize os padeiros para a versão 3.22.2
&#x200B;* Atualize o mecanismo de Substance para a versão 9.4.3
&#x200B;* \[Python\] Salvar um material inteligente em um local específico

**Corrigido:**

&#x200B;* \[Ubuntu\] Falha ao selecionar o material
&#x200B;* \[Mac\] A janela pop-up recorrente aparece para solicitar acesso a dados de outros aplicativos
&#x200B;* \[Preparação\] Artefatos podem aparecer no mapa de curvatura
&#x200B;* \[Preparação\] Preparação é mais lenta em alguns casos
&#x200B;* \[Distorcer para geometria\] Distorcer para geometria é desativado em alguns casos
&#x200B;* \[Bloco UV\] Alfa extraído do ponto de ancoragem ignorado por outros blocos
&#x200B;* \[Python\]\[Mac\] Exceções no console Python com SSL
&#x200B;* \[Python\] Painter falha ao sair com widgets Qt restantes

### 12.0.2

Data de lançamento: **04/2026/07**

Resumo: **Versão secundária**

**Adicionado:**

&#x200B;* [Gerenciamento de cores] Adicione novo OCIO para especificar o espaço de cores padrão do seletor de cores
&#x200B;* [Python] Expor configurações de desajuste automático na API Python

**Corrigido:**

&#x200B;* [Falha] Salvar com espaço em disco insuficiente pode travar ou corromper projetos
&#x200B;* [Falha] [Faixa de opções] O uso da faixa de opções pode causar falhas para alguns projetos
&#x200B;* [Falha] [Backup] falha quando o arquivo .assbin não pode ser gravado na pasta
&#x200B;* [Importar] Malhas OBJ do Stager podem falhar na criação do projeto
&#x200B;* [Importar] O OBJ está sem rosto em alguns casos
&#x200B;* [Import] A malha do USD sem nenhum material atribuído pode falhar na importação
&#x200B;* [Caminho preenchido] Não afetado pela simetria
&#x200B;* A visualização [Estêncil] tem resolução menor do que o resultado pintado
&#x200B;* [UI] “ilha uv” ainda é mencionada na dica de ferramenta de origem de cores do mapa de ID
&#x200B;* [Tela] As sombras aparecem invertidas
&#x200B;* [Visor] A transformação da projeção de distorção permanece após alternar para o modo de cozimento
&#x200B;* [Distorcer] A grade desaparece quando a escala é definida como 0 no eixo Z com a opção Distorcer para geometria ativada
&#x200B;* [Python] Erro inesperado ao adicionar um canal com modificação no escopo

### 12.0.1

Data de lançamento: **03/2026/18**

Resumo: **Versão secundária**

**Corrigido:**

&#x200B;* \[Falha\]\[Congelar\] Exportar de projetos específicos

### 12.0.0

Data de lançamento: <b>03/2026/09</b>
Resumo: <b>Esta é uma versão principal. Esta versão contém os recursos de camadas achatadas, distorção na geometria, novos pós-efeitos, melhoria na janela do novo projeto e outras melhorias.</b>

<b>Adicionado</b>:

&#x200B;* [Achatar camadas] Achatar camadas dentro da pilha de camadas
&#x200B;* [Achatar camadas] Exportar camadas achatadas para disco
&#x200B;* [Distorcer para geometria] Adicionar nova funcionalidade de distorção automática a Projeções de distorção
&#x200B;* [Pós-efeitos] Substituir pós-efeitos pela adição de novos
&#x200B;* [Pós-efeitos] Atualizar mapeador de tom
&#x200B;* [Pós-efeitos] Adicionar novo uso para ativos de Pós-efeitos
&#x200B;* [Conteúdo]&#x200B;[Pós-efeitos] Integrar ativos de pós-efeitos padrão na biblioteca
&#x200B;* [Novo projeto] Aprimorar a interface do usuário para criação de projetos
&#x200B;* [Novo projeto] Alterações na funcionalidade de malha de reimportação
&#x200B;* [Novo projeto] Permitir que arquivos \*.geo.usd sejam abertos
&#x200B;* [Configuração do projeto] Melhorar a interface do usuário para a configuração do projeto
&#x200B;* Atualize a biblioteca do USD para a versão 25.05
&#x200B;* Atualize o Substance Engine para a versão 9.3.4
&#x200B;* Aumente o mínimo de drivers para 25.3.1/25.Q2 para GPUs AMD
&#x200B;* Atualize o Qt para 6. 8. 6
&#x200B;* [Script] Atualize a API JavaScript para a versão 1.1.20
&#x200B;* Atualizar Python para a versão 3.13

<b>Corrigido:</b>

&#x200B;* [Falha] Alterar uma saída de canal de material em uma máscara pode falhar
&#x200B;* [Import] As texturas EXR são forçadas para sRGB em vez de lineares ao importar arquivos USD
&#x200B;* [Blocos UV] A sequência de imagens com uma única imagem também preenche outros blocos UV
&#x200B;* [Preparação] O AO é diferente entre a CPU e a preparação de GPU
&#x200B;* [Gerenciamento de cores]&#x200B;[MacOS] Viewport BaseColor não corresponde ao selecionador de cores
&#x200B;* [USD] Valores uniformes não são importados em alguns casos

## Versão 11

### 11.1.3

Data de lançamento: <b>2026/02/12</b>
Resumo: <b>Versão secundária</b>

<b>Corrigido</b>:

&#x200B;* [Pintura] O estêncil e a simetria não funcionam em alguns casos
&#x200B;* [Caminho] Nenhuma atualização ao alterar o controle deslizante de opacidade do traçado de borrar
&#x200B;* [Projeto] Não é possível pintar em alguma geometria
&#x200B;* [Ribbon] O caminho instanciado desaparece ao alterar a resolução do Conjunto de Texturas
&#x200B;* [IU] O seletor de cores pode diminuir e desaparecer em alguns casos

### 11.1.2

Data de lançamento: <b>1/2026/13</b>
Resumo: <b>Versão secundária</b>

<b>Adicionado</b>:

&#x200B;* [Preparação] Melhorar o tempo de cozimento para projetos de blocos UV com salvamento assíncrono
&#x200B;* [Shaders] Menção nas alterações do API de sombreamentoLog após a migração Vulkan
&#x200B;* Atualizar OpenEXR para a versão 3.4.4

<b>Corrigido</b>:

&#x200B;* [Falha] Falha durante a inicialização na série Nvidia GTX 10xx
&#x200B;* [Falha] Usar o seletor de cores em diferentes conjuntos de texturas pode resultar em uma falha ao sair do aplicativo
&#x200B;* [Desempenho] Problema de desempenho ao pintar em um projeto com muitas camadas
&#x200B;* [Desempenho] Atraso ao pintar com caneta eletrônica gráfica
&#x200B;* [UI] As configurações da câmera permanecem desativadas no modo de renderização (Iray)
&#x200B;* [Ribbon] O caminho pode se sobrepor inesperadamente após um canto em alguns casos
&#x200B;* [Ribbon] Problema de desempenho com blocos UV
&#x200B;* [Substance]&#x200B;[IU] As entradas de imagem desaparecem quando recolhidas
&#x200B;* [Substance]&#x200B;[IU] Os grupos aninhados podem permanecer mesmo se visíveis, se forem ocultados
&#x200B;* [Cozimento]&#x200B;[IU] Não é possível definir o raio de amostragem da curvatura além de 0,01
&#x200B;* [Preparação]&#x200B;[IU] Não é possível definir a Distância máxima do oclusor além de 1
&#x200B;* [Preparação] A configuração “Auto-oclusão” do AO é ignorada com vários conjuntos de textura e baixa como cozimento alto
&#x200B;* [Preparação] O mapa de IDs não cria cores de vértice do FBX no modo Baixo como Alto
&#x200B;* [Content] O filtro Highpass resulta em cores desbotadas em canais com gerenciamento de cores

### 11.1.1

Data de lançamento: <b>2025/12/09</b>
Resumo: <b>Versão secundária</b>

<b>Adicionado</b>:

&#x200B;* [Desempenho] Melhorar o desempenho dos Blocos UV ao computar texturas parciais
&#x200B;* [Baker] Atualização para a versão 3.15.4

<b>Corrigido</b>:

&#x200B;* [Falha]&#x200B;[MacOS] Salvar projeto de versões anteriores sempre falha
&#x200B;* [Falha] Fechar um projeto às vezes pode resultar em uma falha
&#x200B;* [Project] Erro “incompatibilidade de contagem de membros” ao abrir projeto feito em versão anterior
&#x200B;* [Fazendo bake] Blocos UV não são combinados com resultados de fazes bake anteriores, se presentes
&#x200B;* [Fazendo bake] Dispositivo perdido mesmo com Rastreamento de raios desativado na série Nvidia GTX 10XX
&#x200B;* [Fazer bake] O AO com normal tem artefatos nas bordas porque não há preenchimento
&#x200B;* [Fazendo bake] A configuração “Auto-oclusão” do AO é ignorada com vários conjuntos de texturas e “corresponder pelo nome” na
&#x200B;* [Fazendo bake] O mapa de ID será totalmente preto se alguma malha de alto polígono não tiver cores de vértice
&#x200B;* [Faixa de opções] A dica de ferramenta para o modo de mesclagem Alfa menciona o modo de mesclagem de Tela em vez do Subexposição linear
&#x200B;* [Path] As tangentes criam um loop inesperado quando o ponto é movido próximo das extremidades do caminho
&#x200B;* [Ferramenta] A visualização de material não funciona quando a projeção é usada em uma máscara
&#x200B;* [Engine] Pintar traçados pequenos pode resultar em artefatos de blocos
&#x200B;* [Sombreador] Desfazer a criação da instância de sombreamento não a remove corretamente
&#x200B;* [Export] O modo Alpha para exportação de GLTF é sempre definido como MASK
&#x200B;* [Python] Erro inesperado ao editar a pilha de camadas fora do bloco de modificação com escopo

<b>Problemas Conhecidos</b>:

&#x200B;* [Ribbon] Problema de desempenho com Blocos UV
&#x200B;* [Ribbon] O caminho pode se sobrepor inesperadamente após um canto em alguns casos
&#x200B;* [Falha]&#x200B;[Faixa de opções] Criar textos muito longos na Faixa de opções pode falhar
&#x200B;* [Gerenciamento de cores] As conversões do espaço de cores HDR com ACE no Linux produzem cores vivas
&#x200B;* [Regression]&#x200B;[UI] O menu do botão direito do mouse é muito pequeno em telas HD
&#x200B;* [Crash]&#x200B;[Python] Exportação de USD acionada por TextureStateEvent
&#x200B;* [Engine] Pintar com a ferramenta Clonar em cores normais de deslocamento de canal incorretamente
&#x200B;* [Python] O widget fantasma aparece excluído pelo script ainda em funcionamento

### 11.1.0

Data de lançamento: <b>2025/11/18</b>
Resumo: <b>Esta atualização é uma versão importante. Ela contém a nova ferramenta Ribbon com novo conteúdo dedicado, suporte de simetria para camadas de preenchimento, parâmetro de tamanho físico para deslocamento, desempenho aprimorado por meio de padarias atualizadas, suporte completo a Vulkan para Windows e Linux e outras melhorias.</b>

<b>Adicionado</b>:

&#x200B;* Nova ferramenta da faixa de opções
&#x200B;* [Ferramenta] Adicionar nova ferramenta Faixa de opções para criar caminhos perfeitos
&#x200B;* [Faixa de opções] Adicionar atalhos predefinidos da Faixa de opções na janela Propriedades
&#x200B;* [Ribbon] Permite alterar a opacidade da Faixa de Opções por vértice no caminho
&#x200B;* [Ribbon] Permite alterar o tamanho da Faixa de Opções por vértice no caminho
&#x200B;* [Ribbon] Remover o início/fim definido em um Substance quando os caminhos são fechados
&#x200B;* [Ribbon] Remover visualização Caminho/Material na janela de propriedades das ferramentas Pintar/Borracha/Borrar caminho
&#x200B;* [Faixa de opções] Adicione modos de mesclagem para o alfa e alguns canais quando houver autosobreposição
&#x200B;* Simetria de preenchimento
&#x200B;* [Preenchimento] Adicionar suporte para simetria em camadas e efeitos de preenchimento
&#x200B;* [Fill]&#x200B;[UI] Expor configurações de simetria na janela de propriedades para camada de preenchimento e efeitos
&#x200B;* [Fill] Reprocessar a interface de configurações de simetria no menu do visor e na janela de propriedades
&#x200B;* [Fill] Reorientar adequadamente texturas normais ao projetar no modo de distorção
&#x200B;* deslocamento do tamanho físico
&#x200B;* [Deslocamento] Usar o tamanho físico como unidade de deslocamento
&#x200B;* Melhoria de desempenho
&#x200B;* [Desempenho] Melhorar a renderização de pequenos traçados de pincel em triângulos grandes
&#x200B;* [Desempenho] Melhorar o tempo de compilação do Sombreador
&#x200B;* [Performance] Suporte completo à Vulkan para Windows e Linux
&#x200B;* [Desempenho] Padeiros atualizados com renderização mais rápida de GPU e suporte a rastreamento de raios AMD
&#x200B;* [UI] Reorganizar propriedades de ferramentas em grupos e recolher algumas por padrão
&#x200B;* [Engine] Atualização do Substance Engine para a versão 9.2.5
&#x200B;* [Substance] Expor a substituição de resolução para recursos Substance em Ferramentas e Preenchimentos
&#x200B;* [Exportar] Atualizar predefinição de exportação de Mapas de malha para exportar texturas em tons de cinza
&#x200B;* Python
&#x200B;* [Panificação]&#x200B;[Python] Indicar em changelog mudanças de quebra após atualização de padeiros
&#x200B;* [Python] Expor as configurações de simetria de preenchimento no Python
&#x200B;* Conteúdo e novo conteúdo
&#x200B;* [Conteúdo] Adicione 75 novas predefinições de ferramenta para a ferramenta Faixa de opções
&#x200B;* [Conteúdo] Atualize o recurso construtor de gradientes para que seja compatível com a Faixa de opções

<b>Corrigido</b>:

&#x200B;* [Falha] Carregar outro projeto enquanto o encaixe de caminho está ativado pode falhar
&#x200B;* [Falha] Clicar com o botão direito do mouse no painel Caminho com informações de outra sessão na área de transferência pode travar
&#x200B;* [UI] A interface rola para cima nas propriedades da ferramenta ao criar um caminho
&#x200B;* [UI] O cursor do mouse desaparece quando a visualização do visor do caminho está oculta
&#x200B;* [Caminho] Copiar/colar diferentes propriedades da ferramenta no painel Caminho leva a propriedades instáveis
&#x200B;* [Ferramenta] As predefinições da ferramenta Borrar nem sempre atualizam a seleção de canal
&#x200B;* [Ferramenta] O valor pintado é cinza, mas a interface do usuário mostra branco após carregar a predefinição de ferramenta colorida na máscara
&#x200B;* [Ferramenta] A predefinição criada a partir da máscara mantém os valores de canais carregados de outra predefinição
&#x200B;* [Substance] A substituição do espaço da cor normal definida no gráfico não é levada em consideração
&#x200B;* [Content] O recurso de forma de pincel padrão usa um Substance desatualizado

<b>Problemas Conhecidos</b>:

&#x200B;* O histórico da instância do sombreador não foi rastreado corretamente
&#x200B;* [Ribbon] Problema de desempenho com Blocos UV
&#x200B;* [Ribbon] O caminho pode se sobrepor inesperadamente após um canto em alguns casos
&#x200B;* [Ribbon] As tangentes criam um loop indesejado quando o ponto é movido próximo das extremidades do caminho
&#x200B;* [Falha]&#x200B;[Faixa de opções] Criar textos muito longos na Faixa de opções pode falhar
&#x200B;* [Ferramenta] A visualização de material não funciona quando a projeção é usada em uma máscara
&#x200B;* [Fazendo bake] A configuração “Auto-oclusão” do AO é ignorada com vários conjuntos de texturas e a opção “corresponder pelo nome” ativada
&#x200B;* [Fazendo bake] O AO com normal tem artefatos nas bordas devido à falta de preenchimento
&#x200B;* [Gerenciamento de cores] As conversões do espaço de cores HDR com ACE no Linux produzem cores apertadas
&#x200B;* [Regression]&#x200B;[UI] O menu do botão direito do mouse é muito pequeno em telas HD
&#x200B;* [Crash]&#x200B;[Python] Exportação de USD acionada por TextureStateEvent
&#x200B;* [Engine] A pintura com a ferramenta Clonar nas cores normais de mudança de canal é incorreta
&#x200B;* [Python] O widget fantasma aparece excluído pelo script ainda em funcionamento

### 11.0.3

Data de lançamento: <b>08/2025/05</b>
Resumo: <b>Versão secundária</b>

<b>Adicionado</b>:

&#x200B;* [Substance 3D Assets] Adicionar um ponto de notificação ao painel Ativos 3D
&#x200B;* [VFX Platform 2025] Adicionar a configuração ACE 2.0 nas configurações de gerenciamento de cores
&#x200B;* [VFX Platform 2025] Atualize o OCIO para a versão 2.4.2
&#x200B;* Atualize o Iray para a versão 2024.10
&#x200B;* [Engine] Atualização para o Substance Engine v.9.2.3
&#x200B;* [Nvidia] Aumente a versão mínima dos drivers Nvidia para 572.60 (Win) e 570.169 (Linux)

<b>Corrigido</b>:

&#x200B;* [Python] A modificação com escopo não aparece na janela Histórico

<b>Problemas Conhecidos</b>:

&#x200B;* [Gerenciamento de cores] As conversões do espaço de cores HDR com ACE no Linux produzem cores apertadas
&#x200B;* [Regression]&#x200B;[UI] O menu do botão direito do mouse é muito pequeno em telas HD
&#x200B;* [Crash]&#x200B;[Python] Exportação de USD acionada por TextureStateEvent
&#x200B;* [Engine] Pintar com a ferramenta Clonar em cores normais de deslocamento de canal incorretamente
&#x200B;* [Python] O widget fantasma aparece excluído pelo script ainda em funcionamento

### 11.0.2

Data de lançamento: <b>6/2025/10</b>
Resumo: <b>Versão secundária</b>

<b>Adicionado</b>:

&#x200B;* [Mac] Adicionar aviso sobre a versão específica do sistema operacional levando a artefatos
&#x200B;* [Atualização automática] Pequenas melhorias de UX no log de erros de Ativos
&#x200B;* [Desempacotamento automático] Atualize para a versão 1.3.2 com melhorias de costura
&#x200B;* [USD]&#x200B;[FBX] Adicionar suporte para vários conjuntos UV com dados esparsos
&#x200B;* [Exportar] Malhas exportadas como FBX não têm seus conjuntos UV adicionais se algum estava presente na importação

<b>Corrigido</b>:

&#x200B;* [MacOS]&#x200B;[Linux] Falha ao salvar na unidade de rede
&#x200B;* [Win]&#x200B;[Tablet] Cintilação ao deslocar
&#x200B;* [SpaceMouse] Problema ao trabalhar com a ferramenta Caminho
&#x200B;* [Caixa automática] Não é possível assar após um recarregamento de malha
&#x200B;* [Atualização automática] A sequência de imagens não é recarregada quando o primeiro bloco está ausente
&#x200B;* [Caminho] A tangente personalizada pode afetar outra tangente
&#x200B;* [Caminho] O caminho não aparecerá no Conjunto de textura se o primeiro ponto estiver em outro Conjunto de textura
&#x200B;* [IU] Alguns menus são sempre desativados após a abertura de um projeto (por exemplo, simetria)
&#x200B;* [Propriedades] Não é possível usar/carregar predefinições de ferramenta com a ferramenta Caminho preenchido
&#x200B;* [USD] Vários conjuntos UV não são reconhecidos no sombreador personalizado ao usar arquivos USD
&#x200B;* [USD] Câmeras com os mesmos nomes são substituídas
&#x200B;* [Exportar] Enviar para o Photoshop resulta em espaço de cor incorreto para resultados em cores e em tons de cinza
&#x200B;* [Exportar] Os canais em tons de cinza com alfa são exportados como cores em vez de tons de cinza com formato PNG
&#x200B;* [Exportar] Exportar canal em tons de cinza como PSD em arquivo inválido/truncado
&#x200B;* [Conteúdo] O filtro de distorção no modo multidirecional não funciona
&#x200B;* [Python] Não é possível alocar o erro de lista ao rastrear nós de pilha de camadas

<b>Problemas Conhecidos</b>:

&#x200B;* [Gerenciamento de cores] As conversões do espaço de cores HDR com ACE no Linux produzem cores apertadas
&#x200B;* [Regression]&#x200B;[UI] O menu do botão direito do mouse é muito pequeno em telas HD
&#x200B;* [Crash]&#x200B;[Python] Exportação de USD acionada por TextureStateEvent
&#x200B;* [Engine] A pintura com a ferramenta Clonar nas cores normais de mudança de canal é incorreta
&#x200B;* [Python] O widget fantasma aparece excluído pelo script ainda em funcionamento

### 11.0.1

Data de lançamento: <b>4/2025/10</b>
Resumo: <b>Versão secundária</b>

Observação: a versão do CCD do <b>Linux será adiada até 29 de abril</b>

<b>Adicionado:</b>

&#x200B;* Atualize para Qt 6.5.8
&#x200B;* [Substance] Adicionar mensagem de log para filtros quando várias entradas de imagem compartilham o mesmo uso
&#x200B;* [Nvidia] Adicionar aviso sobre os drivers Nvidia mais recentes (572.47)

<b>Corrigido:</b>

&#x200B;* [Falha] Ao arrastar e soltar um sbsar com uso em slots de canal único
&#x200B;* [Falha]&#x200B;[Caminho] A opção Alterar tipo de caminho não fica acinzentada quando você não clica em um caminho específico
&#x200B;* [Preencher caminho] Não deve ser capaz de selecionar o material do substance
&#x200B;* [Engine] Artefatos ao longo de pinceladas
&#x200B;* [Engine] Os caminhos podem ser quebrados com configurações específicas
&#x200B;* Problema com o menu suspenso para o espaço da cor do conta-gotas
&#x200B;* [Atualização automática] [Python] Mensagem de erro incorreta ao usar ResourceID sem versão
&#x200B;* [Shader] Falha ao abrir alguns projetos

<b>Problemas Conhecidos:</b>

&#x200B;* [SpaceMouse] Problema ao trabalhar com a ferramenta Caminho
&#x200B;* [Gerenciamento de cores] As conversões do espaço de cores HDR com ACE no Linux produzem cores vivas
&#x200B;* [Regression]&#x200B;[UI] O menu do botão direito do mouse é muito pequeno em telas HD
&#x200B;* [Crash]&#x200B;[Python] Exportação de USD acionada por TextureStateEvent
&#x200B;* [Engine] Pintar com a ferramenta Clonar em cores normais de deslocamento de canal incorretamente
&#x200B;* [Python] O widget fantasma aparece excluído pelo script ainda em funcionamento

### 11.0.0

Data de lançamento: <b>3/2025/11</b>
Resumo: <b>Versão principal, novo recurso de atualização automática, ferramenta de caminho preenchido e outras melhorias de caminho, bem como novos filtros e uma geração experimental de gaiola automática para cozimento</b>

<b>Adicionado</b>:

&#x200B;* Atualização automática
&#x200B;* [Atualização automática] Atualizar automaticamente os ativos modificados no painel Ativos
&#x200B;* [Atualização automática] Atualizar automaticamente os ativos modificados em todo o projeto
&#x200B;* [Atualização automática] Manter a atualização automática desativada por padrão
&#x200B;* [Atualização automática] Tornar a atualização opcional se os parâmetros de recurso não corresponderem (.sbsar, .glsl, .ai, .svg)
&#x200B;* [Atualização automática] Adicionar variável de ambiente para desativar o recurso de atualização automática
&#x200B;* [Atualização automática]&#x200B;[SBSAR] Tornar a atualização opcional se os parâmetros de recurso não corresponderem
&#x200B;* Caminho preenchido
&#x200B;* [Caminho]&#x200B;[Preenchimento] Adiciona nova ferramenta para criar caminhos preenchidos
&#x200B;* Melhorias de caminho
&#x200B;* [Caminho] Criar um caminho que se ajusta aos polígonos
&#x200B;* [Caminho] Permite alternar tipos de caminho
&#x200B;* [Caminho] Permite copiar e colar dados de vértice de caminho entre conteúdo e máscara
&#x200B;* [Caminho] Permite restringir o ângulo ao criar um novo ponto
&#x200B;* [Caminho] Permite restringir a criação de pontos a uma linha
&#x200B;* [Caminho] Feche a forma com um único clique
&#x200B;* [Caminho] Exibir informações de caminho
&#x200B;* [Caminho] Permite dimensionar e girar vértices de caminho
&#x200B;* [Path]&#x200B;[UX] Facilitar o acesso aos gizmos de transformação
&#x200B;* [Caminho] Adicionar visualização de caminho
&#x200B;* [Caminho] Desativar a visualização do caminho com Shift + P
&#x200B;* [Caminho] Melhorar a edição da tangente da vista lateral
&#x200B;* [Caminho] Permitir foco em um caminho 3D
&#x200B;* [Caminho] Os vértices devem manter o status da seleção ao ativar e desativar a interface novamente
&#x200B;* [Caminho] Permite excluir o caminho usando Backspace
&#x200B;* [Caminho] Mantém a lista de caminhos aberta se o usuário a expandir
&#x200B;* [Caminho]&#x200B;[Pilha de camadas] Renomear duplicatas corretamente ao copiar/colar
&#x200B;* Melhorias na interface do usuário [Caminho] e nas dicas de ferramenta
&#x200B;* Desempenho
&#x200B;* [Desempenho] Aprimorar o desempenho do visor ao usar um alto nível de mosaico
&#x200B;* [Desempenho] Habilita somente o primeiro canal em novas camadas/efeitos de preenchimento
&#x200B;* [Desempenho] Paralelizar o cálculo do traçado do pincel
&#x200B;* Baking
&#x200B;* [Cozimento] Adicione uma nova opção de geração de gaiola totalmente automática para assar com malhas de alto polietileno (experimental)
&#x200B;* Conteúdo
&#x200B;* [Conteúdo] Adicione 6 novos filtros: estilização, quantize, kuwahara anisotrópico, suavização de chanfro, distância direcional, conversão em tons de cinza
&#x200B;* [Conteúdo] Atualize Noises and Grunges para a versão mais recente do Designer (com o novo 2D Voronoi)
&#x200B;* [Content] Adicione 3 novos geradores de textura (Tile Random, Triangle Grid, Scratches Generator)
&#x200B;* [Conteúdo] Renomear modelo do Unreal Engine e exportar predefinições
&#x200B;* Python
&#x200B;* [Shelf]&#x200B;[Python] Salvar material inteligente ou máscara inteligente em disco do Python
&#x200B;* [Python] Adicionar gaiola automática de cozimento à API do Python
&#x200B;* [Python] Permitir a edição de nomes e descrições de Conjuntos de texturas/Blocos UV
&#x200B;* [Python] Compartilhar configurações de resolução em fontes vetoriais e de fonte
&#x200B;* [Atualização automática]&#x200B;[Python] Expor as funcionalidades de atualização automática do projeto no Python
&#x200B;* Diversos
&#x200B;* [Exportar] Facilite o acesso às opções de Enviar para com um novo painel
&#x200B;* [Nvidia] Adicionar aviso sobre os drivers Nvidia mais recentes (572.16)
&#x200B;* O encaixe de ângulo deve ser afetado pela seleção de espaço Objeto/Mundo
&#x200B;* [Lista de conjuntos de texturas] Permite adicionar um nome personalizado aos blocos UV e usá-los na exportação
&#x200B;* Mac
&#x200B;* [Mac] Usar Metal em vez de OpenGL para renderização de gráficos
&#x200B;* [Mac] Soltar o suporte ao Mac Intel

<b>Corrigido</b>:

&#x200B;* [Falha] Excluir entrada de imagem
&#x200B;* Não é possível adicionar o Smart Mat pelo botão de pilha de camadas
&#x200B;* [Python] Efeitos no GroupLayerNode não podem ser encontrados

<b>Problemas Conhecidos</b>:

&#x200B;* [Gerenciamento de cores] As conversões do espaço de cores HDR com ACE no Linux produzem cores vivas
&#x200B;* [Regression]&#x200B;[UI] O menu do botão direito do mouse é muito pequeno em telas HD
&#x200B;* [Crash]&#x200B;[Python] Exportação de USD acionada por TextureStateEvent
&#x200B;* [MacOS Intel] Falha ao importar algumas predefinições
&#x200B;* [Engine] Pintar com a ferramenta Clonar em cores normais de deslocamento de canal incorretamente
&#x200B;* [Python] O widget fantasma aparece excluído pelo script ainda em funcionamento
&#x200B;* [RedHat] Problemas no seletor de cores

## Versão 10

### 10.1.2

Data de lançamento: <b>2024/12/3</b>
Resumo: <b>Versão secundária, correções de erros</b>

<b>Corrigido</b>:

&#x200B;* [Falha] Excluir entrada de imagem
&#x200B;* Não é possível adicionar o smart mat através do botão pilha de camadas
&#x200B;* [Python] Efeitos no GroupLayerNode não podem ser encontrados

<b>Problemas Conhecidos</b>:

&#x200B;* [Gerenciamento de cores] As conversões do espaço de cores HDR com ACE no Linux produzem cores apertadas
&#x200B;* [Regression]&#x200B;[UI] O menu do botão direito do mouse é muito pequeno em telas HD
&#x200B;* [Crash]&#x200B;[Python] Exportação de USD acionada por TextureStateEvent
&#x200B;* [MacOS Intel] Falha ao importar algumas predefinições
&#x200B;* [Engine] A pintura com a ferramenta Clonar nas cores normais de mudança de canal é incorreta
&#x200B;* [Python] O widget fantasma aparece excluído pelo script ainda em funcionamento
&#x200B;* [RedHat] Problemas no seletor de cores

### 10.1.1

Data de lançamento: <b>2024/11/5</b>
Resumo: <b>Versão secundária, correções de erros</b>

<b>Adicionado</b>:

&#x200B;* [Project] Mantém o projeto atual aberto até que a seleção do novo projeto seja validada
&#x200B;* [Contornar automaticamente] A densidade do texel permite dividir melhor as Ilhas UV em UDIMs
&#x200B;* [Fazendo bake] Corrigir cópia ambígua no menu contextual de Mapas de Malha
&#x200B;* [Distorcer] Remover dimensionamento na viewport para o eixo Z (profundidade)
&#x200B;* [Importação/exportação] Remova o suporte a formatos de arquivo de imagem não utilizados
&#x200B;* Atualizar Substance Engine para 9.1.4

<b>Corrigido</b>:

&#x200B;* [Falha] Depois de realocar o recurso no Assets e salvar o projeto
&#x200B;* [Falha] Problemas com a biblioteca do servidor
&#x200B;* [Falha] Falha no servidor Illustrator em alguns casos raros
&#x200B;* [Falha] Ao sair do aplicativo em alguns casos raros
&#x200B;* Não é possível enviar relatórios de falhas em alguns computadores
&#x200B;* [Fazendo bake] A cor do vértice não é lida corretamente
&#x200B;* [IU] O local do Windows e das novidades na inicialização foi alterado
&#x200B;* [Assimp] A StandardSurface do Maya não é reconhecida no fça bake de ID
&#x200B;* [Python] A biblioteca SSL ausente gera um erro
&#x200B;* [Python]&#x200B;[Win] Erro ao chamar QColorConstants.Transparent
&#x200B;* [Python] As miniaturas de camadas criadas por meio do Python não são atualizadas até clicar dentro da pilha de camadas
&#x200B;* [Shader] Link quebrado no API de sombreamento changelog
&#x200B;* [Ativos 3D] Use as configurações de proxy do sistema operacional ao acessar Ativos 3D

<b>Problemas Conhecidos</b>:

&#x200B;* [Gerenciamento de cores] As conversões do espaço de cores HDR com ACE no Linux produzem cores vivas
&#x200B;* [Regressão]&#x200B;[IU] O menu do botão direito do mouse é muito pequeno em telas HD
&#x200B;* [Crash]&#x200B;[Python] Exportação de USD acionada por TextureStateEvent
&#x200B;* [MacOS Intel] Falha ao importar algumas predefinições
&#x200B;* [Engine] Pintar com a ferramenta Clonar em cores normais de deslocamento de canal incorretamente
&#x200B;* [Python] O widget que parece ser excluído por meio do script ainda está funcionando
&#x200B;* [RedHat] Problemas no seletor de cores

### 10.1.0

Data de lançamento: <b>9/2024/17</b>
Resumo: <b>Versão principal, conteúdo novo: máscara de área de preenchimento/filtro de cores, filtro de decalque de bordado e seis filtros de Substance genéricos, importação de USD com propriedades de material e sombreador, melhoria de desempenho, compatibilidade com a plataforma VFX 2024 e migração para Linux RedHat</b>

<b>Adicionado</b>:

&#x200B;* [Conteúdo] Adicionar novo filtro de máscara/cor da área de preenchimento
&#x200B;* [Conteúdo] Adicionar novo filtro de decalque de bordado
&#x200B;* [Conteúdo] Adicione 6 novos filtros de Substance genéricos (FXAA, pixelate, highpass, posterize, smoothstep, threshold)
&#x200B;* [USD] Exportar camada USD com um material ASM definido
&#x200B;* [USD] Importar USD com propriedades de material e sombreador
&#x200B;* [Desempenho] Ativar miniaturas otimizadas de pilha de camadas por padrão
&#x200B;* [Desempenho] Reduzir o tempo de abertura do arquivo de projeto e o consumo de memória (decodificação de dados)
&#x200B;* Compatível com a plataforma VFX 2024
&#x200B;* [VFX Platform 2024] Atualização para Python 3.11
&#x200B;* [VFX Platform 2024] Atualização para OpenEXR 3.2
&#x200B;* [VFX Platform 2024] [USD] Atualização do OpenSubdiv 3.6.0
&#x200B;* [VFX Platform 2024]&#x200B;[Gerenciamento de cores] Atualização para OCIO 2.3.2
&#x200B;* [Linux] Migração para o Linux RedHat
&#x200B;* [Linux] Atualize a versão mínima do driver Nvidia para 535.171.04
&#x200B;* [Importar] Adicionar uma opção para inverter o mapa normal ao importar uma malha GLTF
&#x200B;* [UI] Usar o valor padrão do sistema operacional para a distância de detecção de eventos de arrastar
&#x200B;* [Substance Engine] Adicionar função de faixa de chamada para remover os símbolos do executável
&#x200B;* [Tela inicial] Atualização para o novo formato de tela inicial
&#x200B;* Atualize o Substance Engine para a versão 9.1.3
&#x200B;* [Python] Mostrar link para exemplos no menu de documentação da pilha de camadas
&#x200B;* [JavaScript] Mover plug-ins Javascript para a subpasta javascript/plugins

<b>Corrigido</b>:

&#x200B;* [Illustrator] Falha ao exportar um bloco UV com gráfico .ai em casos específicos
&#x200B;* [Traçados dinâmicos]&#x200B;[Caminho] O aleatório por traçado não funciona em um caminho
&#x200B;* [UI]&#x200B;[Propriedades] O bloqueio é habilitado quando a divisão em blocos gráficos não é uniforme
&#x200B;* O arquivo TXT de depuração é criado ao clicar duas vezes no projeto do Painter
&#x200B;* [USD]&#x200B;[Export] Algumas texturas podem estar ausentes
&#x200B;* [ASM] O canal de dispersão de cores ignora metais
&#x200B;* [Conteúdo] O filtro de desfoque não funciona no espaço de cores “trabalho”
&#x200B;* [Conteúdo] O filtro Ajustar Height também modifica o alfa da camada

<b>Problemas Conhecidos</b>:

&#x200B;* [Gerenciamento de cores] As conversões do espaço de cores HDR com ACE no Linux produzem cores vivas
&#x200B;* [Win]&#x200B;[Crash] [ACE] Não usar espaço da cor sRGB ICE para transformação de exibição
&#x200B;* [Regression]&#x200B;[UI] O menu do botão direito do mouse é muito pequeno em telas HD
&#x200B;* [Crash]&#x200B;[Python] Exportação de USD acionada por TextureStateEvent
&#x200B;* [MacOS Intel] Falha ao importar algumas predefinições
&#x200B;* [Falha] Realocar recurso e salvar projeto
&#x200B;* [Engine] Pintar com a ferramenta Clonar em cores normais de deslocamento de canal incorretamente
&#x200B;* [Python] O widget fantasma aparece excluído pelo script ainda em funcionamento
&#x200B;* [RedHat] Problemas no seletor de cores

### 10.0.1

Data de lançamento: <b>6/2024/11</b>
Resumo: <b>Versão secundária, correções de erros</b>

<b>Adicionado:</b>

&#x200B;* [Biblioteca] Converter fontes de Substance em arquivos de fonte comuns
&#x200B;* [Illustrator]&#x200B;[SVG] Dá às miniaturas na seleção de escopo um fundo cinza claro
&#x200B;* [Python] Adicionar função na origem do bitmap para listar os espaços de cores disponíveis

<b>Corrigido</b>:

&#x200B;* [Pilha de camadas] Pasta sempre fechada quando movida para dentro ou para fora de outras pastas
&#x200B;* [Salvar] O arquivo de projeto é perdido ao “salvar como cópia” ou o salvamento automático falha em casos específicos
&#x200B;* [Import] Ativos com o mesmo nome, mas extensões diferentes, são substituídos
&#x200B;* [Propriedades] Configurações ausentes ao usar o ponto de ancoragem nas entradas da imagem
&#x200B;* [Illustrator] Não é possível importar arquivos do Illustrator após falha do servidor sem reiniciar o Painter
&#x200B;* [Python] O pai da instância não pode ser definido com o tipo “properties”
&#x200B;* [Python] Configurar o alto poli como um parâmetro de cozimento não carrega o alto poli
&#x200B;* [Python] A mensagem de erro para set\_color\_space() é muito genérica
&#x200B;* [Python] As fontes de referência permitem criar ciclos

<b>Problemas Conhecidos</b>:

&#x200B;* [Gerenciamento de cores] As conversões do espaço de cores HDR com ACE no Linux produzem cores vivas
&#x200B;* [Regression]&#x200B;[UI] O menu do botão direito do mouse é muito pequeno em telas HD
&#x200B;* [Crash]&#x200B;[Python] Exportação de USD acionada por TextureStateEvent
&#x200B;* [MacOS Intel] Falha ao importar algumas predefinições
&#x200B;* [Illustrator] Falha ao exportar um bloco UV com gráfico .ai em casos específicos
&#x200B;* [Traçados dinâmicos]&#x200B;[Caminho] O aleatório por traçado não funciona em um caminho

### 10.0.0

Data de lançamento: <b>5/2024/16</b>
Resumo: <b>Versão principal, edição da pilha de camadas com a API Python, leitura de arquivos nativos do Illustrator, integração de ativos 3D e novo recurso de texto</b>

<b>Adicionado</b>:

&#x200B;* [Illustrator] Usar arquivos do Illustrator com painéis de arte no Painter
&#x200B;* [Illustrator]&#x200B;[SVG] Adicionar visualizações na seleção de escopo
&#x200B;* [Substance 3D Assets] Procure, selecione e baixe ativos 3D diretamente no Painter
&#x200B;* [Substance 3D Assets]&#x200B;[IU] Novo painel
&#x200B;* [Substance 3D Assets] Mapas e materiais do ambiente de suporte
&#x200B;* [Substance 3D Assets] Permitir recarregamento e navegar e abrir a pasta de local em novo painel do Substance 3D Assets
&#x200B;* [Substance 3D Assets] Adição de um gerenciador de downloads
&#x200B;* [Recurso de texto] Permitir o uso de fontes incorporáveis
&#x200B;* [Recurso de texto] Permite renderizar uma fonte/texto em uma malha
&#x200B;* [Recurso de texto] Exibir fontes do usuário e outros caminhos compartilhados no painel Ativos com uma nova categoria
&#x200B;* [Recurso de texto]&#x200B;[Propriedades] Adicionar suporte para propriedades avançadas de fonte
&#x200B;* [Recurso de texto] Permitir pesquisar/exibir fontes em miniprateleiras
&#x200B;* [Recurso de texto] Adicionar mensagem/caixa de diálogo de erro ao importar uma fonte incompatível
&#x200B;* Diversos
&#x200B;* [Preencher projeção] Melhorar o comportamento do manipulador de escala ao usar valores pequenos
&#x200B;* [Manipuladores] Adicionar novo modo preciso ao pressionar o atalho CTRL
&#x200B;* [Manipuladores] Melhoram a estabilidade do manipulador de superfície ao traduzir
&#x200B;* [Exportar] Adicionar o nome do espaço de cores nas saídas SBSAR
&#x200B;* [Desempenho] Melhorar o tempo de descoberta da biblioteca de ativos em disco
&#x200B;* [Substance] Atualização do mecanismo de Substance versão 9.1.2
&#x200B;* [Arrastar e soltar] Alinhar a rotação do decalque na câmera ao soltar no visor
&#x200B;* [Python] Edição da pilha de camadas
&#x200B;* [Python] Permitir selecionar camada, efeito, máscara, máscara geográfica na interface do usuário
&#x200B;* [Python] Permitir modos de mesclagem de camada get/set
&#x200B;* [Python] Permitir obter/definir configurações de projeção da camada de preenchimento
&#x200B;* [Python] Permitir consultar a cor do material de Substance de uma camada de preenchimento
&#x200B;* [Python] Permitir consultar e definir cores e recursos uniformes em camadas e efeitos
&#x200B;* [Python] Permitir a criação e edição de recursos de texto no pilha de camadas
&#x200B;* [Python] Permitir a edição de canais ativos em camadas e efeitos
&#x200B;* [Python] Permitir que ações em lote tenham uma única operação de desfazer/refazer
&#x200B;* [Python] Permitir carregar/editar parâmetros de origem vetorial
&#x200B;* [Python] Permitir a edição de propriedades de cores de camadas e efeitos com o gerenciamento de cores
&#x200B;* [Python] Permitir consultar e criar camadas instanciadas
&#x200B;* [Python] Permitir a adição do efeito de seleção de cor
&#x200B;* [Python] Permitir o controle do gerenciamento de cores de imagens de bitmap
&#x200B;* [Python] Permitir pausa/cancelamento de pausa no mecanismo
&#x200B;* [Python] Permitir a navegação para nós irmãos e pai
&#x200B;* [Python] Permitir a criação do efeito filtro/gerador
&#x200B;* [Python] Permitir a adição de efeito de nível
&#x200B;* [Python] Permitir adicionar máscara inteligente em uma camada
&#x200B;* [Python] Permitir a criação/edição de pontos de ancoragem
&#x200B;* [Python] Permitir obter/definir máscara em camadas
&#x200B;* [Python] Permitir a criação do efeito de máscara de comparação
&#x200B;* [Python] Permitir consultar e usar predefinições de recursos Substance
&#x200B;* [Python] Permitir listar predefinições e seus valores por meio da função internal\_properties para recursos Substance
&#x200B;* [Python] Permitir listar predefinições de exportação predefinidas
&#x200B;* [Python] Permitir listar predefinições de exportação disponíveis na biblioteca
&#x200B;* [Python] Permite recuperar o conteúdo das predefinições de exportação

<b>Corrigido</b>:

&#x200B;* [Falha] Desfazer “Remover instância de sombreamento” com Ctrl-Z
&#x200B;* [Falha] Criar uma camada em uma pilha vazia se a última seleção tiver sido um efeito
&#x200B;* [SVG] Problema com o valor personalizado da área cortada
&#x200B;* [Contornar automaticamente] Recalcular apenas a embalagem sem qualquer alteração na orientação UV resulta em falha
&#x200B;* [Arrastar e soltar] Atraso devido a recursos externos pré-carregados várias vezes
&#x200B;* [UI] Arrastar e soltar a miniatura do recurso pode ocultar a mensagem de aviso na pilha de camadas
&#x200B;* [Desempenho] Os blocos UV mascarados ainda são computados
&#x200B;* [USD] Realce incorreto para seleção de escopo
&#x200B;* [Recurso] A imagem de bitmap é corrompida após pintar no canal normal e salvar o projeto
&#x200B;* [USD] Suporte à ordenação de malha de vértice com a mão esquerda
&#x200B;* [Substance] Redefinir para o padrão sempre voltar a zero para o widget de ângulo
&#x200B;* [Engine] Pintar com um SVG em um estêncil não funciona
&#x200B;* [Engine] Os traçados do pincel de Mapa normal se quebram após uma ação de desfazer
&#x200B;* [Conteúdo] O gráfico para Filtro Material tem mistura de alfa e espaço de cor incorretos
&#x200B;* [Conteúdo] Os modos de mesclagem no Tile Generator não estão funcionando
&#x200B;* [Conteúdo] O filtro de exame de histograma produz faixas em alguns casos
&#x200B;* [Conteúdo] A iluminação Feita bake estilizada não leva em conta o height pintado
&#x200B;* [Python] Erro inesperado ao recuperar informações de camada instanciadas após alteração do sombreador
&#x200B;* [Salvar] O arquivo de projeto é perdido quando o “salvar como” falha em casos específicos

<b>Problemas Conhecidos</b>:

&#x200B;* [Gerenciamento de cores] As conversões do espaço de cores HDR com ACE no Linux produzem cores vivas
&#x200B;* [Crash]&#x200B;[Linux]&#x200B;[AMD] Arrastar e soltar recursos na pilha de camadas no sistema operacional Wayland
&#x200B;* [Regression]&#x200B;[UI] O menu do clique com o botão direito é muito pequeno em telas HD
&#x200B;* [Crash]&#x200B;[Python] Exportação de USD acionada por TextureStateEvent
&#x200B;* [Salvar] O arquivo de projeto Spp é perdido quando a opção “salvar como cópia” falha em casos específicos
&#x200B;* [MacOS Intel] Falha ao importar algumas predefinições
&#x200B;* [Illustrator] Não é possível importar arquivos Ai após o travamento do servidor sem reiniciar o Painter
&#x200B;* [Import] Ativos com o mesmo nome, mas extensões diferentes, são substituídos

## Versão 9

### 9.1.2

Data de lançamento: <b>1/2024/30</b>
Resumo: <b>Versão secundária, correções de erros</b>

<b>Adicionado</b>:

&#x200B;* [Desempenho] Melhorar o tempo de criação da primeira camada de preenchimento em novos projetos
&#x200B;* [Desempenho] Reduzir o tempo de carregamento de mapas de ambiente pesado
&#x200B;* [Substance] Permitir salvar/fechar projetos mesmo quando as miniaturas estiverem sendo geradas

<b>Corrigido</b>:

&#x200B;* A gravação falha em projetos de versões anteriores quando o visor é modificado
&#x200B;* [Falha] Reimportar malha ao usar o AO personalizado e o gerenciamento de cores
&#x200B;* [Preencher projeção] Clicar no manipulador de escala exibe a mensagem “não é possível pintar”
&#x200B;* [Pincel] Pintar com alinhamento UV causa artefatos
&#x200B;* [Pilha de camadas] Renomear a camada é lento quando a pilha é muito longa
&#x200B;* [Pilha de camadas] Mensagem de erro incorreta ao usar filtro incompatível na máscara
&#x200B;* [Pilha de camadas] A seleção volta para a camada superior após a exclusão
&#x200B;* [Exportar] A textura normal gerada está sempre no modo de preenchimento Vizinho do Espaço 3D
&#x200B;* [Exportar] A textura alfa não é gerada com a predefinição de exportação Exibição 2D
&#x200B;* [Exportar] A exportação SBSAR tem usos incorretos com mapas convertidos
&#x200B;* [Shader] O log de alterações do API de sombreamento não está atualizado com as alterações mais recentes do ASM

<b>Problemas Conhecidos</b>:

&#x200B;* [Gerenciamento de cores] As conversões do espaço de cores HDR com ACE no Linux produzem cores vivas
&#x200B;* [Crash]&#x200B;[Linux]&#x200B;[AMD] Arrastar e soltar recursos na pilha de camadas no sistema operacional Wayland
&#x200B;* [Regression]&#x200B;[UI] O menu do clique com o botão direito é muito pequeno em telas HD
&#x200B;* [Crash]&#x200B;[Python] Exportação de USD acionada por TextureStateEvent

### 9.1.1

Data de lançamento: <b>2023/12/05</b>
Resumo: <b>Versão secundária, correções de erros e envio para a funcionalidade do After Effects</b>

<b>Adicionado:</b>

&#x200B;* [Interop] Permitir o envio de uma malha texturizada para o After Effects (Ae 24.1)

<b>Corrigido:</b>

&#x200B;* [Preenchimento] UV definido para projeção de conjunto UV não lê mais do que 2 conjuntos UV
&#x200B;* [Falha] Usar o mapa de ambiente de 16K
&#x200B;* [Falha] Exr usado como entrada de imagem
&#x200B;* [Falha] Copiar e colar caminhos entre projetos
&#x200B;* [QoL] Arrastar e soltar o recurso Alpha no modo de decalque cria Projeção UV na máscara
&#x200B;* [Caminho] Copiar vértices de caminho também renomeia o caminho de destino ao reabrir o projeto
&#x200B;* [Linux] A escolha de cores pode ser interrompida com várias telas
&#x200B;* [Desbobinar automaticamente] Problema de interface do usuário para controle de densidade de texel
&#x200B;* [Gerenciamento de cores] O feedback da interface é razoável, mas o mecanismo não
&#x200B;* [Gerenciamento de cores] Seleção incorreta de espaço de cores na máscara com substituição de dados do usuário

<b>Problemas Conhecidos:</b>

&#x200B;* [Gerenciamento de cores] As conversões do espaço de cores HDR com ACE no Linux produzem cores vivas
&#x200B;* [Crash]&#x200B;[Linux] com Linux Wayland no AMD ao arrastar e soltar recursos na pilha de camadas
&#x200B;* [Crash]&#x200B;[Mac] Alterar o valor da filtragem anisotrópica no sistema operacional Monterey
&#x200B;* [Regression]&#x200B;[UI] O menu do clique com o botão direito é muito pequeno na tela hd
&#x200B;* [Python] Falha ao exportar USD acionada por TextureStateEvent

### 9.1.0

Data de lançamento: <b>2023/11/07</b>
Resumo: <b>Versão principal que apresenta suporte a SVG e transparência, bem como melhorias na ferramenta de arrastar e soltar e no caminho</b>

<b>Adicionado:</b>

&#x200B;* [SVG] Permitir a importação de arquivos vetoriais (SVG)
&#x200B;* [SVG]&#x200B;[UI] Adicionar suporte para propriedades específicas de SVG
&#x200B;* [SVG] Adicione uma opção para preservar facilmente as proporções da imagem original
&#x200B;* [SVG] Permite usar automaticamente alfa de SVG com transparência
&#x200B;* [Interop] Permitir o envio de uma malha texturizada para o After Effects (Ae 24.1 beta)
&#x200B;* [Interoperabilidade] Adicionar configurações de Envio ao After Effects
&#x200B;* [QoL]&#x200B;[Assets]&#x200B;[UI] Importar ativo automaticamente ao arrastar e soltar no slot da interface
&#x200B;* [QoL] Permitir arrastar e soltar ativos externos na pilha de camadas
&#x200B;* [QoL]&#x200B;[Pilha de camadas] Arrastar e soltar texturas do painel Ativos na Pilha de camadas
&#x200B;* [QoL]&#x200B;[Janela de visualização] Permite arrastar e soltar o gerador, filtros na malha
&#x200B;* [QoL]&#x200B;[Visor] Permitir soltar ativos externos na malha
&#x200B;* [QoL]&#x200B;[Projeção] Adicionar novo conjunto UV ao modo de projeção do conjunto UV
&#x200B;* [QoL] Arrastar e soltar Máscaras inteligentes como novas camadas no visor e na Pilha de camadas
&#x200B;* [QoL] Adicionar seletor para Geradores com várias saídas quando usado em máscara
&#x200B;* [QoL] Permitir arrastar e soltar imagens de canal único sobre um efeito de preenchimento
&#x200B;* [QoL]&#x200B;[Pilha de camadas] Use modificadores CTRL/ALT com arrastar e soltar para especificar onde/como criar efeitos/camada
&#x200B;* [Caminho] Alterna a visibilidade dos caminhos individualmente no painel Caminho
&#x200B;* [Caminho] Permitir o uso de manipuladores de transformação para pontos de caminho
&#x200B;* [Caminho] Permite controlar manualmente as tangentes por vértice
&#x200B;* [Caminho] Copiar/colar propriedades do caminho
&#x200B;* [Path] Introduzir um atalho vazio para o botão Quebrar tangente
&#x200B;* [Shader] Adicionar suporte para Opacidade e Translucidez no sombreador ASM
&#x200B;* [Shader] Adicionar suporte para canal de Cor de absorção com sombreador ASM
&#x200B;* [Shader] Melhorar dicas de ferramentas de parâmetros de sombreador ASM
&#x200B;* [Shader] Alterar a cor padrão do canal de transparência para preto
&#x200B;* [Configurações de exibição] Ativar Suavização temporal por padrão
&#x200B;* [Configurações de exibição] Ativar configuração de dispersão abaixo da superfície por padrão
&#x200B;* [Substance] Adicionar suporte para a propriedade ColorSpace a partir da entrada/saída do gráfico
&#x200B;* [Substance] Atualize o mecanismo de Substance para a versão 9.0.3
&#x200B;* [IU] Tornar acessível o botão contextual da barra de ferramentas, mesmo se a janela do aplicativo for pequena
&#x200B;* [Auto Unwrap] Controlar o número de ladrilhos UV com densidade de texel
&#x200B;* [Preparação] Desativar Rastreamento de raios do GPU em GPUs AMD por padrão
&#x200B;* [Desempenho] Aplique compactação sem perdas em imagens de 16 bits para reduzir o espaço ocupado pelo projeto
&#x200B;* [Python] Permitir manipular a câmera padrão na visualização 3D
&#x200B;* [Python] Expor a capacidade de exportar malha por meio de scripts
&#x200B;* [Conteúdo]&#x200B;[Amostras] Adicionar novo projeto de amostra “Mesa de restaurante francês”
&#x200B;* [Content] Atualize o logotipo do Substance para a nova versão
&#x200B;* [Conteúdo] Adicione três filtros de material focados em SVG (adesivo personalizado, spray personalizado e gráfico para o material)

<b>Corrigido:</b>

&#x200B;* [Falha] Alterar o tamanho do manipulador quando não estiver usando a ferramenta de simetria
&#x200B;* [Falha] [Pilha de camadas] Criando camada quando nada está selecionado
&#x200B;* [Projeto] Mapas de malha podem ser corrompidos após a remoção de recursos não utilizados
&#x200B;* [Project] Corrupção de recursos após importar ou colocar novamente a imagem no forno
&#x200B;* [Assets] Recarregar um ativo o remove de Favoritos
&#x200B;* [Importar] Não é possível importar recursos quando “Nenhum resultado encontrado” no painel de ativos
&#x200B;* [UI] A seta da barra de ferramentas contextual não aparece em alguns casos
&#x200B;* [Substance] Botão lado a lado para valores booleanos não suportado
&#x200B;* [Level] Rótulo de canal incorreto quando usado na máscara
&#x200B;* [Export]&#x200B;[glTF] Os arquivos glTF/GLB exportados do Painter não têm uma unidade de tamanho físico
&#x200B;* [Conteúdo] A intensidade do filtro de desfoque é fixada em 16
&#x200B;* [Conteúdo] A entrada da imagem de “cor de destino” do filtro Correspondência de Cores não está visível

<b>Problemas conhecidos:</b>

&#x200B;* [Gerenciamento de cores] As conversões do espaço de cores HDR com ACE no Linux produzem cores vivas
&#x200B;* [Crash]&#x200B;[Linux] com Linux Wayland no AMD ao arrastar e soltar recursos na pilha de camadas
&#x200B;* [Crash]&#x200B;[Mac] Alterar o valor da filtragem anisotrópica no sistema operacional Monterey
&#x200B;* [Falha] Exr usado como entrada de imagem
&#x200B;* [Falha] Usar o mapa de ambiente de 16K
&#x200B;* [Desbobinar automaticamente] Problema de interface do usuário para controle de densidade de texel
&#x200B;* [Regression]&#x200B;[UI] O menu do clique com o botão direito é muito pequeno na tela hd
&#x200B;* [Python] Falha ao exportar USD acionada por TextureStateEvent
&#x200B;* [QoL] Arrastar e soltar o recurso Alpha no modo de decalque cria Projeção UV na máscara

### 9.0.1

Data de lançamento: <b>9/2023/19</b>
Resumo: <b>Versão de correção de erro secundária com várias melhorias</b>

<b>Adicionado:</b>

&#x200B;* [Importar] Definir local de importação padrão na janela de importação
&#x200B;* [Modo de Fça bake] Permitir a redefinição de parâmetros para seus valores padrão
&#x200B;* [Fazendo bake] Definir o fça bake como resolução de tinta ao criar um projeto
&#x200B;* [Simetria] Desvincular manipulador específico de simetria do atalho Q
&#x200B;* [Menu] Adicionar a opção “mostrar registro” no menu Ajuda
&#x200B;* [Visor] Melhorar a velocidade de renderização de sombra
&#x200B;* [Substance] Atualizar mecanismo para a versão 9.0.1
&#x200B;* [Gerenciamento de cores] O arquivo de configuração OCIO pode ter qualquer tipo de extensão
&#x200B;* [Assets] O recurso Sbsar com uso de “decalque” deve ser definido automaticamente para distorcer a projeção
&#x200B;* [Caminho] Exibe uma mensagem ao tentar interagir com a ferramenta Caminho enquanto a interface do usuário e os Gizmos estão ocultos

<b>Corrigido:</b>

&#x200B;* [Falha] Alt + Arrastar no painel Caminho
&#x200B;* [Importar Recursos] Falha aleatória ao remover recursos para importar
&#x200B;* Falha ao importar um arquivo GLB compactado
&#x200B;* Problema ao pintar em malhas que compartilham UVs
&#x200B;* Flash de malha preto ao recalcular ou carregar cache
&#x200B;* [Propriedades] O menu do botão direito do mouse para redefinir parâmetros não aparece nas listas suspensas
&#x200B;* [Nível] Controles deslizantes de entrada bloqueados pelo nível anterior
&#x200B;* [AMD]&#x200B;[Esparsa] A opção SVT, se ativada, gera artefatos
&#x200B;* [Projeção]&#x200B;[Distorcer] Falha ao clicar duas vezes nos vértices
&#x200B;* Interface do usuário do [Caminho] e caminho visível no modo de cozimento
&#x200B;* [AMD] Textura perdida ao brincar com a visibilidade
&#x200B;* [Esparso] Resolução muito baixa ao girar a malha

<b>Problemas Conhecidos:</b>

&#x200B;* [Gerenciamento de cores] As conversões do espaço de cores HDR com ACE no Linux produzem cores vivas

### 9.0.0

Data de lançamento: <b>06/2023/20</b>
Resumo: <b>Versão principal com pintura ao longo de um caminho que permite Curvas 3D, novos materiais de base e limpeza de materiais legados e novas predefinições para Curvas 3D</b>

<b>Adicionado:</b>

&#x200B;* [Caminho] Adiciona nova ferramenta Pintura ao longo do caminho
&#x200B;* [Caminho] Adiciona um atalho vazio para a ferramenta de caminho
&#x200B;* [Caminho] Permite adicionar novos pontos a um caminho existente
&#x200B;* [Caminho] Adiciona um atalho para sair da criação do caminho atual
&#x200B;* [Caminho] Permite editar as propriedades do pincel para caminhos
&#x200B;* [Caminho] Ajustar tangentes automaticamente ao inserir um ponto
&#x200B;* [Caminho] Recalcular tangentes quando um ponto for movido
&#x200B;* [Caminho] Ajustar pontos recém-criados à superfície de uma malha
&#x200B;* [Caminho] Permitir a edição da pressão por vértice
&#x200B;* [Caminho] Ajuste a pressão do ponto recém-criado a partir de pontos vizinhos
&#x200B;* [Caminho] Permite converter pontos em suaves/de vértice (quebra tangente)
&#x200B;* [Caminho] Permite mover um ponto recém-adicionado imediatamente
&#x200B;* [Caminho] Permite remover pontos do caminho existente
&#x200B;* [Caminho] Permite inverter a direção de um caminho
&#x200B;* [Caminho] Permite selecionar um caminho na viewport
&#x200B;* [Caminho] Permite selecionar pontos de caminho com seleção de letreiro
&#x200B;* [Caminho] Introduza atalhos de CTRL-A para selecionar todos os pontos de um caminho
&#x200B;* [Caminho] Permite fechar o caminho
&#x200B;* [Caminho] Permite especificar o caminho acima do eixo em Propriedades
&#x200B;* [Caminho] Adiciona um menu de controle de vértice à barra de ferramentas contextual
&#x200B;* [Caminho] Introduza modos de pintura/apagamento/borrar na ferramenta de caminho
&#x200B;* [Caminho] Criar feedback visual para caminhos no visor
&#x200B;* [Caminho] Adiciona um indicador visual para a direção do caminho
&#x200B;* [Caminho] Adiciona thickness de linha às configurações de exibição de caminho
&#x200B;* [Caminho] Permitir ocultar a interface do usuário de caminhos
&#x200B;* [Caminho] Adiciona o painel Caminho para listar os caminhos da camada atualmente selecionada
&#x200B;* [Caminho] Adicionar feedback visual ao passar o mouse sobre um caminho no painel Caminho
&#x200B;* [Caminho] Exibe o painel de caminho sempre que a ferramenta Caminho é selecionada
&#x200B;* [Caminho] Permite renomear, excluir, copiar, recortar, duplicar o caminho no painel Caminho
&#x200B;* [Caminho] Exibe a mensagem ao tentar interagir na viewport 2D com a ferramenta Caminho
&#x200B;* [Biblioteca] Integrar novo conteúdo (ferramentas e materiais de base de caminho)
&#x200B;* [Traçados dinâmicos] Adicionar propriedade de distância para traçados dinâmicos
&#x200B;* [Traçados dinâmicos] Adicionar propriedades de tamanho e espaçamento aos traçados dinâmicos
&#x200B;* [Traçados dinâmicos] Adicionar propriedade início/meio/fim para traçados dinâmicos
&#x200B;* [Python]&#x200B;[USD] Expor parâmetros de configuração de projeto para o formato USD
&#x200B;* [Python]&#x200B;[USD] Expor os parâmetros de criação de projetos para o formato USD
&#x200B;* [Export]&#x200B;[USD] Adicionar informações do caminho do projeto no arquivo USD exportado
&#x200B;* [GLTF] Atualizar texturas na biblioteca ao recarregar um arquivo GLTF
&#x200B;* [Shader] Reduzir artefatos de costura para Ilhas UV com orientação diferente
&#x200B;* [Engine] Atualização para o mecanismo de Substance versão 9.0

<b>Corrigido:</b>

&#x200B;* [Importar] Algumas GLB com texturas não obtêm texturas no Painter
&#x200B;* [AMD] Artefatos em bordas para todos os preenchimentos de projeção 3D
&#x200B;* [Engine] As texturas se quebram ao alternar a visibilidade da camada
&#x200B;* [Engine] As texturas ficam vazias em alguns locais ao alterar o modo de mesclagem
&#x200B;* [Engine] A Textura/Projeção é o modo de distorção vazio em alguns casos
&#x200B;* [Iray] A iteração é redefinida para 0 ao salvar a renderização
&#x200B;* [Log] Mensagem de erro do USD ao executar File > New

<b>Problemas Conhecidos:</b>

&#x200B;* [Gerenciamento de cores] As conversões do espaço de cores HDR com ACE no Linux produzem cores vivas
&#x200B;* [Pilha de camadas] Fonte de entrada não salva por camada

## Versão 8

### 8.3.1

Data de lançamento: <b>2023/04/27</b>

<b>Adicionado:</b>

&#x200B;* [Modo de Fça bake] Adicionar atalho (vazio) para mostrar/ocultar a visualização do visor
&#x200B;* [Modo de cozimento] Sempre mostrar Low Poly ao usar o botão “Ocultar malhas de cozimento”
&#x200B;* [Modo de Fça bake] Mostrar sufixo para Correspondência por Nome com base no Conjunto de Texturas atual
&#x200B;* [Importar] Adicionar suporte para arquivos binários GLTF (glb)
&#x200B;* [Lista de conjuntos de texturas] Adicionar menu para selecionar ou criar instâncias de sombreamento
&#x200B;* [Lista de conjuntos de textura] Permite alterar rapidamente o conjunto de textura e a resolução do Bloco UV
&#x200B;* [Tamanho físico] Melhorar o comportamento do manipulador ao usar tamanho físico no Projeção UV
&#x200B;* [UI] Trazer de volta “Salvar como” para o menu Arquivo principal
&#x200B;* [UI] Salvar seleção de exibição (somente 2D, somente 3D, ambos) no layout da interface do usuário
&#x200B;* [USD] Mensagem de erro menos vaga na criação do projeto com formas USD não suportadas
&#x200B;* [Python] Adicionar eventos de fça bake para seguir o progresso de Fça bake
&#x200B;* [Python] Permitir o cancelamento de um faço bake
&#x200B;* [Python] Expor “Com base no modelo de saída” para o tipo de arquivo e a profundidade de bits na exportação
&#x200B;* [Python] Expor tempo de atualização para TextureStateEvent.Update

<b>Corrigido:</b>

&#x200B;* [Falha] Falha rara ao fechar um projeto
&#x200B;* [Falha] [Fazendo bake] Ativar sincronização de mapa de malha com Height ou curvatura em um projeto específico
&#x200B;* [Falha]&#x200B;[Script] Falha ao adicionar um material após a criação da instância de sombreamento
&#x200B;* [Modo de Fça bake] A intensidade do AO em material neutro não tem efeito
&#x200B;* [Modo de Fça bake] Falha ao alternar para o modo de fça bake antes de carregar o modelo
&#x200B;* [Modo de Fça bake] Mensagem de erro ausente na guia Fazer bake Processo
&#x200B;* [Modo de Fça bake] As configurações de material neutro não têm efeito após a reimportação de uma malha
&#x200B;* [Modo de Fça bake] O separador de visor é salvo globalmente, e não por modo
&#x200B;* [Modo de cozimento] Problema de visualização: o normal médio não altera a superfície da gaiola
&#x200B;* [Gerenciamento de cores] A configuração de detecção automática de espaço de cores é desativada quando a variável de ambiente OCIO está presente
&#x200B;* [Conteúdo] O filtro Contorno de máscara tem artefato com entrada de height
&#x200B;* [Conteúdo] O controle deslizante de intensidade do filtro de desfoque de Inclinação é apertado em 1.0
&#x200B;* [Interop] Não é possível criar projeto com GLTF a partir do Sampler
&#x200B;* [Pilha de camadas] O valor de divisão em blocos gráficos de projeção não é atualizado corretamente com o manipulador
&#x200B;* [Linux] Deslocamento entre a caneta eletrônica gráfica e o cursor com HDPI maior que 100%
&#x200B;* [Python] Falha ao reimportar uma malha após criar um projeto
&#x200B;* [Substance] Ruídos 3D são quebrados após a reimportação de uma malha
&#x200B;* [Blocos UV] O deslocamento da Projeção UV é fixado em 1
&#x200B;* [Visor] O feedback visual em linhas retas não está mais visível
&#x200B;* [WhatsNew] Retorno de linha incorreto em títulos de recursos

<b>Problemas Conhecidos:</b>

&#x200B;* [Importar] Algumas GLB com texturas não obtêm texturas no Painter

### 8.3.0

*(Lançado: 10 De Janeiro De 2023)*
Resumo: <b>Versão principal com novo modo de preparo, nova importação e exportação de arquivos USD e suporte de tamanho físico para Projeção UV</b>

<b>Adicionado:</b>

&#x200B;* [Modo de cozedura] Novo modo de cozedura dedicado ao processo de cozedura
&#x200B;* [Modo de cozimento] Defina o atalho para alternar para o modo de cozimento para F8
&#x200B;* [Modo de cozimento] Botão Adicionar início e Cancelar cozimento no visor
&#x200B;* [Modo de cozimento] Adicionar seleção de cozimento na lista Conjunto de textura
&#x200B;* [Modo de cozimento] Adicionar nova janela de padeiros de mapa de malha para selecionar padeiros
&#x200B;* [Modo de cozimento] Adicionar nova janela Configurações do mapa de malha para editar as configurações de cozimento
&#x200B;* [Modo de cozimento] Adicionar nova janela de registro de cozimento para seguir o processo de cozimento
&#x200B;* [Modo de cozimento] Adicionar parâmetros de cozimento e desfazer ações na janela Histórico
&#x200B;* [Modo Preparação] Adicionar trilhas nas Configurações do mapa de malha
&#x200B;* [Modo de cozimento] Adicione miniaturas de mapas de malha na janela Preparadores de mapas de malha
&#x200B;* [Modo de cozimento] Adicionar menu recolhível de configurações de visualização em uma janela de visualização 3D
&#x200B;* [Modo de cozimento] Adicionar configuração de visualização para mostrar/ocultar a malha de alto polímero
&#x200B;* [Modo de cozimento] Adicionar configuração de visualização para mostrar/ocultar a malha da gaiola e o wireframe
&#x200B;* [Modo de cozimento] Adicionar configuração de visualização para mostrar/ocultar a malha de baixo polímero
&#x200B;* [Modo de cozimento] Adicionar configuração de visualização para mostrar as bordas sólidas sem emendas UV como erros
&#x200B;* [Modo de cozimento] Informar na viewport sobre erros de malha e cozimento se o Registro de cozimento não estiver visível
&#x200B;* [Modo Preparação] Adicionar ação para sincronizar as configurações do padeiro em todos os Conjuntos de Textura

  Na janela Panificadores de mapa de malha, cada panificação (bem como as configurações comuns) pode ser sincronizada entre os conjuntos de textura clicando no ícone de link ao lado de seu nome. Esta ação abrirá uma janela que permite selecionar quais conjuntos de texturas compartilharão os mesmos parâmetros.

&#x200B;* [Modo de cozimento] Adicionar ações para copiar e colar configurações do padeiro

  Na janela Panificadores de mapa de malha estão disponíveis ações para copiar e colar cada configuração de panificação nos Conjuntos de textura por meio do menu dedicado na parte superior da janela ou do menu contextual do botão direito do mouse.

&#x200B;* [Modo de cozimento] Adicione o botão no Log de cozimento para pular do erro para as configurações corretas

  Quando um padeiro falha ou uma malha não é carregada corretamente, uma mensagem de erro aparece no registro de cozimento. Um botão ao lado da mensagem permite alterar a janela Configurações de pás e mapas de malha para mostrar as configurações relacionadas. Isso ajuda a isolar com mais facilidade a origem de um problema para corrigi-lo.

&#x200B;* [Modo Preparação] Adicionar menus para gerenciar conjuntos de texturas e seleções de pincéis

  Tanto na “lista de conjuntos de texturas” quanto na “PANELAS DE MAPA DE MALHA”, foi adicionado um pequeno menu de ação para ajudar a copiar e inverter as seleções.

&#x200B;* [Modo de cozimento] Dividir a lista de seleção do padeiro por conjunto de textura
&#x200B;* [Modo de cozimento] Dividir configurações comuns por conjunto de textura
&#x200B;* [Modo de cozedura] Carregue malhas de alto-poli e gaiola sem congelar a interface
&#x200B;* [Modo de cozimento] Use a barra de progresso do visor para mostrar a carga da malha
&#x200B;* [Modo de cozimento] Adicionar estado de carregamento de malha no Log de cozimento
&#x200B;* [Modo de cozedura] Permite girar a malha no visor durante a cozedura
&#x200B;* [Modo de cozedura] Definir a ordem de cozedura com base na visibilidade atual da janela de malha
&#x200B;* [Modo de cozimento] Exibir gaiola de cozimento implícita no visor

  Se não estiver usando um arquivo de malha de gaiola personalizado, uma malha de gaiola automática será gerada e exibida na janela de visualização. Seu tamanho será baseado no parâmetro Distância frontal máxima das configurações comuns de cozimento. A malha de gaiola é usada para indicar até onde a correspondência entre o poli baixo e alto irá.

&#x200B;* [Modo de cozimento] Mostrar lista correspondente de nomes de malha para correspondência por nome no Log de cozimento
&#x200B;* [Modo de cozimento] Usar material neutro para exibir o modelo 3D na viewport
&#x200B;* [Modo de cozimento] Desativa o cálculo do motor em modo de cozimento
&#x200B;* [Modo de cozimento] Exibir um aviso ao sair do aplicativo enquanto uma torta está em andamento
&#x200B;* [Padeiros] Atualizar rótulos de configuração de suavização de borda

  Os valores de configuração de suavização de borda foram renomeados para “Sobreamostragem” e com um número multiplicador explícito para esclarecer seu comportamento.

&#x200B;* [Padarias] Atualize as padarias para a versão 2.5.7.
&#x200B;* [USD] Importar e exportar arquivos do Universal Scene Description (USD)
&#x200B;* [USD] Adicione opções USD à janela Novo projeto ao selecionar um arquivo USD
&#x200B;* [USD] Adicionar nova janela de seleção de escopo e variantes

  Ao importar um arquivo USD, clicar no botão de alteração na janela Novo projeto ou Configuração de projeto permite selecionar qual parte e variantes de um arquivo USD importar.

&#x200B;* [USD] Opção Adicionar níveis de subdivisão

  Ao criar um novo projeto com um arquivo de malha do USD que contém subdivisões, é possível selecionar o nível de subdivisões usando um controle deslizante. O projeto será criado com a malha subdividida. O nível pode ser modificador por meio da Configuração do projeto.

&#x200B;* [USD] Importar malhas com pele em USD em um quadro específico

  Ao criar um novo projeto com um arquivo de malha USD que contém animação, é possível selecionar a quadro usando um controle deslizante que reflete a sequência de linha do tempo incorporada. O quadro pode ser modificador por meio da Configuração do projeto.

&#x200B;* [USD]&#x200B;[Exportar] Adicione uma opção para exportar arquivos USD

  Nova caixa de seleção Exportar USD adicionada à janela Exportar textura. Quando marcada, permite exportar arquivos USD, bem como mapas de textura usando qualquer modelo.

&#x200B;* [USD]&#x200B;[Exportar] Adicionar formato de arquivo USD à exportação de malha
&#x200B;* [USD] Renomear a predefinição de exportação “USD PBR Metal Roughness” existente para ser mais explícita

  O modelo de exportação de USD anteriormente conhecido como &#39;USD PBR Metal Roughness&#39; ainda é acessível por meio de texturas de exportação > Modelo de saída > USDz (Apple AR).

&#x200B;* [Abrir automaticamente] Adicionar orientação Bloquear para embalagem

  Nova opção para configurações de abertura automática que permitem preservar a orientação de Ilhas UV existentes ao usar o recurso de embalagem. Ele pode ser acessado em Novo projeto > Opções de Contornar automaticamente > Orientação da Ilha UV.

&#x200B;* [Tamanho físico] Adicionar configuração para usar Tamanho físico automaticamente no efeito/camada de preenchimento

  Foi adicionada uma nova opção para alternar automaticamente para a escala de tamanho físico ao usar um material com tamanho físico incorporado. Ele pode ser ativado por projeto por meio de Novo projeto ou de Editar > Configuração do projeto > Tamanho físico > Alternar o dimensionamento da camada de preenchimento para Tamanho físico ao atribuir materiais.

&#x200B;* [Tamanho físico] Expor tamanho físico para Projeção UV

  O dimensionamento de tamanhos físicos agora está disponível para Projeção UV. Ele ativa o redimensionamento automático de um material com base no tamanho físico de uma malha. Pode ser selecionado por meio de Escala > Tamanho físico na janela Propriedades da camada de preenchimento ou do efeito.

&#x200B;* [Scripting]&#x200B;[Python] Permite consultar a versão do aplicativo
&#x200B;* [Scripting]&#x200B;[JavaScript] Atualizar API para corresponder aos novos parâmetros de fça bake
&#x200B;* [Scripting]&#x200B;[Python] módulo de Fça bake: editar parâmetros de fça bake
&#x200B;* [Scripting]&#x200B;[Python] Módulo de Fça bake: iniciar/cancelar fça bake
&#x200B;* [Scripting]&#x200B;[Python] Módulo de Fça bake: selecionar método de curvatura
&#x200B;* [Scripting]&#x200B;[Python] Módulo de Fça bake: seleção de baker/blocos uv
&#x200B;* [Scripting]&#x200B;[Python] Módulo de Fça bake: sincronizar as configurações de baker em todos os conjuntos de texturas
&#x200B;* [SVT] Habilitar suporte a hardware esparso em GPUs AMD

  A aceleração de hardware para o sistema de texturas virtuais esparsas agora pode ser ativada com as GPUs da AMD. Essa configuração é ativada automaticamente nas preferências gerais.

&#x200B;* [Projection] Renomear os parâmetros de projeção cilíndrica

  O parâmetro “Cylinder Cap Culling” foi renomeado para “Backface Culling” para melhor representar sua ação. A dica de ferramenta associada foi ajustada de acordo.

&#x200B;* [Project] Salvar a versão do aplicativo no projeto e recuperá-la por meio de scripts

  Desde a versão 8.2, a versão do aplicativo agora é armazenada dentro do arquivo spp ao salvar.
  Esse número de versão pode ser recuperado com a função last\_saved\_substance\_painter\_version() no módulo do projeto da API Python.
  Para projetos feitos antes de 8.2, o valor retornado será nulo.

&#x200B;* [Importar] Melhorar o tempo de importação geral de modelos 3D

  Melhoramos o tempo geral de importação das malhas. Por exemplo, reduzir o tempo de espera ao carregar malhas de alto-poli para cozimento. Essa otimização aplica-se em particular ao carregamento de arquivos OBJ.

<b>Corrigido:</b>

&#x200B;* [Falha] Alterar canais no filtro com pilha específica
&#x200B;* [Mac]&#x200B;[M1] Falha ao criar uma camada de preenchimento e sair da pilha de camadas

  Esse problema pode ser corrigido atualizando para o Mac OS 13 (Ventura).

&#x200B;* [Scripting]&#x200B;[Python] Falha ao usar ui.add\_dock\_widget() com tipo errado
&#x200B;* [Preparação] Mensagem de erro incompleta no log quando um bake falha
&#x200B;* [Preparação] A memória não é liberada quando a cozedura é concluída
&#x200B;* [Engine] O cache de textura não é atualizado ao alterar a visibilidade do efeito
&#x200B;* [Exportar] Mapa uniforme de exportações em 2D aleatoriamente
&#x200B;* [Project] Erro de alocação de memória ao salvar projeto com malha grande
&#x200B;* [Visor] O TAA causa artefatos ao pintar em alguns casos

<b>Problemas Conhecidos:</b>

&#x200B;* [Gerenciamento de cores] As conversões do espaço de cores HDR com ACE no Linux produzem cores vivas
&#x200B;* [Pilha de camadas] Fonte de entrada não salva por camada

### 8.2.0

*(Lançado: 06 De outubro De 2022)*
Resumo: **Versão principal com novos painéis de integração (novo painel de boas-vindas e painel de novidades), exportação para SBSAR, efeitos para pasta, várias melhorias na qualidade de vida e correções de erros.**

**Adicionado:**

&#x200B;* [Integração] Painel de integração para acolher novos usuários

  Adicionada uma nova tela de boas-vindas quando novos usuários da CC abrem o Painter pela primeira vez.

&#x200B;* [Integração] Painel de novidades para aprimorar a descoberta de novos recursos

  Adicionada uma nova tela Novidades que exibe os novos recursos principais. Ele é exibido automaticamente na primeira vez que o Painter é aberto após uma atualização importante e pode ser acessado novamente em Ajuda > Novidades.

&#x200B;* [Integração] Renomear antigo Bem-vindo à “Tela inicial”

  A tela de boas-vindas antiga foi renomeada para Tela inicial para evitar confusões com a nova tela de boas-vindas.

&#x200B;* [UI] Resolver problemas de dimensionamento para telas de alto DPI

  Adaptação aprimorada da interface do Painter em telas de alta definição com dimensionamento de exibição personalizado.

&#x200B;* [UI] Evitar mensagens de erro persistentes na interface do usuário

  As mensagens de erro de projetos anteriores agora são removidas da barra de status inferior.

&#x200B;* [UI] Menu de salvamento de retrabalho

  Opções adicionais de salvamento agora estão agrupadas em um submenu e algumas são renomeadas para fins de consistência.

&#x200B;* [UI] Salvar e exportar/compartilhar layouts de interface do usuário

  Dentro do menu Janela existem novas ações para salvar o layout da interface em arquivos e recarregá-los. Os layouts de Pintura e Renderização são salvos separadamente.
  Várias funções foram adicionadas a “substance\_painter.ui” para salvar, redefinir e carregar os layouts de interface também.

&#x200B;* Adicionar ações de copiar/colar para modos de mesclagem/opacidade de uma camada

  Adicionada uma nova entrada “Opções de mesclagem” no menu de contexto camadas. Permite copiar e colar o modo de mesclagem e a opacidade de todos os canais de uma camada para outra.

&#x200B;* Aplicar modo de mesclagem/opacidade a todos os canais de uma camada

  Adicionada a funcionalidade de clicar com o botão direito do mouse ao modo de mesclagem de camadas e à opacidade, que permite aplicar a configuração atualmente clicada a todos os canais.

&#x200B;* Recarregar malha com um atalho de teclado (CTRL+SHIFT+R)

  Foi adicionado um atalho editável para recarregar o arquivo de malha com as últimas configurações disponíveis. Também pode ser acessada em Editar > Reimportar malha.

&#x200B;* Redefinir parâmetros de Substance para padrão

  Adicionado um novo botão em Propriedades na parte inferior dos recursos .sbsar que permite redefinir o recurso para padrão.

&#x200B;* Redefinir pincel para padrão

  Adicionado um novo menu à seção Pincel em Propriedades, o que permite redefinir para o pincel básico padrão.

&#x200B;* Clique com o botão direito do mouse para redefinir os parâmetros de Substance individuais como padrão

  Foi adicionada a possibilidade de redefinir parâmetros individuais em um recurso .sbsar com o botão direito do mouse.

&#x200B;* [Painel Ativos] “Fixe” ativos favoritos para aparecerem sobre o painel Ativos

  Adicionada a nova opção de clicar com o botão direito em ativos da biblioteca que permite fixá-los como favoritos na parte superior do painel. Você também pode exibir todos os seus ativos favoritos em Pesquisas salvas.

&#x200B;* [Painel Ativos] Excluir, recarregar e renomear ativos

  Adicionadas as opções do menu de contexto para excluir, recarregar e renomear ativos na biblioteca do usuário. Eles são excluídos diretamente do local da biblioteca no disco e recarregados do local original. Os ativos que fazem parte de um pacote como .abr ou .sbsar não podem ser editados individualmente.

&#x200B;* [Seleção de cores] Adicionar modos de mesclagem ao efeito Seleção de cores
&#x200B;* [Pilha de camadas] Adicionar modo de mesclagem e opacidade em filtros
&#x200B;* [Pilha de camadas] Permitir valores de divisão em blocos maiores que 128 para camada/efeitos de preenchimento
&#x200B;* [Pilha de camadas] Tampas de cilindro para projeção cilíndrica na camada/efeito de preenchimento

  A projeção cilíndrica nas propriedades da camada de preenchimento agora tem a opção de remover as tampas dos cilindros.

&#x200B;* [Log] Mostra uma mensagem de erro se as partes da malha estiverem em espaço negativo ao tentar criar um projeto de Bloco UV

  Adicionada uma mensagem de erro mais clara ao falhar ao criar um projeto de Bloco UV porque as partes UV são encontradas em espaços negativos.

&#x200B;* [Project] Indica a versão na mensagem de erro “dados muito recentes” ao abrir um projeto

  Ao abrir um projeto que é muito recente para o aplicativo, a mensagem de erro agora indicará a versão do projeto para facilitar a identificação da versão correta do aplicativo.

&#x200B;* [Janela de visualização] Permitir a iluminação da malha por baixo

  Foi adicionado um novo parâmetro de Alinhamento de ambiente em Configurações de exibição > Câmera > Configurações de ambiente para alinhar a iluminação do mapa de ambiente à câmera quando definida como “Local”.

&#x200B;* [Visor] Visualize R, G, B e Alpha no visor (modo de exibição individual)

  Em Configurações de exibição > Configurações do visor > Exibição de canal, há uma nova configuração de Canais de cores que permite exibir apenas o componente R, G, B ou Alpha de um canal quando estiver no modo de exibição única.

&#x200B;* [Shader] Permite definir canais do usuário como RGBA em sombreadores de camada de material

  Ao definir a configuração de canais do Conjunto de texturas dentro de um sombreador para camadas de material, agora é possível especificar o formato do canal para se desviar do valor padrão. Isso permite solicitar canais de usuário coloridos em vez de somente tons de cinza.

&#x200B;* [Exportar] Permite exportar texturas como SBSAR

  Ao exportar texturas por meio da janela Arquivo > Exportar texturas, o formato de arquivo SBSAR (Substance Archive) pode ser escolhido para reagrupá-los. O conteúdo do SBSAR é orientado pelo modelo de saída usado.
  O formato de arquivo SBSAR também pode ser definido nas predefinições de exportação. Ao usar texturas de configuração híbrida (SBSAR + Outro formato) que se destinam a um SBSAR são agrupadas enquanto o restante é exportado junto.

&#x200B;* [Exportar] Opção Expor 16 bits para o formato de arquivo EXR

  Ao exportar arquivos de textura EXR, agora é possível escolher bit 16f (Half-Float) ou bit 32f (Float) na janela Exportar texturas (para configurações de exportação e predefinições de exportação). Projetos antigos e predefinições de exportação antigas terão o bit 16f como padrão para refletir o comportamento antigo.

&#x200B;* [Python] Adicionar evento para saber quando os conjuntos de texturas são modificados

  O novo “substance\_painter.event.TextureStateEvent” permite saber quando um conjunto de texturas foi modificado por causa de um traçado de tinta, um novo canal adicionado ou um canal removido.

&#x200B;* [Python] Permitir obter e definir recursos de Mapa de malha nas configurações de conjunto de textura

  Novas funções foram adicionadas ao módulo “substance\_painter.project” para obter e definir recursos de mapas de malha. Essas funções podem ser usadas para atualizar os mapas de malha referenciados pelas configurações do Conjunto de texturas.

&#x200B;* [Plugins] Remover a opção para obter outros plug-ins JS

  Remoção da opção para obter plug-ins JavaScript, pois eles estavam hospedados no site de compartilhamento obsoleto.

&#x200B;* [Content] Adicionar novo modelo Roblox e exportar predefinição

  Um novo modelo de projeto e predefinição de exportação Roblox “Material Variant” e “Surface Appearance” foram adicionados para facilitar a exportação de texturas PBR para Roblox. O modelo pode ser acessado pela janela Arquivo > Novo projeto.

&#x200B;* Atualize o Substance Engine para a última versão (8.6.3)
&#x200B;* [Steam] Compilação otimizada para o chipset Apple Silicon (Apple M1 / M2)

**Corrigido:**

&#x200B;* Falha ao usar exr 16k
&#x200B;* [Falha] Ctrl Z Após excluir uma instância de sombreamento
&#x200B;* [Iray] IoR bloqueada em 1 para alguns sombreadores
&#x200B;* [Win]&#x200B;[Fazendo bake] Falha ao carregar alguns itens com alto índice de polígonos
&#x200B;* [Gerenciamento de cores] Nome do espaço de cores incorreto na interface do usuário com filtros
&#x200B;* [Python] Os objetos de recurso retornados pela função de importação não têm um tipo

  Ao importar um pacote Substance em Python, a função estava retornando o pacote em vez de seu(s) gráfico(s). O módulo de recursos agora fornece funções e parâmetros para recuperar o(s) gráfico(s) de um pacote de Substance.

**Problemas Conhecidos:**

&#x200B;* [Gerenciamento de cores] As conversões do espaço de cores HDR com ACE no Linux produzem cores apertadas
&#x200B;* [Pilha de camadas] A fonte de entrada não é salva por camada
&#x200B;* [Pintura] A suavização temporal causa artefatos ao pintar em alguns casos
&#x200B;* [Exportar] O Visualização 2D exporta um mapa aleatoriamente uniforme

### 8.1.3

*(Lançado: 25 de agosto de 2022)*
Resumo: **Versão de correção de erro secundária**

**Adicionado:**

&#x200B;* Atualização para o Iray SDK 1.6

**Corrigido:**

&#x200B;* [Sombreador] Falha com sombreador antigo com defeito
&#x200B;* [Camada de material] Os materiais podem desaparecer ao reabrir um projeto

**Problemas Conhecidos:**

&#x200B;* [Gerenciamento de cores] As conversões do espaço de cores HDR com ACE no Linux produzem cores apertadas
&#x200B;* [Pilha de camadas] A fonte de entrada não é salva por camada
&#x200B;* [Falha] Ctrl Z Após excluir uma instância de sombreamento
&#x200B;* [Iray] IoR bloqueada em 1 para alguns sombreadores

### 8.1.2

*(Lançado: 19 De julho De 2022)*
Resumo: **Versão de correção de erro secundária**

**Adicionado:**

&#x200B;* [Auto Unwrap] Nova opção “Otimizar para malhas orgânicas” para selecionar o algoritmo de segmentação
&#x200B;* [Tamanho físico] Exponha as opções de unidade em Novo projeto e Configuração de projeto
&#x200B;* [Gerenciamento de cores] Usar a exibição de monitor por padrão ao usar ACE
&#x200B;* [Gerenciamento de cores]&#x200B;[Python] Leve em consideração o arquivo de predefinição ACE env-var ao criar projetos
&#x200B;* [Gerenciamento de cores] Redefinir as configurações de Gerenciamento de cores na janela Novo projeto quando a configuração for alterada
&#x200B;* [Gerenciamento de cores] Desativar o acesso às configurações de OCIO quando env-var estiver presente
&#x200B;* [Gerenciamento de cores] Atualizar com segurança as configurações de ACE quando um parâmetro não existir mais
&#x200B;* Atualize o Substance Engine para a versão 8.6.0
&#x200B;* [Exportar] Adicionar nova predefinição de exportação de GLTF com suporte ao Deslocamento
&#x200B;* [Scripting]&#x200B;[Python] Recuperar informações de recursos (incluindo metadados personalizados)
&#x200B;* [Scripting]&#x200B;[Python] Adicionar função à lista de consulta de nomes de malha por conjunto de textura
&#x200B;* [Conteúdo] Adicionar novo modelo do Blender e exportar predefinição

**Corrigido:**

&#x200B;* [MacOS] Falha ao iniciar o Iray em alguns casos
&#x200B;* [Miniaturas] As miniaturas de prateleira não são carregadas corretamente
&#x200B;* Vários canais UV são ignorados
&#x200B;* [Desempacotar automaticamente] Cálculo desnecessário ao dividir ilhas longas
&#x200B;* [Auto Unwrap] Opção para evitar ilhas alongadas não considerada
&#x200B;* [Desembaçamento automático] Perda de dados extras (cores de vértice) ao recompactar UVs
&#x200B;* [UI] Barra de rolagem horizontal na janela de propriedades quando o Gerenciamento de cores está ativado
&#x200B;* [Gerenciamento de cores] As configurações OCIO não têm a função substance\_3d\_painter\_standard\_srgb
&#x200B;* [Gerador] Uso incorreto de dados do usuário “desativado”
&#x200B;* [Gerenciamento de cores] A lista suspensa Espaço de cor “Não compatível” não deve ser clicável
&#x200B;* [Gerenciamento de cores]&#x200B;[Shader] A definição de substituição sRGB não funciona mais
&#x200B;* [Gerador] Uso incorreto de dados do usuário “disable”
&#x200B;* [Pilha de camadas] Visualizações quebradas com projetos de blocos UV
&#x200B;* [Shader] A documentação da API não está totalmente atualizada com os normais tortos
&#x200B;* [Exportar]&#x200B;[Interoperabilidade] Não é possível enviar para o Stager com caracteres especiais
&#x200B;* [Conteúdo] Algumas miniaturas de predefinições de pincel estão vazias ou muito escuras

**Problemas Conhecidos:**

&#x200B;* [Gerenciamento de cores] As conversões do espaço de cores HDR com ACE no Linux produzem cores vivas
&#x200B;* [Pilha de camadas] A fonte de entrada não é salva por camada
&#x200B;* [Falha] Ctrl Z Após excluir uma instância de sombreador
&#x200B;* [Iray] IoR bloqueada em 1 para alguns sombreadores
&#x200B;* [Shader] Falha com o antigo sombreador defeituoso

### 8.1.1

*(Lançado: 28 de junho de 2022)*
Resumo: **Hotfix de versão secundária**

**Adicionado:**

&#x200B;* [Pilha de camadas] Alt - clicar na máscara não desmarca mais os efeitos

**Corrigido:**

&#x200B;* [Falha] Abrir projeto antigo salvo no modo de exibição solo
&#x200B;* [Falha] Excluir um gerador nas propriedades
&#x200B;* [Configurações do conjunto de textura] A mistura de Oclusão Normal/Ambiente e o height para os métodos normais estão quebrados
&#x200B;* [Exportar] Exportar texturas usando o preenchimento de difusão renderiza mapas em preto

**Problemas Conhecidos:**

&#x200B;* [MacOS] Falha ao lançar Iray em Monterey
&#x200B;* [Visualizar miniatura] As miniaturas simplificadas não são atualizadas quando uma âncora é usada
&#x200B;* [Gerenciamento de cores] As conversões do espaço de cores HDR com ACE no Linux produzem cores vivas

### 8.1.0

*(Lançado: 07 De junho De 2022)*
Resumo: **Versão principal com suporte ICC, dimensionamento de material com base em dados de tamanho físico, novos panificadores, melhorias de conta-gotas de cores e uma variedade de conteúdos adicionais**

**Adicionado:**

&#x200B;* [Gerenciamento de cores] Adicione suporte para perfis ICC com Adobe Color Engine (ACE)
&#x200B;* [Gerenciamento de cores] Adicione suporte para “Adobe 98 RGB” como espaço de cores de trabalho para ICC
&#x200B;* [Gerenciamento de cores] Permita definir as configurações de ACE/ICC por meio de um arquivo de configuração
&#x200B;* [Gerenciamento de cores] Permitir a entrada de valores de cor linear no Seletor de cores com o modo Legado
&#x200B;* [Gerenciamento de cores] Permite especificar o perfil de cores usado para escolher a cor fora da interface do usuário
&#x200B;* [Gerenciamento de cores] Lembrar o último valor de exibição escolhido na viewport
&#x200B;* [Gerenciamento de cores]&#x200B;[Substance] Faça com que os geradores/filtros funcionem corretamente com o Gerenciamento de cores
&#x200B;* [Gerenciamento de cores]&#x200B;[Substance] Adicionar novas palavras-chave de substituição colorspace $working e $standardsrgb
&#x200B;* [Tamanho físico]&#x200B;[Mecanismo] Extrair informações de tamanho físico da malha
&#x200B;* Cálculo do Tamanho físico [Tamanho físico]&#x200B;[Mecanismo]
&#x200B;* [Tamanho físico] Expor as opções para usar o tamanho físico na interface do usuário
&#x200B;* [Tamanho físico] Adicionar auxiliares visuais na viewport
&#x200B;* [Preparação] Adicionar Height
&#x200B;* [Cozimento] Adicionar padeiro de normais curvados
&#x200B;* [Preparação] Adicionar padeiro de opacidade
&#x200B;* [Conta-gotas] Nova visualização de conta-gotas de cor ao lado do mouse e gerenciamento de cores
&#x200B;* [Conta-gotas] O painel Seletor de cores reaparece em sua última posição quando reaberto
&#x200B;* [Conta-gotas] Um novo ícone para o Seletor de materiais
&#x200B;* [Conta-gotas] Gerenciamento de cores da visualização do canal do seletor de cores
&#x200B;* [Conta-gotas] Adicionar a funcionalidade de clicar para selecionar ao conta-gotas
&#x200B;* [Conta-gotas] O seletor de material não ativa mais canais não ativos
&#x200B;* [Conta-gotas] Permitir o uso do conta-gotas com um atalho
&#x200B;* [Conta-gotas] O conta-gotas seleciona o canal relevante, quando aplicável
&#x200B;* [Conta-gotas] Entrar no modo de seletor de cores desativa todos os atalhos
&#x200B;* [Conta-gotas] Remove a seleção automática do campo hexadecimal
&#x200B;* [Conta-gotas] Não fechar o painel ao usar o seletor de material
&#x200B;* [Conta-gotas] Novo estado desativado quando o canal não está disponível para seleção
&#x200B;* [Exportar] Adicionar o atributo tangente à exportação de glTF
&#x200B;* Atualize o Substance Engine para v8.4
&#x200B;* Atualizar a quebra automática para 0. 9. 0
&#x200B;* Atualize para Qt 5.15.8
&#x200B;* Atualização para o Python 3.9
&#x200B;* [Shader] Adicionar suporte para sombreamento Bent Normals
&#x200B;* [MacOS] Suporte a 3DConnection SpaceMouse
&#x200B;* [Python] Documentar a versão Python usada na API
&#x200B;* [Conteúdo] Adicione 6 novos ruídos 3D com 105 predefinições
&#x200B;* [Content] 20 novos mapas de desgaste e 2 padrões de dobras de pano
&#x200B;* [Content] Atualizar a predefinição de exportação “Mapas de malha” para usar novos padeiros
&#x200B;* [Conteúdo] A Inclinação de desfoque e o filtro de distorção dependem da resolução do conjunto de texturas
&#x200B;* [Conteúdo] Atualize projetos de amostra para usar os 3 novos padeiros

**Corrigido:**

&#x200B;* [glTF] Não é possível abrir glTF com caractere especial
&#x200B;* [Engine] Artefatos com anisotropia e SVT desativados
&#x200B;* Os Materiais inteligentes do [MacOS]&#x200B;[M1] não são exibidos corretamente
&#x200B;* [Processamento de malha] Não é possível importar malhas do Modeler
&#x200B;* [UI] Barra de rolagem horizontal na janela do novo projeto com o Gerenciamento de cores ativado
&#x200B;* [Gerenciamento de cores] Valor de espaço de trabalho ausente no seletor de cores com algumas configurações de OCIO
&#x200B;* [Gerenciamento de cores] A visualização do pincel na janela de visualização não é gerenciada por cores
&#x200B;* [SpaceMouse] A tabela dinâmica não é atualizada imediatamente com alteração de foco e às vezes fora do modelo
&#x200B;* [Export]&#x200B;[USD] Os arquivos USD exportados têm uma estrutura incorreta
&#x200B;* Problema de Oclusão de ambiente do [USD] ao exportar
&#x200B;* [Conteúdo] Atualizar a malha da miniatura para corresponder ao projeto de amostra da esfera de visualização

**Problemas Conhecidos:**

&#x200B;* Exportar texturas usando o preenchimento de difusão renderiza mapas em preto
&#x200B;* A mistura normal/Oclusão de ambiente está quebrada
&#x200B;* [MacOS] Falha ao iniciar o Iray em alguns casos raros
&#x200B;* [Visualizar miniatura] As miniaturas simplificadas não são atualizadas quando uma âncora é usada
&#x200B;* [Gerenciamento de cores] As conversões do espaço de cores HDR com ACE no Linux produzem cores apertadas

## Versão 7

### 7.4.3

*(Lançado: 11 De abril De 2022)*
Resumo: **Correção de erro com suporte a SpaceMouse 3Dconnection em Visor 2D**

**Adicionado:**

&#x200B;* [SpaceMouse] Suporte a 3DConnection SpaceMouse em Visor 2D

**Corrigido:**

&#x200B;* [Seletor de cores] Não é possível gravar em campo hexadecimal
&#x200B;* [Gerenciamento de cores] Os recursos usados no modo de projeção não são gerenciados por cores na sobreposição
&#x200B;* [Gerenciamento de cores] Os erros não são relatados no registro
&#x200B;* [SpaceMouse] Remove a mensagem de erro genérica se o usuário não tiver um SpaceMouse
&#x200B;* [SpaceMouse] Ao carregar um projeto, o ponto dinâmico é sempre oculto
&#x200B;* [Baker] A configuração “Média normal” não tem efeito em projetos do Bloco UV
&#x200B;* [Bloco UV] As sobreposições de blocos uv inativos desaparecem ao recarregar a malha com blocos diferentes
&#x200B;* [Scripting]&#x200B;[Python] O script remoto está corrompido
&#x200B;* [Scripting]&#x200B;[Python] Vários canais não podem ser consultados pela API e isso gera um erro
&#x200B;* [Scripting]&#x200B;[Python] Falha ao usar o evento ProjectEditionEntered
&#x200B;* [Scripting]&#x200B;[Python] Falha ao chamar get\_ative\_stack()

**Problemas Conhecidos:**

&#x200B;* Espaço de conexão 3Dsem suporte para mouse no MacOS
&#x200B;* [UI] Barra de rolagem horizontal com gerenciamento de cores exibida em alguns casos em uma nova janela do projeto
&#x200B;* [Mac M1] Os Materiais inteligentes não são exibidos corretamente

### 7.4.2

*(Lançado: 08 De março De 2022)*
Resumo: **Correção de erros com suporte a 3Dconnection SpaceMouse e melhorias no gerenciamento de cores (OCIO)**

**Adicionado:**

&#x200B;* [SpaceMouse]&#x200B;[Windows] Suporte ao SpaceMouse 3Dconnection na Janela de Visualização 3D para navegação
&#x200B;* [SpaceMouse]&#x200B;[Windows] Atalhos/teclas básicos para modelos Pro e Enterprise SpaceMouse no visor 3D
&#x200B;* [SpaceMouse]&#x200B;[Windows] Ícone do centro de rotação dedicado no visor 3D
&#x200B;* [Gerenciamento de cores] Usar funções da configuração OCIO para alterar as configurações padrão
&#x200B;* [Gerenciamento de cores] Gerenciamento de cores na janela de propriedades dos widgets de cores
&#x200B;* [Gerenciamento de cores] Gerenciamento de cores na janela de propriedades para visualização de material
&#x200B;* [Gerenciamento de cores] Amostras de gerenciamento de cores no seletor de cores
&#x200B;* [Gerenciamento de cores] Adicionar uma configuração para definir o espaço de cores sRGB padrão
&#x200B;* [Gerenciamento de cores] Adicionar o espaço de cores sRGB padrão da configuração OCIO no seletor de cores Lista de seletores de exibição
&#x200B;* [Gerenciamento de cores] Melhorias para o menu de substituição do espaço de cores
&#x200B;* [Gerenciamento de cores] Permitir substituição do espaço de cores do mapa de ambiente nas Configurações de exibição
&#x200B;* [Gerenciamento de cores] Desenhar gradientes do seletor de cores com base na exibição atual
&#x200B;* [Gerenciamento de cores] Valores HDR do suporte por padrão no editor de cores
&#x200B;* [Gerenciamento de cores] Usar passagem (sem espaço de cores) para filtros no modo Legado
&#x200B;* [Gerenciamento de cores] Limitar a exibição de gradientes no editor de cores para corresponder ao intervalo [0-1]
&#x200B;* [Gerenciamento de cores] Ocultar seletor de exibição no seletor de cores no modo Legado
&#x200B;* [Gerenciamento de cores] Tornar o seletor de cores hexadecimal sempre no espaço de cores sRGB
&#x200B;* [Gerenciamento de cores] Desativar menu suspenso Exibição do seletor de cores para canais de dados
&#x200B;* [Otimização] A grade de distorção recalcula apenas blocos UV cobertos
&#x200B;* [Exportar] Permitir a exportação de projetos de Bloco UV para Sketchfab, USD e glTF
&#x200B;* [Scripting]&#x200B;[Python] Permitir a alteração da função de mapeamento de tom

**Corrigido:**

&#x200B;* [Sketchfab] A atualização do modelo existente acaba criando um novo modelo
&#x200B;* [Sketchfab] Falha ao procurar modelo atualizado anteriormente
&#x200B;* Falha ao exportar para USD
&#x200B;* Falha ao criar uma nova ocorrência de sombreador na Máscara de geometria ou quando a geometria está oculta
&#x200B;* [Janela Importar ativo] Falha ao alterar o tipo de recursos importados
&#x200B;* Os mapas de malha normal são invertidos quando usados em uma pilha de camadas
&#x200B;* [Substance] O modo de mesclagem de dados do usuário não é levado em consideração
&#x200B;* [Gerenciamento de cores] Bitmaps com espaço de cor no nome do arquivo são importados como sequências de Bloco UV
&#x200B;* [Gerenciamento de cores] As saídas gerenciadas por cores do gráfico de Substance estão no espaço de cores incorreto
&#x200B;* [Gerenciamento de cores] A ferramenta Preenchimento de polígono exibe a cor errada
&#x200B;* [Gerenciamento de cores] O mapeador de tons ACES é aplicado a canais no modo solo
&#x200B;* [Gerenciamento de cores] A visualização da ferramenta de iluminação da esfera não é gerenciada por cores
&#x200B;* [Gerenciamento de cores]&#x200B;[Exportar] Mapas convertidos aplicam uma conversão incorreta
&#x200B;* [Scripting]&#x200B;[Python]&#x200B;[Color Management] Projetos criados com modelo e variável de ambiente OCIO estão no modo Legado
&#x200B;* [Scripting]&#x200B;[Python] Não é possível usar a função de avaliação JavaScript na inicialização
&#x200B;* [Oferta de Adobe 3D] Não é possível iniciar o Painter ao usar configurações regionais com idiomas não compatíveis por padrão

**Problemas Conhecidos:**

&#x200B;* Espaço de conexão 3Dsem suporte para mouse no MacOS
&#x200B;* [UI] Barra de rolagem horizontal com gerenciamento de cores exibida em alguns casos em uma nova janela do projeto
&#x200B;* [Baker] A configuração “Média normal” não tem efeito em projetos do Bloco UV
&#x200B;* [Mac M1] Os Materiais inteligentes não são exibidos corretamente
&#x200B;* [Gerenciamento de cores] Os recursos usados no modo de projeção não são gerenciados por cores na sobreposição
&#x200B;* [Seletor de cores] Não é possível gravar em campo hexadecimal

### 7.4.1

*(Lançado: 14 De dezembro De 2021)*
Resumo: **Correção de erros com melhorias no gerenciamento de cores**

**Adicionado:**

&#x200B;* [Gerenciamento de cores] Usar função de dados em nomes de arquivos exportados
&#x200B;* [Gerenciamento de cores] Expanda a seção Gerenciamento de cores, por padrão, quando o OCIO for selecionado nas janelas de novo projeto e configurações do projeto
&#x200B;* [Gerenciamento de cores] Adicionar mapeador de tons ACE no modo herdado
&#x200B;* [Gerenciamento de cores] Ajuste as configurações padrão
&#x200B;* [Gerenciamento de cores]&#x200B;[Exportar] Preencher $colorSpace nos nomes de arquivos para canais de dados
&#x200B;* [Exportar] Exportar projeto do Bloco UV para o Stager
&#x200B;* [Interoperabilidade] Não disponível para as edições Steam e Substance
&#x200B;* [Interoperabilidade] Permitir o envio de um projeto de Bloco UV para o Stager

**Corrigido:**

&#x200B;* [MacOS]&#x200B;[Falha] O Painter não começa com o Catalina
&#x200B;* [Gerenciamento de cores]&#x200B;[Falha] Falha aleatória ao reproduzir o tipo de dados/gerenciamento de cores no canal do usuário
&#x200B;* [Gerenciamento de cores] Recursos usados como tons de cinza no novo menu Espaço de cores de exibição de máscara
&#x200B;* [Gerenciamento de cores] O canal do usuário é mais escuro na viewport no modo legado + visualização individual
&#x200B;* [Gerenciamento de cores] O mapa de ambiente é sempre linear quando usado no iRay
&#x200B;* [Gerenciamento de cores] O seletor de cores não seleciona o valor correto para o canal de dados no modo herdado
&#x200B;* [Gerenciamento de cores] O seletor de cores está quebrado dentro de um Substance no modo herdado
&#x200B;* [Gerenciamento de cores] Alternar entre exibições de canal solo na viewport não é exibido com o espaço de cor certo ao usar o menu suspenso
&#x200B;* [Gerenciamento de cores] Exportar aplica a conversão incorreta em canais de usuário com gerenciamento de cores no modo herdado
&#x200B;* Os traçados feitos na máscara de exibição individual não são exibidos ao voltar para a exibição de material
&#x200B;* [Exportar] Mapas convertidos não são exportados como canais com gerenciamento de cores
&#x200B;* [Texture Set] A dica de ferramenta com o nome original está ausente em canais de usuário renomeados
&#x200B;* [Steam] Arquivos ausentes ao verificar a integridade do arquivo com o Steam

**Problemas Conhecidos:**

&#x200B;* [Mac M1] Os materiais inteligentes não são exibidos corretamente

### 7.4.0

*(Lançado: 24 De novembro De 2021)*
Resumo: **Versão principal. Introdução da 1ª versão de gerenciamento de cores, desencaixe da exibição 2D ou 3D, nova opção de desencapsulamento automático UV para evitar ilhas alongadas, chame funções JavaScript da API Python e novo conteúdo**

**Adicionado:**

&#x200B;* [Gerenciamento de cores] Suporte ao gerenciamento de cores OpenColorIO versão 2
&#x200B;* [Gerenciamento de cores] Adicionar configurações de gerenciamento de cores às configurações do projeto
&#x200B;* [Gerenciamento de cores] Janela de aviso sobre as alterações de configuração do Gerenciamento de cores ao abrir um projeto
&#x200B;* [Gerenciamento de cores] Exibe uma mensagem de erro se um arquivo de configuração OCIO inválido for selecionado
&#x200B;* [Gerenciamento de cores] Permite substituir a configuração pela variável de ambiente OCIO
&#x200B;* [Gerenciamento de cores] Várias configurações OCIO integradas por padrão ao aplicativo
&#x200B;* [Gerenciamento de cores] Extrair o nome do espaço de cores do nome de arquivo bitmap importado
&#x200B;* [Gerenciamento de cores] Permite substituir o espaço de cores por um espaço de cores da configuração na janela Propriedades
&#x200B;* [Gerenciamento de cores] Adicione opções de gerenciamento de cores nas Configurações do conjunto de texturas
&#x200B;* [Gerenciamento de cores]&#x200B;[Janela de visualização] Permita o gerenciamento de cores de exibições 2D e 3D separadamente
&#x200B;* [Gerenciamento de cores] Carregue e converta o mapa de ambiente para o espaço de cores de trabalho
&#x200B;* [Gerenciamento de cores] Ajustar o seletor e editor de cores com o espaço de cores atual
&#x200B;* [Gerenciamento de cores] Permite selecionar o espaço da cor de transformação de vídeo no visor com um novo menu suspenso
&#x200B;* [Gerenciamento de cores] Aplicar transformação de exibição com resultados de renderização de matriz
&#x200B;* [Gerenciamento de cores] Exportar texturas com espaços de cores diferentes
&#x200B;* [Gerenciamento de cores]&#x200B;[Python] Aplicar configurações de gerenciamento de cores da variável de ambiente (OCIO) aos novos projetos
&#x200B;* [Visor] Permite desencaixar o visor 2D ou 3D
&#x200B;* [Desempacotamento automático] Nova opção para evitar ilhas alongadas
&#x200B;* [Scripting Python] Chamar funções JavaScript da API Python
&#x200B;* [Janela Novo projeto] Tornar a seção de mapas importados flexível
&#x200B;* [Projeção]&#x200B;[Distorcer] Permite ocultar normais como uma opção nas configurações de Distorção
&#x200B;* [Conteúdo] 11 novos mapas de desgaste
&#x200B;* [Conteúdo] 8 novas predefinições de ferramenta (zíper, cabo de aperto, brilho)
&#x200B;* [Conteúdo] 8 novos materiais (cicatriz, bolso, ...)
&#x200B;* [Conteúdo] 1 novo gerador (inflar deformação)

**Problemas Conhecidos:**

&#x200B;* [Mac M1] Os materiais inteligentes não são exibidos corretamente
&#x200B;* [Gerenciamento de cores]&#x200B;[Falha] Falha aleatória ao reproduzir o tipo de dados/gerenciamento de cores no canal do usuário
&#x200B;* [Gerenciamento de cores] O seletor de cores não seleciona o valor correto para o canal de dados no modo herdado
&#x200B;* [Gerenciamento de cores]&#x200B;[Iray] Salvar a renderização em EXR ou TIFF enquanto o Gerenciamento de cores está ativado na janela de visualização sempre será salvo em linear
&#x200B;* [Gerenciamento de cores] Os recursos usados como tons de cinza na máscara exibem o menu Espaço de cores errado
&#x200B;* [Color Management]&#x200B;[Iray] O mapa de ambiente é sempre linear quando usado em Iray
&#x200B;* [Gerenciamento de cores]&#x200B;[Exportar] Os mapas convertidos não são exportados como canais gerenciados por cores
&#x200B;* [Gerenciamento de cores]&#x200B;[Exportar] A exportação ignora se o canal do usuário é gerenciado por cores ou não com o modo legado

### 7.3.1

*(Lançado: 24 De novembro De 2021)*
Resumo: **Correção de erros**

**Adicionado:**

&#x200B;* [Projeção] O dimensionamento deve funcionar somente no Espaço do objeto

**Corrigido:**

&#x200B;* [Mac M1] Camadas de material não funcionam
&#x200B;* [Mac M1]&#x200B;[Projeção] A distorção não funciona
&#x200B;* Os microdetalhes não são exibidos corretamente
&#x200B;* [Projeção]&#x200B;[Falha] Alternar para o modo de distorção com uma camada criada com uma versão anterior
&#x200B;* [Projeção]&#x200B;[Distorcer] O recurso Inverter não funciona quando a transformação está definida como espaço global
&#x200B;* [Projeção]&#x200B;[Distorcer] A opção Dividir permanece selecionada após a conclusão da divisão
&#x200B;* [Projeção]&#x200B;[UV] O ponto dinâmico é redefinido ao inverter a projeção
&#x200B;* [Filtro] O ambiente de Iluminação do forno está mudando ao recarregar ou alterar um parâmetro
&#x200B;* [Interoperabilidade] Não disponível para as edições Steam e Substance
&#x200B;* [Interoperabilidade] O botão “Pesquisar ativos 3D no Marketplace” sempre deve abrir o CCD na guia Stock e Marketplace 3D

**Problemas Conhecidos:**

&#x200B;* [Mac M1] Os materiais inteligentes não são exibidos corretamente

### 7.3.0

*(Lançado: 13 De outubro De 2021)*
Resumo: **Versão principal. Contém uma nova projeção de distorção 3D, uma nova projeção cilíndrica, melhorias no seletor de cores, novas funções na API Python e correções de erros**

**Adicionado:**

&#x200B;* [Projeção]&#x200B;[Distorcer] Expor distorção 3D como um novo modo de projeção
&#x200B;* [Projeção]&#x200B;[Distorcer] Permitir modo de decalque para Alpha, Texturas e Procedimentos com arrastar e soltar no visor
&#x200B;* [Projeção]&#x200B;[Distorcer] Usar projeção de distorção com atalho de decalque (ALT)
&#x200B;* [Projeção]&#x200B;[Distorcer]&#x200B;[Barra de ferramentas] Transformar distorção como um todo ou por vértices
&#x200B;* [Projeção]&#x200B;[Distorcer]&#x200B;[Barra de ferramentas] Adicionar pontos de grade com opções dividir distorção cruzada, horizontal ou verticalmente
&#x200B;* [Projeção]&#x200B;[Distorção]&#x200B;[Barra de ferramentas] Menu dedicado para ações de redefinição
&#x200B;* [Projeção]&#x200B;[Distorção]&#x200B;[Barra de ferramentas] Opção para ajustar automaticamente as tangentes ao mover os pontos
&#x200B;* [Projection]&#x200B;[Warp]&#x200B;[Toolbar] Menu dedicado para edição de grade (tamanho, redefinição, cor e tamanho da alça)
&#x200B;* [Projeção]&#x200B;[Distorcer] Novo atalho de teclado para alternar o modo de edição de distorção de vértices inteiros (SHIFT+V)
&#x200B;* [Projeção]&#x200B;[Distorcer] Clicar + Ctrl permite alternar entre a ferramenta de superfície e outras ferramentas
&#x200B;* [Projeção]&#x200B;[Cilíndrica] Expor o modo de projeção cilíndrica
&#x200B;* [Projeção]&#x200B;[Barra de ferramentas] Configurações do manipulador de grupo (tamanho, etapas da grade, etapas do ângulo)
&#x200B;* [Seletor de cores] Nova interface do seletor de cores
&#x200B;* [Seletor de cores] Usar valores sRGB nos widgets do seletor de cores
&#x200B;* [Seletor de cores] Permite salvar e excluir amostras de cores
&#x200B;* [Seletor de cores] Conta-gotas acessível por meio de cores e slots normais
&#x200B;* [Seletor de cores] Permite editar cores dinâmicas entre 0 e 255 valores
&#x200B;* [Seletor de cores] Tornar o estado HSV/RGB comum no aplicativo
&#x200B;* [Seletor de cores] A janela do Seletor de cores é semipersistente
&#x200B;* [Seletor de cores] Pressionar Esc fecha a janela do seletor de cores
&#x200B;* Melhoria de desempenho para interação de interface e ao pintar
&#x200B;* [Engine] Atualização para a nova versão do mecanismo de Substance (8.3.0)
&#x200B;* [Scripting]&#x200B;[Python] Permite recarregar a malha do projeto atual
&#x200B;* [Scripting]&#x200B;[Python] Permitir atualização de recursos em projetos
&#x200B;* [Scripting]&#x200B;[Python] Permite definir e consultar a resolução de Blocos UV
&#x200B;* [Interoperabilidade] Não disponível para as edições Steam e Substance
&#x200B;* [Interoperabilidade] Receber vários recursos do Bridge

**Corrigido:**

&#x200B;* O seletor de cores não exibe a cor correta
&#x200B;* [Fazendo bake] A lista de conjuntos de texturas não está ordenada corretamente
&#x200B;* [Importação de FBX] As transformações de tabela dinâmica de grupo do 3ds Max não são levadas em consideração
&#x200B;* [Substance Engine] Falha com importação de SBSAR corrompido
&#x200B;* [MacOS] A opção de configuração do projeto em idiomas diferentes não está presente
&#x200B;* Os salvamentos automáticos podem congelar o Painter durante processos longos

**Problemas Conhecidos:**

&#x200B;* [Projeção]&#x200B;[Distorcer] A opção Dividir permanece selecionada após a conclusão da divisão
&#x200B;* [Projeção]&#x200B;[Distorcer] O recurso Inverter não funciona quando a transformação está definida como espaço global
&#x200B;* [Projeção]&#x200B;[Distorção] Linhas de artefato entre correções em alguns casos raros
&#x200B;* [Projeção]&#x200B;[UV] O ponto dinâmico é redefinido ao inverter a projeção
&#x200B;* [Mac M1] Os Materiais inteligentes não são exibidos corretamente
&#x200B;* [M1]&#x200B;[Regressão] Camadas de material não funcionando

### 7.2.3

*(Lançado: 24 De agosto De 2021)*
Resumo: **versão secundária, correção de erro**

**Adicionado:**

&#x200B;* [Bibliotecas] Adicionar uma maneira de impedir que arquivos indesejados sejam rastreados

**Corrigido:**

&#x200B;* [Win] Problemas de suspensão e várias telas
&#x200B;* [MacOS]&#x200B;[Falha] Alternar sombreador ao usar efeitos
&#x200B;* [Visor] O modo de visualização completa não mostra mais o cursor do pincel sem alfa
&#x200B;* [IU] O widget Ângulo gira na direção errada
&#x200B;* [Pilha de camadas] Muitas subpastas criam um congelamento muito longo
&#x200B;* [Iray] Visualizações diferentes em Iray e OpenGL: Visível se não estiver funcionando
&#x200B;* [Iray] Índice de refração não levado em conta e não aparece nas propriedades mdl
&#x200B;* [JavaScript] ShowExportDialog() nunca retorna true
&#x200B;* Não é possível ler o mtl do Adobe Stock

### 7.2.2

*(Lançado: 27 de julho de 2021)*
Resumo: **versão secundária, correção de erro**

**Adicionado:**

&#x200B;* Atualizar versão de requisitos de driver AMD

**Corrigido:**

&#x200B;* [Mac M1] Detecção de memória incorreta
&#x200B;* [Exportar] Caminhos muito longos não são exibidos corretamente

**Problemas Conhecidos:**

&#x200B;* [Conteúdo] Sombreadores desatualizados das amostras

### 7.2.1

*(Lançado em: 2 de julho de 2021)*
Resumo: **Versão secundária, Hotfix**

**Adicionado:**

&#x200B;* [Interop] Adicione uma dica de ferramenta para informar que ainda não há suporte ao envio de projetos do Bloco UV para o Stager
&#x200B;* [Plug-in]&#x200B;[IU] Atualização do ícone do Livelink

**Corrigido:**

&#x200B;* [Nvidia] A versão do driver começando com 30 é considerada desatualizada
&#x200B;* [Bibliotecas] O estado do painel Ativos não é salvo, a menos que um projeto esteja aberto
&#x200B;* [Bibliotecas] A nova pesquisa salva mantém a palavra-chave da pesquisa salva antiga
&#x200B;* [Baker]&#x200B;[UVTiles] Mapas de ID por meshID também levam Blocos UV em consideração
&#x200B;* [Exportar] Arquivos gLTF não importam a cor do vértice
&#x200B;* [Iray] Algumas dicas de ferramentas estão ausentes
&#x200B;* [Interop] Enviar para o Stager nem sempre é desativado quando o Stager não é detectado
&#x200B;* [Resource Updater] O criador do pincel Photoshop não pode ser atualizado
&#x200B;* [Conteúdo] O gerador de desgaste de borda de vidro de fibra está quebrado

### 7.2.0

*(Lançado: 23 de junho de 2021)*
Resumo: **Versão principal, fornece uma atualização para o painel de ativos, um novo sombreador com acesso a novos canais e parâmetros, uma atualização geral da interface do usuário, algumas melhorias de desempenho muito solicitadas, suporte a idiomas expandido e muito mais!**

**Adicionado:**

&#x200B;* [Bibliotecas] Novo painel Ativo para substituir a prateleira
&#x200B;* [Libraries]&#x200B;[UI] Novo layout do painel Ativos
&#x200B;* [Bibliotecas]&#x200B;[IU] Alterar a orientação padrão do painel Ativos e a interface do usuário
&#x200B;* [Bibliotecas]&#x200B;[IU] Introduzir uma opção de exibição de lista na biblioteca
&#x200B;* [Bibliotecas]&#x200B;[IU] Nova navegação de trilha no Painel de ativos
&#x200B;* [Bibliotecas]&#x200B;[IU] Selecione “Todas as bibliotecas” ao selecionar uma pesquisa salva
&#x200B;* [Bibliotecas]&#x200B;[IU] Selecione “Todas as bibliotecas” quando todas as pastas estiverem desmarcadas
&#x200B;* [Libraries]&#x200B;[UI] Nova marca para pincéis de partícula
&#x200B;* [Bibliotecas]&#x200B;[IU] Substituído “prateleira” por “Todas as bibliotecas” no aplicativo
&#x200B;* [Bibliotecas]&#x200B;[IU] Permitir ocultar pastas vazias
&#x200B;* [Libraries]&#x200B;[UI] A biblioteca de usuário padrão deve estar visível mesmo que vazia
&#x200B;* [Bibliotecas]&#x200B;[IU] Novo método de filtragem por meio de ícones de tipo de ativo
&#x200B;* [Bibliotecas] Atalho “CTRL” para selecionar vários tipos de ativos
&#x200B;* [Bibliotecas] Nova variável de ambiente para controlar o orçamento de memória de visualização do ativo
&#x200B;* [Bibliotecas]&#x200B;[Conteúdo] Novos mapas de ambiente
&#x200B;* [Libraries]&#x200B;[Content]&#x200B;[UI] Renderizar deslocamento em materiais padrão
&#x200B;* [Bibliotecas]&#x200B;[Conteúdo] Definir sombreador de Adobe Standard Material (ASM) como padrão para a geração de visualizações
&#x200B;* [Bibliotecas]&#x200B;[Conteúdo]&#x200B;[ASM] Novos Modelos de Projeto para o novo sombreador ASM
&#x200B;* [Bibliotecas]&#x200B;[Miniatura] Usar o novo mapa de ambiente do Studio 6
&#x200B;* [Bibliotecas]&#x200B;[Miniatura] Ler miniatura no recurso em vez de gerá-lo
&#x200B;* [Bibliotecas]&#x200B;[Miniatura] Adicionar deslocamento à geração de miniaturas
&#x200B;* [Configurações do conjunto de texturas]
&#x200B;* [Configurações do conjunto de texturas]&#x200B;[IU] Expor novo height ao método de conversão normal
&#x200B;* [Configurações de conjunto de textura]&#x200B;[IU] Retrabalho da organização da interface do usuário dos canais
&#x200B;* [Configurações do conjunto de textura] Limite de canais do usuário aumentado para 16 canais
&#x200B;* [Configurações do conjunto de texturas]&#x200B;[IU] Indicar quais canais são compatíveis com o sombreador selecionado no momento
&#x200B;* [Shader]&#x200B;[ASM] Novo sombreador de material padrão da Adobe
&#x200B;* [Shader]&#x200B;[ASM] Suporte adicionado para Anisotropia, Revestimento transparente, Dispersão subsuperficial, Specular edge color e Brilho
&#x200B;* [Shader]&#x200B;[ASM] Alterar valores de cor dos canais padrão
&#x200B;* [Shader]&#x200B;[ASM]&#x200B;[Export] Modelo de exportação atualizado do Adobe Dimension para o Adobe Substance 3D Stager
&#x200B;* [Shader]&#x200B;[ASM] Rótulos e dicas de ferramentas adicionados para os parâmetros de sombreador e MDL
&#x200B;* [Shader]&#x200B;[ASM] Tornar a Cor da Dispersão visível na Exibição 2D mesmo se o SSS não for suportado
&#x200B;* [Shader]&#x200B;[ASM]&#x200B;[Iray] Suporte ao sombreador ASM no Iray com o novo MDL
&#x200B;* [Shader]&#x200B;[ASM]&#x200B;[Iray] Espalhamento de subsuperfície atualizado no brilho e na superfície revestida das especificações de PBR legadas
&#x200B;* [Shader]&#x200B;[ASM]&#x200B;[Content] Alterou o tipo de SSS padrão para amostras
&#x200B;* [Shader]&#x200B;[ASM] Documentação adicionada para a API do ASM
&#x200B;* [Shader]&#x200B;[ASM] Otimizar sombreadores para ignorar canais não usados
&#x200B;* [Shader] Expor novos canais de conjunto de textura
&#x200B;* [Shader] Dispersão de subsuperfície aprimorada
&#x200B;* [Shader] Novos parâmetros de sombreador ocultos para alguns sombreadores
&#x200B;* [Sombreador] Visível se for para parâmetros de sombreador
&#x200B;* [Desempenho]
&#x200B;* [Bibliotecas] Melhorias no tempo de carregamento da visualização de recursos e no desempenho do cálculo
&#x200B;* [Engine] Melhorias no desempenho da pintura
&#x200B;* [Abrir Automaticamente]
&#x200B;* [Desencapsulamento automático] Melhorias no desempenho da Embalagem
&#x200B;* [Auto Unwrap] Auto unwrap compatível com o fluxo de trabalho de bloco UV
&#x200B;* [Desenvolver automaticamente] Nova opção para posicionar UVs de acordo com a orientação da malha
&#x200B;* [Outro]
&#x200B;* [Configurações] Direção de zoom padrão alterada
&#x200B;* [UI] Atualização geral da interface do usuário
&#x200B;* [UI] Retrabalho do menu Ajuda
&#x200B;* [IU] Ícone Substituir inversão
&#x200B;* [UI]&#x200B;[Plug-in] Ícone de substituição do link dcc do plug-in
&#x200B;* [UI]&#x200B;[AMD] Atualizar a versão mínima necessária e a mensagem pop-up
&#x200B;* [Pilha de camadas] Cria nova camada dentro da pasta vazia selecionada
&#x200B;* Atualizar Documentação do Python
&#x200B;* [Marca]
&#x200B;* [Branding]&#x200B;[UI] Atualização do nome do aplicativo para Adobe Substance 3D Painter
&#x200B;* [Branding]&#x200B;[UI] Versão autônoma atualizada para &#39;Substance edition&#39;
&#x200B;* [Branding]&#x200B;[UI] Nome executável atualizado do aplicativo, caminho de instalação, pacote e ícones
&#x200B;* [Branding]&#x200B;[UI] Biblioteca e caminho padrão renomeados
&#x200B;* [Branding]&#x200B;[UI] Atualizado Sobre o Windows
&#x200B;* [Branding]&#x200B;[UI] Tela de boas-vindas atualizada
&#x200B;* [Branding]&#x200B;[UI] Número de versão anual removido
&#x200B;* [Localização] Novas traduções para alemão, francês e chinês simplificado
&#x200B;* [Interoperabilidade] Não disponível para as edições Steam e Substance
&#x200B;* [Interoperabilidade] Interoperabilidade com o ecossistema Adobe: Designer, Sampler, Stager e Bridge
&#x200B;* [Interoperabilidade]&#x200B;[IU] Receber e atualizar ativos do Designer
&#x200B;* [Interoperabilidade]&#x200B;[IU] Receber ativo do Sampler
&#x200B;* [Interoperabilidade]&#x200B;[IU] Enviar ativo para o Stager
&#x200B;* [Interoperabilidade]&#x200B;[IU] Mostrar no Adobe Bridge
&#x200B;* [Interoperabilidade]&#x200B;[IU] Permitir acesso rápido a ativos Adobe 3D
&#x200B;* [Interoperabilidade] Novas tags de uso do sbsar
&#x200B;* [Interoperabilidade] Gerenciar tipos de ativos recebidos
&#x200B;* [Interoperabilidade] Os ativos recebidos do Adobe Substance 3D Designer ou do Adobe Substance 3D Sampler são armazenados na biblioteca padrão escolhida pelo usuário
&#x200B;* [Interoperabilidade]&#x200B;[IU] Novo ícone na barra de ferramentas à esquerda para enviar ao Stager ou Photoshop

**Corrigido:**

&#x200B;* [Tablet] Baixo desempenho ao pintar com pressão
&#x200B;* [Tablet] Problema em tablets com controles deslizantes
&#x200B;* [Falha] Incompatibilidade de nome entre a lista do conjunto de texturas e o exportador
&#x200B;* [Falha]&#x200B;[Bibliotecas] Clique duas vezes em uma subbiblioteca
&#x200B;* [Bibliotecas] Problema ao Rastrear diretórios de bibliotecas
&#x200B;* [Bibliotecas] A linha de comando para forçar geração de visualização não funciona conforme o esperado
&#x200B;* [Bibliotecas]&#x200B;[Conteúdo] O filtro Ambiente de luz assada está preto por padrão
&#x200B;* [Linux]&#x200B;[MacOS]&#x200B;[Export Mesh] Não é possível importar glTF criado no Linux/MacOS
&#x200B;* [Linux] Arrastar e soltar um arquivo no painel Ativos pode causar uma falha
&#x200B;* [Desfazer quebra automática] O ajuste automático está disponível mesmo se uma malha não tiver sido selecionada para recarregamento
&#x200B;* [Partículas] Comportamento de partícula incorreto com a gravidade
&#x200B;* [Pilha de camadas] O histograma de nível só pode usar a Luminância com alguns canais
&#x200B;* [Máscara de geometria] O menu do botão direito do mouse em uma pasta quando a edição da máscara de geometria não funciona
&#x200B;* [Projeção] Costura com projeção esférica e filtragem bilinear
&#x200B;* [UV Tiles] Exportar máscara para arquivo exporta somente bloco 0, 0
&#x200B;* [Exportar malha] A exportação de malha FBX está vazia
&#x200B;* [Iray] O mapa normal não é levado em consideração em novos projetos ao renderizar
&#x200B;* [Salvar] Problemas ao salvar em unidades compartilhadas
&#x200B;* [Preparação] Reassentar uma malha com parâmetros modificados exibe um aviso
&#x200B;* [Cozimento]&#x200B;[Regressão] Resultado incorreto quando a caixa delimitadora global de grandes malhas polidas não inclui a origem da cena
&#x200B;* [Python] Bibliotecas de usuários personalizadas não são levadas em consideração

**Problemas Conhecidos:**

&#x200B;* [Bibliotecas] As pesquisas salvas não são salvas se nenhum projeto for aberto
&#x200B;* [NVIDIA] Mensagem para driver desatualizado mesmo se o driver estiver atualizado

### 7.1.1 (2021.1.1)

*(Lançado: 23 De março De 2021)*
Resumo: **Versão secundária, correção de erro com possibilidade de inserir valores hexadecimais no seletor de cores**

**Adicionado:**

&#x200B;* [Log] Avisa os usuários sobre drivers de GPU AMD incompatíveis
&#x200B;* [Seletor de cores] Permite digitar valores hexadecimais

**Corrigido:**

&#x200B;* [Baker] Queda no desempenho
&#x200B;* [Máscara de geometria] Clicar com a tecla Alt pressionada no nome da malha pode levar a um travamento
&#x200B;* [Mecanismo] A pintura não atualiza toda a exibição quando necessário
&#x200B;* [Pilha de camadas] A seleção trava após alterar o sombreador
&#x200B;* [MacOS]&#x200B;[Seletor de cores] A cor é um pouco diferente da selecionada
&#x200B;* [Exportar] O uso do formato de arquivo PSD não gera um arquivo por Bloco UV
&#x200B;* [Scripting]&#x200B;[Javascript] alg.mapexport.getPathsExportDocumentMaps() não retorna todos os valores
&#x200B;* [Scripting]&#x200B;[Python] Os plug-ins desativados são ativados novamente ao reabrir o Painter

### 7.1.0 (2021.1.0)

*(Lançado: 28 De Janeiro De 2021)*
Resumo: **Versão principal, nova Máscara de geometria que permite selecionar e pintar partes da geometria, efeitos de cópia/colagem na pilha de camadas, melhoria do fluxo de trabalho de Bloco UV, atualização do Iray, Padeiros, Substance Engine e novo conteúdo**

**Adicionado:**

&#x200B;* Nova máscara de geometria e pintar partes selecionadas da geometria
&#x200B;* [Máscara de geometria] Permite pintar partes selecionadas da geometria por nomes de malha
&#x200B;* [Máscara de geometria] Seleção retangular em ambas as viewports
&#x200B;* [Máscara de geometria] Permite ocultar/ignorar a geometria excluída em qualquer camada
&#x200B;* [Máscara de geometria]&#x200B;[Propriedades] Seleção rápida de caixas de seleção com clicar e arrastar
&#x200B;* [Máscara de geometria]&#x200B;[Propriedades]&#x200B;[IU] Incluir/Excluir tudo com um menu suspenso na janela Propriedades
&#x200B;* [Máscara de geometria]&#x200B;[Propriedades] Permite selecionar rapidamente um item em uma lista com ALT+CLIQUE ESQUERDO
&#x200B;* [Máscara de geometria]&#x200B;[Propriedades] Sobreposição em viewports ao passar o mouse sobre nomes de malha/blocos UV na janela Propriedades
&#x200B;* [Máscara de geometria]&#x200B;[Pilha de camadas] Adicionar opções de copiar/colar à máscara de geometria
&#x200B;* [Máscara de geometria] Novo ícone do botão Ocultar/ignorar geometria excluída
&#x200B;* [Máscara de geometria] Nova dica de ferramenta para Ocultar/ignorar geometria excluída
&#x200B;* [Máscara de geometria] Atalho de teclado ALT+H para ativar/desativar o botão “ocultar ignorar geometria excluída”
&#x200B;* [Blocos UV]&#x200B;[Pilha de camadas] Nova miniatura de visualização da esfera da camada de preenchimento para blocos UV e modo simplificado
&#x200B;* [Blocos UV]&#x200B;[Pilha de camadas] Permitir sair facilmente da máscara de bloco UV
&#x200B;* [Blocos UV]&#x200B;[Lista de conjuntos de texturas] Permite dar uma descrição por Bloco UV
&#x200B;* [Blocos UV]&#x200B;[Configurações do conjunto de textura]&#x200B;[IU] Dois novos títulos de seção no menu suspenso para alterar a resolução do bloco UV
&#x200B;* [Blocos UV]&#x200B;[Visor] Sair da Máscara de bloco UV ao arrastar um material para o visor
&#x200B;* [Pilha de camadas] Adicionar opções de copiar/colar para efeitos
&#x200B;* [Pilha de camadas] Permitir copiar/colar efeitos de um conjunto de texturas para outro
&#x200B;* [Pilha de camadas] Permitir várias seleções de efeitos
&#x200B;* [Pilha de camadas] Adicionar opções de copiar/colar como atalhos para efeitos de camada
&#x200B;* [Pilha de camadas] Alternar automaticamente entre máscara e conteúdo ao arrastar efeitos para outra camada
&#x200B;* [Pilha de camadas] Criar automaticamente uma máscara ao colar uma máscara de outra camada
&#x200B;* [Pilha de camadas] Adicionar ações de efeito de movimento dentro do menu contextual de clique com o botão direito do mouse dos efeitos
&#x200B;* [Pilha de camadas] Permite arrastar e soltar efeitos de uma camada para outra
&#x200B;* [Pilha de camadas] Arrastar itens para uma pasta os coloca na parte superior da pasta
&#x200B;* Atualize o Iray para a versão 2020.1.0
&#x200B;* [Padeiros] Atualize os Padeiros para a versão 2.5.4
&#x200B;* [Padeiros] Exibir blocos UV individuais na janela de progresso da cozedura
&#x200B;* [Padeiros]&#x200B;[IU] Permita preparar rapidamente o conjunto de textura atual com um novo botão
&#x200B;* [Padeiros] Permite ao usuário selecionar rapidamente um dos padeiros com ALT + CLIQUE ESQUERDO
&#x200B;* Atualize o Substance Engine para a versão 8.0.8
&#x200B;* [Substance Engine] Suporte à cor padrão em novos arquivos .sbsar
&#x200B;* [Desempacotamento automático] Melhoria de desempenho
&#x200B;* [Exportar] Adicionar feedback visual para indicar qual resolução do bloco UV difere do padrão do projeto
&#x200B;* [Exportar] Adicionar o fator de tamanho da cena no arquivo shader json exportado
&#x200B;* [Idioma] Adicionar tradução para japonês
&#x200B;* [UI] Janela Atualizar sobre com controle de versão de dependências internas
&#x200B;* [Scripting]&#x200B;[Python] Permitir gerenciar recursos de prateleira
&#x200B;* [Scripting]&#x200B;[Python] Permitir saber quando um projeto está pronto para assar e exportar
&#x200B;* [Scripting]&#x200B;[Python] Permitir saber quando uma prateleira terminou de rastrear recursos no disco
&#x200B;* [Scripting]&#x200B;[Python] Permite consultar a lista de blocos UV por conjuntos de textura
&#x200B;* [Scripting]&#x200B;[Python] Permitir a atribuição de visualização personalizada aos recursos de prateleira
&#x200B;* [Scripting]&#x200B;[Python] Permitir gerenciar prateleiras personalizadas
&#x200B;* [Scripting]&#x200B;[Python] Adicionar um índice de método em cada submódulo na documentação
&#x200B;* [Scripting]&#x200B;[Python] Novo estilo para a documentação
&#x200B;* [Scripting]&#x200B;[Python] Aprimoramento de recursos e documentação de prateleira
&#x200B;* [Conteúdo] Três novas predefinições de ferramenta para fazer pontos
&#x200B;* [Prateleira] Remova temporariamente a opção “Exportar para Substance share” durante a transição para a nova plataforma de Substance share

**Corrigido:**

&#x200B;* Falha ao usar monitores com diferentes resoluções
&#x200B;* Falha no Substance Engine com alguns projetos raros
&#x200B;* A atualização do visor falha com a opção Ocultar/Ignorar geometria excluída ao alternar as camadas
&#x200B;* [Visualização 2D] A viewport 2D pode estar ausente em alguns projetos
&#x200B;* [Preparação] “Corresponder pelo nome da malha” ignora partes do objeto
&#x200B;* [Pilha de camadas] Clicar em um efeito de camada abre a pasta
&#x200B;* [Máscara de geometria] O bloco UV ainda é contado na máscara mesmo ao reimportar a malha sem ele
&#x200B;* [Máscara de geometria] O menu do botão direito no visor não fornece as ferramentas corretas
&#x200B;* [Motor] Grandes atrasos em projetos específicos
&#x200B;* [Scripting] Alta latência com solicitações remotas de POST JSON no Windows
&#x200B;* [Linux] A quantidade de Vram não é detectada corretamente com GPUs integradas específicas
&#x200B;* [Desfazer quebra automática] Falha ou desquebra longa em alguns projetos

## Versão 6

### 6.2.2 (2020.2.2)

*(Lançado: 28 De setembro De 2020)*
Resumo: **Versão secundária, correção de erro com algumas funções na API Python**

**Adicionado:**

&#x200B;* [Desempenho] Não calcula todos os blocos UV ao usar a seleção de ID de cor
&#x200B;* [Padeiros]&#x200B;[IU] Exibir descrições de conjuntos de texturas
&#x200B;* [Baker] Permitir salvar configurações de faço bake
&#x200B;* [Preparadores] Adicionar todas as opções de recolher/expandir todas à guia Seleção
&#x200B;* [Lista de conjuntos de texturas] Ocultar descrição quando vazia
&#x200B;* [Blocos UV]&#x200B;[Texture Set List] Clicar em Bloco UV deve expandir/recolher a lista
&#x200B;* [Exportar]&#x200B;[IU] Permite redimensionar o painel Lista de conjuntos de texturas horizontalmente
&#x200B;* [Exportar]&#x200B;[IU] Texto de dica de ferramenta consistente para Blocos UV e para o fluxo de trabalho Conjunto de texturas com texturas não selecionadas
&#x200B;* [Scripting]&#x200B;[Python] Permitir o uso de predefinições de exportação para exportar texturas
&#x200B;* [Scripting]&#x200B;[Python] Adicionar um changelog na documentação
&#x200B;* [Scripting]&#x200B;[Python] Permite consultar todos os canais disponíveis em uma determinada pilha
&#x200B;* Melhorias na interface do console do [Scripting]&#x200B;[Python]

**Corrigido:**

&#x200B;* [AMD] Detecção incorreta de versão de driver desatualizada
&#x200B;* Falha ao reimportar uma malha com layout de Blocos UV diferente em alguns casos
&#x200B;* Falha ao usar partículas com UDIMs em malhas muito pesadas
&#x200B;* [Blocos UV] Falha ao exportar uma malha com informações de deslocamento em alguns casos
&#x200B;* [Export]&#x200B;[Falha] Exportar Visualização 2D no formato psd pode causar uma falha
&#x200B;* Importar imagens como sequências ao criar um projeto não funciona
&#x200B;* Mecanismo travado em um loop infinito
&#x200B;* [Atalho] A câmera gira sempre no modo de ajuste ao alterar os atalhos do modo de ajuste
&#x200B;* As malhas são sempre desempacotadas automaticamente quando reimportadas, mesmo que a opção esteja desativada
&#x200B;* [Texture Set List] O campo de texto de descrição às vezes não é totalmente visível durante a edição
&#x200B;* [Lista de conjuntos de texturas] O menu suspenso para ocultar/reexibir conjuntos de texturas não está totalmente visível
&#x200B;* [Lista de conjuntos de texturas] Clicar no ícone de olho não deve inserir o “Editar nome do conjunto de texturas”
&#x200B;* [Configurações do conjunto de texturas] A remoção de um canal também remove o canal abaixo
&#x200B;* [Exportar] Incluir tudo e Redefinir tudo não leva Blocos UV em consideração
&#x200B;* [Baker] Os baker desmarcados aparecem durante o processo de fça bake
&#x200B;* A atualização de resolução não é levada em consideração para mapas baked usados como entrada
&#x200B;* [Blocos UV]&#x200B;[Janela de visualização] A porta de visualização 3D congela ao adicionar a pasta Material inteligente após com a máscara de Bloco UV selecionada
&#x200B;* [Blocos UV]&#x200B;[Visor] O Wireframe ainda está visível para blocos ocultos com o modo tinta
&#x200B;* [Export]&#x200B;[Sketchfab] Problemas com o tipo de assinatura “plus”
&#x200B;* [Sketchfab] A caixa de seleção “Este ativo é privado” não é exibida após alternar a conta
&#x200B;* [Exportar]&#x200B;[Conteúdo] Predefinições de pincel “onduladas” podem levar a problemas de desempenho
&#x200B;* [Plugin Photoshop] Mensagem no registro: não compatível com o fluxo de trabalho do Bloco UV
&#x200B;* [Scripting]&#x200B;[Python] PYTHONPATH env var impede que o aplicativo seja iniciado
&#x200B;* [Scripting]&#x200B;[Python] Erro de digitação na documentação do Python

### 6.2.1 (2020.2.1)

*(Lançado: 29 de julho de 2020)*
Resumo: **Versão secundária, Hotfix**

**Adicionado:**

&#x200B;* Adicione a variável de ambiente “SUBSTANCE\_PAINTER\_VRAM\_BUDGET” para substituir a quantidade de VRam da GPU
&#x200B;* [Blocos UV]&#x200B;[Desempenho] Não calcula todos os blocos UV ao usar a ferramenta Preenchimento de polígono

**Corrigido:**

&#x200B;* [Iray] Salvar renderização retorna um erro e resulta em uma imagem em preto
&#x200B;* [Linux] Falha após a tela inicial no CentOS 7.3
&#x200B;* [Linux] A quantidade de Vram não é detectada corretamente com configurações específicas
&#x200B;* [Falha] Abrir um projeto com o nome do conjunto de texturas duplicado
&#x200B;* [Engine] Problema de invalidação de cache ao modificar uma máscara
&#x200B;* [Lista de conjuntos de texturas] Efeito de fonte incorreto quando o conjunto de texturas está desativado

**Problemas Conhecidos:**

&#x200B;* [Lista de Conjuntos de Texturas] Não é possível ocultar a descrição
&#x200B;* Problemas de interface do [Texture Set List]
&#x200B;* A renderização do PSD [Iray] não abre
&#x200B;* [Plug-in Photoshop] Não compatível com o fluxo de trabalho de blocos UV

### 6.2.0 (2020.2.0)

*(Lançado: 23 de julho de 2020)*
Resumo: **Versão principal com novo fluxo de trabalho de Blocos UV, pintura em Blocos UV e melhoria de desempenho**

**Adicionado:**

&#x200B;* Blocos UV (UDIMs)
&#x200B;* [Blocos UV] Pintar em blocos UV
&#x200B;* [Blocos UV] Permitir a escolha entre o fluxo de trabalho novo e herdado para Blocos UV
&#x200B;* [Blocos UV] Importar sequências de imagem de blocos UDIMs/UV como um recurso
&#x200B;* [Blocos UV] Adicionar lista de blocos UV por conjunto de textura na janela Lista de conjuntos de textura
&#x200B;* [Blocos UV] Permitir a edição da resolução de vários blocos UV de uma só vez nas Configurações do conjunto de textura
&#x200B;* [Blocos UV]&#x200B;[Exibição 2D] Exibir Blocos UV como uma grade
&#x200B;* [UV Tiles]&#x200B;[2D View] Novo botão de visor para exibir ou ocultar informações de UV Tiles
&#x200B;* [Ladrilhos UV] Alternar a ferramenta de pintura para canal único por padrão para projetos de Ladrilho UV
&#x200B;* [Blocos UV] Novo botão na barra de ferramentas contextual para ignorar blocos UV mascarados ao pintar
&#x200B;* [Blocos UV]&#x200B;[Pilha de camadas] Novos ícones de pilha de camadas para melhorar o desempenho
&#x200B;* [Blocos UV]&#x200B;[Pilha de camadas] Aprimorar ícones de pintura e preenchimento na barra de ferramentas
&#x200B;* [Máscara de bloco UV]&#x200B;[Visualização 2D] Permite incluir ou excluir vários blocos UV de uma vez (clique com o botão esquerdo, CTRL+clique com o botão esquerdo)
&#x200B;* [Máscara de bloco UV] Nova máscara de bloco UV para incluir, excluir blocos por camada com um novo ícone
&#x200B;* [Máscara de bloco UV]&#x200B;[Pilha de camadas] Exibir o número de blocos UV no ícone de máscara de blocos UV quando nem todos estiverem incluídos
&#x200B;* [Máscara de bloco UV]&#x200B;[Visualização 2D/3D] Adicionar efeito hover para visualizar blocos UV sob o cursor
&#x200B;* [Blocos UV]&#x200B;[Padeiros] Permitir selecionar e assar blocos UV específicos
&#x200B;* [Blocos UV]&#x200B;[Padeiros] Adicionar opções de seleção para Conjuntos de textura/Blocos UV
&#x200B;* [Blocos UV]&#x200B;[Padeiros] Clique com o botão direito do mouse na opção de menu para selecionar Blocos UV em um conjunto de textura
&#x200B;* [Blocos UV]&#x200B;[Padeiros] Permitem a seleção rápida no Conjunto de textura/Blocos UV arrastando
&#x200B;* [Blocos UV]&#x200B;[Padeiros] Substituir os botões “Todos” e “Nenhum” nos Mapas de malha por opções de seleção mais explícitas
&#x200B;* [Blocos UV]&#x200B;[Padeiros] Exibir o número de texturas a serem assadas
&#x200B;* [Blocos UV]&#x200B;[Exportar] Permite selecionar e exportar blocos UV específicos
&#x200B;* [Blocos UV]&#x200B;[Exportar] Permitir a seleção rápida de blocos UV arrastando
&#x200B;* [Blocos UV]&#x200B;[Exportar] Adicionar opções do menu suspenso para Blocos UV
&#x200B;* [Blocos UV]&#x200B;[Exportar] Torne algumas predefinições de exportação indisponíveis se não funcionarem com Blocos UV (Adobe Dimension, Sketchfab, glTF, USD)
&#x200B;* [Blocos UV]&#x200B;[Conteúdo] Atualizar predefinições de exportação para usar a nova tag $udim
&#x200B;* [Blocos UV] Aprimorar o relatório de erros ao importar malhas com Ilhas UV sobrepostas
&#x200B;* [UV Tiles] Telhas UV compatíveis em Iray
&#x200B;* [UV Tiles]&#x200B;[Scripting] Adicionar documentação de exportação de UV Tile ao documento Python
&#x200B;* Desempenho
&#x200B;* [Desempenho] Botão Novo na barra de ferramentas contextual para pausar o cálculo do mecanismo ao trabalhar (SHIFT+ESC)
&#x200B;* [Desempenho] Abertura mais rápida do projeto com o atraso do cálculo do cache do Conjunto de texturas
&#x200B;* [Desempenho] Não espere os mapas de malha serem carregados ao abrir o projeto
&#x200B;* [Desempenho]&#x200B;[Exibição 2D/3D] Não calcular o canal da Máscara no visor quando não estiver em uso
&#x200B;* [Desempenho] Não bloqueia o aplicativo ao carregar mapas de malha exibidos nas viewports
&#x200B;* [Desempenho] Melhorar a velocidade de salvamento incremental ao salvar um projeto
&#x200B;* [Performance]&#x200B;[Bakers] Alterar as configurações de dilatação padrão para melhorar a economia de tempo e tamanho do projeto
&#x200B;* [Performance]&#x200B;[Bakers] Migre para tons de cinza em padeiros específicos para melhorar a economia de tempo e tamanho do projeto
&#x200B;* [Desempenho]&#x200B;[Exportar] Aprimorar o desempenho do mecanismo para exportar texturas mais rapidamente
&#x200B;* [Desempenho]&#x200B;[Exportar] Melhore a capacidade de resposta ao abrir a caixa de diálogo de exportação com muitos conjuntos de texturas
&#x200B;* [Desempenho]&#x200B;[Exportar] Melhorar o desempenho ao mudar para a guia “Lista de exportações”
&#x200B;* [Performance]&#x200B;[Iray] Reduzir o tempo de inicialização do Iray
&#x200B;* Outro
&#x200B;* [Padeiros] Adicionar opções de seleção para Conjuntos de textura
&#x200B;* Mover gerenciamento de instância de sombreador para Configurações de Conjunto de Textura
&#x200B;* [Exibição 2D/3D] Adiciona uma mensagem na parte inferior da viewport para indicar qual tipo de máscara está editado
&#x200B;* [Pilha de camadas] Nova opção nas configurações para alternar entre miniaturas antigas e novas
&#x200B;* [Pilha de camadas] Adicionar feedback visual para indicar o estado de carregamento das miniaturas
&#x200B;* [Proj] Novo modo de projeção “Fill (Match Per UV-Tile)” para carregar sequências de imagens
&#x200B;* [Proj] Altere o modo de projeção das camadas de preenchimento para “Preencher (corresponder por bloco UV)” em casos específicos
&#x200B;* [Conteúdo] Otimizar as predefinições do pincel a carvão para melhorar o desempenho
&#x200B;* Atualize o Iray para a versão 2020.0.0
&#x200B;* [Exportar] Desative a guia Lista de exportações quando nada estiver selecionado
&#x200B;* Desempacotar automaticamente
&#x200B;* [Desfazer quebra automática] Melhorar a taxa de sucesso do processo de desquebra automática
&#x200B;* [Desempacotamento automático] Parametrização aprimorada para aumentar a velocidade e estabilidade

**Corrigido:**

&#x200B;* [Alembic] Os facesets são ignorados ao importar arquivos
&#x200B;* [Alembic] Tempo de carregamento infinito com arquivos específicos
&#x200B;* [Importar] A sequência de imagens UDIM incorreta é importada quando apenas a extensão do arquivo é diferente
&#x200B;* [Falha] A tentativa de abrir um projeto bloqueado por outro processo leva a uma falha
&#x200B;* [Projeção] Artefatos em malha duplicada ao usar projeção triplanar
&#x200B;* [Exportar] O canal emissivo não é exportado com o formato USD
&#x200B;* [Content] Material inteligente “Carvão” contém traçados de tinta

**Problemas Conhecidos:**

&#x200B;* [Lista de Conjuntos de Texturas] Não é possível ocultar a descrição
&#x200B;* Problemas de interface do [Texture Set List]

### 6.1.3 (2020.1.3)

*(Lançado: 16 De junho De 2020)*
Resumo: **Correção de erros**

**Adicionado:**

&#x200B;* [Exportar] Adicionar configurações de deslocamento no arquivo json de parâmetros do Sombreador

**Corrigido:**

&#x200B;* [Falha]&#x200B;[Mecanismo] Falha ao tentar apagar e substituir canais existentes
&#x200B;* [Falha] Alterar o sombreador após pintar uma máscara em camadas de material
&#x200B;* [Falha]&#x200B;[Mecanismo] Falha com alguns projetos pesados
&#x200B;* [Padeiros] A correspondência por nome não funciona com OBJs exportados do zBrush
&#x200B;* [Deslocamento]&#x200B;[SVT] As texturas não são exibidas na abertura do projeto quando o deslocamento está ativado
&#x200B;* [Exportar] Algumas texturas são exportadas com cinza uniforme
&#x200B;* [Exportar] Os conjuntos de textura desativados não devem ser exportados para predefinições de exportação de Dimension e Sketchfab
&#x200B;* [Scripting]&#x200B;[JavaScript] Falha ao usar a API JavaScript para acessar a configuração de exportação no evento onProjectOpened
&#x200B;* [Scripting]&#x200B;[Javascript] onExportFinished() não é chamado após uma exportação

### 6.1.2 (2020.1.2)

*(Lançado: 28 de maio de 2020)*
Resumo: **Correção de erro com atualização de Substance Engine e Padeiros**

**Adicionado:**

&#x200B;* [Baker] Atualizar para a versão mais recente
&#x200B;* [Padarias] Novo método de amostragem em Oclusão ambiente, curvatura, panificação de Thickness
&#x200B;* Atualize para a versão mais recente do Substance Engine
&#x200B;* [Scripting]&#x200B;[Python] Permitir a criação de ResourceID para recursos do projeto
&#x200B;* [Scripting]&#x200B;[Python] Permitir consulta de informações de canal
&#x200B;* [Scripting]&#x200B;[Python] Adicione funções dryrun e callback para simular a exportação de textura

**Corrigido:**

&#x200B;* [Bakers] Normais incorretos no padeiro World Space Normals usando um mapa normal tangente em casos específicos
&#x200B;* [Bakers] Erro ao assar Oclusão ambiente com Optix quando não há alta poli
&#x200B;* [Traçados dinâmicos] Atraso ao carregar um conjunto de texturas específico
&#x200B;* [Exportar] Não deve exportar os conjuntos de texturas desativados para USD, glTF
&#x200B;* [Script]&#x200B;[JavaScript] Não é possível editar novas configurações do Criador de curvatura
&#x200B;* [Scripting]&#x200B;[JavaScript] alg.texturesets.addChannel() não retorna um erro em alguns casos
&#x200B;* [Scripting]&#x200B;[JavaScript] Erro de digitação na documentação da API Javascript para setProjectExportOptions()
&#x200B;* [Scripts]&#x200B;[JavaScript] Sempre exporta todos os conjuntos de texturas
&#x200B;* [Scripting]&#x200B;[Python] sys.executable retorna um caminho para python.exe em vez de Substance Painter
&#x200B;* Cache de textura não compatível com o sistema operacional Mac e Windows/Linux
&#x200B;* [Livelink UE4] Somente o último material é usado para todos os conjuntos de texturas em uma malha combinada

**Problemas Conhecidos:**

&#x200B;* [Export]&#x200B;[Dimension]&#x200B;[Skecthfab] Não deve exportar os conjuntos de textura desativados
&#x200B;* [Falha] Alterar sombreador depois de pintar uma máscara em camadas de material

### 6.1.1 (2020.1.1)

*(Lançado: 05 de maio de 2020)*
Resumo: **Hotfix**

**Adicionado:**

&#x200B;* [Exportar] Feedback visual de estado substituído no TextureSet

**Corrigido:**

&#x200B;* [Export] Tamanho da janela do exportador muito grande no monitor de resolução especial e não pode ser redimensionado
&#x200B;* [Exportar] As opções não são salvas após a exportação
&#x200B;* [Exportar] Falha ou não é possível exportar com a predefinição de exportação “do cache”
&#x200B;* [Exportar] O cancelamento da exportação gera um mapa vazio adicional inesperado
&#x200B;* [Exportar] Corrigir configurações de predefinição de exportação virtual
&#x200B;* [Python] A variável env PYTHONPATH não é levada em conta
&#x200B;* [Python]&#x200B;[Exportar] O cancelamento da exportação via Python retorna um erro de exceção
&#x200B;* [Python]&#x200B;[Exportar] exportar\_projeto\_texturas resultado incorreto com formato de arquivo psd
&#x200B;* [Bakers] Falha no Linux com Rastreamento de raios do GPU

**Problemas Conhecidos:**

&#x200B;* [JavaScript] Não é possível editar as novas configurações do criador de curvatura
&#x200B;* [JavaScript]&#x200B;[Exportar] Sempre exporta todos os conjuntos de texturas
&#x200B;* [Export]&#x200B;[USD] Não deve exportar os conjuntos de textura desativados
&#x200B;* [Falha] Alterar sombreador depois de pintar uma máscara em camadas de material

### 6.1.0 (2020.1.0)

*(Lançado: 22 De abril De 2020)*
Resumo: **Versão principal com Novo exportador de textura e malha (com deslocamento e mosaico), desempacotamento UV atualizado com mais controles, novos padeiros, nova API python de script, melhor UX para projeção de decalques e novo conteúdo**

**Adicionado:**

&#x200B;* Novo exportador de textura e malha
&#x200B;* [Exportar] Interface de novo exportador
&#x200B;* [Exportar]&#x200B;[guia Exportar] Permite a seleção dos canais de mapas que são exportados por conjunto de textura
&#x200B;* [Exportar]&#x200B;[Guia Exportar] Permite a modificação do tamanho do Conjunto de texturas para todos os Conjuntos de texturas em uma ação
&#x200B;* [Exportar]&#x200B;[guia Exportar] Permite um modelo diferente por conjunto de textura (exceto USD, glTF, Sketchfab e Dimension)
&#x200B;* [Exportar]&#x200B;[guia Exportar] Ativação e desativação rápidas de mapas e conjuntos de texturas
&#x200B;* [Exportar]&#x200B;[Guia Exportar] A resolução de exportação 8192 x 8192 não é mais experimental
&#x200B;* [Exportar]&#x200B;[guia Exportar] Permite a modificação do formato de arquivo e a profundidade de bits por mapa
&#x200B;* [Exportar]&#x200B;[guia Exportar] Permite redefinir os valores dos parâmetros padrão
&#x200B;* [Exportar]&#x200B;[guia Exportar] Permite que as configurações sejam salvas sem exportar
&#x200B;* [Exportar]&#x200B;[guia Modelos de saída] Renomeie a guia “Configuração” para a guia “Modelos de saída”
&#x200B;* [Exportar]&#x200B;[guia Modelos de saída] Permite a definição de formato de arquivo e a profundidade de bits por mapa predefinido
&#x200B;* [Exportar]&#x200B;[Guia Lista de exportações] Nova guia de visualização para resumir e visualizar o processo de exportação
&#x200B;* [Malha de importação/exportação] Otimização de desempenho de tempo de importação/exportação
&#x200B;* [Exportar malha] Exportar malha em FBX
&#x200B;* [Exportar malha] Exportar malha com deslocamento e mosaico
&#x200B;* [Exportar malha]&#x200B;[IU] Novas configurações para recalcular vértice normal, aplicar triangulação
&#x200B;* [Exportar malha] Exporte a topologia de malha original com novos UVs gerados pelo desencapsulamento automático
&#x200B;* Desencapsulamento automático UV atualizado com mais controles
&#x200B;* [Desempacotamento UV]&#x200B;[IU] Adicionar configuração para ativar o desempacotamento UV automático na nova janela do projeto
&#x200B;* [UV Unwrapping]&#x200B;[UI] Novas opções para controlar os passos de abertura (costuras, abertura, embalagem)
&#x200B;* [UV Unwrapping]&#x200B;[UI] Permitir a conservação de emendas de abertura/desembrulho/embalagem existentes
&#x200B;* [UV Unwrapping]&#x200B;[UI] Novas opções para recalcular totalmente as etapas de desencapsulamento
&#x200B;* [UV Unwrapping]&#x200B;[UI] Nova opção para controlar o tamanho da margem (nenhum, pequeno, médio e grande)
&#x200B;* Novos Panificadores
&#x200B;* [Padarias] Substituir a curvatura antiga pela nova curvatura da malha
&#x200B;* [Padeiros] Adicione a opção de correspondência por nome para ignorar a face traseira no padeiro “Oclusão ambiente”
&#x200B;* [Baker] Adicionar a opção de plano horizontal no baker “Oclusão de ambiente”
&#x200B;* Nova API de script do Python (3.7.6)
&#x200B;* [Python]&#x200B;[UI] Novo menu de scripts para o Python
&#x200B;* [Python]&#x200B;[UI] Nova documentação do Python no menu Ajuda
&#x200B;* [Python] Expor módulos Substance Painter python: substance\_painter, alg, display, project.setting, project, texturesets, ui
&#x200B;* [Python] Expor novo módulo Python “substance\_painter”
&#x200B;* [Python] Expor novo submódulo Python: alg, display, log, project, resource, texturesets, ui
&#x200B;* [Python] Ouvinte para alterações de projeto
&#x200B;* [Python] Novos exemplos na documentação do Python
&#x200B;* [JavaScript]&#x200B;[UI] Menu de plug-ins substituído pelo JavaScript
&#x200B;* [Visor] Permite a criação de uma projeção de decalque “arrastando/soltando + ALT” um recurso da prateleira
&#x200B;* Novo conteúdo
&#x200B;* [Content] 5 novos materiais de decalque do Substance Source
&#x200B;* [Content] Adicionar novos modelos de projeto e predefinições de exportação para o renderizador Maxwell
&#x200B;* [Content] Adicionar modelo de projeto para exportação do Keyshot 9
&#x200B;* [Content] Atualize a predefinição de exportação Keyshot 9 para suportar deslocamento e emissivo
&#x200B;* [Conteúdo]&#x200B;[Exportador] Atualização de todas as predefinições de exportação para corresponder às versões mais recentes de mecanismos de jogo e renderizadores
&#x200B;* [Conteúdo]&#x200B;[Exportador] Atualizar arquivos de predefinições de exportação para usar o novo formato e configurações de pontilhamento
&#x200B;* [Content] Novos modelos e sombreadores para suportar material VRay (VRayMtl)
&#x200B;* [Pilha de camadas] Permitir a exclusão de efeitos de camada usando o ícone de lixeira ou o atalho de teclado Excluir
&#x200B;* Remover o Substance Source de plug-in (use o iniciador com a funcionalidade “enviar para”)
&#x200B;* [Windows] Não exibir aviso de TDR em GPUs de alta capacidade

**Corrigido:**

&#x200B;* Problemas de tradução na caixa de diálogo Novo arquivo de projeto
&#x200B;* [Baker] A configuração “Salvar arquivo de cena pré-processado” não funciona mais
&#x200B;* [Projeção planar] A projeção não funciona em malhas com UVs repetidos
&#x200B;* [Decalque] Diferença de comportamento no canal normal ao usar diferentes modos de projeção de camada de preenchimento
&#x200B;* [Borrar]&#x200B;[Clonar] O artefato pode aparecer ao pintar em uma máscara
&#x200B;* [Engine] Falha com conteúdo de camada específico
&#x200B;* [Engine] Falha aleatória ao pintar em alguns casos
&#x200B;* [Ponto de ancoragem] A referência a uma máscara vazia sempre retorna branco
&#x200B;* [Exportar] Camada não considerada em algumas configurações de pilha específicas
&#x200B;* [Exportar malha] Não é possível exportar com caminho que contém caracteres especiais
&#x200B;* [Exportar malha] Não é possível ler arquivos glTF quando exportado do Linux ou MacOS
&#x200B;* [Importar malha] A reimportação do DAE, PLY ou glTF não funciona conforme o esperado

**Problemas Conhecidos:**

&#x200B;* [Script]&#x200B;[JavaScript] Não é possível editar novas configurações do Criador de curvatura
&#x200B;* [Bakers] Falha no Linux com Rastreamento de raios do GPU
&#x200B;* [Export]&#x200B;[USD] Não deve exportar os conjuntos de textura desativados
&#x200B;* [Falha] Alterar sombreador depois de pintar uma máscara em camadas de material

## Versão 5

### 5.3.3 (2019.3.3)

*(Lançado: 06 De fevereiro De 2020)*
Resumo: **Correção de erro com a atualização para o Iray 2019.3**

**Adicionado:**

&#x200B;* Atualização para o Iray 2019.3
&#x200B;* [Log] Indica bios desatualizado para CPU Ryzen levando a falha durante a cozedura
&#x200B;* [ABR] Extrair alfa ABR para prateleira

**Corrigido:**

&#x200B;* [Baker] Falha na cozedura se a malha de alto-poli não tiver UVs
&#x200B;* [Linux] Os atalhos de mouse personalizados não são salvos
&#x200B;* [Pincel] O contorno desaparece com algumas formas alfa
&#x200B;* [Tablet] Detecção incorreta ao mover controles deslizantes
&#x200B;* [Atalhos] Não é possível configurar nenhum atalho com “Ctrl+Alt+Clique do Mouse”
&#x200B;* [Prateleira] Não é possível ver a dica de ferramenta do recurso ao usar um tablet com caneta
&#x200B;* A predefinição [Visualização 2D]&#x200B;[Export] não leva em consideração as informações normais
&#x200B;* Congela ao pintar em alinhamento UV com determinados pincéis
&#x200B;* Pintar sob um filtro cria artefatos no traçado em andamento
&#x200B;* [Visor] Cache de textura incorreto no visor após a reimportação de uma malha
&#x200B;* [Falha] Erro ao salvar após exportar para o Photoshop
&#x200B;* [Falha] Gravar símbolos especiais no prefixo ao importar recursos
&#x200B;* [Falha] Clique na referência em Propriedades de ponto de ancoragem
&#x200B;* [Pontos de ancoragem] O canal não é atualizado quando há um filtro entre o ponto de ancoragem e a referência
&#x200B;* O link de URL do Iray no menu Ajuda não funciona

**Problemas Conhecidos:**

&#x200B;* [Desempacotamento UV] O processamento de malhas de alta polarização pode demorar muito tempo
&#x200B;* [Desempacotamento UV] Os vértices exatamente nas mesmas coordenadas são mesclados
&#x200B;* [UV Unwrapping] A geração de UV pode falhar em algumas partes da malha em alguns casos raros
&#x200B;* [Desempacotamento UV] Proporção de texel não uniforme ou altamente distorcida em uma única Ilha UV em alguns casos
&#x200B;* [Desempacotamento UV] Relação de texel não uniforme entre conjuntos de textura
&#x200B;* [UV Unwrapping] A Ilha UV gerada pode ser muito alongada e não se encaixar no espaço UV em alguns casos
&#x200B;* [Desempacotamento por UV] Faces degeneradas ou faces de malha não triangulares com bordas pequenas ou sobrepostas podem não ter o UV desempacotado

### 5.3.2 (2019.3.2)

*(Lançado: 21 De Janeiro De 2020)*
Resumo: **Correção de erros**

**Corrigido:**

&#x200B;* Abrir um projeto que foi salvo no modo de canal individual não exibe a malha
&#x200B;* A janela de visualização nem sempre é atualizada ao pintar sob uma camada usando a ferramenta clone

**Problemas Conhecidos:**

&#x200B;* [Bakers] Falha relacionada a multi-threading em CPUs Ryzen
&#x200B;* [Desempacotamento UV] O processamento de malhas de alta polarização pode demorar muito tempo
&#x200B;* [Desempacotamento UV] Os vértices exatamente nas mesmas coordenadas são mesclados
&#x200B;* [UV Unwrapping] A geração de UV pode falhar em algumas partes da malha em alguns casos raros
&#x200B;* [Desempacotamento UV] Proporção de texel não uniforme ou altamente distorcida em uma única Ilha UV em alguns casos
&#x200B;* [Desempacotamento UV] Relação de texel não uniforme entre conjuntos de textura
&#x200B;* [UV Unwrapping] A Ilha UV gerada pode ser muito alongada e não se encaixar no espaço UV em alguns casos
&#x200B;* [Desempacotamento por UV] Faces degeneradas ou faces de malha não triangulares com bordas pequenas ou sobrepostas podem não ter o UV desempacotado

### 5.3.1 (2019.3.1)

*(Lançado: 20 de dezembro de 2019)*
Resumo: **Hotfix**

**Corrigido:**

&#x200B;* Falha ao trabalhar em malhas com Projeções UV específicas
&#x200B;* [ABR] Falha ao alternar entre predefinições Photoshop
&#x200B;* [Linux] Não é possível iniciar o Substance Painter no CentOS 7.4 devido a um problema de dependência do libGLX
&#x200B;* [Padeiros] Falha ao assar após usar Arquivo > Limpar
&#x200B;* [Padeiros] A caixa de diálogo de progresso da cozedura congela após o cancelamento
&#x200B;* [Padarias] A malha de cozimento após a exportação de texturas não funciona
&#x200B;* [Padarias] O uso da opção “Corresponder por nome” resulta em mapas de malha pretos
&#x200B;* [Padeiros] A gaiola não é tida em conta
&#x200B;* [Prateleira] Importar arquivos de PSD leva a imagens quebradas
&#x200B;* [Amostra] O projeto de amostra “Mat” possui câmeras quebradas e predefinição de exportação incorreta

**Problemas Conhecidos:**

&#x200B;* [Bakers] Falha relacionada a multi-threading em CPUs Ryzen
&#x200B;* [Desempacotamento UV] O processamento de malhas de alta polarização pode demorar muito tempo
&#x200B;* [Desempacotamento UV] Os vértices exatamente nas mesmas coordenadas são mesclados
&#x200B;* [UV Unwrapping] A geração de UV pode falhar em algumas partes da malha em alguns casos raros
&#x200B;* [Desempacotamento UV] Proporção de texel não uniforme ou altamente distorcida em uma única Ilha UV em alguns casos
&#x200B;* [Desempacotamento UV] Relação de texel não uniforme entre conjuntos de textura
&#x200B;* [UV Unwrapping] A Ilha UV gerada pode ser muito alongada e não se encaixar no espaço UV em alguns casos
&#x200B;* [Desempacotamento por UV] Faces degeneradas ou faces de malha não triangulares com bordas pequenas ou sobrepostas podem não ter o UV desempacotado

### 5.3.0 (2019.3.0)

*(Lançado: 17 de dezembro de 2019)*
Resumo: **Versão principal com melhoria na experiência do usuário de pintura manual, trabalho com tablets, desencapsulamento automático de UV em beta (0.3.0) e conteúdo novo diversificado para pintura manual**

**Adicionado:**

&#x200B;* Integrar a versão 0.3.0 de desenrolamento automático de UV no Substance Painter
&#x200B;* [Desencapsulamento UV] Desencapsulamento UV automático em Substance Painter quando nenhum UV presente ou UVs parciais
&#x200B;* [Desencapsulamento UV] Uma configuração global para ativá-lo e desativá-lo
&#x200B;* [Desencapsulamento UV] Versão relatada no arquivo de log
&#x200B;* [Desencapsulamento UV]&#x200B;[IU] Indicar progresso do desencapsulamento UV
&#x200B;* [UI] Novas configurações na barra de ferramentas contextual para selecionar a visualização do pincel: visualização completa, contorno e mira
&#x200B;* [Ferramenta] Novo modo de mesclagem avançado na seção alfa: Clarear (máximo) além de Normal
&#x200B;* [Pilha de camadas] Opção de correção de gama por camada para alfa ou máscara (menu do botão direito do mouse)
&#x200B;* [Pilha de camadas]&#x200B;[IU] Adicionar ícone &#39;i&#39; quando um alfa de camada for corrigido para a gama
&#x200B;* [Tablet]&#x200B;[Ferramenta] Expor a pressão mínima para tamanho e fluxo
&#x200B;* [Tablet]&#x200B;[IU] Nova configuração na barra de ferramentas contextual para selecionar a pressão da curva: linear, fácil de entrar, fácil de sair
&#x200B;* [Tablet]&#x200B;[UX] Adicionar Ctrl+Alt+clique para rolar
&#x200B;* Importar predefinições de pincel do Photoshop (formato ABR)
&#x200B;* [ABR] Suporte a parâmetros de forma
&#x200B;* [ABR] Suporte a parâmetros de dinâmica de forma
&#x200B;* [ABR] Parâmetros de transferência de suporte
&#x200B;* [ABR] Parâmetros de dispersão de suporte
&#x200B;* [ABR]&#x200B;[Traçados dinâmicos] Redondez e giro de suporte
&#x200B;* [ABR]&#x200B;[Prateleira] Expor a estrutura de pastas de pincéis no Editor de filtros
&#x200B;* [ABR]&#x200B;[Prateleira] Adicionar ícone do Photoshop em miniaturas
&#x200B;* [ABR]&#x200B;[Prateleira] Adicionar lista de parâmetros não suportados na miniatura detalhada do ABR
&#x200B;* [Ferramenta]&#x200B;[Traçados dinâmicos] Nova configuração de traçado dinâmico para controlar a quantidade de semente aleatória a ser gerada
&#x200B;* [Ferramenta]&#x200B;[IU] Adicionar nova distribuição e configurações de eixo para dispersão de tremulação
&#x200B;* [Atalho] Adicione Ctrl+Shift+B para abrir a janela Cozimento
&#x200B;* [UI]&#x200B;[Menu] Adicionar entrada no menu “Editar” para abrir a janela Cozimento
&#x200B;* [UI]&#x200B;[Configurações] Aprimoramento do alinhamento da lista de atalhos
&#x200B;* [IU] Substituir ícones de controles de pressão (tamanho e fluxo) por botões de ligar/desligar
&#x200B;* [Janela de visualização] Permitir focalizar as portas de visualização 2D e 3D separadamente
&#x200B;* Atualize para QT 5.12.5
&#x200B;* [IU] Indicar progresso do carregamento de malha
&#x200B;* [Substance] Adicione suporte para faixa suave e não fixa com controles deslizantes
&#x200B;* [Substance] Aumente a precisão dos parâmetros de Substance até 6 decimais
&#x200B;* [Substance] Considere a etapa definida por um parâmetro
&#x200B;* [Substance] Otimizar a geração de traço dinâmico com suporte a condições nos dados do usuário
&#x200B;* [Substance] Permitir designar uma saída de gráfico como uma máscara para todos os canais via userdata
&#x200B;* [Content] Atualizar projeto de amostra &#39;Mat&#39; com topologia amigável ao deslocamento, novo mapa de ID e novas câmeras
&#x200B;* [Conteúdo] Integrar 3 novos filtros (MatFx): Quadrinhos, Aquarela, Pintura a óleo (inspirada no trabalho de Emrecan Cubukcu)
&#x200B;* [Conteúdo] Integrar 102 predefinições de pincel Photoshop dos pacotes de Kyle T. Webster
&#x200B;* [Content] Integrar 18 novas predefinições de pincel: Seta de rolo de pintura, Texto de aviso de rolo de pintura, Carvão fino e muito mais
&#x200B;* [Content] Integrar 9 novas alfas: rolo de pintura do criador de pincel, Photoshop do criador de pincel, padrões de pincel e muito mais
&#x200B;* [Content] Integrar 2 novas predefinições de ferramenta: Gouache Dense e Gouache Faded
&#x200B;* [Conteúdo] Integrar 1 novo gerador : verificador UV (destacar Ilhas UV e costuras)
&#x200B;* [Content] Integrar 2 novas predefinições de exportação: Keyshot 9+ e Spark AR Studio
&#x200B;* [Content] Integrar 1 novo modelo de projeto: Spark AR Studio (Facebook)

**Corrigido:**

&#x200B;* [Tablet] Desfazer traçados da caneta (Ctrl + Z) atrasa mais do que desfazer traçados do mouse
&#x200B;* [Tablet] A pressão inicial e final não é considerada ao desenhar uma linha reta
&#x200B;* [Tablet] O primeiro carimbo é desenhado duas vezes ao usar uma linha reta
&#x200B;* [Tablet] Aprimorar o suporte para atalhos de tablet Huion
&#x200B;* [Tablet] Aprimorar o suporte para botões de caneta Huion
&#x200B;* [Tablet] Deslocamento entre a visualização do pincel e o carimbo desenhado
&#x200B;* [Tablet] Os atalhos para modificar pincéis com caneta resultam em baixo desempenho em casos raros
&#x200B;* [Tablet] Atraso ao pintar em uma camada específica
&#x200B;* Texturas desfocadas podem ocorrer em casos raros ao alternar entre viewport
&#x200B;* [UI]&#x200B;[Substance] As entradas de imagem nem sempre são exibidas
&#x200B;* Limpar não remove as predefinições da prateleira que foram importadas em um projeto
&#x200B;* [Tool]&#x200B;[Dynamic Stroke] Problema de desempenho ao ajustar a contagem de ciclos de carimbo
&#x200B;* Problemas de atualização ao pintar no modo de visor 3D/2D em casos raros
&#x200B;* Pintar um traçado muito longo pode causar congelamento
&#x200B;* [Ferramenta] Problema de desempenho ao pintar com traçados dinâmicos específicos
&#x200B;* [UI] A barra de ferramentas contextual ainda exibe as propriedades do pincel ao selecionar uma pasta
&#x200B;* Os valores do eixo de simetria não são redefinidos
&#x200B;* A importação de texturas EXR com valores de ponto flutuante é totalmente preta
&#x200B;* Alt+clique em um canal para isolar não funciona para filtro e gerador
&#x200B;* [Export] Falha específica do projeto na exportação
&#x200B;* [Substance] Valor padrão incorreto no menu suspenso se o parâmetro estiver oculto por Visible If
&#x200B;* [Shader] Os canais definidos por meio da Camada de material não são classificados da mesma maneira na interface do usuário
&#x200B;* [Prateleira] Os metadados de predefinições não são salvos no disco

**Problemas Conhecidos:**

&#x200B;* [Desempacotamento UV] O processamento de malhas de alta polarização pode demorar muito tempo
&#x200B;* [Desempacotamento UV] Os vértices exatamente nas mesmas coordenadas são mesclados
&#x200B;* [UV Unwrapping] A geração de UV pode falhar em algumas partes da malha em alguns casos raros
&#x200B;* [Desempacotamento UV] Proporção de texel não uniforme ou altamente distorcida em uma única Ilha UV em alguns casos
&#x200B;* [Desempacotamento UV] Relação de texel não uniforme entre conjuntos de textura
&#x200B;* [UV Unwrapping] A Ilha UV gerada pode ser muito alongada e não se encaixar no espaço UV em alguns casos
&#x200B;* [Desempacotamento por UV] Faces degeneradas ou faces de malha não triangulares com bordas pequenas ou sobrepostas podem não ter o UV desempacotado
&#x200B;* A amostra do metamat tem alguns problemas com câmeras importadas

### 5.2.3 (2019.2.3)

*(Lançado: 23 de outubro de 2019)*
Resumo: **Versão de correção de erros**

**Adicionado:**

&#x200B;* [Texture Set List] Adicionar botão para ativar/desativar rapidamente o modo de foco
&#x200B;* [Log] Adiciona o número de versão do Windows 10 no arquivo de log
&#x200B;* Atualize para a versão mais recente do Substance Engine
&#x200B;* [MacOS] Autenticação do software para atender aos novos requisitos de distribuição do MacOS Catalina

**Corrigido:**

&#x200B;* [Plug-in] A origem do plug-in não funciona
&#x200B;* [MacOS]&#x200B;[Shader] Mac OS 10.14.5 e AMD: a disposição em camadas de material não funciona conforme o esperado

**Problemas Conhecidos:**

&#x200B;* Arquivos Alembic com subdivisões não podem ser importados
&#x200B;* Falhas raras ao importar alguns arquivos Alembic
&#x200B;* A interface não responde temporariamente ao assar com DXR em GPUs Pascal

### 5.2.2 (2019.2.2)

*(Lançado: 20 De setembro De 2019)*
Resumo: **Versão de correção de erros**

**Corrigido:**

&#x200B;* A importação de recursos por scripts pode causar uma falha
&#x200B;* [Plug-in] Baixar material da origem pode levar a uma falha

**Problemas Conhecidos:**

&#x200B;* Arquivos Alembic com subdivisões não podem ser importados
&#x200B;* Falhas raras ao importar alguns arquivos Alembic
&#x200B;* A interface não responde temporariamente ao assar com DXR em GPUs Pascal

### 5.2.1 (2019.2.1)

*(Lançado: 17 de setembro de 2019)*
Resumo: **Versão de correção de erros**

**Corrigido:**

&#x200B;* [Mac]&#x200B;[USD] Arquivos USDZ exportados do MacOS não podem ser abertos
&#x200B;* [Conjunto de texturas] Não é possível isolar um conjunto de texturas com o modificador ALT
&#x200B;* [Prateleira] Predefinições, Materiais inteligentes e Máscaras inteligentes são sempre modificados ao sair do aplicativo
&#x200B;* [Pilha de camadas] Não é possível selecionar o efeito após excluir outro efeito
&#x200B;* Cintilação ao usar um controle deslizante dentro do painel de propriedades da ferramenta
&#x200B;* Falha ao exportar predefinições para prateleira
&#x200B;* Falha ao exportar uma predefinição com espaço insuficiente
&#x200B;* Falha ao criar uma predefinição com espaço insuficiente

**Problemas Conhecidos:**

&#x200B;* Arquivos Alembic com subdivisões não podem ser importados
&#x200B;* Falhas raras ao importar alguns arquivos Alembic
&#x200B;* A interface não responde temporariamente ao assar com DXR em GPUs Pascal

### 5.2.0 (2019.2.0)

*(Lançado: 25 de julho de 2019)*
Resumo: **Lançamento principal com atualizações dos padeiros em termos de desempenho e um novo modo de pré-visualização + novo conteúdo**

**Adicionado:**

&#x200B;* [Padarias] Suporte adicionado para Rastreamento de raios do GPU com DXR e OptiX (Oclusão ambiente, Thickness)
&#x200B;* [Bakers] Otimizações e acelerações para o rastreamento de raio da CPU
&#x200B;* [Padeiros]&#x200B;[Modo Vis]&#x200B;[IU] Novo modo de visualização de cozimento no visor
&#x200B;* [Bakers]&#x200B;[Preferences]&#x200B;[UI] Nova opção de cozimento para ativar/desativar o Rastreamento de raios do GPU
&#x200B;* [Padeiros]&#x200B;[IU] Retrabalho da caixa de diálogo da barra de progresso
&#x200B;* [Padeiros] Melhoria das mensagens de aviso e de erro
&#x200B;* [Padeiros] Permitem o cancelamento mais responsivo do processo de cozimento
&#x200B;* [Padeiros] Reabrir a janela do bolo após clicar em Cancelar
&#x200B;* [Proj]&#x200B;[UX] Melhoria da usabilidade do manipulador de rotação
&#x200B;* [Settings] Opção para melhorar o desempenho reduzindo a resolução do visor para telas HDPI
&#x200B;* [Script] Alterar resolução do conjunto de texturas
&#x200B;* [Script] Obter conjunto de textura selecionado
&#x200B;* [Script] Permite que o usuário selecione um conjunto de texturas
&#x200B;* [Scripting] Função para saber quando a seleção do conjunto de texturas foi alterada
&#x200B;* [Prateleira] Adicionado 40 novos materiais inteligentes
&#x200B;* [Prateleira] Adicionado 20 novas máscaras inteligentes

**Corrigido:**

&#x200B;* [Pilha de camadas] Congelamento da interface do usuário ao selecionar várias camadas
&#x200B;* [Pilha de camadas] Agrupar muitas camadas congela a interface por mais tempo do que o normal
&#x200B;* [Pilha de camadas] Uma camada e um efeito podem ser selecionados ao mesmo tempo em alguns casos
&#x200B;* os gráficos de Substance usados nas ferramentas de pintura não são gerados na resolução correta
&#x200B;* [Baker] O botão “Cozinhar todos os conjuntos de textura” não é desativado quando nenhum padeiro está selecionado
&#x200B;* [MacOS] Desativar a mensagem de aviso sobre o mosaico
&#x200B;* A ferramenta de projeção não tem visualização quando usada com uma máscara
&#x200B;* Falha e projetos corrompidos ao tentar salvar com espaço em disco insuficiente
&#x200B;* [Shelf] Falha ao importar um recurso no disco via shelf com espaço insuficiente
&#x200B;* [Prateleira] Falha ao restaurar a predefinição de sessão
&#x200B;* [Prateleira] Importar uma predefinição com um nome que termina com um espaço leva a uma falha
&#x200B;* [Prateleira] Importar um recurso com um prefixo que termina com um espaço vazio leva a uma falha

**Problemas Conhecidos:**

&#x200B;* Arquivos Alembic com subdivisões não podem ser importados
&#x200B;* Falhas raras ao importar alguns arquivos Alembic
&#x200B;* A interface não responde temporariamente ao assar com DXR em GPUs Pascal

### 5.1.3 (2019.1.3)

*(Lançado em: 01 de julho de 2019)*
Resumo: **Correção de erro com 2 novos recursos**

**Adicionado:**

&#x200B;* Permite especificar o orçamento VRam com uma linha de comando (por exemplo, —vram-budget 4096)
&#x200B;* [QML] Expor as propriedades wrapMode e elide dos botões e caixas de seleção do QML

**Corrigido:**

&#x200B;* “Seguir caminho” não funciona o tempo todo
&#x200B;* O mapeamento de canal não funciona com SBSAR usado em slots de canal único
&#x200B;* [Pilha de camadas] Baixo desempenho ao rolar com camadas ocultas
&#x200B;* [TextureSet] Falha ao clicar entre máscaras
&#x200B;* [SVT] O Deslocamento não é exibido corretamente e pisca em alguns casos
&#x200B;* [Alembic] Falha com malha usando normais de ponto em vez de normais de vértice
&#x200B;* [Alembic]&#x200B;[Log] Relata um erro no Log se o arquivo Alembic não for suportado durante a importação

**Problemas Conhecidos:**

&#x200B;* Arquivos Alembic com subdivisões não podem ser importados
&#x200B;* Falhas raras ao importar alguns arquivos Alembic

### 5.1.2 (2019.1.2)

*(Lançado: 21 de maio de 2019)*
Resumo: **Hotfix**

**Corrigido:**

&#x200B;* Falha ao selecionar dois recursos com uma entrada de imagem

### 5.1.1 (2019.1.1)

*(Lançado: 20 de maio de 2019)*
Resumo: **Hotfix**

**Adicionado:**

&#x200B;* Atualize para a versão mais recente do Substance Engine com a última versão do Substance Designer 2019.1

**Corrigido:**

&#x200B;* [Substance] Visível Se não for levado em consideração para Imagens de entrada
&#x200B;* [SVT]&#x200B;[Mecanismo] Alterar a resolução do conjunto de texturas leva a uma falha em alguns casos
&#x200B;* [Engine] Texturas pretas aleatórias aparecem em alguns casos
&#x200B;* [Pilha de camadas]&#x200B;[IU] Alternar uma máscara com SHIFT pode selecionar várias camadas ao mesmo tempo
&#x200B;* [Pilha de camadas] A opacidade não tem efeito no efeito Pintura com o modo de mistura Passagem
&#x200B;* [Pilha de camadas] A entrada do filtro Height para normal não é atualizada corretamente com o traçado do pincel de borracha
&#x200B;* [LayersStack] Falha ao desfazer o soltar de uma máscara inteligente
&#x200B;* Wireframe piscando com sombras e suavização de borda temporal ativada
&#x200B;* [Deslocamento] Atraso na AMD com algumas malhas pesadas
&#x200B;* [Windows] Falha ao abrir alguns projetos por meio do explorador de arquivos
&#x200B;* [Histograma] Falha ao remover a máscara com o ponto de ancoragem em alguns casos
&#x200B;* Falha na geração de visualização em alguns casos raros
&#x200B;* [Falha] Não é possível reabrir um projeto usando muitas ferramentas de clonar e borrar
&#x200B;* Nenhuma malha exibida no modo de material após salvar em alguns casos
&#x200B;* [Scripting] alg.mapexport.documentStructure() retorna valores incorretos para pastas

**Problemas Conhecidos:**

&#x200B;* Clicar duas vezes no nome do conjunto de texturas o selecionará antes de entrar no modo de renomeação

### 5.1.0 (2019.1.0)

*(Lançado: 23 de abril de 2019)*
Resumo: **Traçado dinâmico com novo conteúdo dedicado, Deslocamento e mosaico em tempo real e Iray, efeito Comparar máscara, simetria radial, Planar e Projeção esférica**

**Adicionado:**

&#x200B;* [Ferramenta] Traçado dinâmico: variação de Substance ao lado de um traçado de pincel
&#x200B;* [Traçado dinâmico] Expor novo parâmetro de índice de carimbo com opções
&#x200B;* [Traço dinâmico] Leve em consideração o parâmetro $time
&#x200B;* [Traço dinâmico] Gera novo parâmetro $randomseed por traço e por carimbo
&#x200B;* [Traçado dinâmico] Iniciar um índice de traçado dinâmico a partir de um número aleatório
&#x200B;* [Dynamic stroke]&#x200B;[Prateleira] Ajuda a encontrar um recurso de traçado dinâmico com novo ícone dedicado
&#x200B;* Deslocamento e mosaico em viewport em tempo real
&#x200B;* Deslocamento e mosaico em Irlanda
&#x200B;* [Configurações do sombreador]&#x200B;[IU] Nova guia para controlar deslocamento e mosaico
&#x200B;* [Pilha de camadas] Novo efeito CompareMask: gerar uma máscara comparando dois canais
&#x200B;* [Pilha de camadas]&#x200B;[IU] Nova entrada no menu do botão direito do mouse “Adicionar máscara com combinação de height” para inserir um efeito CompareMask
&#x200B;* [Simetria] Novo modo de simetria: pintura radial
&#x200B;* [Configurações de simetria] Expande as duas seções “Configurações” e “Exibição”
&#x200B;* [Configurações de simetria]&#x200B;[IU] Visualização para pintura radial
&#x200B;* Exponha dois novos modos de projeção: planar e esférico
&#x200B;* [Proj] Novo modo de corte de forma para todas as projeções
&#x200B;* [Proj] Modo planar com novo manipulador: ferramenta Superfície
&#x200B;* [Proj]&#x200B;[Atalho] Atalho SHIFT+W para a ferramenta Superfície
&#x200B;* [Proj] Máscara de projeção planar com seleção de profundidade e abate de backface
&#x200B;* [Manipulador] Melhoria do manipulador de rotação nos três eixos para triplanar
&#x200B;* [Tool]&#x200B;[UX] Clicar com a tecla Alt pressionada em um canal focaliza esse canal (ativa ou desativa todos os outros)
&#x200B;* [Engine] Atualização para a versão mais recente do Substance Engine
&#x200B;* [Conjunto de textura] Seleção múltipla e resolução de alteração
&#x200B;* [Conjunto de textura] Ativação e desativação rápidas dos conjuntos de textura
&#x200B;* [Conjunto de texturas] Combina solo e todas as opções em um novo menu
&#x200B;* [Conjunto de texturas]&#x200B;[Pilha de camadas] Novo ícone para ativação e desativação
&#x200B;* [Pilha de camadas]&#x200B;[UX] Inserir efeitos acima dos já selecionados
&#x200B;* [Pilha de camadas]&#x200B;[IU] Retrabalhar o estilo de seleção da exibição da pilha de camadas
&#x200B;* [Pilha de camadas] O modo de mesclagem para camadas instanciadas agora está no modo de Passagem por padrão
&#x200B;* [Exportar] Opção para ativar e desativar o pontilhamento
&#x200B;* [Plug-in] Suporte ao modificador de precisão para controles deslizantes (SHIFT)
&#x200B;* [Plug-in]&#x200B;[IU] Novo ícone para salvamento automático
&#x200B;* [Scripts] Lista o conteúdo de uma pasta
&#x200B;* [Script] Permitir exclusão de arquivos
&#x200B;* [Scripts] Ler todas as informações da pilha, inclusive os recursos usados
&#x200B;* [Conteúdo]&#x200B;[Traçado dinâmico] Novas ferramentas e predefinições de pincel
&#x200B;* [Conteúdo]&#x200B;[Traço dinâmico] Dois novos gradientes de procedimento: Matiz de gradiente e Construtor de gradiente
&#x200B;* [Content] 11 novos filtros: Pintura de descascamento MatFx, gotas de água MatFx e muito mais
&#x200B;* [Content] 7 novos geradores: Auto Stitcher, Cor aleatória UV, Densidade de texel UV e muito mais
&#x200B;* [Content] 93 novos alfas: novos textos, setas e várias outras formas
&#x200B;* [Conteúdo] 2 novos procedimentos: Matiz de gradiente, Construtor de gradiente e muito mais
&#x200B;* [Content] 21 novas predefinições de ferramenta e pincel para Traçados dinâmicos: Pebbles, Footprints, Spray e muito mais
&#x200B;* [Content] 2 Novos HDRis: Canopus Ground e Floresta de outono
&#x200B;* [Content] Atualizar conteúdo com curadoria de semente aleatória na prateleira
&#x200B;* [Content] Ícone novo com parâmetro semente aleatório exposto na prateleira

**Corrigido:**

&#x200B;* [Pilha de camadas] A pilha de camadas continua arrastando para sempre
&#x200B;* [Mac] “Mostrar no Finder” pode levar ao congelamento
&#x200B;* [Script] As configurações salvas por meio da interface do usuário personalizada são perdidas se o arquivo de sombreador for movido
&#x200B;* [Scripting] O número de versão da API está incorreto e não está atualizado
&#x200B;* [Efeito] O conteúdo do histograma não é exibido corretamente
&#x200B;* [Efeito] O efeito do histograma não é atualizado em alguns casos
&#x200B;* [Prateleira] Os pontos não estão corretamente alinhados no material “Pirâmide de tecido plástico”

**Problemas Conhecidos:**

&#x200B;* Clicar duas vezes no nome do conjunto de texturas o selecionará antes de entrar no modo de renomeação
&#x200B;* [Pilha de camadas]&#x200B;[IU] Alternar uma máscara com SHIFT pode selecionar várias camadas ao mesmo tempo

## Versão 4

### 4.3.3 (2018.3.3)

*(Lançado em: 07 de março de 2019)*
Resumo: **correção de erros**

**Adicionado:**

&#x200B;* [Content] Integrar novo modelo de projeto: “PBR - Alpha de aspereza metálica”
&#x200B;* A ordem de pesquisa da biblioteca dinâmica Linux foi alterada para priorizar as bibliotecas no diretório de instalação antes do que está instalado no sistema

**Corrigido:**

&#x200B;* A malha às vezes desaparece da viewport 3D (pressione F para redefinir a câmera)
&#x200B;* Atualize o carregador do Substance Painter Sketchfab com os novos tipos de licença do Sketchfab
&#x200B;* [Import]&#x200B;[glTF] Manipulação incorreta de modulação de textura de entrada conforme definido nos arquivos glTF
&#x200B;* [Import]&#x200B;[glTF] O plano horizontal é exibido incorretamente com a importação de glTF em alguns casos
&#x200B;* [Export]&#x200B;[USD] A opacidade não funciona no Arkit
&#x200B;* [Export]&#x200B;[USD] A exportação de USDz falha em alguns casos
&#x200B;* [Export]&#x200B;[USD] Exportar para USD sem salvar leva a falha
&#x200B;* [Export]&#x200B;[USD] Modo de divisão incorreto para texturas, modo de subdivisão para malhas e tipos de saída para sombreadores
&#x200B;* [Export]&#x200B;[USD] Exportações esparsas de apenas alguns conjuntos de textura com toda a geometria
&#x200B;* [Instância] Falha ao tentar excluir uma camada de instância quebrada
&#x200B;* [Regressão]&#x200B;[Exportar] Alguns mapas não são exportados na profundidade de bits escolhida
&#x200B;* [Linux] Problema com a biblioteca libtbb.so.2

**Problemas Conhecidos:**

&#x200B;* O congelamento da computação em alguns casos em GPUs AMD VEGA
&#x200B;* Problema do tablet Huion com atalhos no sistema operacional Windows

### 4.3.2 (2018.3.2)

*(Lançado: 24 De Janeiro De 2019)*
Resumo: **Hotfix com novos recursos (exportação USDZ e filtragem de textura no visor)**

**Adicionado:**

&#x200B;* [Exportar] Permitir exportação para USDZ
&#x200B;* [Visor] Permite controlar a qualidade da textura nas Configurações de exibição
&#x200B;* [Visor] Configuração de polarização mip adicionada nas Configurações de exibição
&#x200B;* [Visor] Filtragem anisotrópica adicionada nas Configurações de Exibição
&#x200B;* [plugins] Atualize os plugins oficiais para usar o estilo do Substance Painter 2018
&#x200B;* [License] Instalar licença por padrão em uma pasta de usuário

**Corrigido:**

&#x200B;* Falha vinculada à descompactação
&#x200B;* Adicionar TAA em material solo
&#x200B;* Ruído com sombra, TAA e sombreador de teste alfa com pontilhamento
&#x200B;* Remover pontilhamento de specular para todos os sombreadores PBR clássicos
&#x200B;* Falha nas configurações do sombreador em alguns casos
&#x200B;* A ativação de dispersão não está sincronizada entre as renderizações OpenGL e Iray
&#x200B;* As ferramentas Borrar e Clonar não funcionam mais em malhas específicas
&#x200B;* Alguns conjuntos de texturas não podem aparecer na renderização Iray
&#x200B;* Os conjuntos de texturas renomeados não são salvos após o fechamento do projeto
&#x200B;* Artefatos de wireframe ao arrastar e soltar materiais em mapas de ID
&#x200B;* [Script] Criação de caminho de arquivo não forçada ao salvar um projeto
&#x200B;* [Scripting] O retorno de chamada “onProjectAboutToSave()” não funciona mais
&#x200B;* Links do fórum quebrados na janela de erro do relatório

**Problemas Conhecidos:**

&#x200B;* O congelamento da computação em alguns casos em GPUs AMD VEGA
&#x200B;* Problema do tablet Huion com atalhos no sistema operacional Windows

### 4.3.1 (2018.3.1)

*(Lançado em: 06 de dezembro de 2018)*
Resumo: **Hotfix**

**Adicionado:**

&#x200B;* [Simetria]&#x200B;[Janela de visualização] A pintura de simetria na exibição 2D está de volta e agora apresenta uma visualização de pincel de clone corrigida

**Corrigido:**

&#x200B;* [Exportar] A exportação de exibição 2D gera uma textura preta em alguns casos
&#x200B;* [Iray] Informações normais se tornam incorretas em Iray após instanciar uma camada de material
&#x200B;* Conjuntos de textura não quadrada podem levar, em alguns casos, a falhas
&#x200B;* [Desfazer] Várias teclas Ctrl+Z podem levar aleatoriamente, em alguns casos, a falhas
&#x200B;* [QML] O AlgScrollView pode criar um aviso no registro em alguns casos (loops de ligação)

**Problemas Conhecidos:**

&#x200B;* O congelamento da computação em alguns casos em GPUs AMD VEGA
&#x200B;* Problema do tablet Huion com atalhos no sistema operacional Windows
&#x200B;* A suavização de borda e as sombras quando ativas em conjunto podem gerar resultados inesperados

### 4.3.0 (2018.3.0)

*(Lançado: 20 de novembro de 2018)*
Resumo: <b>Atualizações de viewport, exportação de visualização 2D adequada, novos auxiliares de interface, uma ferramenta de simetria aprimorada, novo conteúdo e um enorme aumento no desempenho</b>

<b>Adicionado:</b>

&#x200B;* [Suavização de borda]&#x200B;[Janela de visualização] Nova filtragem de suavizações temporais para a janela de visualização 3D (através das Configurações de exibição)
&#x200B;* [Exportar] Exporta o conteúdo da viewport 2D como uma textura única
&#x200B;* [Exportar]&#x200B;[Pontilhamento] Expor pontilhamento na exportação
&#x200B;* [Pilha de camadas] Cores em camadas e pastas
&#x200B;* [Pilha de camadas] Ativação e desativação rápidas de várias camadas e efeitos
&#x200B;* [Pilha de camadas] Navegação mais fácil para modos de mesclagem com teclas para cima e rolagem do mouse
&#x200B;* [Proj]&#x200B;[UI] Manipulador de rotação adicional nos três eixos para triplanar
&#x200B;* [Proj]&#x200B;[Atalhos] - e + para alterar o tamanho do manipulador de Projeção UV
&#x200B;* [Shader] Controle os parâmetros de camada com canais no sombreador revestido por PBR
&#x200B;* [Substance] Expor novas entradas de textura com base em malha para filtros e geradores
&#x200B;* [Simetria]&#x200B;[Visor]&#x200B;[IU] Controla o deslocamento de simetria com manipuladores
&#x200B;* [Simetria]&#x200B;[Barra de ferramentas contextual]&#x200B;[IU] Novo painel de simetria com opções
&#x200B;* [Simetria] Novo modo de interseção de linha de simetria
&#x200B;* [Simetria] Novo cursor de clone de simetria
&#x200B;* [Simetria]&#x200B;[Atalhos] Q para ocultar e -, + para alterar o tamanho e shift para ajustar
&#x200B;* [Log] Aprimorar mensagens de erro quando não for possível exportar texturas
&#x200B;* [Script] Permitir a alteração ou atualização dos recursos em Configurações de exibição
&#x200B;* [Script] Permitir a criação ou a remoção de canais em Conjuntos de Textura
&#x200B;* [Content]&#x200B;[Shaders] Adicionar suporte para anisotropia com um sombreador dedicado (pbr-metal-rough-anisotropia-angle)
&#x200B;* [Conteúdo] Atualização da esfera de visualização com anisotropia e ângulo modificado
&#x200B;* [Content] shutline matFx atualizado
&#x200B;* [Content] New Texturing.XYZ varredura de rosto sem emenda
&#x200B;* [Conteúdo] Novos procedimentos anisotrópicos
&#x200B;* [Content] Novo filtro: ambiente de iluminação baked
&#x200B;* [Content] Novo mapa ambiental: estúdio automotivo neutro
&#x200B;* [Content] Novo modelo de projeto: PBR - ângulo de Anisotropia de aspereza metálica (com canais de anisotropia)
&#x200B;* [Content] Novo modelo de projeto: PBR - aspereza metálica revestida
&#x200B;* [SVT]&#x200B;[Engine] Texturas virtuais esparsas (SVT)
&#x200B;* [SVT]&#x200B;[Preferências]&#x200B;[IU] Opção de aceleração de suporte a hardware SVT
&#x200B;* [SVT]&#x200B;[Log] Informações adicionais para o recurso Texturização Virtual Esparsa (por exemplo, tamanho do disco)
&#x200B;* [SVT]&#x200B;[UI] Janela de mensagem na inicialização se o tamanho no disco for muito baixo para o cache
&#x200B;* Localização do cache global de Substance Painter [SVT]&#x200B;[Preferências]&#x200B;[UI]
&#x200B;* [SVT] Nova variável de ambiente para especificar o caminho do cache de Substance Painter
&#x200B;* [SVT] Nova variável de ambiente para ativar a aceleração de suporte de hardware SVT
&#x200B;* [SVT] Detectar suporte esparso por hardware
&#x200B;* [SVT]&#x200B;[Dispersão de hardware] Aumentar a versão mínima do driver para a GPU Nvidia
&#x200B;* [SVT]&#x200B;[Shader]&#x200B;[Viewport]&#x200B;[UI] Avisa o usuário se artefatos presentes com Texturização virtual esparsa na abertura do projeto

<b>Corrigido:</b>

&#x200B;* [Seletor de cores] Cursor de pintura que aparece ao tentar selecionar uma cor
&#x200B;* A falha ao selecionar ou cancelar a seleção de camadas em uma ordem específica pode causar falha
&#x200B;* Falha ao colar como uma ocorrência uma camada com uma máscara
&#x200B;* [User Channel]&#x200B;[Regression] Falha ao renomear canal de usuário
&#x200B;* [User Channel] Visualização do pincel esmaecido
&#x200B;* [Alembic] Somente uma textura definida de vários materiais após a importação
&#x200B;* [Engine] A textura exportada é diferente da viewport para carimbos de pincel
&#x200B;* [Mecanismo] Inverter com um efeito de nível não afeta totalmente uma textura
&#x200B;* O seletor de material está aplicando um traçado de pincel ao separar
&#x200B;* Alternar a resolução para 128x128px leva a um travamento
&#x200B;* Os links de mapas de malha não são atualizados corretamente ao reorganizar ou instanciar camadas
&#x200B;* [Substance] O espaço de cor UserData não funciona no normal de malha cozida solicitado como entrada
&#x200B;* Incompatibilidade de associação MDL ao usar várias instâncias de sombreadores
&#x200B;* [Simetria]&#x200B;[Camada de preenchimento] Plano de simetria e seu manipulador ativo na Camada de preenchimento
&#x200B;* [Visor] O ponto dinâmico para tradução nem sempre é atualizado após clicar
&#x200B;* [UI] Ícones corrigidos e remoção de espaços reservados para monitores HDPI

<b>Problemas Conhecidos:</b>

&#x200B;* O congelamento da computação em alguns casos em GPUs AMD VEGA
&#x200B;* Problema do tablet Huion com atalhos no sistema operacional Windows
&#x200B;* A suavização de borda e as sombras quando ativas em conjunto podem gerar resultados inesperados

### 4.2.3 (2018.2.3)

*(Lançado: 25 de setembro de 2018)*

**Corrigido:**

&#x200B;* [2D View] A visualização 2D é quebrada com algumas malhas ao criar um novo projeto
&#x200B;* [Falha] Alternar de Projeção UV para projeção triplanar leva a um travamento
&#x200B;* [RayCollider] Várias falhas devido ao “RayCollider”
&#x200B;* [Ferramenta] A alternância de camadas perde as propriedades modificadas do pincel
&#x200B;* As configurações do pincel são redefinidas ao alternar para a borracha

**Problemas Conhecidos:**

&#x200B;* Congelamento de computação em GPUs AMD VEGA
&#x200B;* Problema do tablet Huion com atalhos no sistema operacional Windows

### 4.2.2 (2018.2.2)

*(Lançado: 11 de setembro de 2018)*
Resumo: **Hotfix com atualização de conteúdo, novas funcionalidades de script e capacidade de desabilitar a atualização automática**

**Adicionado:**

&#x200B;* [Conteúdo]&#x200B;[Prateleira] Adicionar uma predefinição de prateleira de pele
&#x200B;* [Content]&#x200B;[shelf] Conversão de 19 normais de pele em materiais para dispersão subsuperficial
&#x200B;* [Script] Criar um modelo de projeto a partir de um projeto aberto
&#x200B;* [Script] Obter/Definir configurações de exportação de um projeto aberto
&#x200B;* [Atualizações] Desative o pop-up de atualização automática nas configurações e na variável de ambiente
&#x200B;* [Atualizações] Não exibir até a próxima versão do pop-up de manutenção desatualizada

**Corrigido:**

&#x200B;* [Câmera] Zoom incorreto ao alternar de ortográfica para Perspectiva
&#x200B;* [Exibir] Alguns mapas são exibidos em linear em vez de sRGB
&#x200B;* [Visores] O foco da malha não se comporta corretamente
&#x200B;* [Visualização 2D] O projeto com a câmera quebrada tem Shells UVs em desaparecimento
&#x200B;* [SSS]&#x200B;[Dica de ferramenta] as dicas de ferramentas de dispersão da subsuperfície aparecem no registro
&#x200B;* Alguns projetos não podem ser abertos em 2018.2 e a mensagem de erro não pode salvar um pacote nulo do substance
&#x200B;* [Máscara] A cor da ferramenta de Tinta pode travar em alguns casos ao trabalhar em uma máscara
&#x200B;* [Material] Mapas que não aparecem em situações específicas
&#x200B;* [Proj]&#x200B;[Tools] Manipulador ativo com um gerador
&#x200B;* [Substance] Grupos de Substance de parâmetros ausentes
&#x200B;* [Scripting] Nome de software incorreto na documentação
&#x200B;* [UDIMs] Não há informações no log sobre shells UVs em vários blocos UVs

**Problemas Conhecidos:**

&#x200B;* Congelamento de computação em GPUs AMD VEGA
&#x200B;* Problema do tablet Huion com atalhos no sistema operacional Windows

### 4.2.1 (2018.2.1)

*(Lançado em: 3 de agosto de 2018)*

**Corrigido:**

&#x200B;* Parâmetros de sombreador de dispersão de subsuperfície ausentes em projetos de atualização

**Problemas Conhecidos:**

&#x200B;* Congelamento de computação em GPUs AMD VEGA
&#x200B;* Problema do tablet Huion com atalhos no sistema operacional Windows

### 4.2.0 (2018.2.0)

*(Lançado em: 2 de agosto de 2018)*
Resumo: **Versão de verão, suporte a dispersão de subsuperfície, melhorias de projeção e preenchimento, importação e seleção de câmera, suporte a Alembic e glTF, arrastar e soltar no mapa de ID, suporte aprimorado ao formato Substance e novo conteúdo**

**Adicionado:**

&#x200B;* [SSS]&#x200B;[Viewport]&#x200B;[Iray] Dispersão genérica de subsuperfície
&#x200B;* [SSS] Sincronizar parâmetros de dispersão da subsuperfície e MDL
&#x200B;* [SSS] Adicionado um novo canal em tons de cinza chamado Dispersão
&#x200B;* [SSS]&#x200B;[Configurações do sombreador] Parâmetro de tipo de dispersão para dispersão subsuperficial (pele ou translúcida)
&#x200B;* [SSS]&#x200B;[Configurações do sombreador] Parâmetro de escala de dispersão para dispersão subsuperficial
&#x200B;* [SSS]&#x200B;[Configurações do sombreador] Parâmetro de cor de dispersão para dispersão subsuperficial
&#x200B;* [SSS]&#x200B;[Configurações de exibição] Contagem de amostra de dispersão para dispersão subsuperfície
&#x200B;* [Shader]&#x200B;[Iray] Integrar MDL de dispersão de subsuperfície para Iray
&#x200B;* [Shader] Atualização do sombreador por meio do atualizador de recursos
&#x200B;* [Shader] Atualizar a API e a documentação do log de alterações
&#x200B;* [Propriedades da ferramenta]&#x200B;[Proj] Novos parâmetros para a projeção triplanar
&#x200B;* [Visor]&#x200B;[Proj] Controlar as propriedades da Camada de preenchimento na exibição 3D diretamente com manipuladores (projeção triplanar)
&#x200B;* [Shortcuts]&#x200B;[Proj] Novos atalhos Q, W, E, R, T para manipuladores de projeção triplanar
&#x200B;* [Viewport]&#x200B;[Proj] Controlar as propriedades da Camada de preenchimento na exibição 2D diretamente com manipuladores (Projeção UV)
&#x200B;* [Shortcuts]&#x200B;[Proj] Novo atalho Q para manipuladores de Projeção UV
&#x200B;* [Barra de ferramentas contextual]&#x200B;[Proj] Controla os manipuladores de projeção triplanar
&#x200B;* [Barra de ferramentas contextual]&#x200B;[Proj] Controlar manipuladores de Projeção UV
&#x200B;* [Propriedades da ferramenta] Desativar a divisão em blocos gráficos de textura com a ferramenta Projeção e Estêncil
&#x200B;* [Estêncil] Usar imagens não quadradas com a ferramenta de projeção/estêncil
&#x200B;* [Estêncil] Permitir o controle do modo de divisão em blocos gráficos na janela Propriedades
&#x200B;* [Estêncil] O zoom não está centralizado em um estêncil sem divisão em blocos gráficos
&#x200B;* [Câmeras] Importar câmeras do Maya, Max, Blender, Modo, DAE
&#x200B;* [Câmeras]&#x200B;[Visor] Selecionar e controlar câmeras importadas no visor
&#x200B;* [Câmeras]&#x200B;[Iray] Selecionar e controlar câmeras importadas no Iray
&#x200B;* [Câmeras]&#x200B;[IU]&#x200B;[Novo projeto]&#x200B;[Configuração do projeto] Importar câmeras é verificado por padrão
&#x200B;* [Câmeras]&#x200B;[Atalhos] Adicionar atalhos para alternar entre câmeras
&#x200B;* [Câmeras]&#x200B;[Visor] Adicionar quadro no visor
&#x200B;* [Câmeras]&#x200B;[Configurações do visor] Controle de opacidade de quadro
&#x200B;* [Câmeras]&#x200B;[Configurações da câmera] distância focal máxima em 500 mm
&#x200B;* [Câmeras]&#x200B;[Configurações da câmera] Taxa de exposição
&#x200B;* [Câmeras]&#x200B;[Configurações da câmera] Adicionar uma opção de bloqueio
&#x200B;* [Câmeras]&#x200B;[Configurações da câmera] Adicionar uma opção de restauração
&#x200B;* [Câmeras]&#x200B;[Configurações de câmera] Adicionar atributo de distância de foco
&#x200B;* [glTF] Importação de um arquivo glTF
&#x200B;* [glTF] Importar mapa de oclusão de ambiente
&#x200B;* [Alembic] Importar quadro Alembic 1 com geometria estática
&#x200B;* [Prateleira] Arraste e solte materiais diretamente na malha usando mapas de ID com um modificador (CTRL/Command)
&#x200B;* [Pilha de camadas] Criação automática de máscara de ID com arrastar e soltar materiais na malha com mapas de ID
&#x200B;* [Pilha de camadas] Rolagem automática de camadas com arrastar e soltar na pilha de camadas
&#x200B;* [UI]&#x200B;[Propriedades da ferramenta] Expor predefinição de Substance
&#x200B;* [UI]&#x200B;[Menu Ajuda] Aprimoramento do menu Ajuda
&#x200B;* [UI]&#x200B;[Novo projeto]&#x200B;[Configuração do projeto] Reorganização da janela
&#x200B;* [UI]&#x200B;[Novo projeto]&#x200B;[Configuração de projeto] Substituir termo de malha por arquivo
&#x200B;* [UI]&#x200B;[Substance] Exibir atributos de Substance na interface
&#x200B;* [Atalhos] F4 alterna entre as exibições 2D e 3D
&#x200B;* [Atalhos] Novos atalhos para alternar estêncil N e máscara rápida U
&#x200B;* [Integração Substance] Leve em consideração as instruções &#39;visible if&#39; nos parâmetros Substance
&#x200B;* [Janela de visualização] As sombras não são forçadas a serem computadas após a movimentação da câmera
&#x200B;* [Content] Atualizar o MeetMat com câmeras importadas
&#x200B;* [Content] Adicionar uma amostra com dispersão subsuperficial ativada - JadeToad
&#x200B;* [Content] Adicionar um novo modelo de projeto PBR com a dispersão subsuperficial ativada
&#x200B;* [Conteúdo] Predefinições de exportação atualizadas para adicionar um novo canal de Dispersão
&#x200B;* [Content]&#x200B;[Prateleira] Adicionado suporte à dispersão de subsuperfície para: pbr-metal-rough, pbr-metal-rough-alpha-test, pbr-coated, pbr-spec-gloss
&#x200B;* [Content]&#x200B;[Prateleira] Adicionado canal de dispersão para 5 materiais inteligentes (mármores e peles)
&#x200B;* [Content]&#x200B;[Shelf] 1 novo material jade
&#x200B;* [Conteúdo]&#x200B;[Prateleira] 1 novo material de cera

**Corrigido:**

&#x200B;* [CMD] Resultados diferentes usando a mesma linha de comando com versões diferentes
&#x200B;* [TDR] Se o TdrLevel estiver configurado, você não tem erros no seu registro
&#x200B;* [Baker] O mapa de oclusão do ambiente está invertido
&#x200B;* [Mapa de ID] Falha ao separar fora do intervalo 0-1
&#x200B;* [Iray] Falha ao alternar conjuntos de texturas e voltar para o modo de Pintura
&#x200B;* [Janela de visualização] Sincronizar áreas de soltar entre portas de visualização para arrastar e soltar
&#x200B;* [Engine] Artefato Moiré ao colocar camadas de preenchimento lado a lado ou pintar um pequeno pincel
&#x200B;* [License] Verificação de versão de software incorreta do serviço de licença
&#x200B;* [Licença] Reformular a maneira como lidamos com a autenticação
&#x200B;* [API] Chamar o evento de API de script onNewProjectCreated mesmo ao criar com um modelo
&#x200B;* [Shader] O sombreador compilado não é carregado do cache quando o arquivo de sombreador não é compilado
&#x200B;* [Prateleira] Exportar arquivo HDR da prateleira exibirá um arquivo com valores fixados
&#x200B;* [Exportar] A exportação de EXR mantém os valores de cor do RGB entre 0 e 1
&#x200B;* [Conteúdo] O fractal de ruído Perlin 3D de ruído de procedimento está pixelado

**Problemas Conhecidos:**

&#x200B;* Congelamento de computação em GPUs AMD VEGA
&#x200B;* Problema do tablet Huion com atalhos no sistema operacional Windows

### 4.1.3 (2018.1.3)

*(Lançado: 28 de junho de 2018)*

**Adicionado:**

&#x200B;* [Preferências] Proponha salvar o projeto quando o Painter for reiniciado

**Corrigido:**

&#x200B;* [Plug-in] O Substance Source de pesquisa não funciona
&#x200B;* [Materiais inteligentes] A importação de materiais inteligentes leva a uma falha em alguns casos
&#x200B;* [Materiais inteligentes] Excluir materiais inteligentes leva a uma falha em alguns casos
&#x200B;* [Salvar] Salvar leva a uma falha em alguns casos raros
&#x200B;* [Prateleira] Inverter não funciona no Células 2 e no Células 3
&#x200B;* [Prateleira] Erro de digitação em alguns Alpha
&#x200B;* [Prateleira] Alguns materiais da substância não renderizam corretamente

**Problemas Conhecidos:**

&#x200B;* Congelamento de computação em GPUs AMD VEGA

### 4.1.2 (2018.1.2)

*(Lançado: 12 de junho de 2018)*
Resumo: **Velocidade de cozimento aprimorada, Sistema de salvamento aprimorado, Controles deslizantes atualizados, API de plug-in atualizada, Tradução para chinês, Preenchimento aprimorado agora opcional**

**Adicionado:**

&#x200B;* [Padeiros] Melhoria de desempenho com nova versão de panificação
&#x200B;* Forçar caixa de diálogo de exibição com GPU incompatível
&#x200B;* [Salvar] Expor a nova funcionalidade de projeto compacto (modo de salvamento completo/compacto)
&#x200B;* [Salvar] Informar o usuário em caso de erro ao salvar
&#x200B;* [Clean] Próxima gravação no modo completo/compacto
&#x200B;* [Controles deslizantes] Aprimoramento da precisão das barras e dos controles deslizantes de cor/escala de cinza
&#x200B;* [Controles deslizantes] Adição de controles de seta para cima ou para baixo
&#x200B;* [Controles deslizantes] Mesma zona de detecção para controles deslizantes de barra colorida e de tons de cinza
&#x200B;* [Plug-in] Salvamento automático sempre em modo incremental
&#x200B;* [Plug-in] Opção para alternar plug-ins para o novo estilo de interface
&#x200B;* [Language] Adicionar tradução para chinês
&#x200B;* [Preenchimento] Opção para alternar entre o preenchimento UV e vizinho de espaço 3D por Textura Definida nas Configurações do conjunto de textura
&#x200B;* [Script] Modo de salvamento de exposição: completo/compacto ou incremental
&#x200B;* [Script] Atualizar script/documentação QML
&#x200B;* [Log] Indica o modo de salvamento no log (completo/compacto ou incremental)

**Corrigido:**

&#x200B;* [Ferramenta] O slot do canal se transforma em um slot de material em preenchimentos de canal único
&#x200B;* Falha ao carregar uma malha (FBX) com algumas faces não atribuídas por um material
&#x200B;* Falha na Iray com NVIDIA GRID 5.2 na máquina virtual
&#x200B;* Falha ao desfazer uma exclusão de predefinição de material
&#x200B;* Falha ao carregar alguns projetos
&#x200B;* [Linha de comando] Nova linha de comando para malhas UDIM divididas por udim
&#x200B;* [Barra de ferramentas] Redução da barra de ferramentas
&#x200B;* [Instanciação] Não é possível instanciar bitmaps em vários conjuntos de texturas
&#x200B;* [Janela de visualização] A atualização não é concluída ao pintar na malha com UVs lado a lado
&#x200B;* [Iray] O mapa normal é aplicado duas vezes para dielétricos
&#x200B;* [Prateleira] Erros de digitação em alguns parâmetros de Substance (alfas, procedimentos e matfx)
&#x200B;* [Shelf] Erro de ortografia no bitmap “Somente Pessoal Autorizado”
&#x200B;* [Script] A função alg.shaders.materials() não funciona mais

**Problemas Conhecidos:**

&#x200B;* Congelamento de computação em GPUs AMD VEGA

### 4.1.1 (2018.1.1)

*(Lançado em: 3 de abril de 2018)*

**Corrigido:**

&#x200B;* [Tablet] Problema ao alterar as opções de interação padrão
&#x200B;* [Bakers] Falha com a biblioteca Assimp
&#x200B;* [Bakers] Regressão no desempenho com mapa A.O.
&#x200B;* [Iray] A Distorção de lente não é aplicada ao canal de Alpha
&#x200B;* [Drivers] Atualização dos requisitos mínimos de drivers
&#x200B;* [3Dview] Normais não gerados corretamente em malhas UDIM sem informações normais
&#x200B;* [Intel] Falha com o Substance Painter 2018.1.0
&#x200B;* [Intel]&#x200B;[Visor] Problema com preenchimento (artefatos pretos)

**Problemas Conhecidos:**

&#x200B;* Congelamento de computação em GPUs AMD VEGA

### 4.1.0 (2018.1.0)

*(Lançado: 15 de março de 2018)*

**Adicionado:**

&#x200B;* Novo estilo geral (ícones, cor, comportamento)
&#x200B;* Novo layout padrão
&#x200B;* [Tablet] Aprimoramento da experiência do usuário ao pintar
&#x200B;* [Menu principal] Classificar itens nativos em exibições e barras de ferramentas primeiro
&#x200B;* [Menu principal] Mover ações de máscara rápida na seção do visor
&#x200B;* [Menu principal] Mover as ações do botão direito do mouse para a seção do visor
&#x200B;* [Menu principal] Renomear o menu “Exibir” como “Janela”
&#x200B;* [Menu rápido] Novas propriedades de ferramenta clicando com o botão direito do mouse no visor
&#x200B;* [Widget de encaixe] Nova barra de ferramentas de encaixe para redução/recuperação rápida
&#x200B;* [Configurações de exibição] Janela de configurações da câmera e do visualizador mesclada
&#x200B;* [Pilha de camadas] Menu contextual de clique com o botão direito
&#x200B;* [Pilha de camadas] Arraste e solte para mover qualquer efeito dentro da mesma camada
&#x200B;* [Barra de ferramentas] Reorganização da barra de ferramentas e da nova barra de ferramentas contextual
&#x200B;* [Barra de ferramentas Ferramentas] Dividir a ferramenta Clonar em duas ferramentas separadas
&#x200B;* [Propriedades das ferramentas] Valor de tons de cinza do plano de fundo mais claro na visualização
&#x200B;* [Propriedades das ferramentas] Organização em guias (preenchimento e ferramentas)
&#x200B;* [Ferramenta] O resultado da pintura corresponde ao estêncil
&#x200B;* [Visor] Novo cursor para camada de preenchimento
&#x200B;* [Visor] Navegação e pintura mais suaves (maior taxa de quadros)
&#x200B;* [Janela de visualização] Caixa de combinação Material/Canal/Seleção de mapa no visor
&#x200B;* [Visor] Reduzir cintilação ao girar (sombra ativada)
&#x200B;* [Prateleira] Exibir materiais por padrão ao abrir o Painter
&#x200B;* [Prateleira] Melhoria do tempo de carregamento de texturas e materiais de Substance (2 a 6 vezes mais rápido)
&#x200B;* [Prateleira] Reorganizar pastas de materiais para se ajustar à estrutura de Substance Source
&#x200B;* [Prateleira] Arraste e solte materiais diretamente na malha no visor
&#x200B;* [Prateleira] Novos ruídos 3D (Perlin, Perlin Fractal, Simplex e Worley)
&#x200B;* [Prateleira] Novo gerador de máscara de 3D linear gradient usando a posição da malha
&#x200B;* [Shelf] Ruídos básicos atualizados para suportar o expansão não quadrada
&#x200B;* [Prateleira] Adicionado novo modelo e predefinição de exportação para o Lens Studio (aplicativo Snap)
&#x200B;* [Prateleira] Materiais inteligentes e Máscaras inteligentes atualizados para usar a versão mais recente do Editor de máscaras (microdetalhes)
&#x200B;* [Shelf] Novo projeto de amostra “TilingMaterial” para criar materiais de revestimento perfeitos
&#x200B;* [Prateleira] Novas predefinições de pincel (Caligrafia, Molhado, Hachura e assim por diante)
&#x200B;* [Controles deslizantes] Novos controles deslizantes e estilo e comportamento de barras de tons de cinza/cores
&#x200B;* [Padeiros] Permitir o uso de uma caixa delimitadora de cena inteira para calcular o mapa de posição
&#x200B;* [Shader] Remove o parâmetro de força de height dos parâmetros de sombreador padrão
&#x200B;* [Engine] Mecanismo de Substance atualizado
&#x200B;* [Engine] Nenhuma ou menos descontinuidades nos blocos UV
&#x200B;* [Plug-ins] Importar materiais baixados do Substance Source mais rapidamente
&#x200B;* [Plug-ins] Atualizar todos os plug-ins para corresponder ao novo estilo geral
&#x200B;* [Preferências] Visualizar alterações de cor de fundo automaticamente
&#x200B;* [Simples] Risco reduzido de corrupção do projeto
&#x200B;* [Aberto] Aperfeiçoamento do tempo do projeto de abertura
&#x200B;* [Novo projeto] Novo projeto - melhoria no tempo de atualização da malha
&#x200B;* [Salvar] Salvando a melhoria no tempo do projeto
&#x200B;* [Log] Tipo de licença relatado no log
&#x200B;* [TextureSet] Renomeie o botão “Bake Textures” como “Bake Mesh Maps”
&#x200B;* Renomear “Mapas adicionais” como “Mapas de malha”

**Corrigido:**

&#x200B;* [Visor] Maus desempenhos com malhas que contêm muitos subobjetos
&#x200B;* [Propriedades de ferramentas] Canal desativado ao arrastar e soltar uma imagem no slot de material
&#x200B;* [Propriedades das ferramentas] A visualização do pincel é interrompida com as ferramentas de borrar e clonar
&#x200B;* [Conjunto de texturas] A ordem dos canais está incorreta ao usar modelos
&#x200B;* [Prateleira] Ícone ausente para o gerador de conversão em tons de cinza
&#x200B;* [Prateleira] O Número de Círculo do Sinal alfa está quebrado (fonte ausente)
&#x200B;* Detecção incorreta de GPUs integradas na inicialização
&#x200B;* [Falha] Arrastar e soltar um recurso importado nomeado com um caractere #
&#x200B;* [Engine] Problema de detecção de Vram na GPU integrada
&#x200B;* [Engine] Corrigidas várias falhas no Substance Engine Linker
&#x200B;* [Engine] Artefatos quadrados ao alterar a resolução
&#x200B;* [Post Effects] O redimensionamento da interface fica lento quando os pós-efeitos estão ativados
&#x200B;* [Padeiros] A unidade de cena não é respeitada corretamente para valores de distância de raio
&#x200B;* [Bakers] A distância do Ocluder da malha é fixada em 1, independentemente do valor de entrada
&#x200B;* [Padeiros] Corresponder pelo nome ignora algumas malhas com nomes específicos
&#x200B;* [Padeiros] A cor da configuração de malha Poligrupo e ID de submalha sempre retorna uma imagem preta
&#x200B;* [Bakers] A cozedura de ID falha com malhas binárias FBX do Blender
&#x200B;* [Sombreador] Ruído no Visualização 2D com brilho dota-2 e não pbr-spec
&#x200B;* [Linux] Somente um thread de CPU é usado ao fazer bake
&#x200B;* [MacOS] Falha com o cursor do pincel se movendo sobre a janela de visualização

**Problemas Conhecidos:**

&#x200B;* Congelamento de computação em GPUs AMD VEGA
&#x200B;* Pós-processo de distorção não levado em conta ao exportar no IRay (alfa)

## Versão 3

### 3.4.2 (2017.4.2)

*(Lançado: 24 de janeiro de 2018)*

**Adicionado:**

&#x200B;* [Exportar] Obter o status de uma exportação com progresso de etapa
&#x200B;* [Exportar] Permitir o cancelamento de uma exportação
&#x200B;* [Exportar] Exportar texturas para o Sketchfab sem perder a qualidade do mapa normal
&#x200B;* [Exportar] Exportar no formato binário glTF (glb)
&#x200B;* [Exportar] Permitir o redimensionamento de colunas na guia Configuração da janela de exportação
&#x200B;* [Sombreador] Adicionar um registro de alterações para o API de sombreamento
&#x200B;* [Script] Adicionar funções de retorno de chamada Antes e Depois ao exportar textura
&#x200B;* [Iray] Atualização para o SDK 2017.1 (suporte a Volta GPUs)

**Corrigido:**

&#x200B;* Falha ao sair do aplicativo antes que a janela principal seja exibida
&#x200B;* [MAC] Falha ao carregar mapas em tons de cinza com IRAY
&#x200B;* [MAC] A detecção de VRAM não está correta com o novo sistema operacional High Sierra
&#x200B;* [Plug-in] Baixar ativos do Substance Source não funciona mais
&#x200B;* [Script] Detecção de versão mínima incorreta do plug-in
&#x200B;* [Exportar] Falha ao salvar a predefinição de exportação após exportar o textura
&#x200B;* [Instanciação] Problema em geradores instanciados em um TextureSet sem Mapas Adicionais
&#x200B;* [Visor] O pontilhamento não funciona com resolução acima de 4k
&#x200B;* [Visor] A exibição de material 2D é coberta por ruído
&#x200B;* [Prateleira] Melhorar o tempo de carregamento das predefinições de prateleira
&#x200B;* [Engine] Mesclagem incorreta ao pintar com seleção de cores

### 3.4.1 (2017.4.1)

*(Lançado: 15 de dezembro de 2017)*

**Adicionado:**

&#x200B;* [Script] Exportar malha por meio da API de script
&#x200B;* [Importação] Desativa a importação de formato de arquivo de malha não suportado (permitir somente obj, fbx, dae, ply)
&#x200B;* [Log] Indique com mais precisão o problema de TDR no arquivo de registro

**Corrigido:**

&#x200B;* Falha se o aplicativo for fechado antes da conclusão do rastreamento de recursos
&#x200B;* Falha ao abrir projetos com a ferramenta Borrar/Clonar
&#x200B;* Falha ao usar a ação de refazer após desfazer uma alteração de Sombreador nas Configurações do visualizador
&#x200B;* [Engine] A texturização difere entre o Painter 2017.2 e 2017.4
&#x200B;* [Visor] A separação em um mapa de ID de uma instância obtém a amostra da cor errada
&#x200B;* [Export] Falha ao exportar uma textura normal ou de oclusão inválida
&#x200B;* [Exportar] Os arquivos de PSD têm seus grupos bloqueados quando abertos no Photoshop CS6
&#x200B;* [Plug-in] O plug-in do Photoshop ignora a seleção de canal e sempre exporta tudo
&#x200B;* [Camadas] As âncoras são rompidas quando copiadas/coladas em conjuntos de texturas
&#x200B;* [Camadas] Algumas referências de âncora não podem ser restauradas se estiverem quebradas
&#x200B;* [Shader] O parâmetro de aspereza secundária revestido com pbr está danificado
&#x200B;* [Steam] O pop-up do verificador de versão não deve estar visível na inicialização

**Problemas Conhecidos:**

&#x200B;* [AMD] Falha/Congela ao tentar pintar em uma malha. Pode ser corrigido com uma atualização de driver de GPU.

### 3.4.0 (2017.4.0)

*(Lançado: 23 de novembro de 2017)*

**Adicionado:**

&#x200B;* [Instanciação] Permite criar instâncias de parâmetros em camadas
&#x200B;* [Instanciação] Permite saltar entre uma camada de origem e uma instância
&#x200B;* [Instanciação] Adicionar uma ação “instanciar em conjuntos de texturas”
&#x200B;* [Instanciação] Indique na pilha de camadas instâncias reentrantes (ciclos)
&#x200B;* [Instância] Excluir instâncias quando uma origem é removida
&#x200B;* [Instanciação] Não permitir referências de Âncora de fora de uma pasta de instância
&#x200B;* [UI] Mova a pilha Desfazer para sua própria janela chamada “History”
&#x200B;* [Plug-in] Plug-in de integração de link dinâmico DCC
&#x200B;* [Mecanismo] Aprimorar o desempenho da pintura com pintura Esparsa
&#x200B;* [Exportar] Adicionar opções de rascunho e reexportação ao exportador do Sketchfab
&#x200B;* [Prateleira] Adicionar controle “virar” para substâncias de fonte
&#x200B;* [Prateleira] Adicione 20 novos materiais de procedimento
&#x200B;* [Prateleira] Adicione 40 novos mapas grunges (bitmap baseado e procedimento)
&#x200B;* [Visor] Ativar colisões de visualização de pincel em outros conjuntos de texturas visíveis
&#x200B;* Atualizar os requisitos mínimos dos drivers de GPU AMD

**Corrigido:**

&#x200B;* Falha ao computar Substance em resoluções muito grandes
&#x200B;* Falha ao pintar fortemente com partículas
&#x200B;* [Visor] Reflexo de specular incorreto na exibição 2D com malhas específicas
&#x200B;* [UI] Algumas ações indesejadas são exibidas na janela Histórico

**Problemas Conhecidos:**

&#x200B;* [Camadas] Algumas referências de âncora não podem ser restauradas se estiverem quebradas
&#x200B;* Falha ao usar a ação de refazer após desfazer uma alteração de Sombreador nas Configurações do visualizador

### 3.3.3 (2017.3.3)

*(Lançado em: 01 de dezembro de 2017)*

**Corrigido:**

&#x200B;* [Steam] O pop-up do verificador de versão não deve estar visível na inicialização
&#x200B;* [Exportar] Os arquivos de PSD têm seus grupos bloqueados quando abertos no Photoshop CS6

### 3.3.2 (2017.3.2)

*(Lançado: 20 De novembro De 2017)*

**Adicionado:**

&#x200B;* [IU] Aprimorar a caixa de diálogo da nova versão e adicionar changelog
&#x200B;* [UI] Indica se a manutenção expirou na caixa de diálogo de nova versão
&#x200B;* [License] Atualizar o sistema de licenças para lidar com as Datas de manutenção
&#x200B;* [Exportar] Renomear material padrão da Adobe para Adobe Dimension

**Corrigido:**

&#x200B;* [Mac] A pintura resulta em quadrados pretos e corrupções de textura
&#x200B;* [Engine] Às vezes, o cache pode desaparecer no visor
&#x200B;* [Engine] Artefatos de bloco aparecem quando o acionador de compactação de memória
&#x200B;* [Fazendo bake] Mensagens de erro estranhas ao fazer bake malhas específicas
&#x200B;* [Export] PSD são gravados incorretamente e não são reconhecidos corretamente pelo Photoshop
&#x200B;* [Camadas] Não deveria ser possível copiar/colar camadas em vários projetos
&#x200B;* [Substance] O espaço de cores UserData para a entrada Normal é invertido em alguns casos
&#x200B;* [Prateleira] Micro-normal em geradores produz curvatura invertida
&#x200B;* [Prateleira] O filtro HSL também afeta o canal alfa
&#x200B;* [Linux] A instalação em Centos falha devido a dependências ausentes
&#x200B;* O instalador não remove todos os recursos da instalação anterior em certos casos

### 3.3.1 (2017.3.1)

*(Lançado: 26 de outubro de 2017)*

**Adicionado:**

&#x200B;* [Exportar] Permite exportar a malha de um projeto
&#x200B;* [Prateleira] Remover “Sub-prateleira” dos títulos das guias
&#x200B;* Salvar configurações de pós-processamento em modelos
&#x200B;* Tornar a mensagem TDR mais compreensível
&#x200B;* Melhorar a janela Configurações para relatar erros

**Corrigido:**

&#x200B;* Falha ao excluir várias subprateleiras
&#x200B;* Falha ao alternar de um nível para algo diferente durante um cálculo do mecanismo
&#x200B;* [Mac] Falha na GPU Intel durante cálculos de mecanismo
&#x200B;* [Mac]&#x200B;[Viewport] Desempenho insatisfatório quando o pontilhamento está habilitado
&#x200B;* [Mac] O MacOS 10.13 é reconhecido como “Versão desconhecida” no arquivo de log
&#x200B;* [Baker] Cozinhar com uma gaiola não funciona mais
&#x200B;* [Camadas] O atalho Ctrl + C (ação de cópia) não funciona mais
&#x200B;* [Camadas] Colar camadas não atualiza a interface com as referências da âncora
&#x200B;* [Âncora] Duplicar ou copiar/colar camada com referências quebra os links
&#x200B;* [Exportar] A exportação em 8K pode travar ou bloquear o aplicativo em alguns casos
&#x200B;* [Exportar] Vários problemas no formato de arquivo glTF gerado
&#x200B;* [Importar] A reimportação de uma malha com o mesmo nome de arquivo não funciona mais
&#x200B;* [Plug-in] A janela de salvamento automático sempre aparece acima de tudo
&#x200B;* [UI] Loop infinito ao pressionar “Escape” na caixa de diálogo TDR
&#x200B;* [UI] Redefinir interface exibe uma segunda barra de título na janela da prateleira

### 3.3.0 (2017.3.0)

*(Lançado: 28 de setembro de 2017)*

**Adicionado:**

&#x200B;* [Exportar] Permitir a exportação de malha e texturas para o Projeto Adobe Felix
&#x200B;* [Exportar] Permite exportar para o formato de arquivo glTF
&#x200B;* [Engine] Otimizar o tamanho das texturas em VRAM usando a compactação de bloco
&#x200B;* [Visor] Ser capaz de arrastar e soltar uma malha ou projeto no visor
&#x200B;* [UI] Melhorar a mensagem de aviso sobre o TDR
&#x200B;* [UI] O log deve ser exibido somente mediante solicitação
&#x200B;* [UI] Permitir limpar o conteúdo da janela de log
&#x200B;* [UI] Exibir avisos e erros na barra de status
&#x200B;* [IU] Exibir guias na parte superior como em navegadores da Web
&#x200B;* [UI] Melhorar contexto e mensagens “não pintáveis”
&#x200B;* [UI] Adicionar uma ação “salvar como cópia” no menu Arquivo
&#x200B;* [Camada] Definir a configuração padrão de divisão em blocos gráficos como 1 por padrão
&#x200B;* [Prateleira] Filtro de gradiente aprimorado para suporte a 10 cores dinâmicas
&#x200B;* [Prateleira] Adicionar um espaço na consulta padrão da prateleira
&#x200B;* [Prateleira] Adicionar uma ação “Abrir no explorador” para recursos locais na prateleira
&#x200B;* [Prateleira] Adicionar modelo e sombreador para Adobe Material Standard (Projeto Felix)
&#x200B;* [Prateleira] Aumentar a divisão em blocos gráficos máxima para 128 em sombreadores de camada de material
&#x200B;* [Prateleira] Adicionado curvatura sobel para microdetalhes de geradores de máscaras
&#x200B;* [Plug-in] Adicionar plug-in de salvamento automático com intervalo de tempo personalizável
&#x200B;* [Script] Adicionar uma função “salvar como cópia”

**Corrigido:**

&#x200B;* [IU] O layout é quebrado na primeira inicialização
&#x200B;* [Export] O PSD gerado na exportação tem erros de formato
&#x200B;* [Exportar] EXR sempre exporta mapa de heights de 8 bits
&#x200B;* [Export] Falha ao exportar mapas adicionais corrompidos
&#x200B;* [Importar] As bordas sólidas não são preservadas em malhas de poli baixo em alguns casos
&#x200B;* [Importar] Mensagens de erro aprimoradas ao importar malhas com problemas
&#x200B;* [Padeiros] Falha no cozimento do mapa de ID com a opção Corresponder pelo nome ativada
&#x200B;* [Visor] O espaço tangente não é sincronizado com padeiros
&#x200B;* [Efeito] Voltar uma camada não restaura a referência de uma âncora
&#x200B;* [Efeito] Problema de atualização ao criar um link entre duas máscaras com âncoras
&#x200B;* [Efeito] As âncoras de máscaras acima da máscara não devem ser listadas
&#x200B;* [Efeito] Extrair configuração de Alpha de Âncoras não funciona
&#x200B;* [Mecanismo] A máscara se inverte após o primeiro traçado do pincel
&#x200B;* [Engine] Falha ao alternar o Conjunto de texturas em um projeto específico
&#x200B;* [Prateleira] Falha ao excluir uma predefinição que está em um projeto
&#x200B;* [Prateleira] Erro de ortografia no filtro Triplanar avançado
&#x200B;* [Prateleira] MG Mask Builder AO Noise Scale não funciona corretamente
&#x200B;* [Prateleira] MG Mask Builder tem parâmetros de curvatura invertidos
&#x200B;* [Prateleira] Os alfa importados geram uma visualização de esfera de material em vez de uma simples

### 3.2.0 (2017.2.0)

*(Lançado: 27 de julho de 2017)*

**Adicionado:**

&#x200B;* Pontos de ancoragem - Sistema de referência de camada e máscara
&#x200B;* [Camadas] Capacidade de renomear efeitos de preenchimento e pintura
&#x200B;* [Plugin] Plug-in Substance Source atualizado
&#x200B;* [Scripting] Permitir consultar Resolução de Conjunto de Textura
&#x200B;* [Script] Permite obter o status do mecanismo de pintura
&#x200B;* [Desempenho] Otimizações aprimoradas de carregamento e carimbo de pincel no projeto

**Corrigido:**

&#x200B;* [Ferramenta] Problemas de desempenho ao ajustar parâmetros de material
&#x200B;* [Engine] Desaparecimento de pinceladas ao alterar a resolução (4K>2K)
&#x200B;* [Exibição 3D] O espaço tangente não é sincronizado com padeiros
&#x200B;* [Prateleira] O caminho de prateleira nos documentos do usuário não é criado automaticamente
&#x200B;* [Prateleira] Fazer predefinições compatíveis com versões anteriores após uma atualização
&#x200B;* [Shader] O sombreador não PBR não funciona mais
&#x200B;* [Padeiros] Falha no cozimento do mapa de ID com a opção Corresponder pelo nome ativada
&#x200B;* [Amostra] Os nomes dos conjuntos de texturas do projeto de amostra do Mat da reunião estão incorretos
&#x200B;* Salvar um projeto antes de criar um modelo retorna erros de permissão de gravação

### 3.1.0 (2017.1.0)

*(Lançado: 20 de junho de 2017)*

**Adicionado:**

&#x200B;* [Plug-in] Novo plug-in Substance Source (permite baixar ativos na prateleira)
&#x200B;* [Prateleira] 4 Novas Fontes (Japonês + Chinês Simplificado, Máquina De Escrever, Segmento)
&#x200B;* [Prateleira] 230 novos Alpha (mistura de padrões, pincéis e digitalizações de impressão digital)
&#x200B;* [Prateleira] 50 Novos Procedurals (Padrões de tecido de roupas medievais e contemporâneas)
&#x200B;* [Prateleira] 2 Novos mapas ambientais (Mondarrain e Villa Nova Street)
&#x200B;* [Prateleira] 9 Novos filtros (Edge Wear de detalhes MatFx, Suporte, HBAO, etc.)
&#x200B;* [Prateleira] Mapa de ambiente de panorama padrão aprimorado
&#x200B;* [Prateleira] Novas predefinições de exportação para Arnold 5
&#x200B;* [Scripting] Permitir a importação de recursos para a Prateleira

**Problemas Conhecidos:**

&#x200B;* [Exportar] A edição de uma predefinição de exportação é muito lenta

## Versão 2

### 2.6.2

*(Lançado: 20 de outubro de 2017)*

<b>Adicionado:</b>

&#x200B;* [Conjunto de texturas] Permite excluir conjuntos de texturas desativados
&#x200B;* [Prateleira] Permite que vários usuários gravem dentro da mesma pasta de prateleira
&#x200B;* [Script] Poder recarregar a pasta de plug-ins
&#x200B;* [Script] Adicione uma versão mínima necessária da API nos metadados do plug-in para garantir a compatibilidade
&#x200B;* [IRay] Melhorias na caixa de diálogo Exportar imagem

<b>Corrigido:</b>

&#x200B;* [Engine] Problema de desaparecimento de traços, ao alterar a resolução (4K>2K)
&#x200B;* [Padeiros] Falha no cozimento do mapa de ID com a opção Corresponder pelo nome ativada
&#x200B;* [Padeiros] As mensagens de erro não são suficientemente explícitas
&#x200B;* [Exibição 3D] O espaço tangente não é sincronizado com padeiros
&#x200B;* [Ferramenta] Artefatos pretos ao usar a ferramenta de borrar
&#x200B;* [Shader] O sombreador não PBR não funciona mais
&#x200B;* [Shader] “pbr-coated” está quebrado
&#x200B;* [Shader] A aspereza do revestimento do sombreador “revestido com pbr” não tem mais impacto
&#x200B;* [Shader] O sombreador de brilho de especificação não corresponde a Iray e SD
&#x200B;* [Prateleira] Falha ao carregar dois arquivos com o mesmo nome, mas com extensões diferentes
&#x200B;* [Prateleira] Não é mais possível editar a predefinição nas prateleiras
&#x200B;* [Prateleira] Não é possível definir uma visualização personalizada para ativos importados na prateleira
&#x200B;* Os recursos carregados do cache perdem seus usos
&#x200B;* Salvar um projeto antes de criar um modelo retorna erros de permissão de gravação
&#x200B;* Salvar projeto incorreto se o nome do arquivo contiver dois pontos
&#x200B;* Importação de arquivos com vários pontos (.) no nome do arquivo causa problemas

### 2.6.1

*(Lançado: 12 de maio de 2017)*

**Adicionado:**

&#x200B;* [TextureSet] Não permitir a reatribuição de materiais de malha a nada

**Corrigido:**

&#x200B;* Falha ao alternar o TextureSet após substituir o mapa baked
&#x200B;* Falha ao fazer “Desfazer e Refazer” após alterar o modo de mesclagem da camada
&#x200B;* Falha ou congelamento ao usar o efeito “seleção de cores” com um mapa de ID grande
&#x200B;* [Exportar] Os conjuntos de texturas renomeados não são classificados em ordem alfabética na janela de exportação
&#x200B;* [TextureSet] Redefinir para o nome padrão não verifica a unicidade
&#x200B;* [TextureSet] O conjunto de texturas renomeado é desativado após a reabertura do projeto
&#x200B;* [Prateleira] Conteúdo de modelos padrão ausente
&#x200B;* [Prateleira] As texturas não quadradas são exibidas como quadradas
&#x200B;* [Shader] Depois que um conjunto de textura é desativado, o sombreador associado é destruído
&#x200B;* [Scripting] alg.baking.setTextureSetBakingParameters() não funciona mais
&#x200B;* [Script] Erro de digitação no tutorial do websocket
&#x200B;* [Scripting] Vários problemas em AlgWidgets
&#x200B;* [Log] Detecção incorreta de memória virtual disponível em alguns casos

### 2.6.0

*(Lançado: 27 de abril de 2017)*

**Adicionado:**

&#x200B;* Adicionar novo projeto de amostra “Meet Mat”
&#x200B;* [Plug-in] Novo plug-in “Atualizador de recursos”
&#x200B;* [TextureSet] Permite renomear e adicionar uma descrição a conjuntos de textura
&#x200B;* [TextureSet] Permitir a reatribuição de materiais
&#x200B;* [TextureSet] Adiciona um botão de configuração na janela de lista do conjunto de textura
&#x200B;* [TextureSet] Mostra os conjuntos de texturas “desativados” na parte inferior da lista
&#x200B;* [Substance] Use mapas adicionais na resolução atual do conjunto de texturas para melhorar o desempenho
&#x200B;* [Script] Permite atualizar um recurso usado em um projeto (material, gerador etc.)
&#x200B;* [Script] Adicionar uma maneira de adicionar/remover uma prateleira
&#x200B;* [Scripts] Permitir a consulta de informações do recurso em projetos
&#x200B;* [Scripting] Permite recuperar uma lista de prateleiras disponíveis
&#x200B;* [Script] Tutorial de aprimoramento de miniatura do AlgWidget
&#x200B;* [Export] Desativar/ativar profundidade de bits com base no suporte ao formato de arquivo
&#x200B;* [Log] Adicionar nome de plug-in para imprimir no console
&#x200B;* [Log] Remover erro sobre conjuntos de texturas ocultos
&#x200B;* Atualizar “Tela de boas-vindas” com novos ícones e texto para amostras

**Corrigido:**

&#x200B;* Falha ao atualizar uma malha em projetos específicos
&#x200B;* [Visor] A cor interna do plano de Simetria não está mais visível
&#x200B;* [Janela de visualização] Alguns efeitos de pós-processo são ativados ao usar a visualização individual
&#x200B;* [Shaders] A mesclagem “over\_premult” não funciona corretamente
&#x200B;* [Shaders] Aviso sobre o teste alfa com o sombreador padrão
&#x200B;* [Prateleira] Análise incorreta de marcas de Substance
&#x200B;* [Shelf] O Envolvimento de Ferrugem do MatFX não funciona corretamente
&#x200B;* [Prateleira] O filtro HSL está habilitado em canais incorretos por padrão
&#x200B;* [Prateleira] A nitidez está ativada no canal Height/Normal por padrão
&#x200B;* [Exportar] As predefinições de exportação do Vray não usam um mapa normal OpenGL
&#x200B;* [Ferramenta] Problemas de imprecisão com a ferramenta clonar/borrar criam artefatos

### 2.5.3

*(Lançado: 15 de março de 2017)*

**Corrigido:**

&#x200B;* [Baker] Falha ao fazer bake com malhas específicas

**Problemas Conhecidos:**

&#x200B;* [Mac] Partículas podem criar corrupção de textura em alguns casos

### 2.5.2

*(Lançado: 14 De março De 2017)*

**Corrigido:**

&#x200B;* [Ferramenta] Os tablets Wacom não funcionam no Linux
&#x200B;* [Ferramenta] Artefatos pretos ao usar a ferramenta de borrar
&#x200B;* [Padarias] A cozedura falha se a opção Coincidir pelo nome for usada com uma caixa
&#x200B;* [Pães] Oclusão ambiente quebrada ao assar apenas com mapa normal
&#x200B;* [Prateleira] Os filtros genéricos não tratam o alfa corretamente (Contraste/Luminosidade, Highpass etc.)
&#x200B;* [Viewport] Problema de desempenho ao carregar um projeto com sombras ativadas
&#x200B;* [Janela de visualização] Problema de pontilhamento na visualização 3D no MacOS
&#x200B;* [Janela de visualização] As visualizações de partículas são exibidas incorretamente quando o perfil de cores está ativado
&#x200B;* [Iray] Falha ao alternar o projeto de volta para OpenGL se o Iray não inicializar
&#x200B;* [IRay] A reluzência é ignorada ao renderizar o sombreador/mdl SpecGloss
&#x200B;* [Shader] O sombreador de espec/brilho não corresponde a Iray e SD
&#x200B;* [Shader] Conversão de sRGB diferente da conversão linear para sRGB LUT
&#x200B;* [Shader] Renderização incorreta ao carregar projeto com sombreadores desatualizados
&#x200B;* [Shader] O sombreador “pbr-coated” não funciona mais
&#x200B;* [Exportar] Alguns canais ainda são exportados, mesmo que não estejam presentes no conjunto de texturas
&#x200B;* [Camadas] O modo de mesclagem “detalhe inverso do mapa normal” não funciona em canais em tons de cinza
&#x200B;* [UI] Problema na “Janela de seleção de cores” com monitor HDPI e zoom de exibição em 150%

**Problemas Conhecidos:**

&#x200B;* [Mac] As partículas podem criar corrupção de textura em alguns casos

### 2.5.1

*(Lançado: 27 de fevereiro de 2017)*

**Corrigido:**

&#x200B;* [Mac] A entrada da mesa digitalizadora Wacom está interrompida na exibição 3D e 2D
&#x200B;* [Padeiros] A correspondência por nome não funciona mais
&#x200B;* [Bakers] A configuração “Average Normals” não funciona mais
&#x200B;* [Iray] Renderização incorreta com mapa normal cozido ausente
&#x200B;* [Iray] Os perfis de cores se comportam de maneira diferente em comparação ao renderizador OpenGL
&#x200B;* [Iray] Exportar renderização como bitmap não inclui correção de perfil de cores
&#x200B;* [Substance] Os filtros de material não funcionam mais
&#x200B;* [Ferramenta] A opacidade do traçado não é armazenada em predefinições de pincel
&#x200B;* [Ferramenta] O alinhamento UV do pincel do clone não funciona mais
&#x200B;* [Exportar] O canal de Deslocamento deve ser centralizado em 0,5 ao exportar em número inteiro
&#x200B;* [Modelo] O caminho absoluto é armazenado em Modelos
&#x200B;* [TextureSet] A textura do canal persiste após a remoção do canal

**Problemas Conhecidos:**

&#x200B;* [Linux] As entradas dos tablets Wacom não funcionam na exibição 3D e 2D
&#x200B;* [Mac] As partículas podem criar corrupção de textura em alguns casos
&#x200B;* [Exportar] Em casos muito raros, retângulos pretos podem aparecer em GPUs da AMD

### 2.5.0

*(Lançado em: 21 de fevereiro de 2017)*

**Adicionado:**

&#x200B;* Adicionar compatibilidade com as GPUs AMD Radeon Pro e AMD FirePro
&#x200B;* [Ferramenta] Adicionar suporte para opacidade de traçado
&#x200B;* [Ferramenta] Adiciona um modificador que permite continuar a última pincelada
&#x200B;* [Iray] Atualização para oferecer suporte a GPUs Pascal
&#x200B;* [Visor] Adicionar suporte para perfis de cores (LUT)
&#x200B;* [Substance] Integrar nova estrutura (mecanismo SD6)
&#x200B;* [UI] Aumentar a lista de tamanhos de “arquivo recente” no menu Arquivo
&#x200B;* [Importar] Use a categoria de substâncias para preencher o prefixo na caixa de diálogo Importar
&#x200B;* [Padeiros] Permitir assar texturas 8K
&#x200B;* [Padarias] Permitam assar resoluções não quadradas
&#x200B;* [Padarias] Melhorar o consumo de memória ao assar malhas pesadas de alta polarização
&#x200B;* [Prateleira] Bloqueie prateleiras (e projetos) para proibir a edição simultânea e evitar corrupções
&#x200B;* [Prateleira] Ler categoria e palavras-chave de substâncias para usá-las para filtragem
&#x200B;* [Prateleira] Permitir a exclusão de recursos do resultado de uma consulta de pesquisa
&#x200B;* [Prateleira] Cálculo de tempo de miniaturas aprimorado
&#x200B;* [Prateleira] Permite incorporar predefinições em projetos
&#x200B;* [Prateleira] Permite recolher/expandir rapidamente a exibição de árvore com SHIFT
&#x200B;* [Prateleira] Permite salvar miniaturas quando os ativos são somente leitura (cache local)
&#x200B;* [Prateleira] Novo conteúdo : novos filtros (transformo, espelho, tri-planar etc.)
&#x200B;* [Prateleira] Novo conteúdo : novos perfis de LUTs (clássicos e artísticos, como Film Noir, Vintage etc.)
&#x200B;* [Prateleira] Novo conteúdo : 10 novas fontes Substance para gerar rapidamente textos personalizados
&#x200B;* [Prateleira] Novos modelos: Unity 5 e Unreal Engine 4
&#x200B;* [Shelf] Filtro HSL aprimorado para ser mais amigável com artistas
&#x200B;* [Sombreador] Adicionar suporte para canal de specular level em sombreadores PBR
&#x200B;* [Sombreador] Adicionar suporte para pontilhamento no sombreador de teste
&#x200B;* [Sombreador] Adicionar suporte para mapeamento de oclusão de paralaxe em sombreadores PBR
&#x200B;* [Shader] Permite definir interface personalizada para parâmetros de sombreador
&#x200B;* [MatLayering] Criar novo canal Máscara para fluxo de trabalho de camada de material
&#x200B;* [Script] Permitir a gravação de metadados em um projeto SP
&#x200B;* [Script] Permitir exportação com uma predefinição de exportação específica
&#x200B;* [Scripts] Permite recuperar parâmetros de sombreador como um JSON
&#x200B;* [Script] Adicionar suporte para conexões WebSocket
&#x200B;* [Script] Adicione a possibilidade de carregar instâncias de sombreamento
&#x200B;* [Script] Adicione a possibilidade de criar um novo projeto
&#x200B;* [Script] Permite recuperar a url da malha importada em um projeto
&#x200B;* [Script] Permitir fça bake não quadrado
&#x200B;* [Script] Relatar erros ao definir dados por meio da API de script
&#x200B;* [Substance] Adicionar tag de dados do usuário para especificar o formato de mapa normal

**Corrigido:**

&#x200B;* Falha ao selecionar cor com substâncias
&#x200B;* Falha ao carregar uma imagem não RGBA32f como mapa de ambiente
&#x200B;* Falha relacionada à pintura em GPUs AMD
&#x200B;* [Mesh] A importação de OBJ não reconhece materiais sem arquivo mtl
&#x200B;* [Mesh] A geração do nome do conjunto de textura UDIM pode estar incorreta em algumas malhas
&#x200B;* [UI] Botão Desfazer/Refazer na Configuração do visualizador roubar foco e parar a rolagem do mouse
&#x200B;* [UI] Alguns rótulos são cortados incorretamente em Hi-DPI
&#x200B;* [Camada] O modo de substituição do efeito de pintura tem um comportamento incorreto na máscara
&#x200B;* [Camada] O modo de mesclagem Subtrair tem um comportamento incorreto com alfa
&#x200B;* [Ferramenta] O tamanho do pincel se torna enorme na visualização 2D ao pintar nas bordas UV
&#x200B;* [Ferramenta] A linha reta encaixada apresenta um comportamento irregular com Hi-DPI
&#x200B;* [Tool] A resolução do estêncil às vezes está incorreta
&#x200B;* [Bakers] Os valores de “Distância Máxima do Ocultador” são bloqueados se “em relação à caixa delimitadora” for “Desativado”
&#x200B;* [Shader] As definições de canal Pilha e Parâmetro automático não correspondem
&#x200B;* [Visualização 3D] Exibição inconsistente do canal normal dependendo da configuração do projeto
&#x200B;* [Janela de visualização] Alguns mapas normais têm valores fixados que aparecem como artefatos
&#x200B;* [Janela de visualização] O pós-efeito é sempre desativado por padrão
&#x200B;* [Export] A configuração de mixagem normal está incorreta se o canal normal estiver ausente
&#x200B;* [Exportar] Geração de textura incorreta em alguns casos em GPUs AMD
&#x200B;* [Exportar] Os parâmetros de sombreador não são exportados corretamente se localizados dentro de um grupo
&#x200B;* [Exportar] Editar uma predefinição de exportação em uma prateleira personalizada gera um erro de log
&#x200B;* [Prateleira] A filtragem do modo de exibição de árvore não corresponde exatamente ao nome da pasta
&#x200B;* [Prateleira] Renomear uma predefinição de prateleira é difícil de ler
&#x200B;* [Prateleira] O recurso de Sombreador importado na Prateleira não é preservado após a reinicialização
&#x200B;* [Prateleira] Conteúdo : Predefinição de ferramenta de solda ausente
&#x200B;* [Prateleira] Conteúdo : Tile Generator não funciona corretamente
&#x200B;* [Prateleira] Conteúdo: Máscara incorreta corrigida no material inteligente sujo do pneu de borracha
&#x200B;* [Shelf] Conteúdo: corrigido o nome incorreto do grupo no material da bolsa de couro
&#x200B;* [Iray] Metade das malhas está ausente em Iray
&#x200B;* [Linux] Falha ao arrastar um recurso acima do Visualização 3D
&#x200B;* [Mac] As preferências são redefinidas em cada lançamento no Sierra

**Problemas Conhecidos:**

&#x200B;* [Exportar] Em casos muito raros, retângulos pretos podem aparecer em GPUs da AMD
&#x200B;* [Iray] Os perfis de cores podem se comportar de maneiras ímpares às vezes

### 2.4.1

*(Lançado: 28 de outubro de 2016)*

**Corrigido:**

&#x200B;* Falha ao criar um projeto com um modelo
&#x200B;* Falha ao fechar a caixa de diálogo de exportação durante uma exportação
&#x200B;* [Mac] Erros ao salvar o projeto (falha ao salvar a predefinição de exportação)
&#x200B;* [Prateleira] Criar uma nova predefinição a exibirá duas vezes
&#x200B;* [Prateleira] As predefinições não podem ser carregadas no modo somente leitura sem direitos administrativos

### 2.4.0

*(Lançado: 27 de outubro de 2016)*

**Adicionado:**

&#x200B;* [Prateleira] Nova interface para procurar recursos (exibição de árvore, filtros e assim por diante)
&#x200B;* [Prateleira] Permite salvar uma pesquisa como predefinição
&#x200B;* [Prateleira] Permite criar uma nova janela a partir de uma predefinição
&#x200B;* [Prateleira] Nova interface para importar recursos
&#x200B;* [Prateleira] Não copiar a prateleira alegorítmica padrão na pasta Documentos
&#x200B;* [Prateleira] Novas predefinições de partículas: Circuito elétrico, Linhas elétricas, Rococó, Veias pequenas
&#x200B;* [Prateleira] Predefinições de partículas mais antigas aprimoradas para serem mais fáceis de usar (como “Chuva”)
&#x200B;* [Prateleira] Adicionar novas informações no menu contextual de recursos
&#x200B;* [Visor] Melhorar o desempenho ao carregar mapas de ambiente
&#x200B;* [Visor] Adicionar suporte a mapas de ambiente que não são potência de dois

**Corrigido:**

&#x200B;* Falha ao remover uma máscara
&#x200B;* Falha ao pintar após salvar uma predefinição
&#x200B;* Falha com desfoque de ambiente em algumas GPUs
&#x200B;* Falha ao atribuir um recurso errado com a miniprateleira
&#x200B;* [Prateleira] Limpar e salvar remove as marcas e metadados dos recursos no projeto
&#x200B;* [Prateleira] importar uma predefinição exibirá seus recursos na prateleira
&#x200B;* [Exportar] O mapa normal gerado a partir do canal de height tem uma intensidade baixa
&#x200B;* [Exportar] O normal da malha nem sempre está presente no mapa normal final
&#x200B;* [Exportar] Às vezes, a dilatação com transparência pode resultar sem transparência
&#x200B;* [Scripting] “alg.plugin\_root\_diretory” pode retornar um caminho de rede truncado
&#x200B;* [TextureSet] O botão Bloquear é ativado ao reabrir projetos não quadrados

### 2.3.1

*(Lançado em: 07 de outubro de 2016)*

**Adicionado:**

&#x200B;* [Plug-in]&#x200B;[Photoshop] Permite especificar qual material/pilha/canais exportar
&#x200B;* [Scripting] Os nomes de função têm algumas inconsistências

**Corrigido:**

&#x200B;* [Exportar] o Alpha pode ser descartado nas predefinições de exportação personalizadas
&#x200B;* [Exportar] o Alpha obtém conversão gama incorreta em canais sRGB
&#x200B;* [Exportar] Documentos não quadrados são exportados como quadrados
&#x200B;* [Exportar] Não é possível exportar mapas adicionais se algum estiver ausente
&#x200B;* [Iray] Alguns parâmetros (como Intensidade de emissivo) não têm efeito
&#x200B;* [NVIDIA] Falha na inicialização com a NVIDIA Quadro K2200/GTX 750/760
&#x200B;* [AMD] Conjunto incorreto de cores para miniaturas e visualizações
&#x200B;* [AMD] Congela e falha de driver em Novo arquivo e Abrir arquivo
&#x200B;* [Log] “software-version” está ausente no arquivo de log

### 2.3.0

*(Lançado: 15 de setembro de 2016)*

**Adicionado:**

&#x200B;* [Plug-in] Novo plug-in “Exportar para o Photoshop” (exportar pilha de camadas completa)
&#x200B;* [Exportar] Permite especificar a largura do preenchimento (em pixels ou infinito)
&#x200B;* [Exportar] Permite definir o tipo de fundo fora dos UVs
&#x200B;* [Prateleira] Novo sombreador de camada de material para misturar 10 materiais
&#x200B;* [Prateleira] Novo sombreador de argila para ver detalhes com o canal height/normal
&#x200B;* [Prateleira] Novo filtro de iluminação cozido com entrada de ambiente
&#x200B;* [Prateleira] Alguns geradores de máscara atualizados para adicionar transformações não quadradas
&#x200B;* [Janela de visualização] Adiciona o mapa normal composto (normal+height+bake) ao modo solo
&#x200B;* [Script] Permitir a exportação de mapas adicionais
&#x200B;* [Scripts] Permitir consultar mapas adicionais disponíveis por conjunto de texturas
&#x200B;* [Script] Permitir recuperação de formato de canal
&#x200B;* [Roteiro] Adicione exemplos na documentação de cozimento
&#x200B;* [Script] Permitir consulta da visibilidade de uma camada
&#x200B;* [Script] Permitir consulta do modo de mesclagem e da opacidade da camada
&#x200B;* [Scripting] Permitir exportar mapas convertidos (mapas normais finais, AO misto, etc.)
&#x200B;* [Substance] Ler e conectar usos personalizados
&#x200B;* [Atalhos] Adicionar tecla modificadora (SHIFT) para percorrer o modo solo para trás
&#x200B;* [Exportar] Predefinição de exportação padrão atualizada para desativar alfa
&#x200B;* [IU] Agora, as miniaturas são calculadas somente se o mecanismo estiver disponível
&#x200B;* [IU] Exibir uma menção quando as miniaturas estiverem em processamento

**Corrigido:**

&#x200B;* Falha com alguns projetos antigos ao abri-los
&#x200B;* Falha com cache de canais de textura corrompido
&#x200B;* Falha ao mesclar mais de 4 materiais com o fluxo de trabalho de Camada de material
&#x200B;* [IU] Os atalhos de ferramenta não funcionam se a barra de ferramentas estiver oculta
&#x200B;* [UI] A barra de ferramentas do Iray está marcada como “Sem título” no menu Exibir
&#x200B;* [UI] As barras de ferramentas do plug-in são chamadas de “Não inclinadas” no menu Exibir
&#x200B;* [Baker] Pressionar Enter durante a edição de uma configuração de cozimento inicia o processo de cozimento
&#x200B;* [Baker] Intervalos incorretos para alguns parâmetros
&#x200B;* [Importar] Não é possível importar malhas OBJ devido a números muito grandes
&#x200B;* [Importar] Alguns arquivos OBJ são importados com muitos subobjetos
&#x200B;* [Exportar] o fundo do canal é preenchido com preto em vez da cor padrão na exportação
&#x200B;* [Ferramenta] As partículas não funcionam corretamente se o CDV for muito baixo
&#x200B;* [Ferramenta] A cor de visualização do pincel está incorreta com máscaras em subpilhas
&#x200B;* [Visor] Quando o pincel vai para áreas vazias na exibição 2D, ele se torna gigantesco
&#x200B;* [Visor] Visualização de pincel em branco ao pintar texturas normais
&#x200B;* [Scripting] Documentação incorreta : “ao” listado em vez de “ambientocclusion”
&#x200B;* [Scripting] O processo iniciado com subprocess() é finalizado ao fechar o Painter
&#x200B;* [Prateleira] Filtro de iluminação Feito bake usa entrada de AO incorreta
&#x200B;* [MacOS] Projeto de hidrante contra incêndio removido (incompatível)
&#x200B;* O projeto padrão é aberto ao carregar um arquivo \*.spt (em vez de \*.spp)

**Problemas Conhecidos:**

&#x200B;* [Plug-in] Por causa do Photoshop, o height e o canal normal não podem ser convertidos como estão

### 2.2.0

*(Lançado: 22 de julho de 2016)*

**Adicionado:**

&#x200B;* [Prateleira] Melhorar o sistema de pesquisa e as consultas
&#x200B;* [Prateleira] Adicionar campo de pesquisa para miniprateleiras
&#x200B;* [Shader] Permite definir a precisão da etapa para controles deslizantes
&#x200B;* [Shader] Adiciona um botão Desfazer/Refazer para parâmetros de sombreador
&#x200B;* [Shader] Recarregar um sombreador não deve redefinir seus parâmetros
&#x200B;* [MatLayering] Adicionar suporte para Camadas de material dinâmico e subpilhas
&#x200B;* [MatLayering] Permite importar arquivo json para definir as configurações do sombreador
&#x200B;* [MatLayering] Limite de desbloqueio de classificadores de textura (alternar para texturas sem associação)
&#x200B;* [Script] Permitir a definição de configurações de padeiros e iniciar seu cálculo
&#x200B;* [Substance] Usar “uso” para conexões de entradas/saídas, além de identificadores
&#x200B;* [Ferramenta] Permite selecionar o canal de visualização no visor para a Ferramenta de projeção

**Corrigido:**

&#x200B;* Falha durante a inicialização se as substâncias estiverem localizadas na pasta errada
&#x200B;* O relatório de falhas às vezes não funciona devido a um arquivo de log incorreto
&#x200B;* [Iray] Os pós-efeitos não são atualizados quando o Iray está pausado
&#x200B;* [Iray] O atalho de foco automático não funciona mais
&#x200B;* [Iray] O comportamento do controle deslizante de abertura muda dependendo do tamanho do ativo
&#x200B;* [Camadas] O primeiro canal de material não é ativado por padrão se estiver desativado
&#x200B;* [Shader] Nenhum erro será impresso se um “param auto” estiver incorreto

**Problemas Conhecidos:**

&#x200B;* [Mac] O limite de amostras de textura está bloqueado em 16 (problema do driver de GPU)

### 2.1.1

*(Lançado em: 01 de julho de 2016)*

**Adicionado:**

&#x200B;* [License] Não será possível alterar o local do arquivo de licença
&#x200B;* [Janela de visualização] Adicionar um atalho “B” para alternar entre mapas adicionais
&#x200B;* [Importar] Permita importar o FBX 2016/2017 corretamente
&#x200B;* [Ferramenta] Remover verificadores ao usar a máscara rápida
&#x200B;* [Iray] Adicionar informações de dimensões de cena
&#x200B;* [Iray] Permita aumentar o número máximo de amostras e o tempo de renderização
&#x200B;* [UI] Atualizar o resultado imediatamente ao usar o botão +/- nos controles deslizantes
&#x200B;* [UI] Permitir maior precisão para controles deslizantes de Tons de Cinza
&#x200B;* [Exportar] Não exporte um canal alfa para texturas que são apenas RGB
&#x200B;* [Exportar] Atualizar predefinição de exportação do Dota 2
&#x200B;* [Prateleira] Novo padrão “Ladrilhos de hexágono”
&#x200B;* [Prateleira] Nova ferramenta “Solda”
&#x200B;* [Prateleira] Filtros de acabamento atualizados para fornecer controles de direção

**Corrigido:**

&#x200B;* [Exportar] Impossível exportar arquivos de PSD em 8 bits
&#x200B;* [Exportar] A exportação em 8K não está disponível em algumas configurações de hardware
&#x200B;* [Export] A janela do Sketchfab foi cortada
&#x200B;* [Exportar] Mapa de aspereza incorreto na predefinição de exportação de Espec/Gloss
&#x200B;* [IU] A digitação em controles deslizantes de tons de cinza não funciona mais
&#x200B;* [IU] Impossibilidade de colocar filtros nas entradas de substância (como Geradores)
&#x200B;* [IU] Alguns controles deslizantes têm comportamentos estranhos
&#x200B;* [UI] A etapa DeltaTime +/- para partículas é muito grande
&#x200B;* [Iray] Alguns projetos bloqueiam o aplicativo ao mudar para o Iray
&#x200B;* [Iray] Falha ao detectar hardware
&#x200B;* [Ferramenta] A cor de visualização de pincel está incorreta no modo Máscara
&#x200B;* [Ferramenta] O seletor de material pode ser usado com ferramentas incompatíveis
&#x200B;* [Ferramenta] A visualização da projeção não alterna para Difusa com o fluxo de trabalho Especificação/Brilho
&#x200B;* [Prateleira] Alterar sombreador padrão quebra as visualizações de tapetes inteligentes/máscaras inteligentes
&#x200B;* [Prateleira] Alguns materiais inteligentes têm nomes incorretos
&#x200B;* [Prateleira] Formas alfa adicionais estão corrompidas e não serão carregadas
&#x200B;* [Viewport] Alternar para o modo “Mapa adicional” exibe “outro” primeiro
&#x200B;* [Viewport] A opção Viewport volta para “other” quando não existe um mapa adicional
&#x200B;* [Crash]&#x200B;[Linux] O relatório de falha não funciona no Ubuntu (Steam)
&#x200B;* [Crash]&#x200B;[Linux] Os links de URL da Web não funcionam no Ubuntu (Steam)
&#x200B;* [Crash]&#x200B;[Windows] Remover o “crashwatcher” quando o Substance painter não estiver mais em execução
&#x200B;* [Falha]&#x200B;[Mac] O sistema de relatório de falhas não funciona corretamente
&#x200B;* [Falha] A importação de uma malha durante a importação de uma malha leva a uma falha
&#x200B;* O atalho de separação do conjunto de textura não é redefinido para nada após uma reinicialização

### 2.1.0

*(Lançado em: 2 de junho de 2016)*

**Adicionado:**

&#x200B;* [UDIM] Importar ladrilhos UDIM de uma malha como conjuntos de texturas
&#x200B;* [Linux] Suporte adicionado para CentOS 6.6 e Ubuntu 12.4
&#x200B;* [Exportar] Adicionar resolução 8K (experimental)
&#x200B;* [Exportar] Permite escolher a profundidade de bits durante a exportação
&#x200B;* [Baker] Permitir assar vários conjuntos de textura de uma só vez
&#x200B;* Suporte a monitores de alta resolução (dimensionamento de DPI alto)
&#x200B;* [Script] Definir resolução personalizada e preenchimento por textura na exportação
&#x200B;* [Visor] Permite alternar entre o conjunto de textura clicando na malha (via Ctrl+Alt+Clique)
&#x200B;* [Visor] Ir para onde está o cursor do mouse ao aplicar zoom com a roda do mouse
&#x200B;* [UI] Atualizar a cor de fundo padrão e a exibição do mapa de ambiente
&#x200B;* [UI] Adicionar dicas de ferramentas com nomes originais para canais do usuário
&#x200B;* [UI] Alterar a cor do plano de fundo de canais que não podem ser renomeados
&#x200B;* [Ferramenta] Remover verificadores ao usar a máscara rápida
&#x200B;* [Sombreador] Permite definir grupos para parâmetros de sombreador e materiais/máscaras
&#x200B;* [Engine] Otimização de carimbo de tamanho pequeno
&#x200B;* [Estêncil] Adicionar “W” como atalho para alternar temporariamente a máscara
&#x200B;* [Prateleira] Adicionar um botão de cruz para limpar o campo de pesquisa
&#x200B;* [Prateleira] Carregue o Alpha com um único clique
&#x200B;* [Prateleira] Nova predefinição de exportação: Vray UDIM, Arnold UDIM, Spec/Gloss from Metal/Rough
&#x200B;* [Prateleira] Alfas novas : formas geométricas, veias e sinais
&#x200B;* Adicionar nome e versão nas propriedades do executável Substance Painter

**Corrigido:**

&#x200B;* [Substance] Impossível usar o canal normal e o mapa adicional ao mesmo tempo
&#x200B;* [Iray] A refração MDL e a configuração de absorção não funcionam
&#x200B;* [Iray] A escala da cena original não é preservada
&#x200B;* [Prateleira] O modelo de Specular/Textura reluzente usa um sombreador incorreto
&#x200B;* [Exportar] A predefinição de exportação padrão não exporta alguns mapas (como AO)
&#x200B;* [Janela de visualização] O ponto dinâmico não é atualizado ao clicar fora dos UVs na visualização 2D
&#x200B;* [UI] Os valores do controle deslizante são arredondados
&#x200B;* [UI] Às vezes, ao editar os valores dos controles deslizantes, há um espaço livre muito pequeno
&#x200B;* [Novo projeto] A lista suspensa do modelo não foi atualizada corretamente (de 1.x para 2.x)
&#x200B;* [Script] Comportamento “hover” corrigido nos botões personalizados
&#x200B;* [Mac] Desfazer em um projeto vazio bloqueia a câmera

**Problemas Conhecidos:**

&#x200B;* O relatório de falha não está disponível no Ubuntu
&#x200B;* Alguns botões de URL podem não funcionar. Consulte nossas Perguntas frequentes para obter uma solução alternativa

### 2.0.5

*(Lançado: 29 de abril de 2016)*

**Adicionado:**

&#x200B;* [Prateleira] Modelo não pbr adicionado/atualizado, sombreador e predefinição de exportação
&#x200B;* [Shelf] Predefinição de exportação UE4 atualizada para incluir Oclusão ambiente

**Corrigido:**

&#x200B;* Falha ao abrir e salvar alguns projetos com recursos corrompidos
&#x200B;* [Visor] O Wireframe aparece quebrado na exibição 2D
&#x200B;* [Prateleira] Desempenho aprimorado de alguns mapas de ambiente de estúdio
&#x200B;* [Prateleira] Alguns mapas de ambiente de estúdio estão duplicados
&#x200B;* [Shelf] “Baked Lighting Material” (Material de iluminação assado) ausente
&#x200B;* [Shelf] Gerador “conversão em tons de cinza” ausente

### 2.0.4

*(Lançado: 26 de abril de 2016)*

**Adicionado:**

&#x200B;* Melhorar colisões de malha e otimizar a renderização de wireframe
&#x200B;* Melhore o desempenho e o gerenciamento de memória com grandes projetos
&#x200B;* Melhorar a precisão e a revisão do controle deslizante
&#x200B;* [UI] Atualizar o mecanismo somente ao validar um controle deslizante (não ao inserir um valor)
&#x200B;* [IU] Mova a opção Iray para um botão dedicado na barra de ferramentas principal (e altere seu atalho)
&#x200B;* [Ferramenta] Adicionar configuração para o comportamento de local de origem da ferramenta Clonar
&#x200B;* [Shader] Permite ler cores de vértice de malha em sombreadores personalizados
&#x200B;* [Scripts] Permite recuperar a lista de conjuntos de texturas, canais e camadas
&#x200B;* [Script] Adicionar funções do auxiliar (URL para caminho, obter caminho de exportação do projeto)
&#x200B;* [Mac] Detectar a versão “El Capitan” do Mac Os no arquivo de registro

**Corrigido:**

&#x200B;* Falha após a segunda exportação para o Substance share
&#x200B;* Falha ao copiar uma camada entre conjuntos de texturas com dados de Máscara rápida.
&#x200B;* Alguns projetos têm um atualizador muito longo que consome muita memória
&#x200B;* [Ferramenta] Falha ao selecionar uma predefinição de partícula com a ferramenta clone/borrar
&#x200B;* [Baker] Carregar arquivos FBX leva muito tempo para malhas pesadas
&#x200B;* [Visor] Mapa de ambiente ampliado em alguns computadores
&#x200B;* [Visor] Conversão de gama incorreta do alfa do pincel
&#x200B;* [Exportar] o Alpha é armazenado como transparência em vez de um canal separado com arquivos Tiff.
&#x200B;* [Exportar] O canal normal é sempre exportado como OpenGL
&#x200B;* [Iray] Nomes de controles deslizantes ausentes para configurações de Iray
&#x200B;* [Iray] A renderização é feita em uma resolução incorreta em Retina/High DPI
&#x200B;* [Iray] Falha ao redimensionar a interface no modo Iray
&#x200B;* [Iray] Enorme redução de desempenho ao renderizar em algumas resoluções baixas
&#x200B;* [Iray] A pausa não funciona (Iray ainda calcula em segundo plano)
&#x200B;* O canal normal às vezes tem artefatos de quadrado preto
&#x200B;* O canal normal é invertido pelos filtros de tons de cinza
&#x200B;* O canal normal não é mesclado corretamente se a pilha tiver algum alfa
&#x200B;* O projeto é editado no disco ao abrir um projeto, mesmo que ele ainda não tenha sido salvo
&#x200B;* A reimportação de uma malha em alguns projetos fornece desempenhos de GPU muito ruins
&#x200B;* A orientação do pincel está incorreta quando não está tocando em uma malha
&#x200B;* O logotipo do substance share está ausente na tela de boas-vindas

### 2.0.2

*(Lançado: 25 de março de 2016)*

**Adicionado:**

&#x200B;* [Iray] Atualize o modelo e o sombreador de Spec/Gloss para serem compatíveis com o Iray
&#x200B;* [Exportar] Conseguir exportar capturas de tela para o ArtStation
&#x200B;* [Scripting] Suporte à execução a partir do diretório de plug-ins
&#x200B;* [Script] Permitir “Salvar como”
&#x200B;* [IU] Permitir que você clique duas vezes em um controle deslizante para editar seu valor
&#x200B;* Mover amostra do Vela para o Substance share
&#x200B;* Novo projeto de amostra: Visualização da esfera
&#x200B;* Avisar os usuários sobre conflito de extensão do shell

**Corrigido:**

&#x200B;* Instalação de substituição do instalador do Substance Painter 1.x
&#x200B;* [IU] O layout da lista de canais está quebrado com filtros
&#x200B;* [IU] Os parâmetros de Sombreador não são exibidos
&#x200B;* [IU] Redimensionar a janela da camada corta incorretamente o conteúdo
&#x200B;* [Ferramenta] O canal de opacidade nem sempre é usado corretamente
&#x200B;* [Ferramenta] Borrar/Clonar não funciona com Simetria
&#x200B;* [Ferramenta] A opacidade da visualização do pincel está incorreta em alguns canais
&#x200B;* [Iray] Falha ao usar o Iray enquanto ele ainda não foi criado
&#x200B;* [Iray] Não é possível carregar dados de configurações de iray do projeto
&#x200B;* [Iray] O Iray não cuida da modificação de configurações após uma pausa
&#x200B;* [Prateleira] Importar um material para a prateleira não funciona
&#x200B;* O estêncil não funciona com o canal Normal
&#x200B;* Falha ao pintar em alguns projetos
&#x200B;* Falha ao pintar com partículas em alguns projetos
&#x200B;* Falha com o Processador de pixels durante alguns cálculos

### 2.0.0

*(Lançado: 16 de março de 2016)*

**Adicionado:**

&#x200B;* Atalho para armazenamento em Substance na barra de ferramentas principal
&#x200B;* Renderizador Iray com modo de visualização e exportação de captura de tela
&#x200B;* Suporte à criação e ao uso do “Máscara inteligente”
&#x200B;* Suporte para o fluxo de trabalho PBR de Specular/Glossários (com o novo canal difuso)
&#x200B;* Substance de encadeamento (conecta substâncias nas entradas de imagem do substance)
&#x200B;* Suporte a scripts com plug-ins personalizados
&#x200B;* Melhorar a conversão de Height em Normal usando um filtro Sobel
&#x200B;* Alternar resolução de visualização de estêncil/projeção para 2K
&#x200B;* Adicionar canal normal por padrão para novos projetos
&#x200B;* Ler a tag de dados do usuário no nó de saída para ativar/desativar os canais de uma substância por padrão
&#x200B;* Expor mesclagem normal/AO nas configurações do TextureSet
&#x200B;* [Ferramenta] Nova ferramenta Borrar para mesclar e espalhar cores
&#x200B;* [Ferramenta] Nova ferramenta Clonar para copiar parte do textura
&#x200B;* [Ferramenta] Permite selecionar canais para as ferramentas Borrar, Clonar e Borracha
&#x200B;* [Camada] Adicionar nome de Substance para o nome do efeito de preenchimento
&#x200B;* [Camada] Permitir exportação de máscara para a área de transferência
&#x200B;* [Visor] Alternar entre o modo de Perspectiva e o modo ortográfica
&#x200B;* [Janela de visualização] Permite controlar o campo de visualização no modo de Perspectiva
&#x200B;* [Janela de visualização] Permitir a definição da distância da Profundidade do campo com CTRL+Clique no botão do meio
&#x200B;* [Visor] Permite arrastar e soltar mapas de ambiente no Visualização 3D.
&#x200B;* [Visor] Feedback aprimorado quando o mecanismo está realizando cálculos fortes
&#x200B;* [Exportar] Permite exportar parâmetros de sombreador em um arquivo json
&#x200B;* [UI] Atualizar interface com novos ícones, cores e layout
&#x200B;* [IU] Adicionar nomes de ativos às miniprateleiras
&#x200B;* [UI] Recolher “Mapeamento de canais” por padrão
&#x200B;* [Sombreador] Escolha uma cor personalizada para os parâmetros de textura de sombreador
&#x200B;* [Prateleira] Perguntar onde importar arquivos ao arrastar e soltar recursos
&#x200B;* [Prateleira] Nova esfera de visualização para Materiais inteligentes e geradores
&#x200B;* [Prateleira] Adicionar sombreador de textura reluzente de Specular
&#x200B;* [Prateleira] Novas formas de Superfície Dura
&#x200B;* [Prateleira] Novas Alpha textura e formas
&#x200B;* [Prateleira] Novas texturas de pele
&#x200B;* [Prateleira] Novos materiais baseados em digitalização e materiais inteligentes
&#x200B;* [Prateleira] Novos materiais inteligentes e suporte a especificações/brilhos dos antigos
&#x200B;* [Prateleira] Novos filtros de acabamento para simulação de superfície metálica
&#x200B;* [Prateleira] Novo gerador de máscara poderoso “Editor de máscaras”
&#x200B;* [Prateleira] Materiais antigos retrabalhados e limpos
&#x200B;* Novo projeto de amostra “Vela”

**Corrigido:**

&#x200B;* [Configurações] A rotação e a velocidade de zoom da câmera são substituídas pelo projeto
&#x200B;* [Visor] Problema de precisão na textura normal padrão leva a reflexos incorretos
&#x200B;* [Visor] A vinheta fica ativada por padrão
&#x200B;* [Visor] Os artefatos aparecem nas bordas do mapa ambiental (GPUs Nvidia)
&#x200B;* [Visor] A miniatura no modo de projeção/estêncil é muito longa para carregar
&#x200B;* [Baker] Armazenar texturas feitas bake em inteiros de 16 bits em vez de 32 bits
&#x200B;* [Camada] Substâncias desatualizadas são exibidas incorretamente na pilha
&#x200B;* A cor padrão e a profundidade de bits de alguns canais estão incorretas (por exemplo: Specular, Textura reluzente)
&#x200B;* Corrigido o comportamento de borracha para desativar a mesclagem no modo de passagem

**Problemas Conhecidos:**

&#x200B;* A simetria não funciona com as ferramentas Borrar e Clonar
&#x200B;* A exportação do ArtStation está ausente

## Versão 1

### 1.7.3

*(Lançado em: 01 de março de 2016)*

**Adicionado:**

&#x200B;* [Exportar] Adicione uma opção para desativar o preenchimento
&#x200B;* [Prateleira] Suporte a hierarquia de subprateleira dentro de uma pasta de prateleira

**Corrigido:**

&#x200B;* Falha ao salvar sobre arquivo somente leitura anterior
&#x200B;* Falha ao abrir um segundo projeto
&#x200B;* Falha ao carregar algumas miniaturas (prateleira, camadas ou dicas de ferramentas)
&#x200B;* A desativação da opção “Preservar posições de traçados na malha” não funciona
&#x200B;* [Exportar] A ampliação de bitmaps é feita com a filtragem mais próxima
&#x200B;* [Prateleira] A descoberta de recursos é muito lenta
&#x200B;* [Prateleira] Os filtros de desfoque não são compatíveis com 16 bits
&#x200B;* [Ferramenta] A Simetria não funciona se você carregar uma predefinição de ferramenta antiga
&#x200B;* A caixa de diálogo de cor do canal de Specular não faz uma conversão do espaço de cor

### 1.7.2

*(Lançado: 13 de janeiro de 2016)*

**Adicionado:**

&#x200B;* [Camadas] Permite especificar a divisão em blocos gráficos padrão para camadas de preenchimento

**Corrigido:**

&#x200B;* [Exportar] A exportação do Sketchfab não funciona mais
&#x200B;* [Camada] A filtragem bilinear é aplicada mesmo no Preenchimento sem nenhuma transformação
&#x200B;* [Ferramenta] Desempenho insatisfatório ao usar o substance com entradas de imagem no modo de projeção
&#x200B;* [Ferramenta] O seletor de material está danificado

### 1.7.1

*(Lançado: 18 de dezembro de 2015)*

**Corrigido:**

&#x200B;* Falha ao alternar o conjunto de textura
&#x200B;* Desempenho lento ao pintar

### 1.7.0

*(Lançado: 17 de dezembro de 2015)*

**Adicionado:**

&#x200B;* [Desempenho] Calcular o conteúdo das camadas e suas miniaturas ao mesmo tempo
&#x200B;* [Exportar] Salvar o caminho de exportação como relativo ao lado do projeto
&#x200B;* [Camadas] Adicionado novo modo de mesclagem: subtrair e adicionar/sub
&#x200B;* [Camadas] Nova filtragem de matriz bilinear para camadas de preenchimento
&#x200B;* [Sombreador] Defina um sombreador padrão para a geração de miniaturas nas preferências.
&#x200B;* [Sombreador] Permite especificar um sombreador por conjunto de texturas
&#x200B;* [Sombreador] Permitir a amostragem de texturas da prateleira
&#x200B;* [Ferramenta] Novo comportamento de pincel “em contorno” para pintura
&#x200B;* [Ferramenta] Filtragem aprimorada e suavização reduzida ao pintar
&#x200B;* [Ferramenta] Qualidade de pintura de subpixels aprimorada
&#x200B;* [Ferramenta] A exibição “básica” das configurações de pincel foi removida e o ícone Abrir/Fechar quadro foi aprimorado
&#x200B;* [Menu] Adicionar ícones de efeito no menu do botão direito do mouse
&#x200B;* Criação de modelo a partir de projetos
&#x200B;* [Prateleira] Novos modelos: PBR, Dota 2
&#x200B;* [Prateleira] Nova predefinição de exportação: Dota 2
&#x200B;* [Prateleira] Novos sombreadores: Dota 2, tinta de carro PBR, PBR Coated, PBR Velvet
&#x200B;* [Prateleira] Novo material : ferrugem de aço e desgaste, iluminação estilizada
&#x200B;* [Prateleira] Novos filtros : Desfocar iluminação direcional, estilizada
&#x200B;* [Prateleira] Novo pincel : padrão suave e padrão rígido com um novo alfa para um melhor controle de dureza
&#x200B;* [Prateleira] Novos geradores: Distância 3D e luz
&#x200B;* [Prateleira] Pincéis atualizados com projeção de quebra e remoção de face de fundo (ativada por padrão)
&#x200B;* [Shelf] Ruído branco atualizado com versão de processador de pixel para computação mais rápida

**Corrigido:**

&#x200B;* [Tela de boas-vindas] link Tutorials enviar para vídeos antigos
&#x200B;* [Canais] Dizer “não” para preencher a criação de camada com o AO ainda cria a camada
&#x200B;* [Canais] Os nomes de canais UserX não se propagam na interface
&#x200B;* [Janela de visualização] A entrada da máscara está vazia na lista de canais individuais
&#x200B;* [Compartilhar] Exportar um alfa para Compartilhar do SP cria um arquivo .image ilegível
&#x200B;* [Licença] Corrigir ativação para nomes de usuário com caracteres não ASCII
&#x200B;* [Shader] A caixa de diálogo Parâmetro de cor desaparece ao escolher uma cor
&#x200B;* [Prateleira] As miniaturas não são descarregadas da memória quando não usadas
&#x200B;* [Prateleira] Filtro de gradiente fixo
&#x200B;* [Ferramenta] A simetria não funciona com estêncil/projeção
&#x200B;* [Ferramenta] Nome incorreto ao criar uma nova predefinição de pincel
&#x200B;* A configuração Preservar traçado permanece desativada mesmo ao reimportar uma malha
&#x200B;* Reinicialização do driver (TDR) ao calcular partículas com tamanho grande.

### 1.6.1

*(Lançado: 09 de novembro de 2015)*

**Corrigido:**

&#x200B;* Falha ao abrir projeto se a exibição 2D estiver visível
&#x200B;* Falha ao criar nova predefinição de exportação se a prateleira atual não existir
&#x200B;* [Ferramenta] O ícone do seletor de material pode permanecer exibido
&#x200B;* [Ferramenta] O seletor de materiais oculta o cursor do mouse ao pintar ao mesmo tempo
&#x200B;* [Prateleira] Os metadados são gravados no disco após cada saída

### 1.6.0

*(Lançado: 29 de outubro de 2015)*

**Adicionado:**

&#x200B;* Suporte oficial para Windows 10
&#x200B;* [Substance] Recolher grupos de parâmetros de substância por padrão
&#x200B;* [Substance] Adicionar nova estrutura (melhorar o desempenho do Processador de pixels)
&#x200B;* [Visor] Permite desativar a exibição do plano de simetria enquanto estiver no modo de simetria.
&#x200B;* [Visor] Aprimorar o desempenho e a renderização de sombras
&#x200B;* [Visor] Pausar o cálculo de sombra ao pintar
&#x200B;* [Visor] Aprimorar os desempenhos da renderização do wireframe
&#x200B;* [Engine] Melhorar o gerenciamento de memória Vram para reduzir seu espaço
&#x200B;* [Engine] Aprimorar a atualização de textura nas GPUs AMD para obter melhores desempenhos
&#x200B;* [Engine] Desativar a configuração de otimização por threads nas GPUs NVIDIA para um melhor desempenho
&#x200B;* [Efeito] Adicionar uma tag para solicitar entrada de imagem “preenchida”
&#x200B;* [Camada] Aumenta a precisão do Deslocamento UV/escala no preenchimento
&#x200B;* [Camada] Tornar o controle deslizante de escala exponencial no preenchimento
&#x200B;* [Camada] Permita arrastar e soltar materiais diretamente na pilha de camadas.
&#x200B;* [Camada] Permite arrastar e soltar filtros diretamente na pilha de camadas
&#x200B;* [Camada] Ajuste a cor do pincel da máscara para a cor de máscara recém-criada
&#x200B;* [Sombreador] Expor várias texcoords
&#x200B;* [Sombreador] Exponha a função de mapeamento de gama/tons para permitir funções personalizadas
&#x200B;* [Baker] Alterar configurações padrão de baker de posição para uso do TriPlanar
&#x200B;* [Ferramenta] Renomear “Decalque de geometria” como “Preenchimento de polígono”
&#x200B;* [Prateleira] Geradores de atualização para apoiar TriPlanar: MG Metal edge wear, MG Mask builder, MG Fiber glass, MG Dirt
&#x200B;* [Prateleira] Atualizar materiais com novas configurações e materiais não utilizados removidos
&#x200B;* [Prateleira] 22 novos materiais inteligentes (plástico, ferro, tecido, aço e mais)
&#x200B;* [Prateleira] Atualize os filtros de Nitidez, Desfoque e Distorção com entrada de imagem preenchida para evitar emendas
&#x200B;* [Prateleira] Melhorar as configurações de Distorção para facilitar o uso
&#x200B;* [Shelf] 2 Novos ruídos processuais: ruído 3D Perlin e ruído 3D Worley

**Corrigido:**

&#x200B;* [Engine] A detecção de quantidade de Vram para GPU dedicada está incorreta no Mac
&#x200B;* [Engine] As Texturas mudam para uma versão mais escura no visor
&#x200B;* [Engine] Mau desempenho ao pintar abaixo de várias camadas
&#x200B;* [Engine] As camadas computadas ao abrir o projeto são diferentes da versão em cache
&#x200B;* [Substance] Resultados incorretos em 4K no Mac
&#x200B;* [Substance] Os parâmetros estão na ordem errada
&#x200B;* [Sombreador] Sombreadores de tons e pixels são totalmente pretos
&#x200B;* [Sombreador] Parâmetros desaparecem após alterar env-map
&#x200B;* [Prateleira] Falha ao colocar arquivos png na pasta do gerador
&#x200B;* [Prateleira] As miniaturas são geradas com baixa aspereza
&#x200B;* [Ferramenta] Falha ao usar um bitmap na alfa do pincel no Windows
&#x200B;* [Export] A predefinição de exportação de mapa adicional agora exporta um mapa de RGB para a Posição

### 1.5.7

*(Lançado: 24 de setembro de 2015)*

**Corrigido:**

&#x200B;* O relatório de falha não funciona mais

### 1.5.6

*(Lançado: 21 de setembro de 2015)*

**Adicionado:**

&#x200B;* [Prateleira] Melhorar a qualidade da renderização de miniaturas (usar texturas de 1 K)

**Corrigido:**

&#x200B;* [Compartilhar] Não é possível assinar com outra conta
&#x200B;* [Prateleira] Miniaturas muito pesadas no disco
&#x200B;* [Prateleira] Materiais inteligentes são muito lentos de carregar
&#x200B;* [Windows] Corrigir a instalação do serviço de licença
&#x200B;* [Canais] O mapa transmissivo é criado como G8 por padrão

### 1.5.5

*(Lançado: 15 de setembro de 2015)*

**Adicionado:**

&#x200B;* [Prateleira] Exportar ativos para o Substance share
&#x200B;* [Prateleira] Adicionar nova visualização de esfera para Materiais
&#x200B;* [Prateleira] Use o mapa de ambiente “Pátio vidrado” para gerar miniaturas
&#x200B;* [Prateleira] Aumentar a resolução do tamanho da miniatura para 512 x 512 pixels
&#x200B;* [Visualização 3D] Expor o valor de rotação do ambiente
&#x200B;* [Windows] Assinar o aplicativo

**Corrigido:**

&#x200B;* [Baker] Resultados incorretos ao fazer bake mapas ao mesmo tempo
&#x200B;* [Visualização 3D] O mapa de ambiente é exibido quando nenhum projeto está aberto
&#x200B;* [Camadas] Os Geradores de máscara não funcionam no conteúdo da camada
&#x200B;* [Camadas] Você pode tinta em camadas ocultas
&#x200B;* [Prateleira] Os ruídos de Dirt\_5 e Dirt\_6 são idênticos
&#x200B;* [Prateleira] Alguns geradores de máscara são pixelados ou de baixa qualidade
&#x200B;* [Ferramenta] Rotação incorreta do cursor em determinados ângulos.
&#x200B;* [Ferramenta] Muitos canais fazem com que os botões do canal sejam cortados
&#x200B;* [Ferramenta] O atalho Inverter máscara para Máscara rápida não funciona
&#x200B;* [Exportar] Sketchfab: o botão Cancelar não foi levado corretamente em consideração
&#x200B;* A ativação do [License] falhou quando a licença não pode ser copiada
&#x200B;* O limitador de taxa de quadros não funciona mais na interface do usuário

### 1.5.0

*(Lançado: 20 de agosto de 2015)*

<b>Adicionado:</b>

&#x200B;* [Sombreador] Adicionar número de linha em mensagens de erro de compilação de Sombreador
&#x200B;* [Prateleira] Melhorar a qualidade das visualizações de miniaturas
&#x200B;* [Prateleira] Automatizar geração de miniaturas para materiais inteligentes
&#x200B;* [Ferramenta] Atalho para controlar a configuração de dureza no substance
&#x200B;* [Ferramenta] Usar o widget de tons de cinza para decalque geométrico quando estiver sobre uma máscara
&#x200B;* [Ferramenta] Atalho para inverter a cor da pintura ao pintar em um mapa em tons de cinza
&#x200B;* [Visor] Permite exibir o wireframe e alterar sua cor
&#x200B;* [Visor] Desfocar o fundo do ambiente
&#x200B;* [Controles] Adicionar rotação aos atalhos de mouse do pincel
&#x200B;* [Exportar] Exportar para o Sketchfab
&#x200B;* [Exportar] Criar predefinições de exportação para renderizadores
&#x200B;* [Exportar] Adicionar Reflexo de mapa convertido, F0 e 1/IOR
&#x200B;* [UI] Tela Adicionar boas-vindas
&#x200B;* [UI] Atualizar layout padrão
&#x200B;* [UI] Adicionar dicas de ferramentas ausentes e renomear alguma entrada de menu
&#x200B;* [Camadas] Exportar máscara selecionada atualmente como bitmap
&#x200B;* [Camadas] Adicionar a ação “inverter máscara” no menu do botão direito do mouse

<b>Corrigido:</b>

&#x200B;* [Projeto] Se os eixos das malhas forem diferentes no FBX, as malhas são explodidas na importação
&#x200B;* [Substance] Os Substance usados nas ferramentas de projeção estão bloqueados em 256\*256
&#x200B;* [Camadas] Falha ao usar limpar máscara
&#x200B;* [Exportar] Conversão de gama incorreta em texturas muito escuras
&#x200B;* [Exportar] O mapa de posição só pode ser usado em predefinições de exportação como um mapa em tons de cinza
&#x200B;* [Ferramenta] A cor inicial do decalque de geometria é preta quando usada em uma máscara
&#x200B;* [Ferramenta] O atalho de rotação não funciona se não houver dureza no alfa

### 1.4.2

*(Lançado: 15 de julho de 2015)*

**Corrigido:**

&#x200B;* [Ferramenta] Falha ao usar o decalque de geometria com máscara rápida
&#x200B;* A atualização do projeto da versão 1.4.0 para a 1.4.1 consome toda a memória do computador
&#x200B;* Importação incorreta do formato do projeto antigo
&#x200B;* Prateleiras personalizadas analisam toda a hierarquia e duplicam ativos em todos os lugares

### 1.4.1

*(Lançado: 23 de junho de 2015)*

**Adicionado:**

&#x200B;* [Visor] Permitir encaixe dos painéis lado a lado
&#x200B;* [Efeito] Adicionar um plano de fundo e uma régua para o efeito de nível
&#x200B;* [Efeito] Adicione um efeito de Tinta que permita trabalhar sobre outro efeito

**Corrigido:**

&#x200B;* [Prateleira] A geração de miniaturas é interrompida se nenhum projeto estiver aberto
&#x200B;* [Prateleira] Falha ao gerar a visualização de predefinição de material
&#x200B;* [Prateleira] As visualizações de material são geradas em uma malha com normais invertidos
&#x200B;* [Prateleira] As miniaturas sempre são recalculadas devido à função de hash incorreta
&#x200B;* [Prateleira] Clicar em um material do substance não conecta mapas adicionais
&#x200B;* [Ferramenta] Valor incorreto amostrado com seletor de material
&#x200B;* [Ferramenta] Cor do cursor do visor de seleção de cores
&#x200B;* [Visualização 2D] Taxa de quadros/desempenho muito baixos
&#x200B;* [Exportar] Falha ao abrir a janela de exportação com predefinições de exportação muito recentes.
&#x200B;* [Exportar] O canal de Height para Mapa normal é convertido no espaço errado
&#x200B;* [Mac] BaseColor dos efeitos de substância é exibido como Linear
&#x200B;* [Mac] O widget de linhas retas é desenhado incorretamente na Retina
&#x200B;* As linhas retas podem permanecer ativadas mesmo com o atalho liberado.
&#x200B;* O guizmo de linhas retas desaparece após girar o mapa ambiental
&#x200B;* As saídas de oclusão ambiente de substâncias não são conectadas ao canal AO automaticamente
&#x200B;* Corrigir problema de cópia de licença no Windows com caractere especial no nome de usuário

### 1.4.0

*(Lançado: 10 de junho de 2015)*

**Adicionado:**

&#x200B;* [Exportar] Adicionar mapas adicionais na lista de mapas de entrada disponíveis
&#x200B;* [Prateleira] Usar materiais sbsar como predefinições de material
&#x200B;* [Prateleira] Permitir o uso de caminhos de biblioteca personalizados
&#x200B;* [Prateleira] Alterar o tamanho mínimo
&#x200B;* [Prateleira] Novo conteúdo: 20 novos materiais inteligentes
&#x200B;* [Prateleira] Novo conteúdo : nova substância processual (tecelagem, malha)
&#x200B;* [Prateleira] Filtro Desfoque atualizado
&#x200B;* Desenhar linhas retas usando uma tecla modificadora
&#x200B;* Adicionar canal de Oclusão ambiente e retrabalhar o comportamento AO/Normal na pilha de camadas
&#x200B;* Ler a cor padrão da Entrada de imagem definida nos dados do usuário Substance
&#x200B;* Permitir a exportação do log a partir do menu Ajuda

**Corrigido:**

&#x200B;* [Baker]&#x200B;[Mac] Falha com normal do padeiro de malha
&#x200B;* [Baker] Falha se não houver UVs no arquivo da caixa
&#x200B;* [Baker] A correspondência por nomes não funciona com OBJs exportados do zBrush
&#x200B;* [Baker] Cozimento com uma gaiola sobrescreve o cozimento se usar vários conjuntos de textura e UVs sobrepostos
&#x200B;* [Baker] Arquivos OBJ específicos resultam em texturas pretas
&#x200B;* [Prateleira] Não é possível ler recursos se definido como somente leitura
&#x200B;* [Prateleira] Os arquivos de ativos estão sendo gravados no Painter se tiverem sido usados no projeto.
&#x200B;* [Prateleira] Recarregamento de substâncias também atualizar a camada
&#x200B;* [Export] O Tiff exporta imagens de 32 bits que não podem ser lidas corretamente pelo Photoshop ou por mecanismos de jogo
&#x200B;* [Exportar] A predefinição de canais padrão sempre é exportar como RGB
&#x200B;* [Material] Canal difuso substitui o mapeamento de BaseColor com substâncias
&#x200B;* [Visualização 3D] Iluminação difusa incorreta com mapas de ambiente específicos
&#x200B;* [Ferramenta] Não é possível girar um pincel para um ângulo específico
&#x200B;* O visor obtém o foco quando o mouse é ativado ao digitar em um campo de texto
&#x200B;* Falha com predefinições muito recentes para a versão atual da prateleira
&#x200B;* Falha após substituir a malha
&#x200B;* Falha ao recarregar uma substância com um número diferente de entradas
&#x200B;* Malhas FBX da importação do Cinema4D com nomes de material incorretos

### 1.3.5

*(Lançado: 29 de maio de 2015)*

**Adicionado:**

&#x200B;* Problema de ativação do [License] quando há um arquivo de licença existente
&#x200B;* [Mac] Falha ao carregar arquivos FBX específicos
&#x200B;* [Mac]&#x200B;[Exibição 3D] Reflexão incorreta para GPU integrada
&#x200B;* [Exibição 3D] A fonte da Máscara rápida está quebrada
&#x200B;* [Exibição 3D] O seletor de materiais torna a janela de visualização totalmente preta
&#x200B;* Falha após abrir projetos criados na versão 1.3.3
&#x200B;* A visualização do material fica vazia ao usar sombreadores com alfa
&#x200B;* Pintura para de funcionar em malhas específicas
&#x200B;* O desempenho diminui muito com malhas OBJ específicas
&#x200B;* Os canais do usuário não são mapeados ao usar efeitos
&#x200B;* As pastas temporárias não são limpas na inicialização

**Corrigido:**

&#x200B;* Melhorias no tempo de computação em projetos extremamente longos para carregar
&#x200B;* Altere a janela “Solução de problemas de GPU” para ser mais compreensível
&#x200B;* [Camadas] Salva o status do bloqueio de proporção para camadas de preenchimento e torna-o “Ativado” por padrão
&#x200B;* [Padeiros] A correspondência por nome agora usa o sufixo como separador

### 1.3.4

*(Lançado: 27 de abril de 2015)*

**Adicionado:**

&#x200B;* [Mac] Falha com o Mac OS X Yosemite (10.10)
&#x200B;* [Mac] Não é possível sair do modo de tela cheia
&#x200B;* [Panificadores] A opção Coincidir pelo nome não funciona
&#x200B;* [Bakers] O espaço tangente Mikk usado no SP não funciona com UE4
&#x200B;* [Padeiros] O padeiro de identidade não pode assar cores de ID de material
&#x200B;* [2D View] O Wireframe não aparece ao usar a ferramenta de decalque Geométrico
&#x200B;* [Ferramenta] O canal alfa do pincel é exibido como verificador em vez de transparência com materiais
&#x200B;* [Ferramenta] Falha com decalque de geometria
&#x200B;* [Camadas] O slot de material é recolhido por padrão na camada de preenchimento
&#x200B;* [Exportar] Falha ao exportar em tamanho maior do que a resolução do conjunto de textura
&#x200B;* O canal do specular não é reconhecido nos filtros.
&#x200B;* Limpar e salvar não remove os recursos do arquivo do spp corretamente
&#x200B;* Não armazenar transformação de baixo polígono em arquivo de alta poliuretagem do compartimento
&#x200B;* O arquivo FBX é importado com muitos conjuntos de textura

**Corrigido:**

&#x200B;* Efeitos: os níveis de fixação devem estar ativados por padrão para imitar os níveis “clássicos”
&#x200B;* Camadas: alterar a divisão mínima e máxima na ação Preencher
&#x200B;* Camadas: salvar e restaurar o status da pilha
&#x200B;* Baker: Baker AO levar o mapa normal em consideração se nenhum HP for especificado
&#x200B;* Baker: dicas de ferramentas e informações adicionais adicionadas à janela de fça bake
&#x200B;* Criar um arquivo de backup ao salvar um projeto

### 1.3.3

*(Lançado em: 01 de abril de 2015)*

**Adicionado:**

&#x200B;* Adicionar versão de software e nome do projeto na barra de título
&#x200B;* Limpar nomes de TextureSet e nomes de Material inteligente
&#x200B;* Atualizar mecanismo de Substance para V5
&#x200B;* [Shelf] Adicionar novos mapas de ambiente: praia da Córsega, estúdio 05, estúdio de Tornoco e muito mais
&#x200B;* [Prateleira] Atualizar MG Mask Builder com novos parâmetros
&#x200B;* [Prateleira] Atualizar e calibrar mapas de ambiente antigos

**Corrigido:**

&#x200B;* Falha ao abrir a janela de exportação
&#x200B;* Não é possível arrastar e soltar no widget da interface do usuário quando desencaixado
&#x200B;* “Verificar atualizações” não está funcionando
&#x200B;* [Camadas] Não selecione a máscara ao pressionar ALT e clicar nela
&#x200B;* [Ferramenta] Triplo-planar não funciona com o canal Normal
&#x200B;* [Visualização 3D] A iluminação da Difusão do mapa de ambiente está incorreta
&#x200B;* [Visualização 3D] O cálculo da exposição é diferente do Designer
&#x200B;* [Visualização 3D] As sombras não devem ser visíveis em uma superfície 100% metálica
&#x200B;* [Visualização 3D] A malha com UVs espelhados tem tangente/binômios invertidos
&#x200B;* [Visualização 3D] As sombras produzem resultados incorretos em determinadas malhas
&#x200B;* [Baker] Remove a pasta “.alg\_meta” criada por arquivos assbin
&#x200B;* [Baker] Falha ao fazer bake se o Painter recalcula um TextureSet ao mesmo tempo
&#x200B;* [Mac] Falha na interface do usuário da caixa branca ao iniciar o aplicativo

### 1.3.2

*(Lançado: 06 de março de 2015)*

**Corrigido:**

&#x200B;* [Visualização 3D] Falha ao recarregar um mapa de ambiente salvo com o projeto

### 1.3.1

*(Lançado: 05 de março de 2015)*

**Adicionado:**

&#x200B;* [Baker] Adicionar uma versão em cache de malhas de alto polígono para acelerar o cálculo
&#x200B;* [Baker] Adicionar um ícone de aviso se nenhuma malha de alto polígono estiver carregada
&#x200B;* [Baker] Se nenhuma malha de alto polígono estiver carregada, use a malha do projeto

**Corrigido:**

&#x200B;* [Baker] Pressionar “enter” ao editar o valor de um controle deslizante fecha a janela
&#x200B;* [Baker] Ativar/desativar um baker também acionará o botão
&#x200B;* [Baker] Impossível fazer bake se você usar o botão “tudo/nenhum”
&#x200B;* [Baker] A classificação dos botões de baker não está na ordem correta
&#x200B;* [Baker] As caixas de seleção são ignoradas e todos os baker são sempre processados
&#x200B;* [Baker] Progresso da barra de progresso corrigido

### 1.3.0

*(Lançado: 04 de março de 2015)*

**Adicionado:**

&#x200B;* [Baker]&#x200B;[Visualização 3D] Usar cálculo de espaço tangente Mikkt se nenhuma tangente/binormal for encontrado
&#x200B;* [Baker] Adicionados novos baker: Normal, ID, Oclusão, Curvatura, Thickness, Posição
&#x200B;* [Efeitos] A pilha de efeitos agora é invertida e exibida de cima para baixo (como camadas)
&#x200B;* [Efeitos] Adicionar novos ícones na pilha de efeitos
&#x200B;* [Efeitos] Adicionar modo de mesclagem entre ações de preenchimento na pilha de efeitos
&#x200B;* [Efeitos] Renomear efeitos (efeito de substância = filtro, etc.)
&#x200B;* Adicionar um arquivo de “bloqueio” durante o processo de salvamento
&#x200B;* [Efeitos] Adicionar ação de preenchimento na pilha de efeitos
&#x200B;* Adicionado novo recurso : Materiais inteligentes
&#x200B;* [Camadas] Permitir a reordenação de efeitos de camada
&#x200B;* [Ferramenta] Adicionar projeção tri-Planar
&#x200B;* [Visualização 3D] Adicionar suporte para sombras
&#x200B;* [Visualização 3D] Capacidade de definir os estados OpenGL necessários em sombreadores personalizados
&#x200B;* [Visualização 3D] Suporte para alfa por meio de novos sombreadores
&#x200B;* [Visualização 3D] Os sombreadores agora possuem versão e foram salvos completamente em um projeto
&#x200B;* [Visualização 3D] Avisa o usuário se o sombreador não for mais compilado

**Corrigido:**

&#x200B;* [Camadas] corrigir soltar em uma pasta recolhida
&#x200B;* [Prateleira] Corrigir filtragem de conteúdo em miniprateleiras
&#x200B;* [Prateleira] Renomear categorias e reorganizar guias

### 1.2.1

*(Lançado em: 12 de fevereiro de 2015)*

**Adicionado:**

&#x200B;* Os arquivos \*.spp agora podem ser abertos com um clique duplo no explorador
&#x200B;* [Exportar] Nova tag “$project” para predefinições de exportação
&#x200B;* [Exportar] Adicionar a lista de mapas (com nomenclatura) abaixo de cada conjunto de textura
&#x200B;* [Exportar] Adicionar um botão Todos/Nenhum para selecionar os conjuntos de texturas
&#x200B;* [Exportar] Mapas vazios são descartados durante a exportação

**Corrigido:**

&#x200B;* [Export] As predefinições do Unity5 têm mapas invertidos
&#x200B;* [Exportar] Adicionar uma barra em um nome predefinido criará uma pasta corrompida
&#x200B;* [Exportar] O canal de Height exportado em formatos de 32 bits está incorretamente compactado
&#x200B;* [Exportar] A lista de conjuntos de texturas não é classificada como no projeto
&#x200B;* [Ferramenta] A remoção de fundo não funciona mais
&#x200B;* Salvar não funciona com caracteres especiais no caminho

### 1.2.0

*(Lançado: 28 de janeiro de 2015)*

**Adicionado:**

&#x200B;* Novo canal Normal permitindo pintar os dados normais do mapa e combinar os resultados
&#x200B;* [Exportar] Nova janela de exportação com a capacidade de criar uma embalagem personalizada e definir nomes personalizados
&#x200B;* O formato de arquivo do projeto agora é um único arquivo em vez de pastas
&#x200B;* [Exportar] Suporte a diferentes formatos Normais (DirectX, OpenGL)
&#x200B;* [Exportar] Criar um arquivo temporário de “bloqueio” durante a exportação
&#x200B;* [Camadas] Shift+Clique com o botão esquerdo do mouse pode ser usado para alternar uma máscara
&#x200B;* [Parâmetros] Expor o espaço de cores na parte inferior de uma entrada de imagem
&#x200B;* [Prateleira] O efeito “MG Mask Builder” agora tem novas configurações
&#x200B;* [Exibição 3D] O mapa de Oclusão ambiente agora oclui a contribuição difusa, não o specular

**Corrigido:**

&#x200B;* A visualização do material de projeção/estêncil não é exibida corretamente no visor
&#x200B;* [Exibição 3D] Dica de ferramenta de atalho não exibida ao usar o atalho “S” (estêncil)
&#x200B;* [Shelf] O efeito “Escala de pele MatFx” agora tem melhores desempenhos em baixa resolução
&#x200B;* [Exportar] As texturas da exportação são ampliadas ao especificar um tamanho de documento maior

### 1.1.2

*(Lançado: 15 de janeiro de 2015)*

**Adicionado:**

&#x200B;* Adicionado: novas configurações de Traduzir, Girar e Dimensionar na camada Preenchimento
&#x200B;* Filtragem aprimorada para camadas de Pincéis e Preenchimento
&#x200B;* A versão de teste agora está completa em recursos (pode exportar), mas é limitada no tempo.

**Corrigido:**

&#x200B;* Impossível importar malhas OBJ com precisão muito pequena
&#x200B;* Problema ao ativar uma licença no Windows 7 e 8
&#x200B;* Falha durante um “Salvar como” de um projeto
&#x200B;* Falha ao excluir o último canal de um conjunto de textura
&#x200B;* Falha ao excluir uma camada em um contexto específico

### 1.1.1

*(Lançado: 25 de dezembro de 2014)*

**Adicionado:**

&#x200B;* [Camada] Selecione a camada na parte superior ao abrir um conjunto de texturas de projeto/alternância
&#x200B;* Velocidade aprimorada de “Salvar” e “Salvar como” com o novo algoritmo de compactação
&#x200B;* Exibir um erro ao abrir um projeto muito recente para o Painter

**Corrigido:**

&#x200B;* [Ferramenta] O decalque geométrico produz corrupções na memória
&#x200B;* [Pincel] Impossível inserir manualmente valores de flutuação abaixo de 1 para o tamanho do pincel
&#x200B;* [Camada] Criar um efeito de seleção de cor não o adiciona à pilha de camadas
&#x200B;* [Camada] Mover o mouse sobre as camadas faz com que o Painter passe rapidamente na barra de tarefas
&#x200B;* [Camada] Adicionar um bitmap como máscara pode levar a uma falha
&#x200B;* A interface gráfica para o modo solo com o canal de Height está incorreta
&#x200B;* “Salvar projeto” pode falhar e corromper um projeto
&#x200B;* Falha ao abrir um projeto após carregar outro com um sombreador desatualizado

### 1.1.0

*(Lançado: 16 de dezembro de 2014)*

**Adicionado:**

&#x200B;* [Efeito] Novo criador de máscara de ID de material
&#x200B;* Nova linha branca/preta pontilhada para o cursor do pincel
&#x200B;* Novo parâmetro de sequência de ângulo
&#x200B;* Novo parâmetro de remoção de tela de fundo
&#x200B;* Novo parâmetro de mouse lento
&#x200B;* [Camadas] Suporte para várias seleções e gerenciamento
&#x200B;* [Camadas] Copiar e colar de um conjunto de texturas para outro
&#x200B;* [Exportar] Formato PSD do Adobe Photoshop
&#x200B;* [Prateleira] Nova ferramenta : pele, pontos de metal e zíper
&#x200B;* [Prateleira] Novo pincel : molde, lápis, linha afiada e ponto
&#x200B;* [Prateleira] Novo alfa : ruído gaussiano, linha afiada, molde, caneta, respingo, ponto, zíper
&#x200B;* O desempenho da pintura melhorou atualizando apenas partes das texturas necessárias

**Corrigido:**

&#x200B;* [Prateleira] Impossível carregar uma substância com gráfico com rótulos idênticos
&#x200B;* [Camadas] O modo de mistura Passagem não funciona com máscaras
&#x200B;* A escala de [Estêncil] está quebrada no Visualização 2D
&#x200B;* Problemas e falha no Mac OS Yosemite

### 1.0.2

*(Lançado: 09 de novembro de 2014)*

**Adicionado:**

&#x200B;* Desempenho aprimorado na visualização de material com substâncias
&#x200B;* Desempenho aprimorado com visualização de traçado de pincel ao atualizar o documento
&#x200B;* Desempenho aprimorado no visor com menor taxa de atualização para a área não funcional
&#x200B;* [Pós-efeitos] Interface aprimorada para gerenciar configurações
&#x200B;* [Pós-efeitos] Redefinir para valores padrão
&#x200B;* efeitos de Substance e operações de camadas no menu do botão direito do mouse
&#x200B;* Apoio a entradas/saídas pré-multiplicadas em substâncias

**Corrigido:**

&#x200B;* [Visualização 3D] Os parâmetros de sombreador personalizados são separados por um espaço grande
&#x200B;* [Exportar] Conversão sRGB para predefinição Unity4 ausente
&#x200B;* Possível falha ao carregar malhas fbx
&#x200B;* Falha às vezes ao carregar malhas obj simples
&#x200B;* A barra de computação permanece bloqueada até 100% no carregamento
&#x200B;* Recarregar uma substância a coloca em todas as categorias
&#x200B;* Chave de DirectX/OpenGL quebrada

### 1.0.1

*(Lançado: 27 de outubro de 2014)*

**Adicionado:**

&#x200B;* [Ferramenta] Uso aprimorado de parâmetros de material
&#x200B;* Novo atalho para o site do UserVoice no menu Ajuda
&#x200B;* Várias melhorias de desempenho no motor

**Corrigido:**

&#x200B;* Os valores dos parâmetros são limitados a 2 decimais para Partículas
&#x200B;* Os Substance carregados do cache não são exibidos na interface como desatualizados
&#x200B;* Falha ao carregar uma malha de uma url de rede
&#x200B;* O Painter agora é reconhecido como assinado no Mac OS X

### 1.0.0

*(Lançado: 15 de outubro de 2014)*

**Adicionado:**

&#x200B;* Suporte a shader personalizado
&#x200B;* Suporte para resolução 4k
&#x200B;* Projetos de personagem de amostra
&#x200B;* Exibir barra de progresso para longos tempos de computação
&#x200B;* [Exportar] Adicionar uma passagem de dilatação antes do pós-processo de difusão
&#x200B;* Argumentos de linha de comando no SP para operações simples
&#x200B;* Novos materiais e efeitos
&#x200B;* Visualização da ferramenta (visualização de material em tempo real separado e área de teste de traçado)
&#x200B;* Não criar um documento padrão quando o Painter for iniciado
&#x200B;* [Ferramenta] Adicionar a possibilidade de editar manualmente um valor em tons de cinza
&#x200B;* Várias melhorias para os estênceis (Ajustar, Redefinir)
&#x200B;* As partículas agora são subferramentas das ferramentas Pincel, Borracha e Projeção
&#x200B;* [Exibição 3D] Usar AO cozido na renderização do visor
&#x200B;* Dividir os controles de estênceis entre a exibição 2D e 3D
&#x200B;* Ajuste pequeno do tamanho do polegar na biblioteca
&#x200B;* Os campos de pesquisa são específicos para cada janela
&#x200B;* Ajustes da interface

**Corrigido:**

&#x200B;* [Substância] O switch não funciona
&#x200B;* [Caixa de diálogo Cor] Degradê de matiz não atualizado
&#x200B;* Não é possível atualizar uma malha se o nome do arquivo é idêntico
&#x200B;* A ferramenta não fica visível nas exibições quando muito pequena
&#x200B;* A ferramenta de decalque na tela Retina não funciona corretamente
&#x200B;* [Substance] Int1 são exibidos como float1
&#x200B;* [Substance] A entrada/saída basecolor não é reconhecida
&#x200B;* Não é possível recarregar os filtros [Substance]
&#x200B;* O widget de tons de cinza [Ferramenta] sempre é recolhido

## Beta

### &#x200B;0. 12. 1- beta

*(Lançado: 18 de setembro de 2014)*

**Adicionado:**

&#x200B;* Predefinição de exportação do Unity 5

**Corrigido:**

&#x200B;* PBR Shader, a qualidade da renderização deve melhorar muito
&#x200B;* A função de foco está quebrada e as malhas são cortadas por padrão

### &#x200B;0. 12. 0- beta

*(Lançado: 17 de setembro de 2014)*

**Adicionado:**

&#x200B;* Ferramenta Conta-gotas
&#x200B;* A opção “Preservar posição de traçado” foi adicionada à reimportação de malha para quando a caixa delimitadora for alterada.
&#x200B;* Mapa normal para a malha padrão de Cymourai
&#x200B;* Aprimorar a interface de exibição da ferramenta (as cores são wip)
&#x200B;* Mova o menu “Ajuda->Configurações” para “Editar->Configurações”
&#x200B;* Salve o caminho de exportação na janela “Exportar todos os canais”
&#x200B;* Novos níveis de GUI com exibição de histograma
&#x200B;* Melhor gerenciamento de ativos (arrastar e soltar, recarregar recursos, excluir não usados)
&#x200B;* Alternar de “difusa” para “basecolor”
&#x200B;* Controles deslizantes que editam ajustes - permitem pontos além de vírgulas
&#x200B;* Camada de preenchimento: aumentar o valor máximo de divisão em blocos gráficos
&#x200B;* Mapa de ambiente padrão

**Corrigido:**

&#x200B;* Artefatos de reflexo inválidos em ângulos extremos
&#x200B;* Exportação de specular/brilho quebrado
&#x200B;* Links na janela “sobre” do pintor não funcionam
&#x200B;* Falha com o OSX Yosemite
&#x200B;* A malha é salva triangulada
&#x200B;* O atalho de cor da janela Ferramenta envia para o emissor em vez da escala de cinza
&#x200B;* O seletor de cores permanece aberto ao alternar de camada para máscara
&#x200B;* Não é possível salvar o material de uma camada de preenchimento
&#x200B;* Habilitar o redimensionamento das três regiões da prateleira

### &#x200B;0. 11. 0- beta

*(Lançado em: 4 de setembro de 2014)*

**Adicionado:**

&#x200B;* Adicionar um divisor entre as visualizações 3D e 2D
&#x200B;* Usar um plano de fundo gradiente nas visualizações 2D/3D
&#x200B;* Interface para o histograma de Níveis
&#x200B;* Mesclar prateleira e biblioteca
&#x200B;* Nenhuma ação de salvamento é necessária ao criar ou atualizar uma predefinição
&#x200B;* Importar ativos de prateleira por meio da funcionalidade de arrastar e soltar

**Corrigido:**

&#x200B;* O nome dos botões é exibido acima na barra de ferramentas principal

### &#x200B;0. 10. 2- beta

*(Lançado: 28 de agosto de 2014)*

**Corrigido:**

&#x200B;* Exportar todos os canais produz resultados incorretos

### &#x200B;0. 10. 1- beta

*(Lançado: 26 de agosto de 2014)*

**Corrigido:**

&#x200B;* Sombreador dá resultado preto com baixa aspereza
&#x200B;* Verificação da GPU: use placas “Quadro”, detecte todos os dispositivos e adapte as mensagens do usuário de acordo
&#x200B;* A maioria dos materiais do Substance está limitada a 256 na versão Beta 9
&#x200B;* O height é bloqueado quando exportado como bitmap
&#x200B;* A visualização do pincel é diferente da sobreposição da projeção no Mac
&#x200B;* O uso da ferramenta Geometria para criar máscaras não é exibido em viewports
&#x200B;* A máscara rápida está quebrada
&#x200B;* Corrigir problema de mesclagem no mac pro antigo

### &#x200B;0. 10. 0- beta

*(Lançado em: 07 de agosto de 2014)*

**Adicionado:**

&#x200B;* Máscaras de estêncil

**Corrigido:**

&#x200B;* Suporte a placas Quadro
&#x200B;* O sombreador dá resultado preto com baixa aspereza
&#x200B;* Os materiais do Substance estão limitados a 256
&#x200B;* A exportação normal de mapa exclui o canal verde

### &#x200B;0. 9. 0- beta

*(Lançado: 17 de julho de 2014)*

**Adicionado:**

&#x200B;* Pós-processamento do Yebis 2
&#x200B;* O assistente para Novo projeto permite importar mapas de entrada (AO, Curvatura, etc.)
&#x200B;* Conectar automaticamente mapas de entrada (AO, curvatura etc.) para Efeitos de Substance
&#x200B;* Controle da escala sobre os materiais aplicados às camadas de preenchimento

### &#x200B;0. 8. 2- beta

*(Lançado: 11 de julho de 2014)*

**Corrigido:**

&#x200B;* O controle deslizante Matiz assume branco como padrão
&#x200B;* Projeto será redefinido se o Nome do material contiver caracteres especiais
&#x200B;* A alteração do nome do material em um único objeto de material não deve invalidar o projeto.
&#x200B;* Os UVs ficam confusos depois de salvar o projeto e reabri-lo

### 0.8.1-beta

*(Lançado em: 4 de julho de 2014)*

**Corrigido:**

&#x200B;* Várias falhas de GPU
&#x200B;* Falha ao exportar canais

### &#x200B;0. 8. 0- beta

*(Lançado: 28 de junho de 2014)*

**Adicionado:**

&#x200B;* Vários materiais - agora você pode pintar em vários materiais no mesmo documento
&#x200B;* Pintura de simetria
&#x200B;* Todos os modos de mesclagem agora estão disponíveis

**Corrigido:**

&#x200B;* Várias falhas de GPU
&#x200B;* Projeto será redefinido se o Nome do material contiver caracteres especiais
&#x200B;* Os UVs ficam confusos depois de salvar o projeto e reabrem com vários UVs

### &#x200B;0. 7. 0- beta

*(Lançado: 18 de junho de 2014)*

**Adicionado:**

&#x200B;* Efeitos de camada
&#x200B;* Novos materiais de estêncil de Substance
&#x200B;* Limpar máscara
&#x200B;* Permitir copiar/colar camada/máscara
&#x200B;* Permitir Duplicar Camada
&#x200B;* Alterar ferramenta ao editar máscara de camada
&#x200B;* Os Substance agora são ativados por GPU

**Corrigido:**

&#x200B;* A pintura do mapa de altura não tinta valores negativos.
&#x200B;* A exibição do Seletor de materiais não deve levar em conta o mapa normal de amostra
&#x200B;* Determinismo de partículas quebrado
&#x200B;* Matriz de estêncil no Visualização 2D
&#x200B;* Ngons em arquivos obj
&#x200B;* Várias falhas

### &#x200B;0. 6. 0- beta

*(Lançado em: 04 de junho de 2014)*

**Adicionado:**

&#x200B;* Nova opção de exportação para exportar um mapa de Specular de um composto de aspereza e canais metálicos

**Corrigido:**

&#x200B;* Compatibilidade com o Windows Vista
&#x200B;* O mapa de altura não tinta valores negativos

### &#x200B;0. 5. 0- beta

*(Lançado em: 07 de maio de 2014)*

**Adicionado:**

&#x200B;* 3D/Visualização 2D switches
&#x200B;* Ferramenta Seleção de partes UV
&#x200B;* A ferramenta muda automaticamente ao pintar em máscaras.
&#x200B;* A resolução dos Substance depende da

**Corrigido:**

&#x200B;* Falha na inicialização
&#x200B;* Falha com malhas ASCII
&#x200B;* Matriz de estêncil fixa no Visualização 2D
&#x200B;* Falha com o Borracha

### &#x200B;0. 4. 0- beta

*(Lançado: 17 de abril de 2014)*

**Adicionado:**

&#x200B;* Visualização 2D contínuo
&#x200B;* Máscaras de camada de bitmap
&#x200B;* Controle de exposição do ambiente
&#x200B;* Preencher camadas agora usa a janela Ferramentas para definir suas propriedades
&#x200B;* Os materiais podem ser aplicados a camadas de preenchimento
&#x200B;* Adicionou mais estênceis à biblioteca de estênceis
&#x200B;* Predefinições de partículas atualizadas para uma computação mais rápida
&#x200B;* Otimização do sombreador PBR e melhoria da qualidade para configurações de qualidade mais baixa

**Corrigido:**

&#x200B;* As miniaturas de camadas são vinculadas ao canal atualmente selecionado
&#x200B;* Muitas falhas

### &#x200B;0. 3. 0- beta

*(Lançado: 04 de abril de 2014)*

**Adicionado:**

&#x200B;* Permitir valores negativos no seletor de cores para pintura do mapa de altura
&#x200B;* Mostrar visualização do material/cor separado
&#x200B;* Adicionar atalhos para as Ferramentas na Barra de Ferramentas (1, 2, 3, 4)
&#x200B;* Alternar o formato normal (OpenGL versus DirectX) globalmente em um projeto
&#x200B;* Assistente para Novo projeto
&#x200B;* O controle deslizante de espaçamento não está mais apertado
&#x200B;* Estilo atualizado dos controles deslizantes
&#x200B;* Tornar o seletor de cores não modal
&#x200B;* Selecionar um material na biblioteca define o tipo de ferramenta adequadamente

**Corrigido:**

&#x200B;* Corrigido: o caminho da malha de importação não é preservado
&#x200B;* Correção: geração de texturas incorreta
&#x200B;* Corrigido: falha na inicialização

### &#x200B;0. 2. 0- beta

*(Lançado: 17 de março de 2014)*

**Adicionado:**

&#x200B;* Conta-gotas de material (atalho P)
&#x200B;* Miniaturas na visualização da ferramenta 3D
&#x200B;* Sistema de licenciamento para versões autônomas
&#x200B;* Atalhos [ e ] para Tamanho do pincel
&#x200B;* Preenchimento em mapas exportados
&#x200B;* Estilo de Janela de Ferramenta Atualizado
&#x200B;* Estilo atualizado dos controles deslizantes
&#x200B;* Ambiente HDR padrão atualizado

**Corrigido:**

&#x200B;* Estêncil: alterar o valor do fluxo na exibição 3D para em 52
&#x200B;* Loop infinito no motor ao adicionar teclas de pressão 0 ao traço é fixo
&#x200B;* Ferramenta: a tremulação de ângulo não retorna valores acima de +/- 90%
&#x200B;* A exibição 3D muda quando uma máscara de camada é selecionada
&#x200B;* Zoom invertido

### 0.1.0-beta

*(Lançado: 02 de março de 2014)*

**Adicionado:**

&#x200B;* Novo gerenciamento de biblioteca
&#x200B;* Novo conteúdo de pincéis e partículas
&#x200B;* Visualização do pincel 3D
&#x200B;* Estilo de Janela de Ferramenta Atualizado
&#x200B;* Estilo atualizado dos controles deslizantes
&#x200B;* Desempenho atualizado do cache

**Corrigido:**

&#x200B;* Controles de câmera
&#x200B;* Rotação do pincel
