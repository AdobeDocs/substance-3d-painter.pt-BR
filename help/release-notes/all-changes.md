---
breadcrumb-title: ''
description: Revise todas as alterações e atualizações nas versões do Substance 3D Painter para acompanhar a evolução e as melhorias de recursos ao longo do tempo.
title: Todas as alterações
user-guide-description: ''
user-guide-title: ''
source-git-commit: 479eb327180dd223bbff362e3f200995565cbcfa
workflow-type: tm+mt
source-wordcount: '40713'
ht-degree: 0%
---

# Todas as alterações

Esta página contém notas de versão de todas as versões anteriores do Substance 3D Painter, classificadas da mais recente para a mais antiga.

>[!NOTE]
>
> Para exibir os problemas conhecidos que podem afetar o Painter, consulte a [página de documentação dedicada](known-issues.md).

## Versão 12

### 12.2.0

Data de lançamento: **2026/10/21**

Resumo: **Esta atualização é uma versão principal. Ela adiciona um novo recurso de Pintura em gaiola para fça bake e faz melhorias na funcionalidade de preenchimento de Polígono. Para obter mais detalhes, consulte as notas de versão completas.**

**Adicionado:**

* Fazendo bake, pintura em gaiola
* &preto;Pintura em gaiola&rbrack; Criar interface de Tinta básica em gaiola
* &preto;Pintura em gaiola&rbrack; Novas opções de Visualização em gaiola
* &preto;Pintura em gaiola&rbrack; Editável Ferramenta Selecionar / Preencher
* &preto;Pintura em gaiola&rbrack; Mostrar Modo Combinar na barra de ferramentas
* &preto;Pintura em gaiola&rbrack; Alterações na interface do controle deslizante HDR
* &preto;Pintura de gaiola&rbrack; sombreador de visualização
* &preto;Pintura em gaiola&rbrack; Redefinir opções da pilha
* Melhorias na ferramenta Preenchimento de polígono
* &amp;Preenchimento de polígono&rbrack; Adicionar correção de polígono
* &amp;Preenchimento de polígono&rbrack; Adicionar loop de polígono
* &amp;Preenchimento de polígono&rbrack; suporte para Simetria com Loop/Correção
* &amp;Preenchimento do polígono&rbrack; visualização da borda da Simetria
* &amp;Preenchimento de polígono&rbrack; Remover triângulos com loops e loops parciais
* &preto;Preenchimento de polígono&rbrack; Wireframe visível somente para o Conjunto de texturas ativo
* &preto;Preenchimento de polígono&rbrack; Realce de borda vermelha em triângulos não clicáveis
* &preenchimento;Preenchimento de polígono&rbrack; Não desative as opções do modo de preenchimento
* &amp;Preenchimento de polígono&rbrack; Permitir a definição de todas as propriedades de canal com o Preenchimento de polígono
* &amp;Preenchimento de polígono&rbrack; Retomar traçado anterior funciona com Preenchimento de polígono
* &preto;Preenchimento de polígono&rbrack; Mostrar cursor proibido em conjuntos de texturas não ativos
* &amp;Preenchimento do polígono&rbrack; ALT visualização instantânea
* &amp;Preenchimento de Polígono&rbrack; Atalho para alternar temporariamente para Polyloop (SHIFT+A)
* &preto;Visor&rbrack; Mostrar conjunto de texturas / realce de seleção de Bloco UV
* &lbrack;Visor&rbrack; Adicionar suporte para Transparência Independente da Ordem no visor em tempo real
* &lbrack;Configurações de exibição&rbrack; Reorganizar as configurações de exibição em novos grupos
* &lbrack;Tool&brack; Adicionar suporte para mesclagem aditiva com pinceladas
* &lbrack;Tool&brack; Adicionar suporte para mesclagem aditiva com Preenchimento de Polígono
* &lbrack;USD&rbrack; O USD exportado com mapa de opacidade torna tudo transparente em Arnold
* &lbrack;Nvidia&rbrack; Adicionar aviso sobre os drivers Nvidia mais recentes (616.56 a 617.14)
* Adicionar nova entrada de mapa do mecanismo “mesh_uv_neighbor”
* Atualize os baker para a versão 3.23.0
* Atualize o mecanismo de Substance para a versão 9.6.1

**Corrigido:**

* &lbrack;Fazendo bake&rbrack; A Oclusão de ambiente Ignorar face de fundo pelo nome da malha não funciona
* &lbrack;Fazendo bake&rbrack; &lbrack;AMD&rbrack; Dispositivo perdido ao fazer bake com malhas pesadas de alta espessura
* &lbrack;Desempenho&rbrack; Painter hogs VRAM uso
* &lbrack;Viewport&rbrack; texturas ausentes ao abrir projetos em telas HDPI
* O modo de mesclagem &preto;Tool&rbrack; fica esmaecido ao pintar em uma máscara
* Pastas temporárias não excluídas após a exportação na rede
* &lbrack;USD&rbrack; A geometria USD exportada é dividida ao longo das bordas UV
* &lbrack;USD&rbrack; Congelar ao carregar USDz malformado

### 12.1.5

Data de lançamento: **09/2026/15**

Resumo: **Versão secundária**

**Corrigido:**

* Exportar imagem de prateleira para uma rede não funciona mais
* &lbrack;Gerador&rbrack; Configurar “usar textura” como falso não desativa o uso da entrada de textura
* O visor congela ao salvar enquanto edita a projeção 3D
* A resolução da camada de material é muito baixa

### 12.1.4

Data de lançamento: **9/2026/04**

Resumo: **Versão secundária**

**Corrigido:**

* &lbrack;Falha&rbrack; Falha ao importar ou exportar arquivos cujos nomes de arquivo contenham caracteres não-ASCII

### 12.1.3

Data de lançamento: **2026/08/26**

Resumo: **Versão secundária**

**Adicionado:**

* Atualize o mecanismo de Substance para a versão 9.4.6

**Corrigido:**

* &preto;Seletor de tons de cinza&rbrack; permanece aberto após alterar a ferramenta
* &preto;Inclinar Fazendo bake&rbrack; Inclinar interrupções de correção ao pintar e desfazer
* &lbrack;Ferramenta de Projeção&rbrack; A interação do visor está bloqueada pela ferramenta de projeção
* &preto;Traçado dinâmico&rbrack; Parâmetros de traçado dinâmico ausentes nas propriedades do pincel
* Exportar para uma rede não funciona mais

### 12.1.2

Data de lançamento: **08/2026/03**

Resumo: **Versão secundária**

**Corrigido:**

* &lbrack;Crash&rbrack; Alguns Substance podem levar a uma falha quando renderizados
* &lbrack;Crash&rbrack; Reimportar malha enquanto estiver no modo de fça bake
* &lbrack;Crash&rbrack; A falha ao inicializar a exibição de gráficos pode levar a um travamento
* &lbrack;Falha&rbrack; A exportação de texturas pode falhar em alguns casos ao atualizar o registro
* &lbrack;Falha&rbrack; Falha no modo de fça bake em alguns casos ao carregar/atualizar o mapa de ambiente
* &lbrack;Fazendo bake&rbrack; A reinicialização do faço bake após a modificação do arquivo poly alto pode levar a um congelamento
* &preto;Enviar para o Photoshop&rbrack; Falha ao exportar a máscara da camada
* &lbrack;O resultado do ponto de ancoragem do Engine&brack; não é renderizado entre uma máscara e um canal de cor

### 12.1.1

Data de lançamento: **07/2026/09**

Resumo: versão secundária

Adicionado:

* &preto;Inclinar Fazendo bake&rbrack; Expor Inclinação Base Modo Normal: malha ou por triângulo
* &lbrack;Propriedades&rbrack; Fazer com que as cores uniformes sempre redefinam para o valor padrão de seus canais
* &lbrack;OpenPBR&rbrack; Reagrupar canais por categorias na janela Exportar Texturas para criação de modelos de saída
* Atualize o mecanismo de Substance para a versão 9.4.5

Corrigido:

* &lbrack;Projeto&rbrack; Abrir e salvar alguns projetos pode demorar mais do que o normal
* &lbrack;Crash&rbrack; Recarregar várias malhas pode levar a um travamento
* &lbrack;Crash&rbrack; Excluir um canal enquanto estiver no modo de exibição de máscara leva a um travamento
* &lbrack;Crash&rbrack; Alguns Substance podem levar a uma falha quando renderizados
* &lbrack;Inclinação da Tinta&rbrack; A ferramenta selecionada na inclinação da tinta permanece selecionada após alternar para o Modo de Pintura
* &lbrack;Fazendo bake configurações comuns&rbrack; As configurações de distância da gaiola não atualizam a visualização do wireframe e do sombreador da gaiola
* &lbrack;Engine&rbrack; O preenchimento UV “Vizinho do espaço 3D” não funciona bem em triângulos finos
* &lbrack;O resultado do ponto de ancoragem do Engine&brack; não é renderizado entre uma máscara e um canal de cor

### 12.1.0

Data de lançamento: **2026/06/23**

Resumo: **Esta atualização é uma versão principal. Ela contém melhorias de baker com Novo estado de interface do usuário padrão de fça bake, mapa de inclinação da pintura, retoque automático, nova opção de desencapsulamento automático UV para malhas de superfície dura e OpenPBR. Para obter mais detalhes, consulte as notas de versão completas.**

**Adicionado**:

* &preto;Inclinar fazendo bake&rbrack; Inclinar Ferramentas de Pintura
* &Preencher;Inclinar Fazendo bake&rbrack; Adicionar Inclinar Visualizar sombreador e Inclinar direção Vetor visuais ao pintar mapa de inclinação
* &preto;Inclinar Fazendo bake&rbrack; Adicionar proteção de borda
* &preto;Inclinar fazendo bake&rbrack; Recozimento automático
* &lbrack;Inclinar Fazendo bake&rbrack; Retrabalhar mapa de malha Interface do usuário da lista
* &preto;Inclinar Fazendo bake&rbrack; Dividir mapa de malha / Configurações de Fça bake comuns + Mover configurações comuns para fora da lista de mapas de malha apenas com base em cores ou máscaras
* &preto;Inclinar Fazendo bake&rbrack; Alterar botões da barra de ferramentas do visor
* &preto;Inclinar Fazendo bake&rbrack; Mostrar alternância de Simetria para o pincel na barra de ferramentas superior
* &lbrack;Inclinar Fazendo bake&rbrack; Renomear opções no menu de Sincronização de lista do mapa de malha
* &lbrack;Inclinar Fazendo bake&rbrack; Atualizar Sincronização e Verificado caixas de diálogo de estado
* &preto;Fça bake de inclinação&rbrack; Criar variante do seletor de cores em tons de cinza
* &preto;Inclinar Fazendo bake&rbrack; Atualizar ícone do modo de fça bake
* &lbrack;Desenvolver automaticamente&rbrack; opção Integrar superfície rígida
* &lbrack;OpenPBR&rbrack; Adicionar suporte para OpenPBR 1.1
* &lbrack;OpenPBR&rbrack; Tornar o OpenPBR o fluxo de trabalho e o sombreador padrão
* &lbrack;OpenPBR&rbrack; Importar materiais e texturas de OpenPBR via USD
* &lbrack;OpenPBR&rbrack; Exportar materiais e texturas de OpenPBR via USD
* &lbrack;OpenPBR&rbrack; Janela Atualizar Texturas de Exportação para mostrar a convenção de nomenclatura do OpenPBR
* &lbrack;OpenPBR&rbrack; Adicionar documentação sobre alterações para suportar o OpenPBR
* &lbrack;OpenPBR&rbrack;&lbrack;Iray&rbrack; Adicionar novo MDL para oferecer suporte ao OpenPBR 1.1 no Iray
* Várias melhorias menores nas exportações de USD
* &lbrack;UI&rbrack; Adicionar aviso no visor ao tentar tinta em outro Conjunto de Texturas
* &Preenchimento;Nivelar&Preenchimento; Permite nivelar todas as camadas instanciadas nos Conjuntos de Textura
* &preto;Configurações do conjunto de texturas&rbrack; Permite selecionar vários canais de uma vez através de uma nova janela
* &lbrack;Histórico&rbrack; Atualizar “valor” Desfazer texto de entrada para refletir o nome do parâmetro
* &lbrack;Pilha de camadas&rbrack; Tornar os efeitos de preenchimento em máscaras padrão em branco (1.0)
* &lbrack;Substance&rbrack; Adicionar nova entrada de mapa do mecanismo “mesh_hard_edges_triangle”
* &lbrack;Substance&rbrack; Adicionar nova entrada de mapa de mecanismo “mesh_hard_edges”
* &lbrack;Sombreador&rbrack; Impedir que instâncias de sombreamento compartilhem os mesmos nomes
* &lbrack;Sombreador&rbrack; Usar o sombreador do modelo do projeto ao importar um arquivo USD ou GLTF
* Atualize o Adobe Color Engine para a versão 7.0
* Atualização mínima da versão do MacOSX para a versão 13.0 (Ventura)
* &lbrack;Content&rbrack; Novos modelos de projeto para OpenPBR
* &lbrack;Content&rbrack; Atualiza projetos de amostra para usar o novo sombreador de OpenPBR
* &lbrack;Python&rbrack; Expandir a API da Máscara de Geometria para permitir modos de inclusão e exclusão, como na interface do usuário

**Corrigido**:

* &lbrack;Crash&rbrack;&lbrack;Configurações de mapas de malha&rbrack; Aplicar configurações a outros conjuntos de textura
* &lbrack;Crash&rbrack; Ao fazer bake a curvatura do mapa sem o espaço global normal
* &lbrack;Falha&rbrack;&lbrack;Fazendo bake&rbrack; Fazendo bake com gaiola personalizada ativada, mas nenhum arquivo selecionado falha
* &lbrack;Falha&rbrack; Cancelando fça bake AO
* &lbrack;Caixa Automática&rbrack; Carga infinita quando o caminho do arquivo poli alto é inválido
* &lbrack;Linux&rbrack;&lbrack;Windows&rbrack; O seletor de cores às vezes pode ficar totalmente preto ou não aparecer
* &preto;Ferramenta Preenchimento de polígono&rbrack; A ferramenta não funciona com não-PBR
* &lbrack;&lbrack;Tinta&rbrack; Excluir o canal de cor de base não exclui a cor pintada anteriormente
* As Instâncias de sombreamento do &lbrack;USD&rbrack; não são detectadas corretamente
* &lbrack;Substance&rbrack; Somente o primeiro uso de um nó de entrada/saída é levado em consideração
* A Oclusão de ambiente do &lbrack;Sombreador&rbrack; é aplicada duas vezes com Conjuntos de Texturas usando diferentes métodos de mistura
* &lbrack;Motor&rbrack; texturas normais com canal azul vazio (preto) podem levar a resultados de mesclagem errados
* &lbrack;GLTF Import&rbrack; A mesclagem de alfa está habilitada em todos os conjuntos de texturas
* &lbrack;GLTF Export&rbrack; A mesclagem de alfa está sempre habilitada na exportação
* &lbrack;Export&brack; A geometria de dupla face está sempre desativada ao importar um arquivo GLTF
* &lbrack;Javascript&rbrack; A modificação das configurações de sombreadores não contribui para o histórico de desfazer
* &lbrack;Amostras&rbrack; A dispersão da subsuperfície não está ativada nas Configurações de Exibição do Mat. da Reunião

### 12.0.3

Data de lançamento: **5/2026**

Resumo: **Versão secundária**

**Adicionado:**

* Atualize os baker para a versão 3.22.2
* Atualize o mecanismo de Substance para a versão 9.4.3
* &lbrack;Python&rbrack; Salva uma material inteligente em um local específico

**Corrigido:**

* &lbrack;Ubuntu&rbrack; Falha ao selecionar material
* &lbrack;O pop-up recorrente do Mac&rbrack; aparece para pedir acesso aos dados de outros aplicativos
* &lbrack;Fazendo bake&rbrack; Artefatos podem aparecer no mapa de curvatura
* &lbrack;Fazendo bake&rbrack; Fazendo bake é mais lento em alguns casos
* &preto;Distorcer para geometria&rbrack; A opção Distorcer para geometria fica desativada em alguns casos
* &lbrack;Bloco UV&rbrack; Alfa extraída do ponto de ancoragem ignorada por outras peças
* &lbrack;Python&rbrack;&lbrack;Mac&rbrack; Exceções no console Python com SSL
* &lbrack;Python&rbrack; Painter falha ao sair com widgets Qt restantes

### 12.0.2

Data de lançamento: **04/2026/07**

Resumo: **Versão secundária**

**Adicionado:**

* &lbrack;Gerenciamento de cores&rbrack; Adicionar novo OCIO para especificar o espaço de cores padrão do seletor de cores
* &lbrack;Python&rbrack; Expor configurações de desajuste automático na API Python

**Corrigido:**

* &lbrack;Falha&rbrack; Salvar com espaço em disco insuficiente pode travar ou corromper projetos
* &lbrack;Crash&rbrack; &lbrack;Ribbon&rbrack; Usar a faixa de opções pode causar falhas para alguns projetos
* &lbrack;Falha&rbrack; &lbrack;Fazendo bake&rbrack; falha quando o arquivo .assbin não pode ser gravado na pasta
* &lbrack;Malhas OBJ do Stager podem falhar na criação do projeto
* &lbrack;Import&brack; OBJ tem rosto ausente em alguns casos
* &lbrack;Import&brack; malha USD sem nenhum material atribuído pode falhar na importação
* &lbrack;Caminho preenchido&rbrack; Não afetado pela simetria
* &prec;Estêncil&brack; A visualização tem resolução menor do que o resultado pintado
* &lbrack;UI&rbrack; &#39;uv island&#39; ainda é mencionado na dica de ferramenta de origem de cores do mapa de ID
* &lbrack;Display&brack; As sombras aparecem invertidas
* O transformo de projeção &lbrack;Viewport&rbrack; Warp permanece após alternar para o modo de fça bake
* &lbrack;Distorcer&brack; A grade desaparece quando a escala é definida como 0 no eixo Z com Distorcer para geometria ativado
* &lbrack;Python&rbrack; Erro inesperado ao adicionar um canal com modificação no escopo

### 12.0.1

Data de lançamento: **03/2026/18**

Resumo: **Versão secundária**

**Corrigido:**

* &lbrack;Crash&rbrack;&lbrack;Congelar&rbrack; Exportar de projetos específicos

### 12.0.0

Data de lançamento: **03/2026/09** Resumo: **esta é uma versão principal. Esta versão contém os recursos de camadas achatadas, distorção na geometria, novos pós-efeitos, melhoria na janela do novo projeto e outras melhorias.**

**Adicionado**:

* &Preencher;Nivelar camadas&rbrack; Nivelar camadas dentro da pilha de camadas
* &Preenchimento;Achatar camadas&rbrack; Exportar camadas achatadas para o disco
* &lbrack;Distorcer para geometria&rbrack; Adicionar nova funcionalidade de deformação automática a Distorcer projeções
* &lbrack;Pós-efeitos&rbrack; Substituir pós-efeitos pela adição de novos
* &lbrack;Pós-efeitos&rbrack; Atualizar mapeador de tons
* &lbrack;Pós-efeitos&rbrack; Adicionar novo uso para ativos de Pós-efeitos
* &lbrack;Content&brack;&lbrack;Post-effects&rbrack; Integra os ativos padrão de pós-efeitos na biblioteca
* &lbrack;Novo Projeto&rbrack; Melhorar a interface para a criação de projetos
* &lbrack;Novo projeto&rbrack; Alterações na funcionalidade de malha de reimportação
* &lbrack;Novo projeto&rbrack; Permitir que arquivos \*.geo.usd sejam abertos
* &lbrack;Configuração do projeto&rbrack; Melhorar interface para a configuração do projeto
* Atualizar a biblioteca USD para a versão 25.05
* Atualize o Substance Engine para a versão 9.3.4
* Aumente o mínimo de drivers para 25.3.1/25.Q2 para GPUs AMD
* Atualize o Qt para 6. 8. 6
* &lbrack;Scripting&rbrack; Atualiza a API JavaScript para a versão 1.1.20
* Atualizar Python para a versão 3.13

**Corrigido:**

* &lbrack;Crash&rbrack; Alterar uma saída de canal de material em uma máscara pode travar
* &lbrack;Import&rbrack; As texturas EXR são forçadas para sRGB em vez de lineares ao importar arquivos USD
* &lbrack;Blocos UV&rbrack; A sequência de imagens com uma única imagem também preenche outros Blocos UV
* &lbrack;Fazendo bake&rbrack; O AO é diferente entre o fça bake de CPU e GPU
* &lbrack;Color Management&rbrack;&lbrack;MacOS&rbrack; Viewport BaseColor não corresponde ao selecionador de cores
* &lbrack;USD&rbrack; Valores uniformes não são importados em alguns casos

## Versão 11

### 11.1.3

Data de lançamento: **2026/02/12** Resumo: **versão secundária**

**Corrigido**:

* &lbrack;Tinta&rbrack; Estêncil e simetria não funcionam em alguns casos
* &lbrack;Caminho&rbrack; Nenhuma atualização ao alterar o controle deslizante de opacidade de traçado de borrar
* &lbrack;Projeto&rbrack; Não é possível tinta em alguma geometria
* &lbrack;Ribbon&rbrack; O caminho instanciado desaparece ao alterar a resolução do Conjunto de Texturas
* &lbrack;UI&rbrack; O seletor de cores pode encolher e desaparecer em alguns casos

### 11.1.2

Data de lançamento: **01/2026/13** Resumo: **versão secundária**

**Adicionado**:

* &lbrack;Fazendo bake&rbrack; Melhorar o tempo de fça bake de projetos de Blocos UV com salvamento assíncrono
* &lbrack;Shaders&rbrack; A menção no API de sombreamento muda após a migração Vulkan
* Atualizar OpenEXR para a versão 3.4.4

**Corrigido**:

* &lbrack;Crash&rbrack; Falha durante a inicialização na série Nvidia GTX 10xx
* &lbrack;Crash&rbrack; Usar o seletor de cores em diferentes Conjuntos de texturas pode resultar em uma falha ao sair do aplicativo
* &preto;Desempenho&rbrack; Problema de desempenho ao pintar no projeto com muitas camadas
* &lbrack;Desempenho&rbrack; Atraso ao pintar com caneta eletrônica gráfica
* &lbrack;UI&rbrack; As configurações da câmera permanecem desativadas no modo de renderização (Iray)
* &lbrack;Ribbon&rbrack; O caminho pode se sobrepor inesperadamente após um canto em alguns casos
* &lbrack;Ribbon&rbrack; Problema de desempenho com Blocos UV
* &lbrack;Substance&rbrack;&lbrack;UI&rbrack; As entradas de imagem desaparecem quando recolhidas
* &lbrack;Substance&rbrack;&lbrack;UI&rbrack; Os grupos aninhados podem permanecer mesmo se Visíveis Se os ocultarem
* &lbrack;Fazendo bake&rbrack;&lbrack;UI&rbrack; Não é possível definir o Raio de Amostragem da Curvatura além de 0,01
* &lbrack;Fazendo bake&rbrack;&lbrack;UI&rbrack; Não é possível definir a Distância Máxima do Ocultador além de 1
* &lbrack;Fazendo bake&rbrack; A configuração do AO “Auto-oclusão” é ignorada com vários Conjuntos de Textura e Baixo como Alto fazendo bake
* O mapa de ID do &lbrack;Fazendo bake&rbrack; não faz bake as cores dos vértices do FBX no modo Baixo como Alto
* O filtro &lbrack;Content&brack; Highpass resulta em cores esmaecidas em canais com gerenciamento de cores

### 11.1.1

Data de lançamento: **12/2025/09** Resumo: **versão secundária**

**Adicionado**:

* &lbrack;Desempenho&rbrack; Melhorar o desempenho dos Blocos UV ao calcular texturas parciais
* &lbrack;Baker&rbrack; Atualize para a versão 3.15.4

**Corrigido**:

* &lbrack;Falha&rbrack;&lbrack;MacOS&rbrack; Salvar projeto de versão anterior sempre falha
* &lbrack;Falha&rbrack; Fechar um projeto às vezes pode resultar em uma falha
* &lbrack;Projeto&rbrack; Erro “incompatibilidade na contagem de membros” ao abrir o projeto feito na versão anterior
* Os Blocos UV &lbrack;Fazendo bake&rbrack; não são combinados com resultados de fazes bake anteriores, se presentes
* &lbrack;Fazendo bake&rbrack; Dispositivo perdido mesmo com Rastreamento de raios desativado na série Nvidia GTX 10XX
* &lbrack;Fazendo bake&rbrack; AO com normal tem artefatos nas bordas porque não há preenchimento
* &lbrack;Fazendo bake&rbrack; A configuração do AO “Auto-oclusão” é ignorada com vários Conjuntos de Texturas e “corresponder pelo nome” em
* O Mapa de ID do &lbrack;Fazendo bake&rbrack; é totalmente preto se alguma malha de alto polígono não tiver cores de vértice
* &lbrack;Faixa de opções&rbrack; A dica de ferramenta para o modo de mesclagem Alfa menciona o modo de mesclagem Tela em vez do Subexposição linear
* &lbrack;Caminho&rbrack; Tangentes criam loop inesperado quando o ponto é movido próximo às extremidades do caminho
* &lbrack;Tool&brack; A visualização do material não funciona quando a projeção é usada em uma máscara
* &preto;Engine&brack; Pintar traçados pequenos pode resultar em artefatos em blocos
* &lbrack;Sombreador&rbrack; Se você desfizer a criação da instância de sombreamento, ela não será removida corretamente
* &lbrack;O modo de Alpha de Exportação&rbrack; para exportação de GLTF é sempre definido como MASK
* &lbrack;Python&rbrack; Erro inesperado ao editar a pilha de camadas fora do bloco de modificação com escopo

**Problemas Conhecidos**:

* &lbrack;Ribbon&rbrack; Problema de desempenho com Blocos UV
* &lbrack;Ribbon&rbrack; O caminho pode se sobrepor inesperadamente após um canto em alguns casos
* &lbrack;Crash&rbrack;&lbrack;Ribbon&rbrack; Criar textos muito longos na Faixa de Opções pode falhar
* &lbrack;Gerenciamento de cores&rbrack; As conversões do espaço de cores HDR com ACE no Linux produzem cores fixas
* &lbrack;Regressão&rbrack;&lbrack;UI&rbrack; O menu do botão direito do mouse é muito pequeno em telas HD
* &lbrack;Crash&rbrack;&lbrack;Python&rbrack; Exportação de USD acionada por TextureStateEvent
* &lbrack;Engine&brack; Pintura com ferramenta Clonar nas cores normais de mudança de canal incorretamente
* &lbrack;Python&rbrack; O widget fantasma aparece excluído pelo script ainda em funcionamento

### 11.1.0

Data de lançamento: **2025/11/18** Resumo: **esta atualização é uma versão principal; ela contém a nova ferramenta Faixa de Opções com conteúdo novo dedicado, suporte a simetria para camadas de preenchimento, parâmetro de tamanho físico para deslocamento, desempenho aprimorado através dos baker atualizados, suporte completo a Vulkan para Windows e Linux e outras melhorias.**

**Adicionado**:

* Nova ferramenta da faixa de opções
* &lbrack;Tool&brack; Adicionar nova ferramenta de Faixa de Opções para criar caminhos perfeitos
* &preto;Faixa de opções&rbrack; Adicionar atalhos predefinidos da Faixa de opções na janela Propriedades
* &lbrack;Ribbon&rbrack; Permite alterar a opacidade da Faixa de Opções por vértice no caminho
* &lbrack;Ribbon&rbrack; Permite alterar o tamanho da Faixa por vértice no caminho
* &lbrack;Ribbon&rbrack; Remove o início/fim definido em um Substance quando os caminhos são fechados
* &lbrack;Ribbon&rbrack; Remover Caminho/Visualização de material na janela de propriedades das ferramentas Tinta/Borracha/Borrar caminho
* &lbrack;Ribbon&rbrack; Adicionar modos de mesclagem para o alfa e alguns canais quando autosobrepostos
* Preencher simetria
* &Preencher;Preencher&preencher; Adicionar suporte para simetria em camadas e efeitos de preenchimento
* &lbrack;Preenchimento&rbrack;&lbrack;UI&rbrack; Expor as configurações de simetria na janela de propriedades para a camada de preenchimento e efeitos
* &lbrack;Fill&brack; Interface de configuração de simetria de Retrabalho no menu do visor e na janela de propriedades
* &lbrack;Fill&brack; Reorientar adequadamente as texturas normais ao projetar no modo de distorção
* deslocamento do tamanho físico
* &lbrack;Deslocamento&rbrack; Usar tamanho físico como unidade de deslocamento
* Melhoria de desempenho
* &lbrack;Desempenho&rbrack; Melhorar a renderização de pinceladas pequenas em triângulos grandes
* &lbrack;Desempenho&rbrack; Melhorar o tempo de compilação do Sombreador
* &lbrack;Performance&rbrack; Suporte completo a Vulkan para Windows e Linux
* &lbrack;Desempenho&rbrack; baker atualizados com renderização de GPU mais rápida e suporte ao Rastreamento de raios AMD
* &lbrack;UI&rbrack; Reorganizar as propriedades das ferramentas em grupos e recolher algumas por padrão
* &lbrack;Engine&rbrack; Atualização Substance Engine para a versão 9.2.5
* &lbrack;Substance&rbrack; Expor substituição de resolução para recursos Substance em Ferramentas e Preenchimentos
* &preto;Exportar&rbrack; Atualizar predefinição de exportação de Mapas de Malha para exportar texturas em tons de cinza
* Python
* &lbrack;Fazendo bake&rbrack;&lbrack;Python&rbrack; Indicar em changelog mudanças de quebra após atualização de baker
* &lbrack;Python&rbrack; Expor as configurações de simetria de preenchimento no Python
* Conteúdo e novo conteúdo
* &lbrack;Content&brack; Adicionar 75 novas predefinições de ferramenta para a ferramenta Faixa de Opções
* &lbrack;Content&brack; Atualiza o recurso construtor de gradientes para que seja compatível com a Faixa de Opções

**Corrigido**:

* &lbrack;Falha&rbrack; Carregar outro projeto enquanto o ajuste de caminho está ativado pode falhar
* &lbrack;Falha&rbrack; Clique com o botão direito do mouse no painel Caminho com informações de outra sessão na área de transferência pode falhar
* A interface do &lbrack;UI&rbrack; rola para cima nas propriedades da ferramenta ao criar um caminho
* &lbrack;UI&rbrack; O cursor do mouse desaparece quando a visualização do visor do caminho está oculta
* &lbrack;Caminho&rbrack; Copiar/colar diferentes propriedades de ferramenta no painel Caminho levam a propriedades instáveis
* As predefinições da ferramenta &Preenchimento; Borracha e Borrar nem sempre atualizam a seleção de canal
* &lbrack;Tool&brack; O valor pintado é cinza, mas a interface mostra branco após carregar a predefinição de ferramenta colorida na máscara
* &lbrack;A predefinição &amp;Tool&rbrack; criada a partir da máscara mantém os valores de canais carregados de outra predefinição
* &lbrack;Substance&rbrack; A substituição do espaço de cores normal definida no gráfico não é levada em consideração
* &lbrack;Content&brack; O recurso de forma de pincel padrão usa um Substance desatualizado

**Problemas Conhecidos**:

* Histórico de Instância de sombreamento não controlado corretamente
* &lbrack;Ribbon&rbrack; Problema de desempenho com Blocos UV
* &lbrack;Ribbon&rbrack; O caminho pode se sobrepor inesperadamente após um canto em alguns casos
* &lbrack;Ribbon&rbrack; As tangentes criam um loop indesejado quando o ponto é movido próximo das extremidades do caminho
* &lbrack;Crash&rbrack;&lbrack;Ribbon&rbrack; Criar textos muito longos na Faixa de Opções pode falhar
* &lbrack;Tool&brack; A visualização do material não funciona quando a projeção é usada em uma máscara
* &lbrack;Fazendo bake&rbrack; A configuração do AO “Auto-oclusão” é ignorada com vários Conjuntos de Texturas e a opção “corresponder pelo nome” ativada
* &lbrack;Fazendo bake&rbrack; O AO com normal possui artefatos nas bordas devido à falta de preenchimento
* &lbrack;Gerenciamento de cores&rbrack; As conversões do espaço de cores HDR com ACE no Linux produzem cores fixas
* &lbrack;Regressão&rbrack;&lbrack;UI&rbrack; O menu do botão direito do mouse é muito pequeno em telas HD
* &lbrack;Crash&rbrack;&lbrack;Python&rbrack; Exportação de USD acionada por TextureStateEvent
* &lbrack;Engine&brack; Pintura com ferramenta Clonar nas cores normais de mudança de canal incorretamente
* &lbrack;Python&rbrack; O widget fantasma aparece excluído pelo script ainda em funcionamento

### 11.0.3

Data de lançamento: **08/2025/05** Resumo: **versão secundária**

**Adicionado**:

* &lbrack;Substance 3D Assets&rbrack; Adicionar um ponto de notificação ao painel Ativos 3D
* &lbrack;VFX Platform 2025&rbrack; Adicionar configuração ACE 2.0 nas configurações de gerenciamento de cores
* &lbrack;VFX Platform 2025&rbrack; Atualização do OCIO para a versão 2.4.2
* Atualize o Iray para a versão 2024.10
* &lbrack;Engine&rbrack; Atualização para o Substance Engine v.9.2.3
* &lbrack;Nvidia&rbrack; Eleva a versão mínima dos drivers Nvidia para 572.60 (Win) e 570.169 (Linux)

**Corrigido**:

* &lbrack;Python&rbrack; A Modificação com Escopo não aparece na janela Histórico

**Problemas Conhecidos**:

* &lbrack;Gerenciamento de cores&rbrack; As conversões do espaço de cores HDR com ACE no Linux produzem cores fixas
* &lbrack;Regressão&rbrack;&lbrack;UI&rbrack; O menu do botão direito do mouse é muito pequeno em telas HD
* &lbrack;Crash&rbrack;&lbrack;Python&rbrack; Exportação de USD acionada por TextureStateEvent
* &lbrack;Engine&brack; Pintura com ferramenta Clonar nas cores normais de mudança de canal incorretamente
* &lbrack;Python&rbrack; O widget fantasma aparece excluído pelo script ainda em funcionamento

### 11.0.2

Data de lançamento: **06/2025/10** Resumo: **versão secundária**

**Adicionado**:

* &lbrack;Mac&rbrack; Adicionar aviso sobre a versão específica do sistema operacional levando a artefatos
* &lbrack;Atualização automática&rbrack; Pequenas melhorias de UX no registro de erros de Ativos
* &lbrack;Contornar automaticamente&rbrack; Atualize para a versão 1.3.2 com melhorias de costura
* &lbrack;USD&rbrack;&lbrack;FBX&rbrack; Adicionar suporte para vários conjuntos UV com dados esparsos
* &lbrack;Export&rbrack; As malhas exportadas como FBX não têm seus conjuntos UV adicionais, se houver algum presente na importação

**Corrigido**:

* &lbrack;MacOS&rbrack;&lbrack;Linux&rbrack; Falha ao salvar na unidade de rede
* &lbrack;Win&rbrack;&lbrack;Tablet&rbrack; cintilando ao deslocar
* &lbrack;SpaceMouse&rbrack; Problema ao trabalhar com a ferramenta Caminho
* &lbrack;Caixa automática&rbrack; Não é possível fazer bake após um recarregamento de malha
* &lbrack;Atualização automática&rbrack; A sequência de imagens não é recarregada quando o primeiro bloco está ausente
* &lbrack;Caminho&rbrack; A tangente personalizada pode afetar a outra tangente
* &lbrack;O caminho&rbrack; não aparece no Conjunto de texturas se o primeiro ponto estiver em outro Conjunto de texturas
* &lbrack;UI&rbrack; Alguns menus são sempre desativados após a abertura de um projeto (por exemplo: simetria)
* &lbrack;Propriedades&rbrack; Não é possível usar/carregar predefinições de ferramenta com a ferramenta Caminho preenchido
* &lbrack;USD&rbrack; Vários conjuntos UV não são reconhecidos no sombreador personalizado ao usar arquivos USD
* &brack;USD&rbrack; Câmeras com os mesmos nomes são substituídas
* &preto;Exportar&rbrack; Enviar para o Photoshop resulta em espaço de cor incorreto para os resultados em cores e em tons de cinza
* &preto;Exportar&rbrack; canais em tons de cinza com alfa são exportados como cor em vez de escala de cinza com formato PNG
* &lbrack;Export&brack; Exportar canal em tons de cinza como resultado de PSD em arquivo inválido/truncado
* &lbrack;Content&brack; O filtro Distorcer em modo multidirecional não funciona
* &lbrack;Python&rbrack; Não é possível alocar erros de lista ao rastrear nós de pilha de camadas

**Problemas Conhecidos**:

* &lbrack;Gerenciamento de cores&rbrack; As conversões do espaço de cores HDR com ACE no Linux produzem cores fixas
* &lbrack;Regressão&rbrack;&lbrack;UI&rbrack; O menu do botão direito do mouse é muito pequeno em telas HD
* &lbrack;Crash&rbrack;&lbrack;Python&rbrack; Exportação de USD acionada por TextureStateEvent
* &lbrack;Engine&brack; Pintura com ferramenta Clonar nas cores normais de mudança de canal incorretamente
* &lbrack;Python&rbrack; O widget fantasma aparece excluído pelo script ainda em funcionamento

### 11.0.1

Data de lançamento: **04/2025/10** Resumo: **versão secundária**

Observação: a versão do CCD do **Linux será adiada até 29 de abril**

**Adicionado:**

* Atualize para Qt 6.5.8
* &lbrack;Substance&rbrack; Adicionar mensagem de log para filtros quando várias entradas de imagem compartilham o mesmo uso
* &lbrack;Nvidia&rbrack; Adicionar aviso sobre os drivers Nvidia mais recentes (572.47)

**Corrigido:**

* &lbrack;Crash&rbrack; Ao arrastar e soltar um sbsar com um uso em slots de canal único
* &lbrack;Crash&rbrack;&lbrack;Caminho&rbrack; A opção Alterar tipo de caminho não fica esmaecida quando não se clica em um caminho específico
* &lbrack;Caminho de preenchimento&rbrack; Não deve ser capaz de selecionar o material da substância
* &lbrack;Engine&brack; Artefatos ao longo de pinceladas
* &lbrack;Engine&rbrack; Os caminhos podem ser quebrados com configurações específicas
* Problema com o menu suspenso para o espaço da cor do conta-gotas
* &lbrack;Atualização automática&rbrack; &lbrack;Python&rbrack; Mensagem de erro incorreta ao usar ResourceID sem versão
* &lbrack;Sombreador&rbrack; Falha ao abrir alguns projetos

**Problemas Conhecidos:**

* &lbrack;SpaceMouse&rbrack; Problema ao trabalhar com a ferramenta Caminho
* &lbrack;Gerenciamento de cores&rbrack; As conversões do espaço de cores HDR com ACE no Linux produzem cores fixas
* &lbrack;Regressão&rbrack;&lbrack;UI&rbrack; O menu do botão direito do mouse é muito pequeno em telas HD
* &lbrack;Crash&rbrack;&lbrack;Python&rbrack; Exportação de USD acionada por TextureStateEvent
* &lbrack;Engine&brack; Pintura com ferramenta Clonar nas cores normais de mudança de canal incorretamente
* &lbrack;Python&rbrack; O widget fantasma aparece excluído pelo script ainda em funcionamento

### 11.0.0

Data de lançamento: **03/2025/11** Resumo: **Versão principal, novo recurso de atualização automática, ferramenta de caminho preenchido e outras melhorias no caminho, bem como novos filtros e uma geração experimental de gaiola automática para fça bake**

**Adicionado**:

* Atualização automática
* &lbrack;Atualização automática&rbrack; Atualizar automaticamente os ativos modificados no painel Ativos
* &lbrack;Atualização automática&rbrack; Atualizar automaticamente os ativos modificados em todo o projeto
* &lbrack;Atualização automática&rbrack; Manter a atualização automática desativada por padrão
* &lbrack;Atualização automática&rbrack; Tornar a atualização opcional se os parâmetros de recurso não corresponderem (.sbsar, .glsl, .ai, .svg)
* &lbrack;Atualização automática&rbrack; Adicionar variável de ambiente para desativar o recurso de atualização automática
* &lbrack;Atualização automática&rbrack;&lbrack;SBSAR&rbrack; Tornar a atualização opcional se os parâmetros do recurso não corresponderem
* Caminho preenchido
* &lbrack;Caminho&rbrack;&lbrack;Preenchimento&rbrack; Adicionar nova ferramenta para criar caminhos preenchidos
* Melhorias de caminho
* &lbrack;Caminho&rbrack; Cria um caminho que se ajusta aos polígonos
* &lbrack;Caminho&rbrack; Permitir alternar tipos de caminho
* &lbrack;Caminho&rbrack; Permite copiar e colar dados de vértice de caminho entre conteúdo e máscara
* &lbrack;Caminho&rbrack; Permite restringir o ângulo ao criar um novo ponto
* &lbrack;Caminho&rbrack; Permite restringir a criação de pontos a uma linha
* &lbrack;Path&brack; Fechar forma com um único clique
* &lbrack;Caminho&rbrack; Exibir informações de caminho
* &lbrack;Caminho&rbrack; Permite dimensionar e girar vértices de caminho
* &lbrack;Path&rbrack;&lbrack;UX&rbrack; Facilitar o acesso aos gizmos de transformação
* &lbrack;Caminho&rbrack; Adicionar visualização de caminho
* &lbrack;Caminho&rbrack; Desativar a visualização do caminho com Shift + P
* &lbrack;Caminho&rbrack; Melhorar a edição da tangente na visão lateral
* &lbrack;Caminho&rbrack; Permite focalizar em um caminho 3D
* &lbrack;Caminho&rbrack; Os vértices devem manter o status da seleção ao alternar a interface entre desativada e ativada novamente
* &lbrack;Caminho&rbrack; Permite excluir o Caminho usando o Backspace
* &lbrack;Caminho&rbrack; Mantém a lista de caminhos aberta se o usuário a expandir
* &lbrack;Caminho&rbrack;&lbrack;Pilha de camadas&rbrack; Renomeia duplicatas corretamente ao copiar/colar
* &lbrack;Caminho&rbrack; UI e melhorias na dica de ferramenta
* Desempenho
* &lbrack;Desempenho&rbrack; Melhorar o desempenho do visor ao usar um alto nível de mosaico
* &lbrack;Desempenho&rbrack; Habilita somente o primeiro canal em novas camadas/efeitos de preenchimento
* &lbrack;Desempenho&rbrack; Paralelizar computação de traçado de pincel
* Baking
* &lbrack;Fazendo bake&rbrack; Adicionar nova opção de geração de gaiola totalmente automática para fazer bake com malhas de alto-polietileno (experimental)
* Conteúdo
* &lbrack;Content&rbrack; Adicionar 6 novos filtros: estilização, quantize, kuwahara anisotrópico, suavização de chanfro, distância direcional, conversão em tons de cinza
* &lbrack;Content&rbrack; Atualizar ruídos e grunhidos para a versão mais recente do Designer (com o novo 2D Voronoi)
* &lbrack;Content&brack; Adicionar 3 novos geradores de textura (Telha Aleatória, Triangle Grid, Gerador de Scratches)
* &lbrack;Content&rbrack; Renomear modelo de Mecanismo Irreal e exportar predefinições
* Python
* &lbrack;Shelf&rbrack;&lbrack;Python&rbrack; Salvar material inteligente ou máscara inteligente em disco do Python
* &lbrack;Python&rbrack; Adicionar gaiola automática feita bake à API Python
* &lbrack;Python&rbrack; Permitir a edição de nomes e descrições de Conjuntos/Blocos UV de Textura
* &lbrack;Python&rbrack; Compartilhar configurações de resolução em fontes vetoriais e de fonte
* &lbrack;Atualização automática&rbrack;&lbrack;Python&rbrack; Expor as funcionalidades de atualização automática do projeto em Python
* Diversos
* &brack;Export&brack; Facilite o acesso às opções Enviar para com um novo painel
* &lbrack;Nvidia&rbrack; Adicionar aviso sobre os drivers Nvidia mais recentes (572.16)
* O encaixe de ângulo deve ser afetado pela seleção de espaço Objeto/Mundo
* &preto;Lista do conjunto de texturas&rbrack; Permite adicionar um nome personalizado aos Blocos UV e usá-los na exportação
* Mac
* &lbrack;Mac&rbrack; Usar Metal em vez de OpenGL para renderização gráfica
* &lbrack;Mac&rbrack; Soltar suporte ao Mac Intel

**Corrigido**:

* &lbrack;Crash&brack; Excluir entrada de imagem
* Não é possível adicionar o smart mat através do botão pilha de camadas
* Não é possível encontrar os efeitos do &lbrack;Python&brack; no GroupLayerNode

**Problemas Conhecidos**:

* &lbrack;Gerenciamento de cores&rbrack; As conversões do espaço de cores HDR com ACE no Linux produzem cores fixas
* &lbrack;Regressão&rbrack;&lbrack;UI&rbrack; O menu do botão direito do mouse é muito pequeno em telas HD
* &lbrack;Crash&rbrack;&lbrack;Python&rbrack; Exportação de USD acionada por TextureStateEvent
* &lbrack;MacOS Intel&rbrack; Falha ao importar algumas predefinições
* &lbrack;Engine&brack; Pintura com ferramenta Clonar nas cores normais de mudança de canal incorretamente
* &lbrack;Python&rbrack; O widget fantasma aparece excluído pelo script ainda em funcionamento
* &lbrack;RedHat&rbrack; Problemas no seletor de cores

## Versão 10

### 10.1.2

Data de lançamento: **2024/12/3** Resumo: **versão secundária, correções de erros**

**Corrigido**:

* &lbrack;Crash&brack; Excluir entrada de imagem
* Não é possível adicionar o smart mat através do botão pilha de camadas
* Não é possível encontrar os efeitos do &lbrack;Python&brack; no GroupLayerNode

**Problemas Conhecidos**:

* &lbrack;Gerenciamento de cores&rbrack; As conversões do espaço de cores HDR com ACE no Linux produzem cores fixas
* &lbrack;Regressão&rbrack;&lbrack;UI&rbrack; O menu do botão direito do mouse é muito pequeno em telas HD
* &lbrack;Crash&rbrack;&lbrack;Python&rbrack; Exportação de USD acionada por TextureStateEvent
* &lbrack;MacOS Intel&rbrack; Falha ao importar algumas predefinições
* &lbrack;Engine&brack; Pintura com ferramenta Clonar nas cores normais de mudança de canal incorretamente
* &lbrack;Python&rbrack; O widget fantasma aparece excluído pelo script ainda em funcionamento
* &lbrack;RedHat&rbrack; Problemas no seletor de cores

### 10.1.1

Data de lançamento: **2024/11/5** Resumo: **versão secundária, correções de erros**

**Adicionado**:

* &lbrack;Projeto&rbrack; Mantém o projeto atual aberto até que a seleção do novo projeto seja validada
* &lbrack;Contornar automaticamente&rbrack; A densidade do texel permite dividir melhor as Ilhas UV em UDIMs
* &lbrack;Fazendo bake&rbrack; Corrigir cópia ambígua no menu contextual de Mapas de Malha
* &lbrack;Distorcer&brack; Remover escala no visor para o eixo Z (profundidade)
* &lbrack;Importar/Exportar&rbrack; Remove o suporte de formatos de arquivo de imagem não utilizados
* Atualizar Substance Engine para 9.1.4

**Corrigido**:

* &lbrack;Falha&rbrack; Após realocar recursos em Ativos e salvar projeto
* &lbrack;Crash&rbrack; Problemas com a biblioteca do servidor auxiliar
* &lbrack;Falha&rbrack; falha no servidor Illustrator em alguns casos raros
* &lbrack;Crash&rbrack; Ao sair do aplicativo em alguns casos raros
* Não é possível enviar relatórios de falhas em alguns computadores
* &lbrack;Fazendo bake&rbrack; A cor do vértice não é lida corretamente
* &lbrack;UI&rbrack; A localização das janelas e das Novidades na inicialização é alterada
* &lbrack;Assimp&rbrack; StandardSurface do Maya não reconhecida no fça bake de ID
* &lbrack;Python&rbrack; A biblioteca SSL ausente gera um erro
* &lbrack;Python&rbrack;&lbrack;Win&rbrack; Erro ao chamar QColorConstants.Transparent
* &lbrack;Python&rbrack; As miniaturas de camadas criadas através do Python não são atualizadas até clicar dentro da pilha de camadas
* &lbrack;Sombreador&rbrack; Link quebrado no log de alterações
* &brack;Ativos 3D&rbrack; Usar configurações de proxy do SO ao acessar Ativos 3D

**Problemas Conhecidos**:

* &lbrack;Gerenciamento de cores&rbrack; As conversões do espaço de cores HDR com ACE no Linux produzem cores fixas
* &lbrack;Regressão&rbrack;&lbrack;UI&rbrack; O menu do botão direito do mouse é muito pequeno em telas HD
* &lbrack;Crash&rbrack;&lbrack;Python&rbrack; Exportação de USD acionada por TextureStateEvent
* &lbrack;MacOS Intel&rbrack; Falha ao importar algumas predefinições
* &lbrack;Engine&brack; Pintura com ferramenta Clonar nas cores normais de mudança de canal incorretamente
* &lbrack;Python&rbrack; Widget que parece excluído via script ainda funcionando
* &lbrack;RedHat&rbrack; Problemas no seletor de cores

### 10.1.0

Data de lançamento: **2024/09/17** Resumo: **Versão principal, conteúdo novo: máscara de área de preenchimento/filtro de cor, filtro de decalque de bordado e seis filtros de Substance genéricos, importação de USD com propriedades de material e sombreador, melhoria de desempenho, compatibilidade com a plataforma VFX 2024 e migração para Linux RedHat**

**Adicionado**:

* &preto;Content&brack; Adicionar novo filtro de máscara/cor da área de preenchimento
* &lbrack;Content&brack; Adicionar novo filtro de decalque de bordado
* &lbrack;Content&rbrack; Adicionar 6 novos filtros Substance genéricos (FXAA, pixelate, highpass, posterize, smoothstep, threshold)
* &lbrack;USD&rbrack; Exportar camada de USD com um material ASM definido
* &lbrack;USD&rbrack; Importar USD com propriedades de material e sombreador
* &lbrack;Desempenho&rbrack; Ativar miniaturas de pilha de camadas otimizadas por padrão
* &lbrack;Desempenho&rbrack; Reduz o tempo de abertura do arquivo do projeto e o consumo de memória (decodificação de dados)
* Compatível com a plataforma VFX 2024
* &lbrack;VFX Platform 2024&rbrack; Atualização para Python 3.11
* &lbrack;VFX Platform 2024&rbrack; Atualização para OpenEXR 3.2
* &lbrack;Plataforma VFX 2024&rbrack; &lbrack;USD&rbrack; Atualizar o OpenSubdiv 3.6.0
* &lbrack;VFX Platform 2024&rbrack;&lbrack;Color Management&rbrack; Atualizar para OCIO 2.3.2
* &lbrack;Linux&rbrack; Migração para o Linux RedHat
* &lbrack;Linux&rbrack; Atualize a versão mín do driver Nvidia para 535.171.04
* &lbrack;Import&brack; Adicionar uma opção para inverter o mapa normal ao importar uma malha GLTF
* &lbrack;UI&rbrack; Usar o valor padrão do sistema operacional para a distância de detecção de eventos de arrastar
* &lbrack;Substance Engine&rbrack; Adicionar função de faixa de chamada para remover os símbolos do executável
* &Preenchimento;Tela inicial&rbrack; Atualização para o novo formato de tela inicial
* Atualize o Substance Engine para a versão 9.1.3
* &lbrack;Python&rbrack; Mostrar link para exemplos no menu pilha de camadas documentação
* &lbrack;JavaScript&rbrack; Move plug-ins Javascript para a subpasta javascript/plugins

**Corrigido**:

* &lbrack;Illustrator&rbrack; Falha ao exportar um Bloco UV com gráfico .ai em casos específicos
* &lbrack;Traçados dinâmicos&rbrack;&lbrack;Caminho&rbrack; Aleatório por traçado não funciona em um caminho
* &lbrack;UI&rbrack;&lbrack;Propriedades&rbrack; Bloqueio ativado quando a divisão em blocos gráficos não é uniforme
* O arquivo TXT de depuração é criado ao clicar duas vezes no projeto do Painter
* &lbrack;USD&rbrack;&lbrack;Export&rbrack; Algumas texturas podem estar ausentes
* &lbrack;ASM&rbrack; Dispersão O canal de cores ignora o metal
* O filtro &lbrack;Content&brack; Blur não funciona no espaço de cor “funcionando”
* &lbrack;Content&brack; o filtro Ajustar Height também modifica o alfa da camada

**Problemas Conhecidos**:

* &lbrack;Gerenciamento de cores&rbrack; As conversões do espaço de cores HDR com ACE no Linux produzem cores fixas
* &lbrack;Win&rbrack;&lbrack;Crash&rbrack; &lbrack;ACE&rbrack; Não usar o espaço de cores sRGB ICE para o transformo de exibição
* &lbrack;Regressão&rbrack;&lbrack;UI&rbrack; O menu do botão direito do mouse é muito pequeno em telas HD
* &lbrack;Crash&rbrack;&lbrack;Python&rbrack; Exportação de USD acionada por TextureStateEvent
* &lbrack;MacOS Intel&rbrack; Falha ao importar algumas predefinições
* &lbrack;Crash&rbrack; Realocar recurso e salvar projeto
* &lbrack;Engine&brack; Pintura com ferramenta Clonar nas cores normais de mudança de canal incorretamente
* &lbrack;Python&rbrack; O widget fantasma aparece excluído pelo script ainda em funcionamento
* &lbrack;RedHat&rbrack; Problemas no seletor de cores

### 10.0.1

Data de lançamento: **06/2024/11** Resumo: **versão secundária, correções de erros**

**Adicionado:**

* &lbrack;Library&rbrack; Converte fontes de Substance em arquivos de fonte comuns
* &lbrack;Illustrator&rbrack;&lbrack;SVG&rbrack; Dá às miniaturas na seleção de escopo um fundo cinza claro
* &lbrack;Python&rbrack; Adicionar função na origem do bitmap para listar os espaços de cores disponíveis

**Corrigido**:

* &lbrack;Pilha de camadas&rbrack; Pasta sempre fechada quando movida para dentro ou para fora de outras pastas
* &lbrack;Salvar&rbrack; O arquivo de projeto é perdido quando “salvar como cópia” ou o salvamento automático falha em casos específicos
* &lbrack;Import&brack; Ativos com o mesmo nome, mas com diferentes extensões são substituídos
* &lbrack;Propriedades&rbrack; Configurações ausentes ao usar o ponto de ancoragem nas entradas da imagem
* &lbrack;Illustrator&rbrack; Não é possível importar arquivos do Illustrator após falha no servidor sem reiniciar o Painter
* &lbrack;Python&rbrack; A instância pai não pode ser definida com o tipo “properties”
* &lbrack;Python&rbrack; Configurar o alto poli como um parâmetro de fça bake não carrega o alto poly
* &lbrack;Python&rbrack; A mensagem de erro para set_color_space() é muito genérica
* &lbrack;Python&rbrack; As fontes de referência permitem criar ciclos

**Problemas Conhecidos**:

* &lbrack;Gerenciamento de cores&rbrack; As conversões do espaço de cores HDR com ACE no Linux produzem cores fixas
* &lbrack;Regressão&rbrack;&lbrack;UI&rbrack; O menu do botão direito do mouse é muito pequeno em telas HD
* &lbrack;Crash&rbrack;&lbrack;Python&rbrack; Exportação de USD acionada por TextureStateEvent
* &lbrack;MacOS Intel&rbrack; Falha ao importar algumas predefinições
* &lbrack;Illustrator&rbrack; Falha ao exportar um Bloco UV com gráfico .ai em casos específicos
* &lbrack;Traçados dinâmicos&rbrack;&lbrack;Caminho&rbrack; Aleatório por traçado não funciona em um caminho

### 10.0.0

Data de lançamento: **05/2024/16** Resumo: **Versão principal, edição da pilha de camadas com a API Python, leitura de arquivos nativos do Illustrator, integração de ativos 3D e novo recurso de texto**

**Adicionado**:

* &lbrack;Illustrator&rbrack; Usar arquivos do Illustrator com quadros de arte no Painter
* &lbrack;Illustrator&rbrack;&lbrack;SVG&rbrack; Adicionar visualizações na seleção de escopo
* &lbrack;Substance 3D Assets&rbrack; Procure, selecione e baixe Ativos 3D diretamente no Painter
* &lbrack;Substance 3D Assets&rbrack;&lbrack;UI&rbrack; Novo painel
* &lbrack;Substance 3D Assets&rbrack; Mapas e materiais do ambiente de suporte
* &lbrack;Substance 3D Assets&rbrack; Permitir recarregar, navegar e abrir a pasta do local no novo painel do Substance 3D Assets
* &lbrack;Substance 3D Assets&rbrack; Adição de um gerenciador de downloads
* &lbrack;Recurso de texto&rbrack; Permitir o uso de fontes incorporáveis
* &lbrack;Recurso de texto&rbrack; Permite renderizar uma fonte/texto em uma malha
* &lbrack;Recurso de texto&rbrack; Exibe fontes do usuário e outros caminhos compartilhados no painel Ativos com uma nova categoria
* &lbrack;Recurso de texto&rbrack;&lbrack;Propriedades&rbrack; Adicionar suporte para propriedades avançadas de fontes
* &lbrack;Recurso de texto&rbrack; Permitir pesquisar/exibir fontes em minisprateleiras
* &lbrack;Recurso de texto&rbrack; Adicionar mensagem/caixa de diálogo de erro ao importar uma fonte incompatível
* Diversos
* &lbrack;Preencher projeção&rbrack; Melhorar o comportamento do manipulador de escala ao usar valores pequenos
* &lbrack;Manipuladores&rbrack; Adicionar novo modo preciso ao pressionar o atalho CTRL
* &lbrack;Manipuladores&rbrack; Melhorar a estabilidade do manipulador de superfície ao traduzir
* &lbrack;Export&brack; Adicionar o nome do espaço de cores nas saídas SBSAR
* &lbrack;Desempenho&rbrack; Melhorar o tempo de descoberta de bibliotecas de ativos em disco
* &lbrack;Substance&rbrack; Atualização para o mecanismo de Substance versão 9.1.2
* &lbrack;Arrastar e soltar&rbrack; Alinhar a rotação do decalque à câmera ao soltar no visor
* &lbrack;Python&rbrack; Edição da pilha de camadas
* &lbrack;Python&rbrack; Permite selecionar camada, efeito, máscara, máscara geográfica na interface
* &lbrack;Python&rbrack; Permitir obter/definir modos de mesclagem de camadas
* &lbrack;Python&rbrack; Permitir obter/definir configurações de projeção da camada de preenchimento
* &lbrack;Python&rbrack; Permitir a consulta da cor do material de Substance a partir de uma camada de preenchimento
* &lbrack;Python&rbrack; Permite consultar e definir cores uniformes e recursos em camadas e efeitos
* &lbrack;Python&rbrack; Permite criar e editar recursos de texto na pilha de camadas
* &lbrack;Python&rbrack; Permitir a edição de canais ativos em camadas e efeitos
* &lbrack;Python&rbrack; Permitir que as ações em lote tenham uma única operação de desfazer/refazer
* &lbrack;Python&rbrack; Permitir carregar/editar parâmetros de origem vetorial
* &lbrack;Python&rbrack; Permitir a edição de propriedades de cores de camadas e efeitos com o gerenciamento de cores
* &lbrack;Python&rbrack; Permite consultar e criar camadas instanciadas
* &lbrack;Python&rbrack; Permitir a adição do efeito de seleção de cor
* &lbrack;Python&rbrack; Permitir o controle do gerenciamento de cores de imagens de bitmap
* &lbrack;Python&rbrack; Permitir pausa/cancelamento de pausa do mecanismo
* &lbrack;Python&rbrack; Permite navegar para nós irmãos e pais
* &lbrack;Python&brack; Permitir criar efeito de filtro/gerador
* &lbrack;Python&rbrack; Permitir adicionar efeito de nível
* &lbrack;Python&rbrack; Permite adicionar máscara inteligente em uma camada
* &lbrack;Python&rbrack; Permitir criar/editar pontos de ancoragem
* &lbrack;Python&rbrack; Permitir obter/definir máscara em camadas
* &lbrack;Python&rbrack; Permitir criar efeito de máscara de comparação
* &lbrack;Python&rbrack; Permitir consultar e usar predefinições de recursos Substance
* &lbrack;Python&rbrack; Permite listar predefinições e seus valores por meio da função internal_properties para recursos Substance
* &lbrack;Python&rbrack; Permitir listar predefinições de exportação predefinidas
* &lbrack;Python&rbrack; Permitir listar predefinições de exportação disponíveis na biblioteca
* &lbrack;Python&rbrack; Permite recuperar o conteúdo das predefinições de exportação

**Corrigido**:

* &lbrack;Crash&rbrack; Desfazer “Remover instância de sombreamento” com Ctrl-Z
* &lbrack;Crash&rbrack; Criar uma camada em pilha vazia se a última seleção tiver sido um efeito
* &lbrack;SVG&rbrack; Problema com um valor personalizado da área recortada
* &lbrack;Contornar automaticamente; Recalcular apenas a embalagem sem qualquer alteração na orientação UV resulta em falha
* &lbrack;Arrastar e soltar&rbrack; Atraso devido a recursos externos são pré-carregados várias vezes
* &lbrack;UI&rbrack; Arrastar e soltar a miniatura do recurso pode ocultar a mensagem de aviso na pilha de camadas
* &lbrack;Performance&rbrack; Os blocos UV mascarados ainda são computados
* &lbrack;USD&rbrack; Realce incorreto para seleção de escopo
* &lbrack;Recurso&rbrack; A imagem de bitmap é corrompida após pintar no canal normal e salvar o projeto
* &lbrack;USD&rbrack; Suporte para ordenação de malha de vértice com a mão esquerda
* &lbrack;Substance&rbrack; Redefinir para padrão sempre voltar a zero para widget de ângulo
* &lbrack;Engine&brack; Pintar com um SVG em um estêncil não funciona
* &lbrack;Engine&brack; as pinceladas do Mapa normal se partem após uma ação de desfazer
* &lbrack;O gráfico para o Filtro Material do Content&brack; tem mesclagem alfa e espaço de cores incorretos
* &lbrack;Content&brack; Os modos de mesclagem no Tile Generator não estão funcionando
* O filtro de digitalização do histograma &lbrack;Content&brack; produz faixas em alguns casos
* &lbrack;Conteúdo&rbrack; iluminação Feita bake estilizada não leva em conta o height pintado
* &lbrack;Python&rbrack; Erro inesperado ao recuperar informações de camada da instância após alteração do sombreador
* &lbrack;Salvar&rbrack; O arquivo de projeto é perdido quando “salvar como” falha em casos específicos

**Problemas Conhecidos**:

* &lbrack;Gerenciamento de cores&rbrack; As conversões do espaço de cores HDR com ACE no Linux produzem cores fixas
* &lbrack;Crash&rbrack;&lbrack;Linux&rbrack;&lbrack;AMD&rbrack; Arrastar e soltar recursos em pilha de camadas no Wayland OS
* &lbrack;Regressão&rbrack;&lbrack;UI&rbrack; O Menu do Clique com o Botão Direito é muito pequeno em telas HD
* &lbrack;Crash&rbrack;&lbrack;Python&rbrack; Exportação de USD acionada por TextureStateEvent
* &lbrack;Save&rbrack; O arquivo de projeto Spp é perdido quando “salvar como cópia” falha em casos específicos
* &lbrack;MacOS Intel&rbrack; Falha ao importar algumas predefinições
* &lbrack;Illustrator&rbrack; Não é possível importar arquivos Ai após falha do servidor sem reiniciar o Painter
* &lbrack;Import&brack; Ativos com o mesmo nome, mas com diferentes extensões são substituídos

## Versão 9

### 9.1.2

Data de lançamento: **01/2024/30** Resumo: **versão secundária, correções de erros**

**Adicionado**:

* &lbrack;Desempenho&rbrack; Melhorar o tempo de criação da primeira camada de preenchimento em novos projetos
* &lbrack;Performance&rbrack; Reduz o tempo de carregamento de mapas de ambiente pesado
* &lbrack;Substance&rbrack; Permite salvar/fechar projetos mesmo quando miniaturas estão sendo geradas

**Corrigido**:

* A gravação falha em projetos de versões anteriores quando o visor é modificado
* &lbrack;Crash&rbrack; Reimportando malha ao usar o AO personalizado e o gerenciamento de cores
* &lbrack;Preencher projeção&rbrack; Clicar no manipulador de escala exibe a mensagem “não é possível pintar”
* &lbrack;Pincel&rbrack; Pintar com alinhamento UV causa artefatos
* &lbrack;Pilha de camadas&rbrack; A renomeação da camada é lenta quando a pilha é muito longa
* &lbrack;Pilha de camadas&rbrack; Mensagem de erro incorreta ao usar filtro incompatível na máscara
* &lbrack;Pilha de camadas&rbrack; A seleção volta para a camada superior após a exclusão
* &lbrack;Export&brack; A textura normal gerada está sempre no modo de preenchimento do vizinho de espaço 3D
* &lbrack;A Textura alfa do &rbrack; não é gerada com a predefinição Visualização 2D export
* &lbrack;Export&brack; a exportação de SBSAR tem usos incorretos com mapas convertidos
* &lbrack;Sombreador&rbrack; o registro de alterações do API de sombreamento não está atualizado com as alterações mais recentes do ASM

**Problemas Conhecidos**:

* &lbrack;Gerenciamento de cores&rbrack; As conversões do espaço de cores HDR com ACE no Linux produzem cores fixas
* &lbrack;Crash&rbrack;&lbrack;Linux&rbrack;&lbrack;AMD&rbrack; Arrastar e soltar recursos em pilha de camadas no Wayland OS
* &lbrack;Regressão&rbrack;&lbrack;UI&rbrack; O Menu do Clique com o Botão Direito é muito pequeno em telas HD
* &lbrack;Crash&rbrack;&lbrack;Python&rbrack; Exportação de USD acionada por TextureStateEvent

### 9.1.1

Data de lançamento: **2023/12/05** Resumo: **versão secundária, correções de erros e envio para a funcionalidade do After Effects**

**Adicionado:**

* &lbrack;Interop&rbrack; Permite enviar uma malha texturizada para o After Effects (Ae 24.1)

**Corrigido:**

* &lbrack;Fill&brack; UV definido para projeção de conjunto UV não lê mais de 2 conjuntos UV
* &lbrack;Crash&rbrack; Usando mapa de ambiente de 16K
* &lbrack;Crash&rbrack; Exr usado como entrada de imagem
* &lbrack;Crash&rbrack; Copiar e colar caminhos entre projetos
* &lbrack;QoL&rbrack; Arrastar e soltar o recurso Alpha no modo de decalque cria Projeção UV na máscara
* &lbrack;Caminho&rbrack; Copiar vértices de caminho também renomeia o caminho de destino ao reabrir o projeto
* &lbrack;Linux&rbrack; A escolha de cores pode ser interrompida com várias telas
* &lbrack;Auto Unwrap&brack; problema na interface do usuário para controle de densidade do texel
* O feedback da IU do &lbrack;Color Management&rbrack; é adequado para maiúsculas e minúsculas, mas o mecanismo não
* &lbrack;Gerenciamento de cores&rbrack; Seleção de espaço de cores incorreta na máscara com substituição de dados do usuário

**Problemas Conhecidos:**

* &lbrack;Gerenciamento de cores&rbrack; As conversões do espaço de cores HDR com ACE no Linux produzem cores fixas
* &lbrack;Crash&rbrack;&lbrack;Linux&rbrack; com Linux Wayland no AMD ao arrastar e soltar recursos na Pilha de camadas
* &lbrack;Crash&rbrack;&lbrack;Mac&rbrack; Alterando o valor da filtragem anisotrópica no sistema operacional Monterey
* &lbrack;Regressão&rbrack;&lbrack;UI&rbrack; O menu do botão direito é muito pequeno na tela hd
* &lbrack;Python&rbrack; Falha ao exportar USD acionada por TextureStateEvent

### 9.1.0

Data de lançamento: **2023/11/07** Resumo: **Versão principal que apresenta suporte a SVG e transparência, bem como melhorias na ferramenta de arrastar e soltar e no caminho**

**Adicionado:**

* &lbrack;SVG&rbrack; Permitir importação de arquivos vetoriais (SVG)
* &lbrack;SVG&rbrack;&lbrack;UI&rbrack; Adicionar suporte para propriedades específicas de SVG
* &lbrack;SVG&rbrack; Adicionar uma opção para preservar facilmente as proporções da imagem original
* &lbrack;SVG&rbrack; Permite usar automaticamente alfa de SVG com transparência
* &lbrack;Interop&rbrack; Permite enviar uma malha texturizada para o After Effects (Ae 24.1 beta)
* &lbrack;Interop&rbrack; Adicionar configurações de Enviar para o After Effects
* &lbrack;QoL&rbrack;&lbrack;Assets&rbrack;&lbrack;UI&rbrack; Importar ativo automaticamente ao arrastar e soltar no slot da interface
* &lbrack;QoL&rbrack; Permite arrastar e soltar ativos externos na pilha de camadas
* &lbrack;QoL&rbrack;&lbrack;Pilha de camadas&rbrack; Arraste e solte texturas do painel Ativos para a Pilha de camadas
* &lbrack;QoL&rbrack;&lbrack;Viewport&rbrack; Permitir arrastar e soltar o gerador, filtros na malha
* &lbrack;QoL&rbrack;&lbrack;Viewport&rbrack; Permitir soltar ativos externos na malha
* &lbrack;QoL&rbrack;&lbrack;Projeção&rbrack; Adicionar novo conjunto UV ao modo de projeção do conjunto UV
* &lbrack;QoL&rbrack; Arrastar e soltar Máscaras inteligentes como novas camadas no visor e na Pilha de camadas
* &lbrack;QoL&rbrack; Adicionar seletor para Geradores com múltiplas saídas quando usado em uma máscara
* &lbrack;QoL&rbrack; Permite arrastar e soltar imagens de canal único sobre um efeito de preenchimento
* &lbrack;QoL&rbrack;&lbrack;Pilha de camadas&rbrack; Use modificadores CTRL/ALT com arrastar e soltar para especificar onde/como criar efeitos/camada
* &lbrack;Caminho&rbrack; Alterna a visibilidade dos caminhos individualmente no painel de caminhos
* &lbrack;Caminho&rbrack; Permitir o uso de manipuladores de transformação para pontos de caminho
* &lbrack;Path&brack; Permite controlar manualmente tangentes por vértice
* &lbrack;Caminho&rbrack; Copiar/colar propriedades do caminho
* &lbrack;Caminho&rbrack; Introduzir um atalho vazio para o botão Quebrar tangente
* &lbrack;Sombreador&rbrack; Adicionar suporte para Opacidade e Translucidez no sombreador ASM
* &lbrack;Sombreador&rbrack; Adicionar suporte para canal de Cor de absorção com sombreador ASM
* &lbrack;Sombreador&rbrack; Melhorar dicas de ferramentas de parâmetros de sombreador do ASM
* &lbrack;Sombreador&rbrack; Alterar a cor padrão do canal de Translucidez para preto
* &lbrack;Configurações de exibição&rbrack; Ativar Suavização temporal por padrão
* &preto;Configurações de exibição&rbrack; Ativar configuração de dispersão abaixo da superfície por padrão
* &lbrack;Substance&rbrack; Adicionar suporte para a propriedade ColorSpace a partir da entrada/saída do gráfico
* &lbrack;Substance&rbrack; Atualize o mecanismo de Substance para a versão 9.0.3
* &lbrack;UI&rbrack; Torna o botão contextual da barra de ferramentas acessível mesmo se a janela do aplicativo for pequena
* &preto;Desempacotar automaticamente&rbrack; Controlar o número de Blocos UV com Densidade de texel
* &lbrack;Fazendo bake&rbrack; Desativar Rastreamento de raios do GPU em GPUs AMD por padrão
* &lbrack;Performance&rbrack; Aplicar compactação sem perdas em imagens de 16 bits para reduzir o espaço ocupado pelo projeto
* &lbrack;Python&rbrack; Permite manipular a Câmera padrão no Visualização 3D
* &lbrack;Python&rbrack; Expor a capacidade de exportar malha via script
* &lbrack;Content&rbrack;&lbrack;Amostras&rbrack; Adicionar novo projeto de amostra “Tabela de restaurantes franceses”
* &lbrack;Conteúdo&rbrack; Atualizar o logotipo do Substance alfa para a nova versão
* &lbrack;Content&brack; Adicionar três filtros de material focados em SVG (adesivo personalizado, spray personalizado e gráfico para o material)

**Corrigido:**

* &lbrack;Crash&rbrack; Alterar o tamanho do manipulador quando não estiver usando a ferramenta simetria
* &lbrack;Crash&rbrack; &lbrack;Pilha de camadas&rbrack; Criando camada quando nada estiver selecionado
* &lbrack;Projeto&rbrack; Mapas de malha podem ser corrompidos após a remoção de recursos não utilizados
* &lbrack;Projeto&rbrack; Corrupção de recurso após reimportar ou fazer bake imagem
* &lbrack;Assets&rbrack; Recarregar um ativo o remove de Favoritos
* &lbrack;Import&rbrack; Não é possível importar recursos quando “Nenhum resultado encontrado” no painel de ativos
* &lbrack;UI&rbrack; A seta da barra de ferramentas contextual não aparece em alguns casos
* &lbrack;Substance&rbrack; O botão lado a lado para valores booleanos não é suportado
* &lbrack;Level&rbrack; Rótulo de canal incorreto quando usado na máscara
* &lbrack;Export&rbrack;&lbrack;glTF&rbrack; os arquivos glTF/GLB exportados do Painter não têm uma unidade de tamanho físico
* &lbrack;Content&rbrack; A intensidade do filtro de Desfoque é fixada em 16
* &lbrack;Content&brack; A entrada da imagem do filtro de Correspondência de Cores “cor de destino” não está visível

**Problemas conhecidos:**

* &lbrack;Gerenciamento de cores&rbrack; As conversões do espaço de cores HDR com ACE no Linux produzem cores fixas
* &lbrack;Crash&rbrack;&lbrack;Linux&rbrack; com Linux Wayland no AMD ao arrastar e soltar recursos na Pilha de camadas
* &lbrack;Crash&rbrack;&lbrack;Mac&rbrack; Alterando o valor da filtragem anisotrópica no sistema operacional Monterey
* &lbrack;Crash&rbrack; Exr usado como entrada de imagem
* &lbrack;Crash&rbrack; Usando mapa de ambiente de 16K
* &lbrack;Auto Unwrap&brack; problema na interface do usuário para controle de densidade do texel
* &lbrack;Regressão&rbrack;&lbrack;UI&rbrack; O menu do botão direito é muito pequeno na tela hd
* &lbrack;Python&rbrack; Falha ao exportar USD acionada por TextureStateEvent
* &lbrack;QoL&rbrack; Arrastar e soltar o recurso Alpha no modo de decalque cria Projeção UV na máscara

### 9.0.1

Data de lançamento: **09/2023/19** Resumo: **Versão de correção de bug secundária com várias melhorias**

**Adicionado:**

* &lbrack;Import&rbrack; Definir local de importação padrão na janela de importação
* &lbrack;Modo de Fça bake&rbrack; Permite redefinir parâmetros para seus valores padrão
* &lbrack;Fazendo bake&rbrack; Define o fça bake com resolução de tinta ao criar um projeto
* &lbrack;Simetria&rbrack; Desvincular manipulador específico de simetria do atalho Q
* &lbrack;Menu&rbrack; Adicionar opção “mostrar registro” no menu Ajuda
* &preto;Visor&rbrack; Melhorar a velocidade de renderização da sombra
* &lbrack;Substance&rbrack; Atualize o mecanismo para a versão 9.0.1
* O arquivo de configuração OCIO do &lbrack;Color Management&rbrack; pode ter qualquer tipo de extensão
* &lbrack;Assets&rbrack; O recurso Sbsar com o uso de “decalque” deve ser definido automaticamente para distorcer a projeção
* &lbrack;Caminho&rbrack; Exibir uma mensagem ao tentar interagir com a ferramenta Caminho enquanto a interface do usuário e os Gizmos estiverem ocultos

**Corrigido:**

* &lbrack;Crash&rbrack; Alt + Arrastar no painel Caminho
* &lbrack;Importar Recursos&rbrack; Falha aleatória ao remover recursos para importar
* Falha ao importar um arquivo GLB compactado
* Problema ao pintar em malhas que compartilham UVs
* Flash de malha preto ao recalcular ou carregar cache
* &lbrack;Propriedades&rbrack; O menu do botão direito do mouse para redefinir parâmetros não aparece nas listas suspensas
* &lbrack;Nível&rbrack; Controles deslizantes de entrada bloqueados pelo nível anterior
* &lbrack;AMD&rbrack;&lbrack;Esparsa&rbrack; opção SVT se ativada gera artefatos
* &lbrack;Projeção&rbrack;&lbrack;Distorcer&rbrack; Falha ao clicar duas vezes nos vértices
* &lbrack;Caminho&rbrack; UI e caminho visíveis no modo de fça bake
* &lbrack;AMD&rbrack; Textura perdida ao brincar com a visibilidade
* &lbrack;Sparse&brack; Resolução muito baixa ao girar a malha

**Problemas Conhecidos:**

* &lbrack;Gerenciamento de cores&rbrack; As conversões do espaço de cores HDR com ACE no Linux produzem cores fixas

### 9.0.0

Data de lançamento: **2023/06/20** Resumo: **Versão principal com Tinta ao longo de um caminho que permite curvas 3D, novos materiais de base e limpeza de materiais herdados e novas predefinições para curvas 3D**

**Adicionado:**

* &lbrack;Caminho&rbrack; Adicionar nova Tinta ao longo da ferramenta Caminho
* &lbrack;Caminho&rbrack; Adiciona um atalho vazio para a ferramenta de caminho
* &lbrack;Caminho&rbrack; Permite adicionar novos pontos a um caminho existente
* &lbrack;Caminho&rbrack; Adicionar atalho para sair da criação do caminho atual
* &lbrack;Caminho&rbrack; Permitir a edição de propriedades de pincéis para caminhos
* &lbrack;Caminho&rbrack; Ajusta tangentes automaticamente ao posicionar um ponto
* &lbrack;Caminho&rbrack; Recalcular tangentes quando um ponto for movido
* &lbrack;Caminho&rbrack; Ajustar pontos recém-criados à superfície de uma malha
* &lbrack;Caminho&rbrack; Permite editar a pressão por vértice
* &lbrack;Caminho&rbrack; Ajusta a pressão do ponto recém-criado a partir de pontos vizinhos
* &lbrack;Caminho&rbrack; Permite converter pontos para suavizar/canto (quebra tangente)
* &lbrack;Caminho&rbrack; Permite mover um ponto recém-adicionado imediatamente
* &lbrack;Caminho&rbrack; Permite remover pontos do caminho existente
* &lbrack;Caminho&rbrack; Permite inverter a direção de um caminho
* &lbrack;Caminho&rbrack; Permite selecionar um caminho no visor
* &lbrack;Caminho&rbrack; Permite selecionar pontos do caminho com seleção de letreiro
* &lbrack;Caminho&rbrack; Introduza os atalhos CTRL-A para selecionar todos os pontos de um caminho
* &lbrack;Caminho&rbrack; Permitir fechar caminho
* &lbrack;Caminho&rbrack; Permite especificar o caminho até o eixo em Propriedades
* &lbrack;Caminho&rbrack; Adiciona um menu de controle de vértice à barra de ferramentas contextual
* &lbrack;Caminho&rbrack; Introduzir modos de tinta/apagar/borrar na ferramenta de caminho
* &lbrack;Caminho&rbrack; Criar feedback visual para os caminhos no visor
* &lbrack;Caminho&rbrack; Adicionar um indicador visual para a direção do caminho
* &lbrack;Caminho&rbrack; Adicionar thickness de linha às configurações de exibição do caminho
* &lbrack;Caminho&rbrack; Permitir ocultar caminhos UI
* &lbrack;Caminho&rbrack; Adicionar painel Caminho para listar os caminhos da camada atualmente selecionada
* &lbrack;Caminho&rbrack; Adicionar feedback visual ao passar o mouse sobre um caminho no painel Caminho
* &lbrack;Caminho&rbrack; Exibir painel de caminho sempre que a ferramenta Caminho for selecionada
* &lbrack;Caminho&rbrack; Permite renomear, excluir, copiar, recortar, duplicar caminho no painel Caminho
* &lbrack;Caminho&rbrack; Exibir mensagem ao tentar interagir no visor 2D com a ferramenta Caminho
* &lbrack;Biblioteca&rbrack; Integrar novo conteúdo (ferramentas e materiais de base de caminho)
* &lbrack;Traçados dinâmicos&rbrack; Adicionar propriedade de distância para traçados dinâmicos
* &lbrack;Traçados dinâmicos&rbrack; Adicionar propriedades de tamanho e espaçamento aos traçados dinâmicos
* &lbrack;Traçados dinâmicos&rbrack; Adicionar propriedade início/meio/fim para traçados dinâmicos
* &lbrack;Python&rbrack;&lbrack;USD&rbrack; Expor os parâmetros de configuração do projeto para o formato USD
* &lbrack;Python&rbrack;&lbrack;USD&rbrack; Expor os parâmetros de criação do projeto para o formato USD
* &lbrack;Export&rbrack;&lbrack;USD&rbrack; Adicionar informações de caminho do projeto no arquivo USD exportado
* &lbrack;GLTF&rbrack; Atualiza texturas na biblioteca ao recarregar um arquivo GLTF
* &lbrack;Sombreador&rbrack; Reduzir artefatos de costura para Ilhas UV com orientação diferente
* &lbrack;Engine&rbrack; Atualização para o mecanismo Substance versão 9.0

**Corrigido:**

* &lbrack;Import&rbrack; Algumas GLB com texturas não obtêm texturas no Painter
* &lbrack;AMD&rbrack; Artefatos em bordas para todos os preenchimentos de projeção 3D
* &lbrack;As Texturas do motor&rbrack; são interrompidas ao alternar a visibilidade da camada
* &lbrack;Engine&rbrack; as Texturas estão vazias em alguns locais ao alterar o modo de mesclagem
* &lbrack;Motor&rbrack; Textura/Projeção é um modo de distorção vazio em alguns casos
* &lbrack;Iray&rbrack; a Iteração é redefinida para 0 ao salvar a renderização
* &lbrack;Log&brack; mensagem de erro de USD ao executar Arquivo > Novo

**Problemas Conhecidos:**

* &lbrack;Gerenciamento de cores&rbrack; As conversões do espaço de cores HDR com ACE no Linux produzem cores fixas
* &lbrack;Pilha de camadas&rbrack; Fonte de entrada não salva por camada

## Versão 8

### 8.3.1

Data de lançamento: **2023/04/27**

**Adicionado:**

* &lbrack;Modo de Fça bake&rbrack; Adicionar atalho (vazio) para mostrar/ocultar a visualização do visor
* &lbrack;Modo de Fça bake&rbrack; Sempre mostrar Low Poly ao usar o botão “Ocultar malhas de fça bake”
* &preto;Modo de Fça bake&rbrack; Mostrar sufixo para correspondência por nome com base no conjunto de texturas atual
* &lbrack;Import&rbrack; Adicionar suporte para arquivos binários GLTF (glb)
* &preto;Lista do conjunto de texturas&rbrack; Adicionar menu para selecionar ou criar instâncias de sombreamento
* &preto;Lista do conjunto de texturas&rbrack; Permite alterar rapidamente o conjunto de texturas e a resolução do Bloco UV
* &lbrack;Tamanho físico&rbrack; Melhorar o comportamento do manipulador ao usar tamanho físico na Projeção UV
* &lbrack;UI&rbrack; Trazer de volta &#39;Salvar como&#39; para o menu Arquivo principal
* &lbrack;UI&rbrack; Salvar seleção de visualização (somente 2D, somente 3D, ambos) no layout da interface
* &lbrack;USD&rbrack; Mensagem de erro menos vaga na criação do projeto com formas de USD não suportadas
* &lbrack;Python&rbrack; Adicionar eventos de fça bake para seguir o progresso de Fça bake
* &lbrack;Python&rbrack; Permitir cancelamento de um faço bake
* &lbrack;Python&rbrack; Expor &#39;Baseado no modelo de saída&#39; para Tipo de Arquivo e Profundidade de bits na exportação
* &lbrack;Python&rbrack; Expor tempo de atualização para TextureStateEvent.Update

**Corrigido:**

* &lbrack;Falha&rbrack; Falha rara ao fechar um projeto
* &lbrack;Crash&rbrack; &lbrack;Fazendo bake&rbrack; Ativa a sincronização do mapa de malha com Height ou curvatura em um projeto específico
* &lbrack;Crash&rbrack;&lbrack;Scripting&rbrack; Falha ao adicionar um material após a criação da instância de sombreamento
* &lbrack;Modo de Fça bake&rbrack; A intensidade do AO em material neutro não tem efeito
* &lbrack;Modo de Fça bake&rbrack; Falha ao alternar para o modo de fça bake antes do modelo ser carregado
* &lbrack;Modo de Fça bake&rbrack; Mensagem de erro ausente na guia Processo de Fça bake
* &lbrack;Modo de Fça bake&rbrack; As configurações de materiais neutros não têm efeito após a reimportação de uma malha
* &lbrack;Modo de Fça bake&rbrack; O separador de Janela é salvo globalmente e não por modo
* &lbrack;Modo de Fça bake&rbrack; Problema de visualização: o normal médio não altera a superfície da caixa
* &lbrack;Gerenciamento de cores&rbrack; A configuração de detecção automática de espaço de cores está desativada quando a variável de ambiente OCIO está presente
* &lbrack;O filtro Contorno da Máscara do Content&brack; possui artefato com entrada de height
* O controle deslizante de intensidade do filtro de desfoque de Inclinação do &lbrack;Content&rbrack; está fixado em 1.0
* &lbrack;Interop&rbrack; Não é possível criar projetos com GLTF a partir do Sampler
* &lbrack;Pilha de camadas&rbrack; O valor da divisão em blocos gráficos da projeção não é atualizado corretamente com o manipulador
* &lbrack;Linux&rbrack; Deslocamento entre a caneta eletrônica gráfica e o cursor com HDPI maior que 100%
* &lbrack;Python&rbrack; Falha ao reimportar uma malha após criar um projeto
* &lbrack;Substance&rbrack; os ruídos 3D são quebrados após a reimportação de uma malha
* &lbrack;Blocos UV&rbrack; O deslocamento da Projeção UV é fixado em 1
* O feedback visual em &preto;Visor&rbrack; linhas retas não está mais visível
* &lbrack;WhatsNew&rbrack; Retorno de linha incorreto em títulos de recurso

**Problemas Conhecidos:**

* &lbrack;Import&rbrack; Algumas GLB com texturas não obtêm texturas no Painter

### 8.3.0

*(Lançado: 10 de janeiro de 2023*)Resumo: **Versão principal com novo modo de fça bake, nova importação e exportação de arquivos USD e suporte a tamanho físico para Projeção UV**

**Adicionado:**

* &lbrack;Modo de Fça bake&rbrack; Novo modo de fça bake dedicado ao processo de fça bake

* &lbrack;Modo de Fça bake&rbrack; Define o atalho para alternar para o modo de fça bake para F8

* &lbrack;Modo de Fça bake&rbrack; Adiciona os botões Iniciar e Cancelar fça bake no visor

* &preto;Modo de Fça bake&rbrack; Adicionar seleção de fça bake na lista Conjunto de Texturas

* &lbrack;Modo de Fça bake&rbrack; Adicionar nova janela de Baker do Mapa de Malha para selecionar baker

* &lbrack;Modo de Fça bake&rbrack; Adicionar nova janela Configurações do Mapa de Malha para editar as configurações de fça bake

* &lbrack;Modo de Fça bake&rbrack; Adicionar nova janela de Log de Fça bake para seguir o processo de fça bake

* &lbrack;Modo de Fça bake&rbrack; Adicionar parâmetros de fça bake e desfazer ações na janela de histórico

* &lbrack;Modo de Fça bake&rbrack; Adicionar trilhas nas Configurações do Mapa de Malha

* &lbrack;Modo de Fça bake&rbrack; Adicionar miniaturas de mapas de malha na janela Baker de mapas de malha

* &lbrack;Modo de Fça bake&rbrack; Adicionar menu recolhível de configurações de visualização na janela de visualização 3D

* &lbrack;Modo de Fça bake&rbrack; Adicionar configuração de visualização para mostrar/ocultar a malha de alto polígono

* &lbrack;Modo de Fça bake&rbrack; Adicionar configuração de visualização para mostrar/ocultar a malha do compartimento e o wireframe

* &lbrack;Modo de Fça bake&rbrack; Adicionar configuração de visualização para mostrar/ocultar a malha de baixa poli

* &preto;Modo de Fça bake&rbrack; Adicionar configuração de visualização para mostrar as bordas sólidas sem emendas UV como erros

* &lbrack;Modo de Fça bake&rbrack; Informar no visor sobre a malha e fazer bake erros se o Log de Fça bake não estiver visível

* &preto;Modo de Fça bake&rbrack; Adicionar ação para sincronizar as configurações de baker em todos os Conjuntos de Textura

  Na janela Baker do mapa de malha, cada baker (bem como as configurações comuns) pode ser sincronizado entre os conjuntos de textura clicando no ícone de link ao lado de seu nome. Esta ação abrirá uma janela que permite selecionar quais conjuntos de texturas compartilharão os mesmos parâmetros.

* &preto;Modo de Fça bake&rbrack; Adicionar ações para copiar e colar configurações de baker

  Na janela Baker do Mapa de malha estão disponíveis ações para copiar e colar cada configuração de baker nos Conjuntos de textura por meio do menu dedicado na parte superior da janela ou do menu contextual do botão direito do mouse.

* &lbrack;Modo de Fça bake&rbrack; Adicionar botão ao Fazer bake Log para saltar do erro para as configurações corretas

  Quando um baker falha ou uma malha não é carregada corretamente, uma mensagem de erro aparece no registro de Fça bake. Um botão ao lado da mensagem permite alterar a janela Baker do mapa de malha e Configurações do mapa de malha para mostrar as configurações relacionadas. Isso ajuda a isolar com mais facilidade a origem de um problema para corrigi-lo.

* &Preenchimento;Modo de Fça bake&rbrack; Adiciona menus para gerenciar Conjuntos de Texturas e seleções de Baker

  Tanto na lista “Texture Set” quanto na janela “Mesh Map Baker” foi adicionado um pequeno menu de ação para ajudar a copiar e inverter seleções.

* &lbrack;Modo de Fça bake&rbrack; Dividir lista de seleção de baker por Conjunto de Textura

* &preto;Modo de Fça bake&rbrack; Dividir configurações comuns por Conjunto de Textura

* &lbrack;Modo de Fça bake&rbrack; Carregue malhas de alto-polígono e em gaiola sem congelar a interface

* &lbrack;Modo de Fça bake&rbrack; Use a barra de progresso do visor para mostrar o carregamento da malha

* &lbrack;Modo de Fça bake&rbrack; Adicionar estado de carregamento de malha no Log de Fça bake

* &lbrack;Modo de Fça bake&rbrack; Permite virar a malha no visor durante a faz bake

* &lbrack;Modo de Fça bake&rbrack; Definir ordem de fça bake com base na visibilidade atual do visor da malha

* &lbrack;Modo de Fça bake&rbrack; Exibir gaiola de fça bake implícita no visor

  Se não estiver usando um arquivo de malha de gaiola personalizado, uma malha de gaiola automática será gerada e exibida na janela de visualização. Seu tamanho será baseado no parâmetro Distância frontal máxima das configurações comuns de fça bake. A malha de gaiola é usada para indicar até onde a correspondência entre o poli baixo e alto irá.

* &lbrack;Modo de Fça bake&rbrack; Mostrar lista correspondente de nomes de malha para Correspondência por Nome no Log de Fça bake

* &lbrack;Modo de Fça bake&rbrack; Usar material neutro para exibir modelo 3D no visor

* &lbrack;Modo de Fça bake&rbrack; Desativa o cálculo do motor no modo de fça bake

* &lbrack;Modo de Fça bake&rbrack; Exibir um aviso ao sair do aplicativo enquanto um faço bake estiver em andamento

* &lbrack;Baker&rbrack; Atualizar rótulos de configuração de suavização de serrilhado

  Os valores de configuração de suavização de borda foram renomeados para “Sobreamostragem” e com um número multiplicador explícito para esclarecer seu comportamento.

* &lbrack;Baker&rbrack; Atualize os baker para a versão 2.5.7.

* &lbrack;USD&rbrack; Importar e exportar arquivos de Universal Scene Description (USD)

* &lbrack;USD&rbrack; Adiciona opções de USD à janela Novo Projeto ao selecionar um arquivo USD

* &lbrack;USD&rbrack; Adicionar nova janela de seleção de Escopo e Variantes

  Ao importar um arquivo USD, clicar no botão de alteração na janela Novo projeto ou Configuração do projeto permite selecionar qual parte e variantes de um arquivo USD importar.

* &lbrack;USD&rbrack; Adicionar opções de níveis de subdivisão

  Ao criar um novo projeto com um arquivo de malha USD que contém subdivisões, é possível selecionar o nível de subdivisões usando um controle deslizante. O projeto será criado com a malha subdividida. O nível pode ser modificador por meio da Configuração do projeto.

* &lbrack;USD&rbrack; Importar malhas com pele USD em um quadro específico

  Ao criar um novo projeto com um arquivo de malha USD que contém animação, é possível selecionar a quadro usando um controle deslizante que reflete a sequência de linha do tempo incorporada. O quadro pode ser modificador por meio da Configuração do projeto.

* &lbrack;USD&rbrack;&lbrack;Export&rbrack; Adicionar uma opção para exportar arquivos USD

  Nova caixa de seleção Exportar USD adicionada à janela Exportar textura. Quando marcada, permite exportar arquivos USD, bem como mapas de textura usando qualquer modelo.

* &lbrack;USD&rbrack;&lbrack;Exportar&rbrack; Adicionar formato de arquivo USD à exportação em malha

* &lbrack;USD&rbrack; Renomeie a predefinição de exportação “USD PBR Metal Roughness” existente para ser mais explícita

  O modelo de exportação de USD anteriormente conhecido como &#39;USD PBR Metal Roughness&#39; ainda é acessível por meio de texturas de exportação > Modelo de saída > USDz (Apple AR).

* &presilha;Desenvolver presilha automaticamente&rbrack; Adicionar orientação de bloqueio para embalagem

  Nova opção para configurações de abertura automática que permitem preservar a orientação de Ilhas UV existentes ao usar o recurso de embalagem. Ele pode ser acessado em Novo projeto > Opções de Contornar automaticamente > Orientação da Ilha UV.

* &lbrack;Tamanho físico&rbrack; Adicionar configuração para usar automaticamente Tamanho físico no efeito/camada de preenchimento

  Foi adicionada uma nova opção para alternar automaticamente para a escala de tamanho físico ao usar um material com tamanho físico incorporado. Ele pode ser ativado por projeto por meio de Novo projeto ou de Editar > Configuração do projeto > Tamanho físico > Alternar o dimensionamento da camada de preenchimento para Tamanho físico ao atribuir materiais.

* &lbrack;Tamanho físico&rbrack; Expor tamanho físico para Projeção UV

  O dimensionamento de tamanhos físicos agora está disponível para Projeção UV. Ele ativa o redimensionamento automático de um material com base no tamanho físico de uma malha. Pode ser selecionado por meio de Escala > Tamanho físico na janela Propriedades da camada de preenchimento ou do efeito.

* &lbrack;Scripting&rbrack;&lbrack;Python&rbrack; Permitir consultar a versão do aplicativo

* &lbrack;Scripting&rbrack;&lbrack;JavaScript&rbrack; Atualizar API para corresponder aos novos parâmetros de fça bake

* &lbrack;Scripting&rbrack;&lbrack;Python&rbrack; Fazendo bake módulo: editar parâmetros de fça bake

* &lbrack;Scripting&rbrack;&lbrack;Python&rbrack; Fazendo bake módulo: iniciar/cancelar fça bake

* &lbrack;Scripting&rbrack;&lbrack;Python&rbrack; Fazendo bake módulo: selecione o método de curvatura

* &lbrack;Scripting&rbrack;&lbrack;Python&rbrack; Fazendo bake módulo: seleção de baker/blocos uv

* &lbrack;Scripting&rbrack;&lbrack;Python&rbrack; módulo de Fça bake: sincronizar as configurações de baker em todos os Conjuntos de texturas

* &lbrack;SVT&rbrack; Ativar suporte a hardware esparso em GPUs AMD

  A aceleração de hardware para o sistema de texturas virtuais esparsas agora pode ser ativada com as GPUs da AMD. Essa configuração é ativada automaticamente nas preferências gerais.

* &lbrack;Projeção&rbrack; Renomear parâmetros de projeção cilíndrica

  O parâmetro “Cylinder Cap Culling” foi renomeado para “Backface Culling” para melhor representar sua ação. A dica de ferramenta associada foi ajustada de acordo.

* &lbrack;Projeto&rbrack; Salva a versão do aplicativo no projeto e recupera-a através de scripts

  Desde a versão 8.2, a versão do aplicativo agora é armazenada dentro do arquivo spp ao salvar. Este número de versão pode ser recuperado com a função last_saved_substance_painter_version() no módulo do projeto da API Python. Para projetos feitos antes de 8.2, o valor retornado será nulo.

* &lbrack;Import&brack; Melhorar tempo de importação geral de modelos 3D

  Melhoramos o tempo geral de importação das malhas. Por exemplo, reduzir o tempo de espera ao carregar malhas de alto polígono para fazer bake. Esta otimização aplica-se em particular ao carregamento de arquivos OBJ.

**Corrigido:**

* &lbrack;Crash&rbrack; Alterar canais no filtro com pilha específica

* &lbrack;Mac&rbrack;&lbrack;M1&rbrack; Falha ao criar uma camada de preenchimento e sair da pilha de camadas

  Esse problema pode ser corrigido atualizando para o Mac OS 13 (Ventura).

* &lbrack;Scripting&rbrack;&lbrack;Python&rbrack; Falha ao usar ui.add_dock_widget() com o tipo errado

* &lbrack;Fazendo bake&rbrack; Mensagem de erro incompleta no registro quando um faço bake falha

* &lbrack;Fazendo bake&rbrack; A memória não é liberada quando a faz bake é concluída

* &lbrack;O cache de Textura do Engine&rbrack; não é atualizado ao alterar a visibilidade do efeito

* &lbrack;Exportar&rbrack; Visualização 2D exportações aleatoriamente mapa uniforme

* &lbrack;Projeto&rbrack; Erro de alocação de memória ao salvar o projeto com malha grande

* &lbrack;Viewport&rbrack; TAA causa artefatos ao pintar em alguns casos

**Problemas Conhecidos:**

* &lbrack;Gerenciamento de cores&rbrack; As conversões do espaço de cores HDR com ACE no Linux produzem cores fixas
* &lbrack;Pilha de camadas&rbrack; Fonte de entrada não salva por camada

### 8.2.0

*(Lançado em: 06 de outubro de 2022*)Resumo: **Versão principal com novos painéis de integração (novo painel de boas-vindas e novo painel), exportação para SBSAR, efeitos para pasta, várias melhorias na qualidade de vida e correções de erros.**

**Adicionado:**

* &lbrack;Integração&rbrack; Painel de integração para acolher novos usuários

  Adicionada uma nova tela de boas-vindas quando novos usuários da CC abrem o Painter pela primeira vez.

* &lbrack;Integração&rbrack; Painel de novidades para aprimorar a capacidade de descoberta de novos recursos

  Adicionada uma nova tela Novidades que exibe os novos recursos principais. Ele é exibido automaticamente na primeira vez que o Painter é aberto após uma atualização importante e pode ser acessado novamente em Ajuda > Novidades.

* &lbrack;Integração&rbrack; Renomear antigo Bem-vindo à “Tela inicial”

  A tela de boas-vindas antiga foi renomeada para Tela inicial para evitar confusões com a nova tela de boas-vindas.

* &lbrack;UI&rbrack; Resolver problemas de dimensionamento para telas de DPI alto

  Adaptação aprimorada da interface do Painter em telas de alta definição com dimensionamento de exibição personalizado.

* &lbrack;UI&rbrack; Evitar mensagens de erro persistentes na interface

  As mensagens de erro de projetos anteriores agora são removidas da barra de status inferior.

* &lbrack;UI&rbrack; Menu de salvamento de retrabalho

  Opções adicionais de salvamento agora estão agrupadas em um submenu e algumas são renomeadas para fins de consistência.

* &lbrack;UI&rbrack; Salvar e exportar/compartilhar layouts de interface

  Dentro do menu Janela existem novas ações para salvar o layout da interface em arquivos e recarregá-los. Os layouts de Pintura e Renderização são salvos separadamente. Várias funções foram adicionadas a “substance_painter.ui” para salvar, redefinir e carregar os layouts de interface também.

* Adicionar ações de copiar/colar para modos de mesclagem/opacidade de uma camada

  Adicionada uma nova entrada “Opções de mesclagem” no menu de contexto camadas. Permite copiar e colar o modo de mesclagem e a opacidade de todos os canais de uma camada para outra.

* Aplicar modo de mesclagem/opacidade a todos os canais de uma camada

  Adicionada a funcionalidade de clicar com o botão direito do mouse ao modo de mesclagem de camadas e à opacidade, que permite aplicar a configuração atualmente clicada a todos os canais.

* Recarregar malha com um atalho de teclado (CTRL+SHIFT+R)

  Foi adicionado um atalho editável para recarregar o arquivo de malha com as últimas configurações disponíveis. Também pode ser acessada em Editar > Reimportar malha.

* Redefinir parâmetros de Substance para padrão

  Adicionado um novo botão em Propriedades na parte inferior dos recursos .sbsar que permite redefinir o recurso para padrão.

* Redefinir pincel de tinta para padrão

  Adicionado um novo menu à seção Pincel em Propriedades, o que permite redefinir para o pincel básico padrão.

* Clique com o botão direito do mouse para redefinir os parâmetros de Substance individuais como padrão

  Foi adicionada a possibilidade de redefinir parâmetros individuais em um recurso .sbsar com o botão direito do mouse.

* &lbrack;Painel de ativos&rbrack; “Fixar” de ativos favoritos para aparecerem sobre o painel de ativos

  Adição de uma nova opção de clicar com o botão direito em ativos da biblioteca que permite fixar-los como favoritos para a parte superior do painel. Você também pode exibir todos os seus ativos favoritos em Pesquisas salvas.

* &lbrack;Painel Ativos&rbrack; Excluir, recarregar e renomear ativos

  Adicionadas as opções do menu de contexto para excluir, recarregar e renomear ativos na biblioteca do usuário. Eles são excluídos diretamente do local da biblioteca no disco e recarregados do local original. Os ativos que fazem parte de um pacote como .abr ou .sbsar não podem ser editados individualmente.

* &preto;Seleção de cores&rbrack; Adicionar modos de mesclagem ao efeito Seleção de cores

* &lbrack;Pilha de camadas&rbrack; Adicionar modo de mesclagem e opacidade em filtros

* &lbrack;Pilha de camadas&rbrack; Permitir valores de divisão em blocos maiores que 128 para camada/efeitos de preenchimento

* &lbrack;Pilha de camadas&rbrack; Tampas de cilindro para projeção cilíndrica em camada/efeito de preenchimento

  A projeção cilíndrica nas propriedades da camada de preenchimento agora tem a opção de remover as tampas dos cilindros.

* &lbrack;Log&brack; Mostra uma mensagem de erro se as partes da malha estiverem em espaço negativo ao tentar criar um projeto de Bloco UV

  Adicionada uma mensagem de erro mais clara ao falhar ao criar um projeto de Bloco UV porque as partes UV são encontradas em espaços negativos.

* &lbrack;Projeto&rbrack; Indica a versão na mensagem de erro “dados muito recentes” ao abrir um projeto

  Ao abrir um projeto que é muito recente para o aplicativo, a mensagem de erro agora indicará a versão do projeto para facilitar a identificação da versão correta do aplicativo.

* &lbrack;Viewport&rbrack; Permitir a iluminação da malha por baixo

  Foi adicionado um novo parâmetro de Alinhamento de ambiente em Configurações de exibição > Câmera > Configurações de ambiente para alinhar a iluminação do mapa de ambiente à câmera quando definida como “Local”.

* &lbrack;Visor&rbrack; Visualizar R, G, B e Alpha no visor (modo de exibição solo)

  Em Configurações de exibição > Configurações do visor > Exibição de canal, há uma nova configuração de Canais de cores que permite exibir apenas o componente R, G, B ou Alpha de um canal quando estiver no modo de exibição única.

* &lbrack;Sombreador&rbrack; Permite definir canais do usuário como RGBA em sombreadores de camadas de material

  Ao definir a configuração dos canais do Conjunto de texturas dentro de um sombreador para camadas de material, agora é possível especificar o formato do canal para se desviar do valor padrão. Isso permite solicitar canais de usuário coloridos em vez de somente tons de cinza.

* &lbrack;Export&brack; Permitir exportação de texturas como SBSAR

  Ao exportar o textura pela janela Arquivo > Exportar Textura, o formato de arquivo SBSAR (Arquivo Substance) pode ser escolhido para reagrupá-los. O conteúdo do SBSAR é orientado pelo modelo de saída usado. O formato de arquivo SBSAR também pode ser definido nas predefinições de exportação. Ao usar configurações híbridas (SBSAR + outro formato), as texturas direcionadas a um SBSAR são agrupadas enquanto o restante é exportado junto com ele.

* &lbrack;Export&brack; Expor opção de 16 bits para o formato de arquivo EXR

  Ao exportar arquivos de textura EXR, agora é possível escolher 16f bits (meia Precisão decimal) ou 32f bits (Precisão decimal) na janela Exportar Textura (para configurações de exportação e predefinições de exportação). Projetos antigos e predefinições de exportação antigas terão o bit 16f como padrão para refletir o comportamento antigo.

* &lbrack;Python&rbrack; Adicionar evento para saber quando os Conjuntos de Texturas são modificados

  O novo “substance_painter.event.TextureStateEvent” permite saber quando um conjunto de texturas foi modificado por causa de um traçado de tinta, um novo canal adicionado ou um canal removido.

* &lbrack;Python&rbrack; Permite obter e definir recursos de Mapa de malha nas configurações do Conjunto de texturas

  Novas funções foram adicionadas ao módulo “substance_painter.project” para obter e definir recursos de mapas de malha. Essas funções podem ser usadas para atualizar os mapas de malha referenciados pelas configurações do Conjunto de texturas.

* &Brack;Plug-ins&rbrack; Remover opção para obter outros plug-ins JS

  Remoção da opção para obter plug-ins JavaScript, pois eles estavam hospedados no site de compartilhamento obsoleto.

* &lbrack;Content&rbrack; Adicionar novo modelo Roblox e exportar predefinição

  Um novo modelo de projeto e predefinição de exportação Roblox “Material Variant” e “Surface Appearance” foram adicionados para facilitar a exportação de texturas PBR para Roblox. O modelo pode ser acessado pela janela Arquivo > Novo projeto.

* Atualize o Substance Engine para a última versão (8.6.3)

* &lbrack;Steam&brack; Compilação otimizada para o chipset Apple Silicon (Apple M1 / M2)

**Corrigido:**

* Falha ao usar exr 16k

* &lbrack;Crash&rbrack; Ctrl Z Depois de excluir uma instância de sombreamento

* &lbrack;Iray&rbrack; IoR está bloqueada em 1 para alguns sombreadores

* &lbrack;Win&rbrack;&lbrack;Fazendo bake&rbrack; Alguns alto-polígonos falham ao carregar

* &lbrack;Gerenciamento de cores&rbrack; Nome do espaço de cores incorreto na interface do usuário com filtros

* &lbrack;Python&rbrack; Os objetos de recursos retornados pela função de importação não têm um tipo

  Ao importar um pacote Substance em Python, a função estava retornando o pacote em vez de seu(s) gráfico(s). O módulo de recursos agora fornece funções e parâmetros para recuperar o(s) gráfico(s) de um pacote de Substance.

**Problemas Conhecidos:**

* &lbrack;Gerenciamento de cores&rbrack; As conversões do espaço de cores HDR com ACE no Linux produzem cores fixas
* &lbrack;Pilha de camadas&rbrack; Fonte de entrada não salva por camada
* &preto;Pintura&rbrack; A suavização temporal causa artefatos ao pintar em alguns casos
* &lbrack;Exportar&rbrack; Visualização 2D exportações aleatoriamente mapa uniforme

### 8.1.3

*(Lançado: 25 de agosto de 2022*)Resumo: **Versão de correção de erro secundária**

**Adicionado:**

* Atualização para o Iray SDK 1.6

**Corrigido:**

* &lbrack;Sombreador&rbrack; Falha com sombreador antigo com defeito
* &lbrack;Camada de material&rbrack; Os materiais podem desaparecer ao reabrir um projeto

**Problemas Conhecidos:**

* &lbrack;Gerenciamento de cores&rbrack; As conversões do espaço de cores HDR com ACE no Linux produzem cores fixas
* &lbrack;Pilha de camadas&rbrack; Fonte de entrada não salva por camada
* &lbrack;Crash&rbrack; Ctrl Z Depois de excluir uma instância de sombreamento
* &lbrack;Iray&rbrack; IoR está bloqueada em 1 para alguns sombreadores

### 8.1.2

*(Lançado em: 19 de julho de 2022*)Resumo: **Versão de correção de erro secundária**

**Adicionado:**

* &lbrack;Auto Unwrap&rbrack; Nova opção “Otimizar para malhas orgânicas” para selecionar o algoritmo de segmentação
* &lbrack;Tamanho físico&rbrack; Expor opções de unidade em Novo Projeto e Configuração de Projeto
* &lbrack;Gerenciamento de cores&rbrack; Usar a tela do monitor por padrão ao usar ACE
* &lbrack;Gerenciamento de cores&rbrack;&lbrack;Python&rbrack; Leve em consideração o arquivo de predefinição ACE env-var ao criar o projeto
* &lbrack;Gerenciamento de cores&rbrack; Redefinir configurações de Gerenciamento de cores na janela Novo projeto quando a configuração mudar
* &lbrack;Gerenciamento de cores&rbrack; Desativar acesso às configurações de OCIO quando env-var estiver presente
* &lbrack;Gerenciamento de cores&rbrack; Atualizar com segurança as configurações de ACE quando um parâmetro não existir mais
* Atualize o Substance Engine para a versão 8.6.0
* &lbrack;Export&brack; Adicionar nova predefinição de exportação de GLTF com suporte para Deslocamento
* &lbrack;Scripting&rbrack;&lbrack;Python&rbrack; Recuperar informações de recursos (incluindo metadados personalizados)
* &lbrack;Scripting&rbrack;&lbrack;Python&rbrack; Adicionar função à lista de consulta de nomes de malha por Conjunto de textura
* &preset;Content&brack; Adicionar novo modelo do Blender e exportar predefinição

**Corrigido:**

* &lbrack;MacOS&rbrack; Falha ao iniciar o Iray em alguns casos
* &lbrack;Miniaturas&rbrack; Miniaturas de prateleira não carregam corretamente
* Vários canais UV são ignorados
* &lbrack;Auto Unwrap&rbrack; Cálculo desnecessário ao dividir ilhas longas
* &lbrack;Auto Unwrap&rbrack; Opção para evitar ilhas alongadas não levadas em consideração
* &lbrack;Desempacotar Automaticamente&rbrack; Perda de dados extras (cores de vértice) ao recompactar UVs
* &lbrack;UI&rbrack; Barra de rolagem horizontal na janela de propriedades quando o Gerenciamento de Cores está habilitado
* &lbrack;Gerenciamento de cores&rbrack; As configurações de OCIO não têm a função substance_3d_painter_standard_srgb
* &lbrack;Generator&rbrack; Uso incorreto de dados do usuário “desabilitado”
* &lbrack;Gerenciamento de cores&rbrack; O menu suspenso Espaço de cores “Não compatível” não deve ser clicável
* &lbrack;Gerenciamento de cores&rbrack;&lbrack;Sombreador&rbrack; sRGB override define não funciona mais
* &lbrack;Generator&rbrack; Uso incorreto de dados do usuário “disable”
* &lbrack;Pilha de camadas&rbrack; Visualizações quebradas com projetos do Bloco UV
* A documentação da API do &lbrack;Sombreador&rbrack; não está totalmente atualizada com o Dobra normal
* &lbrack;Export&brack;&lbrack;Interoperabilidade&rbrack; Não é possível enviar para o Stager com caracteres especiais
* &lbrack;Content&brack; Algumas miniaturas de predefinições de pincel estão vazias ou muito escuras

**Problemas Conhecidos:**

* &lbrack;Gerenciamento de cores&rbrack; As conversões do espaço de cores HDR com ACE no Linux produzem cores fixas
* &lbrack;Pilha de camadas&rbrack; A fonte de entrada não é salva por camada
* &lbrack;Crash&rbrack; Ctrl Z Depois de excluir uma instância de sombreamento
* &lbrack;Iray&rbrack; IoR está bloqueada em 1 para alguns sombreadores
* &lbrack;Sombreador&rbrack; Falha com sombreador antigo com defeito

### 8.1.1

*(Lançado: 28 de junho de 2022*)Resumo: **Hotfix de versão secundária**

**Adicionado:**

* &lbrack;Pilha de camadas&rbrack; Clicar com a tecla Alt pressionada na máscara não desmarca mais os efeitos

**Corrigido:**

* &lbrack;Crash&rbrack; Abrindo projeto antigo salvo no modo de visualização individual
* &lbrack;Crash&brack; Excluir um Gerador nas propriedades
* &lbrack;Configurações do conjunto de texturas&rbrack; A mistura Normal/Oclusão de ambiente e o height para métodos normais estão quebrados
* &brack;Export&brack; Exportar texturas usando o preenchimento de difusão renderiza mapas em preto

**Problemas Conhecidos:**

* &lbrack;MacOS&rbrack; Falha ao iniciar o Iray no Monterey
* &preto;Visualizar miniatura&rbrack; miniaturas simplificadas não são atualizadas quando uma âncora é usada
* &lbrack;Gerenciamento de cores&rbrack; As conversões do espaço de cores HDR com ACE no Linux produzem cores fixas

### 8.1.0

*(Lançado em: 07 de junho de 2022*)Resumo: **Versão principal com suporte ICC, dimensionamento de material com base em dados de tamanho físico, novos baker, melhorias no conta-gotas de cores e uma variedade de conteúdos adicionais**

**Adicionado:**

* &lbrack;Gerenciamento de cores&rbrack; Adicionar suporte para perfis ICC com Adobe Color Engine (ACE)
* &lbrack;Gerenciamento de cores&rbrack; Adicionar suporte para “Adobe 98 RGB” como espaço de cores de trabalho para ICC
* &lbrack;Color Management&rbrack; Permite definir configurações ACE/ICC através de um arquivo de configuração
* &lbrack;Gerenciamento de cores&rbrack; Permitir a entrada de valores de cor lineares no Seletor de Cores com o modo Legado
* &lbrack;Gerenciamento de cores&rbrack; Permite especificar o perfil de cores usado para escolher cores fora da interface
* &lbrack;Gerenciamento de cores&rbrack; Lembrar o último valor de exibição escolhido no visor
* &lbrack;Gerenciamento de cores&rbrack;&lbrack;Substance&rbrack; Faça com que os geradores/filtros funcionem corretamente com o Gerenciamento de cores
* &lbrack;Gerenciamento de cores&rbrack;&lbrack;Substance&rbrack; Adicionar novas palavras-chave de substituição colorspace $working e $standardsrgb
* &lbrack;Tamanho físico&rbrack;&lbrack;Motor&rbrack; Extrair informações de tamanho físico da malha
* &lbrack;Tamanho físico&rbrack;&lbrack;Computação de Tamanho físico do motor&rbrack;
* &lbrack;Tamanho físico&rbrack; Expor opções para usar tamanho físico na interface
* &lbrack;Tamanho físico&rbrack; Adicionar auxiliares visuais no visor
* &lbrack;Fazendo bake&rbrack; Adicionar baker de Height
* &lbrack;Fazendo bake&rbrack; Adicionar baker do Dobra normal
* &preto;Fazendo bake&rbrack; Adicionar baker de Opacidade
* &preto;Conta-gotas&rbrack; Nova visualização de conta-gotas de cor ao lado do mouse e cor gerenciada
* &lbrack;Conta-gotas&rbrack; O painel do seletor de cores reaparece em sua última posição quando reaberto
* &lbrack;Conta-gotas&rbrack; Um novo ícone para o Seletor de materiais
* &lbrack;Conta-gotas&rbrack; Cor gerencia a visualização do canal do seletor de cores
* &preto;Conta-gotas&rbrack; Adicionar a funcionalidade de clicar para selecionar ao conta-gotas
* &lbrack;Conta-gotas&rbrack; O seletor de materiais não ativa mais os canais não ativos
* &preto;Conta-gotas&rbrack; Permitir o uso do conta-gotas com um atalho
* &preto;Conta-gotas&rbrack; O conta-gotas seleciona o canal relevante, quando aplicável
* &preto;Conta-gotas&rbrack; Entrar no modo de seleção de cores desativa todos os atalhos
* &preto;Conta-gotas&rbrack; Remove a seleção automática do campo hexadecimal
* &preto;Conta-gotas&rbrack; Não feche o painel ao usar o seletor de material
* &lbrack;Conta-gotas&rbrack; Novo estado desativado quando o canal não está disponível para seleção
* &lbrack;Export&brack; Adicionar atributo tangente à exportação de glTF
* Atualize o Substance Engine para v8.4
* Atualizar a quebra automática para 0. 9. 0
* Atualize para Qt 5.15.8
* Atualização para o Python 3.9
* &lbrack;Sombreador&rbrack; Adicionar suporte para o Dobra normal sombreamento
* &lbrack;MacOS&rbrack; Suporte ao 3DConnection SpaceMouse
* &lbrack;Python&rbrack; Documenta a versão do Python usada na API
* &lbrack;Content&rbrack; Adicionar 6 novos ruídos 3D com 105 predefinições
* &lbrack;Content&rbrack; 20 novos mapas de desgaste e 2 padrões de dobras de pano
* &lbrack;Content&rbrack; Atualizar predefinição de exportação “Mapas de malha” para usar novos baker
* &lbrack;Content&brack; O filtro de Inclinação e distorção de desfoque depende da resolução do conjunto de texturas
* &lbrack;Content&rbrack; Atualiza projetos de amostra para usar os 3 novos baker

**Corrigido:**

* &lbrack;glTF&rbrack; Não é possível abrir glTF com caractere especial
* &lbrack;Engine&rbrack; Artefatos com anisotropia e SVT desativados
* Os Materiais inteligentes &lbrack;MacOS&rbrack;&lbrack;M1&rbrack; não são exibidos corretamente
* &lbrack;Processamento de malha&rbrack; Não é possível importar malhas do Modeler
* &lbrack;UI&rbrack; Barra de rolagem horizontal na nova janela do projeto com o Gerenciamento de cores ativado
* &lbrack;Gerenciamento de cores&rbrack; Valor do espaço de trabalho ausente no seletor de cores com algumas configurações de OCIO
* &lbrack;Gerenciamento de cores&rbrack; A visualização do pincel no visor não tem gerenciamento de cores
* A Tabela Dinâmica do &amp;SpaceMouse&rbrack; não é atualizada imediatamente com a alteração de foco e às vezes fora do modelo
* &lbrack;Export&rbrack;&lbrack;USD&rbrack; Os arquivos USD exportados têm uma estrutura incorreta
* &lbrack;USD&rbrack; problema de Oclusão de ambiente ao exportar
* &lbrack;Content&rbrack; Atualiza a malha da miniatura para corresponder ao projeto de amostra da Esfera de visualização

**Problemas Conhecidos:**

* Exportar texturas usando o preenchimento de difusão renderiza mapas em preto
* A mistura normal/Oclusão de ambiente está quebrada
* &lbrack;MacOS&rbrack; Falha ao iniciar o Iray em alguns casos raros
* &preto;Visualizar miniatura&rbrack; miniaturas simplificadas não são atualizadas quando uma âncora é usada
* &lbrack;Gerenciamento de cores&rbrack; As conversões do espaço de cores HDR com ACE no Linux produzem cores fixas

## Versão 7

### 7.4.3

*(Lançado em: 11 de abril de 2022*)Resumo: **Correção de erro com suporte para 3Dconnection SpaceMouse em 2D Viewport**

**Adicionado:**

* &lbrack;SpaceMouse&rbrack; Suporte a 3DConnection SpaceMouse em Visor 2D

**Corrigido:**

* &preto;Seletor de cores&rbrack; Não é possível gravar em campo hexadecimal
* &lbrack;Gerenciamento de cores&rbrack; Os recursos usados no modo de projeção não são gerenciados por cores na sobreposição
* &lbrack;Gerenciamento de cores&rbrack; Erros não são relatados no registro
* &lbrack;SpaceMouse&rbrack; Remove uma mensagem de erro genérica se o usuário não tiver um SpaceMouse
* &lbrack;SpaceMouse&rbrack; Ao carregar um projeto, o ponto dinâmico fica sempre oculto
* &lbrack;Baker&rbrack; A configuração de “Média normal” não tem efeito em projetos de Bloco UV
* &lbrack;Bloco UV&rbrack; As sobreposições de blocos uv inativos desaparecem ao recarregar a malha com blocos diferentes
* &lbrack;Scripting&rbrack;&lbrack;Python&rbrack; O script remoto está danificado
* &lbrack;Scripting&rbrack;&lbrack;Python&rbrack; Vários canais não podem ser consultados pela API e isso gera um erro
* &lbrack;Scripting&rbrack;&lbrack;Python&rbrack; Falha ao usar o evento ProjectEditionEntered
* &lbrack;Scripting&rbrack;&lbrack;Python&rbrack; Falha ao chamar get_ative_stack()

**Problemas Conhecidos:**

* Espaço de conexão 3Dsem suporte para mouse no MacOS
* &lbrack;UI&rbrack; Barra de rolagem horizontal com gerenciamento de cores sendo exibida em alguns casos na janela do novo projeto
* &lbrack;Os Materiais inteligentes do Mac M1&rbrack; não são exibidos corretamente

### 7.4.2

*(Lançado: 08 de março de 2022*)Resumo: **Correção de erro com suporte a 3Dconnection SpaceMouse e melhorias no gerenciamento de cores (OCIO)**

**Adicionado:**

* &lbrack;SpaceMouse&rbrack;&lbrack;Windows&rbrack; Suporte ao SpaceMouse 3Dconnection na Janela de Visualização 3D para navegação
* &lbrack;SpaceMouse&rbrack;&lbrack;Windows&rbrack; Atalhos/teclas básicos para modelos Pro e Enterprise SpaceMouse no Visor 3D
* &lbrack;SpaceMouse&rbrack;&lbrack;Windows&rbrack; Ícone do centro de rotação dedicado no Visor 3D
* &lbrack;Gerenciamento de cores&rbrack; Usar funções da configuração do OCIO para alterar as configurações padrão
* &lbrack;Gerenciamento de cores&rbrack; Gerenciamento de cores Gerencia a janela de propriedades dos widgets de cores
* &lbrack;Gerenciamento de cores&rbrack; Cor gerencia a janela de propriedades para visualização do material
* &preto;Gerenciamento de cores&rbrack; Cor gerenciar amostras no seletor de cores
* &lbrack;Gerenciamento de cores&rbrack; Adicionar uma configuração para definir o espaço de cores sRGB padrão
* &lbrack;Gerenciamento de cores&rbrack; Adicionar o espaço de cor sRGB padrão da configuração OCIO na lista de seletores de exibição do seletor de cores
* &preto;Gerenciamento de cores&rbrack; Melhorias para o menu de substituição do espaço de cores
* &lbrack;Gerenciamento de cores&rbrack; Permitir substituição do espaço de cores do mapa de ambiente nas Configurações de exibição
* &preto;Gerenciamento de cores&rbrack; Desenhar gradientes do seletor de cores com base na exibição atual
* &lbrack;Gerenciamento de cores&rbrack; Restringir valores HDR por padrão no editor de cores
* &lbrack;Gerenciamento de cores&rbrack; Usar passagem (sem espaço de cor) para filtros no modo Legado
* &lbrack;Gerenciamento de cores&rbrack; Limitar exibição de gradientes no editor de cores para corresponder ao intervalo do &lbrack;0-1&rbrack;
* &lbrack;Gerenciamento de cores&rbrack; Ocultar seletor de exibição no seletor de cores no modo Legado
* &preto;Gerenciamento de cores&rbrack; Fazer com que o seletor de cores tenha um campo hexadecimal sempre no espaço de cores sRGB
* &lbrack;Gerenciamento de cores&rbrack; Desativar menu suspenso Exibição do seletor de cores para canais de dados
* &lbrack;Otimization&rbrack; A grade de distorção recalcula somente os blocos UV cobertos
* &lbrack;Export&rbrack; Permitir a exportação de projetos do Bloco UV para Sketchfab, USD e glTF
* &lbrack;Scripting&rbrack;&lbrack;Python&rbrack; Permitir alteração da função de mapeamento de tom

**Corrigido:**

* &lbrack;Sketchfab&rbrack; A atualização do modelo existente acaba criando um novo modelo
* &lbrack;Sketchfab&rbrack; Falha ao procurar modelo atualizado anteriormente
* Falha ao exportar para USD
* Falha ao criar uma nova instância de sombreamento em Máscara de geometria ou quando a geometria está oculta
* &Lbrack;Janela Importar Ativo&rbrack; Falha ao alterar o tipo de recursos importados
* Mapas de malha normal são invertidos quando usados em pilha de camadas
* &lbrack;Substance&rbrack; O modo de mesclagem de dados do usuário não é levado em consideração
* &preto;Gerenciamento de cores&rbrack; Bitmaps com espaço de cor no nome do arquivo são importados como sequências de Bloco UV
* &lbrack;Gerenciamento de cores&rbrack; As saídas gerenciadas por cores do gráfico de Substance estão no espaço de cores incorreto
* A ferramenta Preenchimento de polígono do &preto;Gerenciamento de cores&rbrack; exibe a cor errada
* &lbrack;Gerenciamento de cores&rbrack; O mapeador de tons ACE é aplicado aos canais no modo solo
* &lbrack;Gerenciamento de cores&rbrack; A visualização da ferramenta de iluminação da esfera não é gerenciada por cores
* &lbrack;Gerenciamento de cores&rbrack;&lbrack;Exportar&rbrack; Mapas convertidos aplica uma conversão incorreta
* &lbrack;Scripting&rbrack;&lbrack;Python&rbrack;&lbrack;Gerenciamento de cores&rbrack; Os projetos criados com o modelo e a variável de ambiente OCIO estão no modo Legado
* &lbrack;Scripting&rbrack;&lbrack;Python&rbrack; Não é possível usar a função de avaliação do JavaScript na inicialização
* &lbrack;Oferta de Adobe 3D&rbrack; Não é possível iniciar o Painter ao usar configurações regionais com idiomas não suportados por padrão

**Problemas Conhecidos:**

* Espaço de conexão 3Dsem suporte para mouse no MacOS
* &lbrack;UI&rbrack; Barra de rolagem horizontal com gerenciamento de cores sendo exibida em alguns casos na janela do novo projeto
* &lbrack;Baker&rbrack; A configuração de “Média normal” não tem efeito em projetos de Bloco UV
* &lbrack;Os Materiais inteligentes do Mac M1&rbrack; não são exibidos corretamente
* &lbrack;Gerenciamento de cores&rbrack; Os recursos usados no modo de projeção não são gerenciados por cores na sobreposição
* &preto;Seletor de cores&rbrack; Não é possível gravar em campo hexadecimal

### 7.4.1

*(Lançado: 14 de dezembro de 2021*)Resumo: **Correção de erros com melhorias no gerenciamento de cores**

**Adicionado:**

* &preto;Gerenciamento de cores&rbrack; Usar função de dados nos nomes de arquivos exportados
* &preto;Gerenciamento de cores&rbrack; Expande a seção Gerenciamento de cores, por padrão, quando o OCIO for selecionado nas novas janelas de configurações do projeto e do projeto
* &lbrack;Gerenciamento de cores&rbrack; Adicionar mapeador de tons ACE no modo legado
* &preto;Gerenciamento de cores&rbrack; Ajustar as definições de configuração padrão
* &lbrack;Gerenciamento de cores&rbrack;&lbrack;Exportar&rbrack; Preencher $colorSpace nos nomes de arquivos para canais de dados
* &prec;Exportar &prec; Exportar projeto de Bloco UV para o Stager
* &lbrack;Interoperabilidade&rbrack; Não disponível para as edições Steam e Substance
* &lbrack;Interoperabilidade&rbrack; Permitir o envio de um projeto de Bloco UV para o Stager

**Corrigido:**

* &lbrack;MacOS&rbrack;&lbrack;Crash&rbrack; o Painter não começa com o Catalina
* &lbrack;Gerenciamento de cores&rbrack;&lbrack;Falha&rbrack; Falha aleatória ao reproduzir o gerenciamento de cores/tipo de dados no canal do usuário
* &preto;Gerenciamento de cores&rbrack; Recursos usados como tons de cinza no novo menu espaço de cores de exibição de máscara
* &lbrack;Gerenciamento de cores&rbrack; O canal do usuário é mais escuro na viewport no modo legado + visualização individual
* &lbrack;Gerenciamento de cores&rbrack; O mapa de ambiente é sempre linear quando usado no iRay
* &lbrack;Gerenciamento de cores&rbrack; O seletor de cores não seleciona o valor correto para o canal de dados no modo herdado
* &lbrack;Gerenciamento de cores&rbrack; O seletor de cores está quebrado dentro de um Substance no modo herdado
* &lbrack;Gerenciamento de cores&rbrack; Alternar entre exibições de canal individual na viewport não é exibido com o espaço de cor correto ao usar o menu suspenso
* &lbrack;Gerenciamento de cores&rbrack; Exportar aplica a conversão incorreta em canais de usuário com gerenciamento de cores no modo herdado
* Os traçados feitos na máscara de exibição individual não são exibidos ao voltar para a exibição de material
* &preto;Exportar&rbrack; Mapas convertidos não são exportados como canais com gerenciamento de cores
* &lbrack;Textura Set&rbrack; A dica de ferramenta com o nome original está ausente em canais de usuário renomeados
* &lbrack;Steam&brack; Arquivos ausentes ao verificar a integridade do arquivo com o Steam

**Problemas Conhecidos:**

* &lbrack;Os Materiais inteligentes do Mac M1&rbrack; não são exibidos corretamente

### 7.4.0

*(Lançado: 24 De novembro De 2021*)Resumo: **Versão Principal. Introdução da 1ª versão de gerenciamento de cores, desencaixe da exibição 2D ou 3D, nova opção de desencapsulamento automático UV para evitar ilhas alongadas, chame funções JavaScript da API Python e novo conteúdo**

**Adicionado:**

* &lbrack;Gerenciamento de cores&rbrack; Suporte ao gerenciamento de cores OpenColorIO versão 2
* &preto;Gerenciamento de cores&rbrack; Adicionar configurações de gerenciamento de cores às configurações do projeto
* &lbrack;Gerenciamento de cores&rbrack; Janela de aviso sobre as alterações de configuração do Gerenciamento de cores ao abrir um projeto
* &lbrack;Gerenciamento de cores&rbrack; Exibir uma mensagem de erro se um arquivo de configuração OCIO inválido for selecionado
* &lbrack;Gerenciamento de cores&rbrack; Permitir substituir a configuração pela variável de ambiente OCIO
* &lbrack;Gerenciamento de cores&rbrack; Várias configurações de OCIO integradas por padrão com o aplicativo
* &preto;Gerenciamento de cores&rbrack; Extrair o nome do espaço de cores do nome de arquivo bitmap importado
* &lbrack;Color Management&brack; Permite substituir o espaço de cor por um espaço de cor da configuração na janela Propriedades
* &preto;Gerenciamento de cores&rbrack; Adicionar opções de gerenciamento de cores nas Configurações do conjunto de texturas
* &lbrack;Gerenciamento de cores&rbrack;&lbrack;Visor&rbrack; Permitir gerenciamento de cores de exibições 2D e 3D separadamente
* &preto;Gerenciamento de cores&rbrack; Carrega e converte o mapa de ambiente para o espaço de cores de trabalho
* &preto;Gerenciamento de cores&rbrack; Ajustar seletor e editor de cores com o espaço de cores atual
* &lbrack;Color Management&rbrack; Permite selecionar o espaço de cores do transformo de exibição na viewport com um novo menu suspenso
* &lbrack;Gerenciamento de cores&rbrack; Aplicar transformo de exibição com resultados de renderização de matriz
* &preto;Gerenciamento de cores&rbrack; Exportar texturas com espaços de cores diferentes
* &lbrack;Gerenciamento de cores&rbrack;&lbrack;Python&rbrack; Aplicar configurações de gerenciamento de cores da variável de ambiente (OCIO) a novos projetos
* &lbrack;Visor&rbrack; Permitir desencaixar o visor 2D ou 3D
* &lbrack;Auto Unwrap&rbrack; Nova opção para evitar ilhas alongadas
* &lbrack;Script Python&rbrack; Chamar funções JavaScript a partir da API Python
* &preto;Janela Novo projeto&rbrack; Torna a seção de mapas importada flexível
* &lbrack;Projeção&rbrack;&lbrack;Distorcer&rbrack; Permite ocultar normais como uma opção nas configurações de Distorção
* &lbrack;Content&rbrack; 11 novos mapas de desgaste
* &lbrack;Content&brack; 8 novas predefinições de ferramenta (zíper, apertar fio, brilho)
* &lbrack;Content&brack; 8 novos materiais (cicatriz, bolso, ...)
* &lbrack;Content&rbrack; 1 novo gerador (inflar deformação)

**Problemas Conhecidos:**

* &lbrack;Os Materiais inteligentes do Mac M1&rbrack; não são exibidos corretamente
* &lbrack;Gerenciamento de cores&rbrack;&lbrack;Falha&rbrack; Falha aleatória ao reproduzir o gerenciamento de cores/tipo de dados no canal do usuário
* &lbrack;Gerenciamento de cores&rbrack; O seletor de cores não seleciona o valor correto para o canal de dados no modo herdado
* &lbrack;Gerenciamento de cores&rbrack;&lbrack;Iray&rbrack; Salvar a renderização em EXR ou TIFF enquanto o Gerenciamento de cores está ativado na janela de visualização sempre salvará em formato linear
* &preto;Gerenciamento de cores&rbrack; Os recursos usados como tons de cinza na máscara exibem o menu Espaço de cor errado
* &lbrack;Gerenciamento de cores&rbrack;&lbrack;Iray&rbrack; O mapa de ambiente é sempre linear quando usado em Iray
* &lbrack;Gerenciamento de cores&rbrack;&lbrack;Exportar&rbrack; Mapas convertidos não são exportados como canais gerenciados por cores
* &lbrack;Gerenciamento de cores&rbrack;&lbrack;Exportar&rbrack; ignora se o canal do usuário tem gerenciamento de cores ou não com o modo legado

### 7.3.1

*(Lançado: 24 De novembro De 2021*)Resumo: **Correção De Erros**

**Adicionado:**

* &lbrack;Projeção&rbrack; O dimensionamento deve funcionar somente no Espaço do objeto

**Corrigido:**

* &lbrack;O Mac M1&rbrack; Camadas de material não está funcionando
* &lbrack;Mac M1&rbrack;&lbrack;Projeção&rbrack; Warp não funciona
* Os microdetalhes não são exibidos corretamente
* &lbrack;Projeção&rbrack;&lbrack;Falha&rbrack; Alternando para o modo de distorção com uma camada criada com uma versão anterior
* &lbrack;Projeção&rbrack;&lbrack;Distorcer&rbrack; não funciona quando a transformação está definida para o espaço global
* &lbrack;Projection&rbrack;&lbrack;Warp&rbrack; Split option permanece selecionada após a divisão ser feita
* &lbrack;Projeção&rbrack;&lbrack;UV&rbrack; O ponto dinâmico é redefinido ao inverter a projeção
* &lbrack;Filtro&rbrack; Faço bake O ambiente de iluminação está mudando ao recarregar ou alterar um parâmetro
* &lbrack;Interoperabilidade&rbrack; Não disponível para as edições Steam e Substance
* &lbrack;Interoperabilidade&rbrack; O botão “Procurar ativos 3D no Marketplace” deve sempre abrir o CCD na guia Stock e Marketplace 3D

**Problemas Conhecidos:**

* &lbrack;Os Materiais inteligentes do Mac M1&rbrack; não são exibidos corretamente

### 7.3.0

*(Lançado: 13 De outubro De 2021*)Resumo: **Versão Principal. Contém uma nova projeção de distorção 3D, uma nova projeção cilíndrica, melhorias no seletor de cores, novas funções na API Python e correções de erros**

**Adicionado:**

* &lbrack;Projeção&rbrack;&lbrack;Distorcer&rbrack; Expor distorção 3D como um novo modo de projeção
* &lbrack;Projeção&rbrack;&lbrack;Distorcer&rbrack; Permitir modo de decalque para Alpha, Texturas e Procedimentos com arrastar e soltar no visor
* &lbrack;Projeção&rbrack;&lbrack;Distorcer&rbrack; Usar distorcer projeção com atalho de decalque (ALT)
* &lbrack;Projeção&rbrack;&lbrack;Distorcer&rbrack;&lbrack;Barra de ferramentas&rbrack; Transformar distorção como um todo ou por vértices
* &lbrack;Projeção&rbrack;&lbrack;Distorcer&rbrack;&lbrack;Barra de ferramentas&rbrack; Adicionar pontos de grade com distorção dividida nas opções transversal, horizontal ou vertical
* &lbrack;Projeção&rbrack;&lbrack;Distorcer&rbrack;&lbrack;Barra de ferramentas&rbrack; Menu dedicado para ações de redefinição
* &lbrack;Projeção&rbrack;&lbrack;Distorcer&rbrack;&lbrack;Barra de ferramentas&rbrack; Opção para ajustar automaticamente tangentes ao mover pontos
* &lbrack;Projeção&rbrack;&lbrack;Distorção&rbrack;&lbrack;Barra de ferramentas&rbrack; Menu dedicado para edição de grade (tamanho, redefinição, cor e tamanho da alça)
* &lbrack;Projeção&rbrack;&lbrack;Distorção&rbrack; Novo atalho de teclado para alternar o modo de edição de distorção de vértices inteiros (SHIFT+V)
* &lbrack;Projeção&rbrack;&lbrack;Distorcer&rbrack; O clique+Ctrl permite alternar entre a ferramenta de superfície e outras ferramentas
* &lbrack;Projeção&rbrack;&lbrack;Cilíndrico&rbrack; Expor o modo de projeção cilíndrica
* &lbrack;Projeção&rbrack;&lbrack;Barra de ferramentas&rbrack; Configurações do manipulador de grupos (tamanho, etapas da grade, etapas do ângulo)
* &preto;Seletor de cores&rbrack; Nova interface do seletor de cores
* &preto;Seletor de cores&rbrack; Usar valores sRGB nos widgets do seletor de cores
* &preto;Seletor de cores&rbrack; Permite salvar e excluir amostras de cores
* &preto;Seletor de cores&rbrack; Conta-gotas acessível de cor e slots normais
* &lbrack;Seletor de cores&rbrack; Permite editar a cor dinâmica entre 0 e 255 valores
* &preto;Seletor de cores&rbrack; Tornar o estado HSV/RGB comum no aplicativo
* &lbrack;Seletor de Cores&rbrack; A janela do Seletor de Cores é semipersistente
* &preto;Seletor de cores&rbrack; pressionar Esc fecha a janela do seletor de cores
* Melhoria de desempenho para interação de interface e ao pintar
* &lbrack;Engine&rbrack; Atualização para a nova versão do mecanismo de Substance (8.3.0)
* &lbrack;Scripting&rbrack;&lbrack;Python&rbrack; Permitir recarregar a malha do projeto atual
* &lbrack;Scripting&rbrack;&lbrack;Python&rbrack; Permitir atualização de recursos em projetos
* &lbrack;Scripting&rbrack;&lbrack;Python&rbrack; Permite definir e consultar a resolução de Blocos UV
* &lbrack;Interoperabilidade&rbrack; Não disponível para as edições Steam e Substance
* &lbrack;Interoperabilidade&rbrack; Receber vários recursos do Bridge

**Corrigido:**

* O seletor de cores não exibe a cor correta
* &lbrack;Fazendo bake&rbrack; A lista de conjuntos de texturas não está ordenada corretamente
* As transformações dinâmicas de grupo do &lbrack;FBX import&rbrack; 3ds Max não são levadas em consideração
* &lbrack;Substance Engine&rbrack; Falha com importação de SBSAR corrompido
* &lbrack;A opção de configuração do projeto do MacOS&rbrack; em idiomas diferentes não está presente
* Os salvamentos automáticos podem congelar o Painter durante processos longos

**Problemas Conhecidos:**

* &lbrack;Projection&rbrack;&lbrack;Warp&rbrack; Split option permanece selecionada após a divisão ser feita
* &lbrack;Projeção&rbrack;&lbrack;Distorcer&rbrack; não funciona quando a transformação está definida para o espaço global
* &lbrack;Projeção&rbrack;&lbrack;Distorcer&rbrack; Linhas de artefato entre as correções em alguns casos raros
* &lbrack;Projeção&rbrack;&lbrack;UV&rbrack; O ponto dinâmico é redefinido ao inverter a projeção
* &lbrack;Os Materiais inteligentes do Mac M1&rbrack; não são exibidos corretamente
* &lbrack;M1&rbrack;&lbrack;Regressão&rbrack; Camadas de material não funcionam

### 7.2.3

*(Lançado: 24 de agosto de 2021*)Resumo: **Versão secundária, correção de erro**

**Adicionado:**

* &lbrack;Bibliotecas&rbrack; Adicionar uma maneira de impedir que arquivos indesejados sejam rastreados

**Corrigido:**

* &lbrack;Win&rbrack; Vários telas e problemas de suspensão
* &lbrack;MacOS&rbrack;&lbrack;Falha&rbrack; Alternando sombreador ao usar efeitos
* &preto;Visor&rbrack; O modo de visualização completa não mostra mais o cursor do pincel sem alfa
* O widget Ângulo do &lbrack;UI&rbrack; vira da maneira errada
* &lbrack;Pilha de camadas&rbrack; Muitas subpastas criam um congelamento muito longo
* &lbrack;Iray&rbrack; Diferentes vistas em Iray e OpenGL: Visível se não estiver funcionando
* &lbrack;Iray&rbrack; Índice de refração não levado em consideração e não aparece nas propriedades mdl
* &lbrack;JavaScript&rbrack; ShowExportDialog() nunca retorna verdadeiro
* Não é possível ler o mtl do Adobe Stock

### 7.2.2

*(Lançado: 27 de julho de 2021*)Resumo: **Versão secundária, correção de erros**

**Adicionado:**

* Atualizar versão de requisitos de driver AMD

**Corrigido:**

* &lbrack;Mac M1&rbrack; Detecção de memória incorreta
* &lbrack;Export&brack; Os caminhos muito longos não são exibidos corretamente

**Problemas Conhecidos:**

* &lbrack;Content&brack; Sombreadores desatualizados das amostras

### 7.2.1

*(Lançado em: 2 de julho de 2021*)Resumo: **Versão secundária, Hotfix**

**Adicionado:**

* &lbrack;Interop&rbrack; Adicionar dica de ferramenta para informar que o envio de projetos do Bloco UV para o Stager ainda não é suportado
* &lbrack;Plug-in&rbrack;&lbrack;UI&rbrack; Atualização do ícone do Livelink

**Corrigido:**

* &lbrack;A versão do driver Nvidia&rbrack; que começa com 30 é considerada desatualizada
* &lbrack;Bibliotecas&rbrack; O estado do painel Ativos não é salvo, a menos que um projeto esteja aberto
* &lbrack;Bibliotecas&rbrack; A nova pesquisa salva mantém a palavra-chave da pesquisa salva antiga
* &lbrack;Baker&rbrack;&lbrack;UVTiles&rbrack; os mapas de ID por meshID também levam Blocos UV em consideração
* &lbrack;Exportar&rbrack; arquivos gLTF não importam a cor do vértice
* &lbrack;Iray&rbrack; Algumas dicas estão faltando
* O &lbrack;Interop&rbrack; Enviar para o Stager nem sempre é desativado quando o Stager não é detectado
* &lbrack;Atualizador de Recursos&rbrack; O criador de pincéis do Photoshop não pode ser atualizado
* &lbrack;Content&brack; O gerador de desgaste de borda de fibra de vidro está quebrado

### 7.2.0

*(Lançado: 23 de junho de 2021*)Resumo: **Versão principal, fornece uma atualização para o painel de ativos, um novo sombreador com acesso a novos canais e parâmetros, uma atualização geral da interface do usuário, algumas melhorias de desempenho muito solicitadas, suporte a idiomas expandido e muito mais!**

**Adicionado:**

* &lbrack;Bibliotecas&rbrack; Novo painel de ativos para substituir a prateleira
* &lbrack;Bibliotecas&rbrack;&lbrack;UI&rbrack; Novo layout do painel Ativos
* &lbrack;Bibliotecas&rbrack;&lbrack;UI&rbrack; Alterar a orientação e a interface padrão do Painel de ativos
* &lbrack;Bibliotecas&rbrack;&lbrack;UI&rbrack; Introduzir uma opção de exibição em lista para a biblioteca
* &lbrack;Bibliotecas&rbrack;&lbrack;UI&rbrack; Navegação por novas trilhas no Painel de ativos
* &lbrack;Bibliotecas&rbrack;&lbrack;UI&rbrack; Selecione “Todas as bibliotecas” ao selecionar uma pesquisa salva
* &lbrack;Bibliotecas&rbrack;&lbrack;UI&rbrack; Selecione “Todas as bibliotecas” quando todas as pastas estiverem desmarcadas
* &lbrack;Bibliotecas&rbrack;&lbrack;UI&rbrack; Nova marca para pincéis de partícula
* &lbrack;Bibliotecas&rbrack;&lbrack;UI&rbrack; Substituído “prateleira” por “Todas as bibliotecas” no aplicativo
* &lbrack;Bibliotecas&rbrack;&lbrack;UI&rbrack; Permitir ocultar pastas vazias
* &lbrack;Libraries&rbrack;&lbrack;UI&rbrack; A biblioteca padrão do usuário deve estar visível mesmo se estiver vazia
* &lbrack;Bibliotecas&rbrack;&lbrack;UI&rbrack; Novo método de filtragem por meio de ícones de tipo de ativo
* &lbrack;Bibliotecas&rbrack; Atalho “CTRL” para selecionar vários tipos de ativos
* &lbrack;Bibliotecas&rbrack; Nova variável de ambiente para controlar o orçamento de memória de visualização do ativo
* &lbrack;Libraries&rbrack;&lbrack;Content&rbrack; Novos mapas de ambiente
* &lbrack;Bibliotecas&rbrack;&lbrack;Conteúdo&rbrack;&lbrack;IU&rbrack; Renderizar deslocamento em materiais padrão
* &lbrack;Bibliotecas&rbrack;&lbrack;Conteúdo&rbrack; Definir Adobe Standard Material (ASM) sombreador como padrão para a geração de visualizações
* &lbrack;Bibliotecas&rbrack;&lbrack;Conteúdo&rbrack;&lbrack;ASM&rbrack; Novos Modelos de Projeto para o novo sombreador ASM
* &lbrack;Libraries&rbrack;&lbrack;Thumbnail&rbrack; Usar novo mapa de ambiente do Studio 6
* &lbrack;Bibliotecas&rbrack;&lbrack;Miniatura&rbrack; Ler miniatura no recurso em vez de gerá-lo
* &lbrack;Bibliotecas&rbrack;&lbrack;Miniatura&rbrack; Adicionar deslocamento à geração de miniaturas
* &preto;Configurações do conjunto de texturas&rbrack;
* &lbrack;Configurações do conjunto de texturas&rbrack;&lbrack;UI&rbrack; Expor o novo height ao método de conversão normal
* &lbrack;Configurações do conjunto de texturas&rbrack;&lbrack;UI&rbrack; Retrabalho da organização da interface do usuário dos canais
* &lbrack;Configurações do conjunto de texturas&rbrack; Limite dos canais do usuário aumentado para 16 canais
* &lbrack;Configurações do conjunto de texturas&rbrack;&lbrack;IU&rbrack; Indica quais canais são compatíveis com o sombreador selecionado atualmente
* &lbrack;Sombreador&rbrack;&lbrack;ASM&rbrack; Novo sombreador
* &lbrack;Sombreador&rbrack;&lbrack;ASM&rbrack; Suporte adicionado para Anisotropia, Revestimento transparente, Dispersão da subsuperfície, Specular edge color e Brilho
* &lbrack;Sombreador&rbrack;&lbrack;ASM&rbrack; Alterar os valores de cor dos canais padrão
* &lbrack;Sombreador&rbrack;&lbrack;ASM&rbrack;&lbrack;Exportar&rbrack; Modelo de exportação atualizado do Adobe Dimension para o Adobe Substance 3D Stager
* &lbrack;Sombreador&rbrack;&lbrack;ASM&rbrack; Rótulos e dicas de ferramentas adicionados para os parâmetros sombreador e MDL
* &lbrack;Sombreador&rbrack;&lbrack;ASM&rbrack; Torna a cor da Dispersão visível no Visualização 2D, mesmo se o SSS não for suportado
* &lbrack;Sombreador&rbrack;&lbrack;ASM&rbrack;&lbrack;Iray&rbrack; Suporte ao sombreador ASM no Iray com o novo MDL
* &lbrack;Sombreador&rbrack;&lbrack;ASM&rbrack;&lbrack;Iray&rbrack; Atualização da dispersão de subsuperfície no brilho de especificação PBR herdado e revestido
* &lbrack;Sombreador&rbrack;&lbrack;ASM&rbrack;&lbrack;Conteúdo&rbrack; Alterou o tipo padrão de SSS para amostras
* &lbrack;Sombreador&rbrack;&lbrack;ASM&rbrack; Documentação adicionada para API ASM
* &lbrack;Sombreador&rbrack;&lbrack;ASM&rbrack; Otimizar sombreadores para ignorar canais não utilizados
* &lbrack;Sombreador&rbrack; Expor novos canais do Conjunto de Texturas
* &lbrack;Sombreador&rbrack; Dispersão de subsuperfície aprimorada
* &lbrack;Sombreador&rbrack; Novos parâmetros de sombreador ocultos para alguns sombreadores
* &lbrack;Sombreador&rbrack; Visível se para parâmetros de sombreador
* &preto;Desempenho&rbrack;
* &lbrack;Bibliotecas&rbrack; Visualização do recurso carregando melhorias de tempo e desempenho de cálculo
* &lbrack;Mecanismo&rbrack; Melhorias no desempenho da pintura
* &lbrack;Desempacotar automaticamente&rbrack;
* &lbrack;Retirar quebra automática&rbrack; melhorias no desempenho da Embalagem
* &lbrack;Desempacotamento automático&rbrack; Desempacotamento automático compatível com o fluxo de trabalho do Bloco UV
* &lbrack;Contornar automaticamente&rbrack; Nova opção para posicionar UVs de acordo com a orientação da malha
* &prego;Outro&preto;
* &lbrack;Configurações&rbrack; Mudou a direção padrão do zoom
* &lbrack;UI&rbrack; Atualização geral da IU
* &lbrack;UI&rbrack; Retrabalho do Menu Ajuda
* &lbrack;UI&rbrack; Substituir ícone de inversão
* &lbrack;UI&rbrack;&lbrack;Plug-in&rbrack; Ícone Substituir do link dcc do plug-in
* &lbrack;UI&rbrack;&lbrack;AMD&rbrack; Atualizar versão mínima necessária e mensagem pop-up
* &lbrack;Pilha de camadas&rbrack; Cria nova camada dentro da pasta vazia selecionada
* Atualizar Documentação do Python
* &brack;Marca&rbrack;
* &lbrack;Branding&rbrack;&lbrack;UI&rbrack; Nome do aplicativo atualizado para Adobe Substance 3D Painter
* &lbrack;Branding&rbrack;&lbrack;UI&rbrack; Versão autônoma atualizada para &#39;Substance edition&#39;
* &lbrack;Branding&rbrack;&lbrack;UI&rbrack; Nome executável do aplicativo atualizado, caminho de instalação, pacote e ícones
* &lbrack;Branding&rbrack;&lbrack;UI&rbrack; Biblioteca e caminho padrão renomeados
* &lbrack;Marca&rbrack;&lbrack;IU&rbrack; Atualizado Sobre a Janela
* &lbrack;Marca&rbrack;&lbrack;IU&rbrack; Tela de Boas-vindas atualizada
* &lbrack;Marca&rbrack;&lbrack;IU&rbrack; Removido número da versão baseada no ano
* &lbrack;Localização&rbrack; Novas traduções para alemão, francês e chinês simplificado
* &lbrack;Interoperabilidade&rbrack; Não disponível para as edições Steam e Substance
* &lbrack;Interoperabilidade&rbrack; Interoperabilidade com o Ecossistema Adobe: Designer, Sampler, Stager e Bridge
* &lbrack;Interoperabilidade&rbrack;&lbrack;UI&rbrack; Receber e atualizar ativos do Designer
* &lbrack;Interoperabilidade&rbrack;&lbrack;UI&rbrack; Receber ativo do Sampler
* &lbrack;Interoperabilidade&rbrack;&lbrack;UI&rbrack; Enviar ativo para o Stager
* &lbrack;Interoperabilidade&rbrack;&lbrack;UI&rbrack; Mostrar no Adobe Bridge
* &lbrack;Interoperabilidade&rbrack;&lbrack;IU&rbrack; Permitir acesso rápido a Ativos 3D do Adobe
* &lbrack;Interoperabilidade&rbrack; Novas marcas de uso de sbsar
* &lbrack;Interoperabilidade&rbrack; Manipular tipos de ativos recebidos
* &lbrack;Interoperabilidade&rbrack; Os ativos recebidos do Adobe Substance 3D Designer ou Adobe Substance 3D Sampler são armazenados na biblioteca padrão escolhida pelo usuário
* &lbrack;Interoperabilidade&rbrack;&lbrack;IU&rbrack; Novo ícone na barra de ferramentas esquerda para enviar para o Stager ou Photoshop

**Corrigido:**

* &lbrack;Tablet&rbrack; Baixo desempenho ao pintar com pressão
* &lbrack;Problema no tablet com controles deslizantes
* &lbrack;Falha&rbrack; Nome incompatível entre a lista de Conjuntos de Texturas e o Exportador
* &lbrack;Crash&rbrack;&lbrack;Bibliotecas&rbrack; Clique duas vezes em uma subbiblioteca
* &lbrack;Bibliotecas&rbrack; Problema ao Rastrear diretórios de bibliotecas
* &lbrack;Bibliotecas&rbrack; Forçar geração de visualização linha de comando não funciona como esperado
* &lbrack;Bibliotecas&rbrack;&lbrack;Conteúdo&rbrack; O filtro Ambiente de Luz Feito bake é preto por padrão
* &lbrack;Linux&rbrack;&lbrack;MacOS&rbrack;&lbrack;Exportar malha&rbrack; Não é possível importar glTF criado no Linux/MacOS
* &lbrack;Linux&rbrack; Arrastar e soltar um arquivo no Painel de ativos pode causar um travamento
* O &lbrack;Contornar automaticamente&rbrack; Contornar automaticamente disponível mesmo se uma malha não tiver sido selecionada para recarregamento
* &lbrack;Partículas&rbrack; Comportamento de partícula incorreto com a gravidade
* O histograma de nível do &lbrack;Pilha de camadas&rbrack; só pode usar a Luminância com alguns canais
* &preto;Máscara de geometria&rbrack; Menu do botão direito do mouse em uma pasta quando a edição da máscara de geometria não funcionar
* &lbrack;Projeção&rbrack; Costura com projeção esférica e filtragem bilinear
* &lbrack;Blocos UV&rbrack; Exportar máscara para arquivo exporta somente bloco 0, 0
* &preto;Exportar malha&rbrack; A exportação de malha FBX está vazia
* O Mapa normal &lbrack;Iray&rbrack; não é levado em consideração em novos projetos ao renderizar
* &lbrack;Salvar&rbrack; Salvar problemas em unidades compartilhadas
* &lbrack;Fazendo bake&rbrack; Reativar uma malha com parâmetros modificados exibe um aviso
* &lbrack;Fazendo bake&rbrack;&lbrack;Regressão&rbrack; Resultado incorreto quando a caixa delimitadora global de grandes malhas não inclui a origem da cena
* &lbrack;Python&rbrack; As bibliotecas de usuário personalizadas não são levadas em consideração

**Problemas Conhecidos:**

* &lbrack;Bibliotecas&rbrack; Pesquisas salvas não são salvas se nenhum projeto for aberto
* &lbrack;NVIDIA&rbrack; Mensagem para driver desatualizado mesmo se o driver estiver atualizado

### 7.1.1 (2021.1.1)

*(Lançado: 23 de março de 2021*)Resumo: **Versão secundária, correção de erro com possibilidade de inserir valores hexadecimais no seletor de cores**

**Adicionado:**

* &lbrack;Log&rbrack; Avisa os usuários sobre drivers de GPU AMD incompatíveis
* &preto;Seletor de cores&rbrack; Permitir digitar valores hexadecimais

**Corrigido:**

* &lbrack;Baker&rbrack; Queda de desempenho
* &lbrack;Máscara de geometria&rbrack; clicar com a tecla Alt no nome da malha pode levar a um travamento
* &lbrack;Engine&brack; A pintura não atualiza toda a exibição quando necessário
* &lbrack;Pilha de camadas&rbrack; A seleção fica parada após alterar o sombreador
* &lbrack;MacOS&rbrack;&lbrack;Seletor de cores&rbrack; A cor é ligeiramente diferente da escolhida
* &lbrack;Export&rbrack; Usar o formato de arquivo PSD não gera um arquivo por Bloco UV
* &lbrack;Scripting&rbrack;&lbrack;Javascript&rbrack; alg.mapexport.getPathsExportDocumentMaps() não retorna todos os valores
* &lbrack;Scripting&rbrack;&lbrack;Python&rbrack; Os plug-ins desativados são ativados novamente ao reabrir o Painter

### 7.1.0 (2021.1.0)

*(Lançado: 28 de janeiro de 2021*)Resumo: **Versão principal, nova Máscara de Geometria que permite selecionar e tinta partes da geometria, copiar/colar efeitos na pilha de camadas, melhoria do fluxo de trabalho do Bloco UV, atualização do Iray, Baker, Substance Engine e novo conteúdo**

**Adicionado:**

* Nova máscara de geometria e tinta partes selecionadas da geometria
* &preto;Máscara de geometria&rbrack; Permitir a tinta de partes selecionadas da geometria por nomes de malha
* &preto;Máscara de geometria&rbrack; Seleção retangular em ambas as portas de visualização
* &preto;Máscara de geometria&rbrack; Permite ocultar/ignorar a geometria excluída em qualquer camada
* &lbrack;Máscara de geometria&rbrack;&lbrack;Propriedades&rbrack; Seleção rápida de caixas de seleção com clicar e arrastar
* &lbrack;Máscara de geometria&rbrack;&lbrack;Propriedades&rbrack;&lbrack;UI&rbrack; Incluir/Excluir tudo com uma lista suspensa na janela Propriedades
* &lbrack;Máscara de geometria&rbrack;&lbrack;Propriedades&rbrack; Permite selecionar rapidamente um item em uma lista com ALT+CLIQUE ESQUERDO
* &lbrack;Máscara de geometria&rbrack;&lbrack;Propriedades&rbrack; Sobreposição em viewports ao passar o mouse sobre nomes/Blocos UV de malha na janela Propriedades
* &lbrack;Máscara de geometria&rbrack;&lbrack;Pilha de camadas&rbrack; Adicionar opções de copiar/colar à máscara de geometria
* &preto;Máscara de geometria&rbrack; Novo ícone para o botão Ocultar/ignorar geometria excluída
* &preto;Máscara de geometria&rbrack; Nova dica de ferramenta para Ocultar/ignorar geometria excluída
* &lbrack;Máscara de geometria&rbrack; Atalho de teclado ALT+H para ativar/desativar o botão “ocultar ignorar geometria excluída”
* &lbrack;Blocos UV&rbrack;&lbrack;Pilha de camadas&rbrack; Nova miniatura de visualização da esfera da camada de preenchimento para Blocos UV e modo simplificado
* &lbrack;Blocos UV&rbrack;&lbrack;Pilha de camadas&rbrack; Permite sair facilmente da máscara de Bloco UV
* &lbrack;Blocos UV&rbrack;&lbrack;Lista do conjunto de texturas&rbrack; Permitir fornecer uma descrição por Bloco UV
* &lbrack;Blocos UV&rbrack;&lbrack;Configurações do conjunto de textura&rbrack;&lbrack;UI&rbrack; Dois novos títulos de seção no menu suspenso para alterar a resolução do Bloco UV
* &lbrack;Blocos UV&rbrack;&lbrack;Visor&rbrack; Sair da Máscara do Bloco UV ao arrastar um material para o visor
* &preto;Pilha de camadas&rbrack; Adicionar opções de Copiar/Colar para efeitos
* &lbrack;Pilha de camadas&rbrack; Permitir copiar/colar efeitos de um Conjunto de Texturas para outro
* &lbrack;Pilha de camadas&rbrack; Permitir seleção múltipla de efeitos
* &preto;Pilha de camadas&rbrack; Adicionar opções de copiar/colar como atalhos para efeitos de camada
* &lbrack;Pilha de camadas&rbrack; Alterna automaticamente entre máscara e conteúdo ao arrastar efeitos para outra camada
* &lbrack;Pilha de camadas&rbrack; Cria automaticamente uma máscara ao colar uma máscara de outra camada
* &lbrack;Pilha de camadas&rbrack; Adicionar ações de efeito de movimento dentro do menu contextual de clique com o botão direito do mouse dos efeitos
* &lbrack;Pilha de camadas&rbrack; Permite arrastar e soltar efeitos de uma camada para outra
* &lbrack;Pilha de camadas&rbrack; Arrastar itens para uma pasta os coloca na parte superior da pasta
* Atualize o Iray para a versão 2020.1.0
* &lbrack;Baker&rbrack; Atualize os Baker para a versão 2.5.4
* &lbrack;Baker&rbrack; Exibir Blocos UV individuais na janela de progresso de fça bake
* &lbrack;Baker&rbrack;&lbrack;UI&rbrack; Permite fazer bake rapidamente o Conjunto de Texturas atual por um novo botão
* &lbrack;Baker&rbrack; Permite ao usuário selecionar rapidamente um dos baker com ALT+CLIQUE ESQUERDO
* Atualize o Substance Engine para a versão 8.0.8
* &lbrack;Substance Engine&rbrack; Suporte a Cor Padrão em novos arquivos .sbsar
* &lbrack;Desempacotamento Automático&rbrack; Melhoria de desempenho
* &lbrack;Export&brack; Adicionar feedback visual para indicar qual resolução do Bloco UV difere do padrão do projeto
* &lbrack;Export&brack; Adicionar fator de tamanho de cena ao arquivo json de sombreador exportado
* &lbrack;Language&brack; Adicionar tradução para japonês
* &lbrack;UI&rbrack; Atualizar Sobre janela com controle de versão de dependências internas
* &lbrack;Scripting&rbrack;&lbrack;Python&rbrack; Permitir o gerenciamento de recursos de prateleira
* &lbrack;Scripting&rbrack;&lbrack;Python&rbrack; Permite saber quando um projeto está pronto para fazer bake e exportar
* &lbrack;Scripting&rbrack;&lbrack;Python&rbrack; Permitir saber quando uma prateleira terminou de rastrear recursos no disco
* &lbrack;Scripting&rbrack;&lbrack;Python&rbrack; Permitir a consulta da lista de blocos UV por Conjuntos de texturas
* &lbrack;Scripting&rbrack;&lbrack;Python&rbrack; Permitir atribuir visualização personalizada aos recursos de prateleira
* &lbrack;Scripting&rbrack;&lbrack;Python&rbrack; Permitir gerenciar prateleiras personalizadas
* &lbrack;Scripting&rbrack;&lbrack;Python&rbrack; Adicionar um índice de método em cada submódulo na documentação
* &lbrack;Scripting&rbrack;&lbrack;Python&rbrack; Novo estilo para a documentação
* &lbrack;Scripting&rbrack;&lbrack;Python&rbrack; Aprimoramento de recursos e documentação de prateleira
* &lbrack;Content&brack; Três novas predefinições de ferramenta para fazer pontos
* &lbrack;Shelf&rbrack; remove temporariamente “Exportar para o Substance share” durante a transição para a nova plataforma de Substance share

**Corrigido:**

* Falha ao usar monitores com diferentes resoluções
* Falha no Substance Engine com alguns projetos raros
* A atualização do visor falha com a opção Ocultar/Ignorar geometria excluída ao alternar as camadas
* &lbrack;Visualização 2D&rbrack; A Janela de visualização 2D pode estar ausente em alguns projetos
* &lbrack;Fazendo bake&rbrack; “Corresponder pelo nome da malha” ignora partes do objeto
* &lbrack;Pilha de camadas&rbrack; Clicar em um efeito de camada abre a pasta
* O Bloco UV &lbrack;Máscara de geometria&rbrack; ainda é contado na máscara mesmo ao reimportar a malha sem ela
* &lbrack;Máscara de geometria&rbrack; O menu do botão direito no visor não fornece as ferramentas corretas
* &lbrack;Engine&rbrack; Atrasos intensos em projetos específicos
* &lbrack;Scripting&rbrack; Alta latência com solicitações remotas de POST JSON no Windows
* A quantidade de Vram do &lbrack;Linux&rbrack; não é detectada corretamente com GPUs integradas específicas
* &lbrack;Auto desempacotar&rbrack; Trava ou desempacota longamente em alguns projetos

## Versão 6

### 6.2.2 (2020.2.2)

*(Lançado: 28 de setembro de 2020*)Resumo: **Versão secundária, correção de erro com algumas funções na API Python**

**Adicionado:**

* &lbrack;Desempenho&rbrack; Não calcula todos os Blocos UV ao usar a seleção de ID de cor
* &lbrack;Baker&rbrack;&lbrack;UI&rbrack; Exibir descrições do conjunto de texturas
* &lbrack;Baker&rbrack; Permitir salvar configurações do faço bake
* &lbrack;Baker&rbrack; Adicionar recolher tudo/expandir todas as opções para a guia Seleção
* &preto;Lista do conjunto de texturas&rbrack; Ocultar descrição quando vazio
* &lbrack;Blocos UV&rbrack;&lbrack;Lista do conjunto de texturas&rbrack; Clicar no Bloco UV deve expandir/recolher a lista
* &lbrack;Export&rbrack;&lbrack;UI&rbrack; Permitir o redimensionamento horizontal do painel Lista do conjunto de texturas
* &lbrack;Export&rbrack;&lbrack;UI&rbrack; Texto de dica de ferramenta consistente para Blocos UV e fluxo de trabalho do Conjunto de texturas com texturas não selecionadas
* &lbrack;Scripting&rbrack;&lbrack;Python&rbrack; Permitir o uso de predefinições de exportação para exportar texturas
* &lbrack;Scripting&rbrack;&lbrack;Python&rbrack; Adicionar um changelog na documentação
* &lbrack;Scripting&rbrack;&lbrack;Python&rbrack; Permite consultar todos os canais disponíveis em uma determinada pilha
* Melhorias na interface do console do &lbrack;Scripting&rbrack;&lbrack;Python&rbrack;

**Corrigido:**

* &lbrack;AMD&rbrack; Detecção incorreta de versão de driver desatualizada
* Falha ao reimportar uma malha com layout de Blocos UV diferente em alguns casos
* Falha ao usar partículas com UDIMs em malhas muito pesadas
* &lbrack;Blocos UV&rbrack; Falha ao exportar uma malha com informações de deslocamento em alguns casos
* &lbrack;Export&brack;&lbrack;Crash&rbrack; Exportar Visualização 2D no formato psd pode causar um travamento
* Importar imagens como sequências ao criar um projeto não funciona
* Mecanismo travado em um loop infinito
* &brack;Atalho&rbrack; A câmera gira sempre no modo de ajuste ao alterar os atalhos do modo de ajuste
* As malhas são sempre desempacotadas automaticamente quando reimportadas, mesmo que a opção esteja desativada
* &preto;Lista do conjunto de texturas&rbrack; O campo de texto da descrição às vezes não está totalmente visível durante a edição
* &preto;Lista do conjunto de texturas&rbrack; O menu suspenso para ocultar/revelar Conjuntos de texturas não está totalmente visível
* &preto;Lista do conjunto de texturas&rbrack; Clicar no ícone de olho não deve inserir o “Editar nome do conjunto de texturas”
* &preto;Configurações do conjunto de texturas&rbrack; A remoção de um canal também remove o canal abaixo
* &lbrack;Export&rbrack; Incluir tudo e Redefinir tudo não leva Blocos UV em consideração
* &lbrack;Baker&rbrack; Os baker desmarcados aparecem durante o processo de fça bake
* A atualização de resolução não é levada em consideração para mapas baked usados como entrada
* &lbrack;Blocos UV&rbrack;&lbrack;Visor&rbrack; Congelamento do Visor 3D ao adicionar Material inteligente após pasta com a máscara de Bloco UV selecionada
* &lbrack;Blocos UV&rbrack;&lbrack;Visor&rbrack; o Wireframe ainda está visível para ladrilhos ocultos com o modo tinta por
* &lbrack;Export&brack;&lbrack;Sketchfab&rbrack; Problemas com o tipo de assinatura “plus”
* &lbrack;Sketchfab&rbrack; A caixa de seleção “Este ativo é privado” não é exibida após alternar a conta
* &lbrack;Export&brack;&lbrack;Content&rbrack; “Ondulado” predefinições de pincel podem levar a problemas de desempenho
* &lbrack;Plug-in Photoshop&rbrack; Mensagem no registro: não compatível com o fluxo de trabalho do Bloco UV
* &lbrack;Scripting&rbrack;&lbrack;Python&rbrack; PYTHONPATH env var impede que o aplicativo seja iniciado
* &lbrack;Scripting&rbrack;&lbrack;Python&rbrack; Erro de ortografia na documentação do Python

### 6.2.1 (2020.2.1)

*(Lançado Em: 29 De julho De 2020*)Resumo: **Versão Secundária, Hotfix**

**Adicionado:**

* Adicione a variável de ambiente “SUBSTANCE_PAINTER_VRAM_BUDGET” para substituir o valor de VRam da GPU
* &lbrack;Blocos UV&rbrack;&lbrack;Desempenho&rbrack; Não calcular todos os blocos UV ao usar a ferramenta Preenchimento de polígono

**Corrigido:**

* &lbrack;Iray&rbrack; Salvar renderização retorna um erro e resulta em uma imagem em preto
* &lbrack;Linux&rbrack; Falha após a tela inicial no CentOS 7.3
* A quantidade de Vram do &lbrack;Linux&rbrack; não é detectada corretamente com configurações específicas
* &lbrack;Crash&rbrack; Abrindo um projeto com o nome do conjunto de texturas duplicado
* &lbrack;Engine&brack; Problema de invalidação de cache ao modificar uma máscara
* &preto;Lista do conjunto de texturas&rbrack; Efeito de fonte incorreto quando o conjunto de texturas está desativado

**Problemas Conhecidos:**

* &preto;Lista do conjunto de texturas&rbrack; Não é possível ocultar a descrição
* &preto;Lista do conjunto de texturas&rbrack; problemas de interface do usuário
* &lbrack;Iray&rbrack; a renderização de PSD não abre
* &lbrack;Plug-in Photoshop&rbrack; Não compatível com o fluxo de trabalho de Blocos UV

### 6.2.0 (2020.2.0)

*(Lançado em: 23 de julho de 2020*)Resumo: **Versão principal com novo fluxo de trabalho de Blocos UV, tinta entre Blocos UV e melhoria de desempenho**

**Adicionado:**

* Blocos UV (UDIMs)
* &lbrack;Blocos UV&rbrack; Tinta em blocos UV
* &lbrack;Blocos UV&rbrack; Permite escolher entre o fluxo de trabalho novo e herdado para Blocos UV
* &lbrack;Blocos UV&rbrack; Importar sequências de imagens UDIMs/Bloco UV como um recurso
* &lbrack;Blocos UV&rbrack; Adicionar lista de Blocos UV por conjunto de textura na janela Lista de conjuntos de textura
* &lbrack;Blocos UV&rbrack; Permite editar a resolução de vários Blocos UV de uma vez nas Configurações do Conjunto de Texturas
* &lbrack;Blocos UV&rbrack;&lbrack;Visualização 2D&rbrack; Exibir Blocos UV como uma grade
* &lbrack;Blocos UV&rbrack;&lbrack;Visualização 2D&rbrack; Novo botão de visor para exibir ou ocultar informações de Blocos UV
* &lbrack;Blocos UV&rbrack; Alterna a ferramenta de pintura para canal único por padrão para projetos de Bloco UV
* &lbrack;Blocos UV&rbrack; Novo botão na barra de ferramentas contextual para ignorar Blocos UV mascarados ao pintar
* &lbrack;Blocos UV&rbrack;&lbrack;Pilha de camadas&rbrack; Novos ícones de pilha de camadas para melhorar o desempenho
* &lbrack;Blocos UV&rbrack;&lbrack;Pilha de camadas&rbrack; Aprimorar ícones de Tinta e Preenchimento na barra de ferramentas
* &lbrack;Máscara de Bloco UV&rbrack;&lbrack;Visualização 2D&rbrack; Permite incluir ou excluir vários Blocos UV de uma vez (clique com o botão esquerdo, CTRL+clique com o botão esquerdo)
* &preto;Máscara de Bloco UV&rbrack; Nova máscara de Bloco UV a ser incluída, exclui blocos por camada com um novo ícone
* &lbrack;Máscara de Bloco UV&rbrack;&lbrack;Pilha de camadas&rbrack; Exibir o número de Blocos UV no ícone de máscara de Blocos UV quando nem todos estiverem incluídos
* &lbrack;Máscara de Bloco UV&rbrack;&lbrack;2D/Visualização 3D&rbrack; Adicionar efeito hover para visualizar Blocos UV sob o cursor
* &lbrack;Blocos UV&rbrack;&lbrack;Baker&rbrack; Permite selecionar e fazer bake Blocos UV específicos
* &lbrack;Blocos UV&rbrack;&lbrack;Baker&rbrack; Adicionar opções de seleção para Conjuntos/Blocos UV de Textura
* &lbrack;Blocos UV&rbrack;&lbrack;Baker&rbrack; Clique com o botão direito do mouse na opção de menu para selecionar Blocos UV em um Conjunto de Texturas
* &lbrack;Blocos UV&rbrack;&lbrack;Baker&rbrack; Permite a seleção rápida no Conjunto de Texturas/Blocos UV arrastando
* &lbrack;Blocos UV&rbrack;&lbrack;Baker&rbrack; Substituir os botões “Tudo” e “Nenhum” nos Mapas de malha por opções de seleção mais explícitas
* &lbrack;Blocos UV&rbrack;&lbrack;Baker&rbrack; Exibir o número de texturas a serem feitas bake
* &lbrack;Blocos UV&rbrack;&lbrack;Exportar&rbrack; Permite selecionar e exportar Blocos UV específicos
* &lbrack;Blocos UV&rbrack;&lbrack;Exportar&rbrack; Permite a seleção rápida de Blocos UV arrastando
* &lbrack;Blocos UV&rbrack;&lbrack;Exportar&rbrack; Adicionar opções de menu suspenso para Blocos UV
* &lbrack;Blocos UV&rbrack;&lbrack;Exportar&rbrack; Tornar algumas predefinições de exportação indisponíveis se não funcionarem com Blocos UV (Adobe Dimension, Sketchfab, glTF, USD)
* &lbrack;Blocos UV&rbrack;&lbrack;Conteúdo&rbrack; Atualiza as predefinições de exportação para usar a nova tag $udim
* &lbrack;Blocos UV&rbrack; Melhorar o relatório de erros ao importar malhas com Ilhas UV sobrepostas
* &lbrack;Blocos UV&rbrack; Blocos UV compatíveis no Iray
* &lbrack;Blocos UV&rbrack;&lbrack;Scripting&rbrack; Adicionar documentação de exportação de Bloco UV ao documento Python
* Desempenho
* &lbrack;Desempenho&rbrack; Novo botão na barra de ferramentas contextual para pausar o cálculo do mecanismo ao trabalhar (SHIFT+ESC)
* &lbrack;Desempenho&rbrack; Abertura mais rápida do projeto atrasando o cálculo do cache do Conjunto de Texturas
* &lbrack;Performance&brack; Não espere até que os mapas de malha sejam carregados ao abrir o projeto
* &lbrack;Performance&rbrack;&lbrack;2D/Visualização 3D&rbrack; Não calcular o canal da Máscara no visor quando não estiver em uso
* &lbrack;Desempenho&rbrack; Não bloqueia o aplicativo ao carregar mapas de malha exibidos nas viewports
* &lbrack;Desempenho&rbrack; Melhorar a velocidade de salvamento incremental ao salvar um projeto
* &lbrack;Desempenho&rbrack;&lbrack;Baker&rbrack; Alterar configurações de dilatação padrão para melhorar o tempo de salvamento e o tamanho do projeto
* &lbrack;Desempenho&rbrack;&lbrack;Baker&rbrack; Alterne para tons de cinza em Baker específicos para melhorar o tempo de salvamento e o tamanho do projeto
* &lbrack;Performance&rbrack;&lbrack;Export&rbrack; Melhorar o desempenho do mecanismo para exportar texturas mais rapidamente
* &lbrack;Desempenho&rbrack;&lbrack;Exportar&rbrack; Melhorar a capacidade de resposta ao abrir a caixa de diálogo de exportação com muitos Conjuntos de textura
* &lbrack;Performance&rbrack;&lbrack;Export&rbrack; Melhorar o desempenho ao alternar para a guia “Lista de exportações”
* &lbrack;Performance&rbrack;&lbrack;Iray&rbrack; Reduzir tempo de inicialização do Iray
* Outro
* &lbrack;Baker&rbrack; Adicionar opções de seleção para Conjuntos de Textura
* Mover o gerenciamento de instância de sombreamento para as configurações do conjunto de textura
* &lbrack;2D/Visualização 3D&rbrack; Adiciona mensagem na parte inferior do visor para indicar qual tipo de máscara é editado
* &lbrack;Pilha de camadas&rbrack; Nova opção nas configurações para alternar entre miniaturas novas e antigas
* &lbrack;Pilha de camadas&rbrack; Adicionar feedback visual para indicar o estado de carregamento das miniaturas
* &lbrack;Proj&rbrack; Novo modo de projeção “Preenchimento (Corresponder por UV-Tile)” para carregar as sequências de imagens
* &lbrack;Proj&rbrack; Alterar modo de projeção de camadas de preenchimento para “Preenchimento (Corresponder por UV-Tile)” em casos específicos
* &lbrack;Content&brack; Otimizar predefinições do pincel a carvão para melhorar o desempenho
* Atualize o Iray para a versão 2020.0.0
* &lbrack;Export&brack; Desabilitar a guia Lista de Exportações quando nada estiver selecionado
* Desempacotar automaticamente
* &lbrack;Auto Unwrap&rbrack; Melhorar a taxa de sucesso do processo de desencapsulamento automático
* &lbrack;Auto Unwrap&rbrack; Parametrização aprimorada para aumentar a velocidade e estabilidade

**Corrigido:**

* &lbrack;Alembic&rbrack; Facesets são ignoradas ao importar arquivos
* &lbrack;Alembic&rbrack; Tempo de carregamento infinito com arquivos específicos
* &lbrack;Import&rbrack; Sequência de imagem UDIM incorreta é importada quando apenas a extensão do arquivo difere
* &lbrack;Falha&rbrack; Tentar abrir um projeto bloqueado por outro processo leva a uma falha
* &lbrack;Projeção&rbrack; Artefatos em malha duplicada ao usar projeção triplanar
* O canal de Emissivo do &lbrack;Export&rbrack; não é exportado com o formato USD
* &lbrack;Content&brack; Material inteligente “Carvão” contém traços de tinta

**Problemas Conhecidos:**

* &preto;Lista do conjunto de texturas&rbrack; Não é possível ocultar a descrição
* &preto;Lista do conjunto de texturas&rbrack; problemas de interface do usuário

### 6.1.3 (2020.1.3)

*(Lançado: 16 De junho De 2020*)Resumo: **Correção De Erros**

**Adicionado:**

* &lbrack;Export&brack; Adicionar configurações de deslocamento no arquivo json de parâmetros de Sombreador

**Corrigido:**

* &lbrack;Falha&rbrack;&lbrack;Motor&rbrack; Falha ao tentar apagar e substituir canais existentes
* &lbrack;Crash&rbrack; Alterar sombreador após pintar uma máscara em camadas de material
* &lbrack;Crash&rbrack;&lbrack;Engine&rbrack; Falha com alguns projetos pesados
* &lbrack;Baker&rbrack; Corresponder por nome não funciona com OBJ exportado do zBrush
* &lbrack;Deslocamento&rbrack;&lbrack;SVT&rbrack; Texturas não são exibidas na abertura do projeto quando o deslocamento está ativado
* &lbrack;Export&brack; Algumas texturas são exportadas cinza uniforme
* &brack;Exportar&rbrack; Conjuntos de Textura Desativados não devem ser exportados para predefinições de exportação Dimension e Sketchfab
* &lbrack;Scripting&rbrack;&lbrack;JavaScript&rbrack; Falha ao usar a API JavaScript para acessar a configuração de exportação no evento onProjectOpened
* &lbrack;Scripting&rbrack;&lbrack;Javascript&rbrack; onExportFinished() não é chamado após uma exportação

### 6.1.2 (2020.1.2)

*(Lançado: 28 de maio de 2020*)Resumo: **Correção de erros com atualização de Substance Engine e Baker**

**Adicionado:**

* &lbrack;Baker&rbrack; Atualiza para a versão mais recente
* &lbrack;Baker&rbrack; Novo método de amostragem em Oclusão de ambiente, Curvatura, baker de Thickness
* Atualize para a versão mais recente do Substance Engine
* &lbrack;Scripting&rbrack;&lbrack;Python&rbrack; Permitir criação de ResourceID para recursos do projeto
* &lbrack;Scripting&rbrack;&lbrack;Python&rbrack; Permitir consulta de informações de canal
* &lbrack;Scripting&rbrack;&lbrack;Python&rbrack; Adicionar funções dryrun e callback para simular a exportação de textura

**Corrigido:**

* &lbrack;Baker&rbrack; Normais incorretos no baker World Space Normals usando um Mapa normal tangente em casos específicos
* &lbrack;Baker&rbrack; Erro ao fazer bake Oclusão de ambiente com Optix quando não há poli alto
* &lbrack;Traçados dinâmicos&rbrack; Atraso ao carregar um Conjunto de Texturas específico
* &lbrack;Export&brack; Não deve exportar os conjuntos de texturas desativados para USD, glTF
* &lbrack;Scripting&rbrack;&lbrack;JavaScript&rbrack; Não é possível editar as novas configurações de baker de curvatura
* &lbrack;Scripting&rbrack;&lbrack;JavaScript&rbrack; alg.texturesets.addChannel() não retorna um erro em alguns casos
* &lbrack;Scripting&rbrack;&lbrack;JavaScript&rbrack; Erro de ortografia na documentação da API Javascript para setProjectExportOptions()
* &lbrack;Scripting&rbrack;&lbrack;JavaScript&rbrack; Sempre exporta todos os conjuntos de texturas
* &lbrack;Scripting&rbrack;&lbrack;Python&rbrack; sys.executable retorna um caminho para python.exe em vez de Substance Painter
* Cache de textura não compatível com o sistema operacional Mac e Windows/Linux
* &lbrack;Livelink UE4&rbrack; Somente o último material é usado para todos os conjuntos de texturas em uma malha combinada

**Problemas Conhecidos:**

* &lbrack;Export&brack;&lbrack;Dimension&rbrack;&lbrack;Skecthfab&rbrack; Não deve exportar os conjuntos de textura desativados
* &lbrack;Crash&rbrack; Alterar sombreador depois de pintar uma máscara em camadas de material

### 6.1.1 (2020.1.1)

*(Lançado: 05 De maio De 2020*)Resumo: **Hotfix**

**Adicionado:**

* &preto;Exportar&rbrack; Estado substituído de feedback visual no TextureSet

**Corrigido:**

* &lbrack;O tamanho da janela do Exportador Export&brack; é muito grande no monitor de resolução especial e não pode ser redimensionado
* &preto;Opções de exportação&rbrack; não são salvas após a exportação
* &lbrack;Export&brack; Falha ou não é possível exportar com a predefinição de exportação “do cache”
* &lbrack;Export&brack; Cancelar a exportação gera um mapa vazio adicional inesperado
* &preto;Exportar&rbrack; Corrigir configurações de predefinição de exportação virtual
* &lbrack;Python&rbrack; a variável env PYTHONPATH não é levada em consideração
* &lbrack;Python&rbrack;&lbrack;Exportar&rbrack; cancelar a exportação via Python retorna um erro de exceção
* &lbrack;Python&rbrack;&lbrack;Export&rbrack; export_project_textura resultado incorreto com o formato de arquivo psd
* &lbrack;Baker&rbrack; Falha no Linux com Rastreamento de raios do GPU

**Problemas Conhecidos:**

* &lbrack;JavaScript&rbrack; Não é possível editar as novas configurações de baker de curvatura
* &lbrack;JavaScript&rbrack;&lbrack;Exportar&rbrack; Sempre exporta todos os conjuntos de texturas
* &lbrack;Export&rbrack;&lbrack;USD&rbrack; Não deve exportar os conjuntos de texturas desativados
* &lbrack;Crash&rbrack; Alterar sombreador depois de pintar uma máscara em camadas de material

### 6.1.0 (2020.1.0)

*(Lançado: 22 de abril de 2020*)Resumo: **Versão principal com nova textura e exportador de malha (com deslocamento e mosaico), desencapsulamento UV atualizado com mais controles, novos baker, nova API python de script, melhor UX para projeção de decalques e novo conteúdo**

**Adicionado:**

* Nova textura e exportador de malha
* &lbrack;Exportar&rbrack; Nova interface de exportador
* &lbrack;Export&brack;&lbrack;Guia Exportar&rbrack; Permite a seleção dos canais de mapas que são exportados por Conjunto de Textura
* &lbrack;Export&brack;&lbrack;Guia Exportar&rbrack; Permite a modificação do tamanho do Conjunto de Textura para todos os Conjuntos de Textura em uma ação
* &lbrack;Export&brack;&lbrack;Guia Exportar&rbrack; Permite um modelo diferente por Conjunto de Textura (exceto para USD, glTF, Sketchfab e Dimension)
* &lbrack;Export&brack;&lbrack;Guia Exportar&rbrack; Ativação e desativação rápidas de mapas e Conjuntos de texturas
* &lbrack;Export&brack;&lbrack;Guia Exportar&rbrack; A resolução de exportação 8192x8192 não é mais experimental
* &lbrack;Export&brack;&lbrack;Guia Exportar&rbrack; Permite a modificação do formato do arquivo e a profundidade de bits por mapa
* &lbrack;Export&brack;&lbrack;Guia Exportar&rbrack; Permitir redefinição para os valores de parâmetros padrão
* &lbrack;Export&brack;&lbrack;Guia Exportar&rbrack; Permite que as configurações sejam salvas sem exportar
* &lbrack;Exportar&rbrack;&lbrack;guia Modelos de saída&rbrack; Renomeia a guia “Configuração” para a guia “Modelos de saída”
* &lbrack;Export&brack;&lbrack;guia Modelos de saída&rbrack; Permitir definição de formato de arquivo e profundidade de bits por mapa predefinido
* &lbrack;Export&brack;&lbrack;Lista de guias de exportação&rbrack; Nova guia de visualização para resumir e visualizar o processo de exportação
* &lbrack;Importar/Exportar malha&rbrack; Otimização do desempenho do tempo de importação/exportação
* &lbrack;Exportar malha&rbrack; Exportar malha em FBX
* &preto;Exportar malha&rbrack; Exportar malha com deslocamento e mosaico
* &lbrack;Exportar malha&rbrack;&lbrack;UI&rbrack; Novas configurações para recalcular o vértice normal, aplicar triangulação
* &lbrack;Exportar malha&rbrack; Exportar topologia de malha original com novos UVs gerados pelo desencapsulamento automático
* Desencapsulamento automático UV atualizado com mais controles
* &lbrack;Desempacotamento UV&rbrack;&lbrack;UI&rbrack; Adicionar configuração para ativar o desempacotamento UV automático na nova janela do projeto
* &lbrack;UV Unwrapping&rbrack;&lbrack;UI&rbrack; Novas opções para controlar as etapas de abertura (emendas, abertura, embalagem)
* &lbrack;Desempacotamento UV&rbrack;&lbrack;UI&rbrack; Permitir a conservação de emendas/desempacotamento/embalagem de abertura existentes
* &lbrack;Desempacotamento UV&rbrack;&lbrack;UI&rbrack; Novas opções para recalcular totalmente as etapas de desempacotamento
* &lbrack;UV Unwrapping&rbrack;&lbrack;UI&rbrack; Nova Opção para controlar o tamanho da margem (nenhum, pequeno, médio e grande)
* Novos Baker
* &lbrack;Baker&rbrack; Substituir a curvatura antiga pela nova curvatura da malha
* &lbrack;Baker&rbrack; Adicionar a opção corresponder pelo nome para ignorar a face de fundo no baker “Oclusão de ambiente”
* &lbrack;Baker&rbrack; Adicionar opção de plano horizontal no baker “Oclusão de ambiente”
* Nova API de script do Python (3.7.6)
* &lbrack;Python&rbrack;&lbrack;UI&rbrack; Novo menu de scripts para Python
* &lbrack;Python&rbrack;&lbrack;UI&rbrack; Nova documentação em Python no menu Ajuda
* &lbrack;Python&rbrack; Expor módulos Substance Painter python: substance_painter, alg, display, project.setting, project, texturesets, ui
* &lbrack;Python&rbrack; Expor novo módulo Python “substance_painter”
* &lbrack;Python&rbrack; Expor novo submódulo Python: alg, display, log, projeto, recurso, conjuntos de texturas, ui
* &lbrack;Python&rbrack; Ouvinte para alterações no projeto
* &lbrack;Python&rbrack; Novos exemplos na documentação do Python
* &lbrack;JavaScript&rbrack;&lbrack;UI&rbrack; Menu de plug-ins substituído pelo JavaScript
* &lbrack;Viewport&rbrack; Permitir a criação de uma projeção de decalque “arrastando/soltando + ALT” um recurso da prateleira
* Novo conteúdo
* &lbrack;Content&brack; 5 novos materiais de decalque do Substance Source
* &lbrack;Content&brack; Adicionar novos modelos de projeto e exportar predefinições para o renderizador Maxwell
* &lbrack;Content&brack; Adicionar modelo de projeto para exportação do Keyshot 9
* &lbrack;Content&rbrack; Atualizar a predefinição de exportação do Keyshot 9 para suportar deslocamento e emissivo
* &lbrack;Conteúdo&rbrack;&lbrack;Exportador&rbrack; Atualização de todas as predefinições de exportação para corresponder às versões mais recentes dos mecanismos de jogo e renderizadores
* &lbrack;Content&rbrack;&lbrack;Exportador&rbrack; Atualiza arquivos de predefinições de exportação para usar o novo formato e configurações de pontilhamento
* &lbrack;Content&rbrack; Novos modelos e sombreadores para suportar material VRay (VRayMtl)
* &lbrack;Pilha de camadas&rbrack; Permitir exclusão de efeitos de camada usando ícone de lixeira ou atalho de teclado Excluir
* Remover o Substance Source de plug-in (use o iniciador com a funcionalidade “enviar para”)
* &lbrack;Windows&rbrack; Não exibir aviso TDR em GPUs sofisticadas

**Corrigido:**

* Problemas de tradução na caixa de diálogo Novo arquivo de projeto
* &lbrack;Baker&rbrack; Configurar “Salvar arquivo de cena pré-processado” não funciona mais
* &lbrack;Projeção Planar&rbrack; A projeção não funciona em malhas com UVs repetidos
* &lbrack;Decalque&rbrack; Diferença de comportamento no canal normal ao usar modos diferentes de projeção da camada de preenchimento
* &lbrack;Borrar&rbrack;&lbrack;Clonar&rbrack; O artefato pode aparecer ao pintar na máscara
* &lbrack;Engine&brack; Falha com conteúdo de camada específico
* &lbrack;Engine&rbrack; Falha aleatória ao pintar em alguns casos
* &preto;Ponto de ancoragem&rbrack; A referência a uma máscara vazia sempre retorna branco
* &lbrack;Export&brack; Camada não considerada em algumas configurações de pilha específicas
* &lbrack;Exportar malha&rbrack; Não é possível exportar com caminho que contém caracteres especiais
* &lbrack;Exportar malha&rbrack; Não é possível ler arquivos glTF quando exportados do Linux ou MacOS
* &lbrack;Importar malha&rbrack; Reimportar DAE, PLY ou glTF não funciona como pretendido

**Problemas Conhecidos:**

* &lbrack;Scripting&rbrack;&lbrack;JavaScript&rbrack; Não é possível editar as novas configurações de baker de curvatura
* &lbrack;Baker&rbrack; Falha no Linux com Rastreamento de raios do GPU
* &lbrack;Export&rbrack;&lbrack;USD&rbrack; Não deve exportar os conjuntos de texturas desativados
* &lbrack;Crash&rbrack; Alterar sombreador depois de pintar uma máscara em camadas de material

## Versão 5

### 5.3.3 (2019.3.3)

*(Lançado em: 06 de fevereiro de 2020*)Resumo: **Correção de erros com a atualização para o Iray 2019.3**

**Adicionado:**

* Atualização para o Iray 2019.3
* &lbrack;Log&rbrack; Indica bios desatualizado para CPU Ryzen levando a falha durante fça bake
* &lbrack;ABR&rbrack; Extrair ABR alfa para prateleira

**Corrigido:**

* &lbrack;Baker&rbrack; falha na Faz bake se a malha de alto-polígono não tiver UVs
* &lbrack;Linux&rbrack; Os atalhos de mouse personalizados não são salvos
* &lbrack;Pincel&rbrack; O contorno desaparece com algumas formas alfa
* &lbrack;Tablet&rbrack; Detecção incorreta ao mover controles deslizantes
* &lbrack;Atalhos&rbrack; Não é possível configurar nenhum atalho com “Ctrl+Alt+MouseClick”
* &lbrack;Shelf&rbrack; Não é possível ver a dica de ferramenta do recurso ao usar um tablet com caneta
* A predefinição &lbrack;Visualização 2D&rbrack;&lbrack;Export&rbrack; não leva em consideração as informações normais
* Congela ao pintar em alinhamento UV com determinados pincéis
* Pintar sob um filtro cria artefatos no traçado em andamento
* &lbrack;Visor&rbrack; Cache de textura incorreto no visor após a reimportação de uma malha
* &lbrack;Crash&rbrack; Erro ao salvar após exportar para o Photoshop
* &lbrack;Crash&rbrack; Gravando símbolos especiais no prefixo ao importar recursos
* &lbrack;Crash&rbrack; Clique na referência nas Propriedades do Ponto de Ancoragem
* &preto;Pontos de ancoragem&rbrack; O canal não é atualizado quando há um filtro entre o ponto de ancoragem e a referência
* O link de URL do Iray no menu Ajuda não funciona

**Problemas Conhecidos:**

* &lbrack;Desempacotamento UV&rbrack; O processamento de malhas de alta polarização pode demorar muito tempo
* &lbrack;Desempacotamento UV&rbrack; Vértices nas mesmas coordenadas são mesclados
* &lbrack;Desempacotamento UV&rbrack; A Geração UV pode falhar em algumas partes da malha em alguns casos raros
* &lbrack;UV Unwrapping&rbrack; Proporção de texel não uniforme ou altamente distorcida em uma única Ilha UV em alguns casos
* &lbrack;Desempacotamento UV&rbrack; Proporção de texel não uniforme entre Conjuntos de Textura
* A Ilha UV gerada pelo &lbrack;UV Unwrapping&rbrack; pode ser muito alongada e, em alguns casos, não cabe no espaço UV
* &preto;Desempacotamento UV&rbrack; Faces degeneradas ou faces de malha não triangulares com bordas pequenas ou sobrepostas podem não ter o UV desempacotado

### 5.3.2 (2019.3.2)

*(Lançado: 21 De Janeiro De 2020*)Resumo: **Correção De Erros**

**Corrigido:**

* Abrir um projeto que foi salvo no modo de canal individual não exibe a malha
* A janela de visualização nem sempre é atualizada ao pintar sob uma camada usando a ferramenta clone

**Problemas Conhecidos:**

* &lbrack;Baker&rbrack; Falha relacionada a multi-threading em CPUs Ryzen
* &lbrack;Desempacotamento UV&rbrack; O processamento de malhas de alta polarização pode demorar muito tempo
* &lbrack;Desempacotamento UV&rbrack; Vértices nas mesmas coordenadas são mesclados
* &lbrack;Desempacotamento UV&rbrack; A Geração UV pode falhar em algumas partes da malha em alguns casos raros
* &lbrack;UV Unwrapping&rbrack; Proporção de texel não uniforme ou altamente distorcida em uma única Ilha UV em alguns casos
* &lbrack;Desempacotamento UV&rbrack; Proporção de texel não uniforme entre Conjuntos de Textura
* A Ilha UV gerada pelo &lbrack;UV Unwrapping&rbrack; pode ser muito alongada e, em alguns casos, não cabe no espaço UV
* &preto;Desempacotamento UV&rbrack; Faces degeneradas ou faces de malha não triangulares com bordas pequenas ou sobrepostas podem não ter o UV desempacotado

### 5.3.1 (2019.3.1)

*(Lançado: 20 De dezembro De 2019*)Resumo: **Hotfix**

**Corrigido:**

* Falha ao trabalhar em malhas com Projeções UV específicas
* &lbrack;ABR&rbrack; Falha ao alternar entre predefinições Photoshop
* &lbrack;Linux&rbrack; Não é possível iniciar o Substance Painter no CentOS 7.4 devido a um problema de dependência do libGLX
* &lbrack;Baker&rbrack; Falha ao fazer bake após usar Arquivo > Limpar
* &lbrack;Baker&rbrack; Fazendo bake o diálogo de progresso congela após cancelar
* &lbrack;Baker&rbrack; Fazer bake a malha após exportar as texturas não funciona
* &lbrack;Baker&rbrack; Usar “Corresponder por nome” resulta com mapas de malha pretos
* &lbrack;Baker&rbrack; A gaiola não é levada em consideração
* &lbrack;Shelf&rbrack; Importar arquivos de PSD leva a imagens quebradas
* &lbrack;Amostra&rbrack; O projeto de amostra “Mat” possui câmeras quebradas e predefinição de exportação incorreta

**Problemas Conhecidos:**

* &lbrack;Baker&rbrack; Falha relacionada a multi-threading em CPUs Ryzen
* &lbrack;Desempacotamento UV&rbrack; O processamento de malhas de alta polarização pode demorar muito tempo
* &lbrack;Desempacotamento UV&rbrack; Vértices nas mesmas coordenadas são mesclados
* &lbrack;Desempacotamento UV&rbrack; A Geração UV pode falhar em algumas partes da malha em alguns casos raros
* &lbrack;UV Unwrapping&rbrack; Proporção de texel não uniforme ou altamente distorcida em uma única Ilha UV em alguns casos
* &lbrack;Desempacotamento UV&rbrack; Proporção de texel não uniforme entre Conjuntos de Textura
* A Ilha UV gerada pelo &lbrack;UV Unwrapping&rbrack; pode ser muito alongada e, em alguns casos, não cabe no espaço UV
* &preto;Desempacotamento UV&rbrack; Faces degeneradas ou faces de malha não triangulares com bordas pequenas ou sobrepostas podem não ter o UV desempacotado

### 5.3.0 (2019.3.0)

*(Lançado em: 17 de dezembro de 2019*)Resumo: **Versão principal com aprimoramento da experiência do usuário de pintura manual, trabalho com tablets, desencapsulamento UV automático em beta (0.3.0) e conteúdo novo diversificado para pintura manual**

**Adicionado:**

* Integrar a versão 0.3.0 de desenrolamento automático de UV no Substance Painter
* &lbrack;Desencapsulamento UV&rbrack; Desencapsulamento UV automático no Substance Painter quando nenhum UV estiver presente ou UVs parciais
* &lbrack;UV unwrapping&rbrack; Uma configuração global para ativá-lo e desativá-lo
* &lbrack;UV unwrapping&rbrack; Versão relatada no arquivo de registro
* &lbrack;Desempacotamento UV&rbrack;&lbrack;UI&rbrack; Indicar progresso do Desempacotamento UV
* &lbrack;UI&rbrack; Novas configurações na barra de ferramentas contextual para selecionar a visualização do pincel: visualização completa, contorno e mira
* &lbrack;Tool&brack; Novo modo de mesclagem avançado na seção alfa: Clarear (máximo) além de Normal
* &lbrack;Pilha de camadas&rbrack; Opção de correção de gama por camada para alfa ou máscara (menu do botão direito do mouse)
* &lbrack;Pilha de camadas&rbrack;&lbrack;UI&rbrack; Adicionar ícone &#39;i&#39; quando uma camada alfa for corrigida quanto à gama
* &lbrack;Tablet&rbrack;&lbrack;Tool&rbrack; Expor pressão mínima para tamanho e fluxo
* &lbrack;Tablet&rbrack;&lbrack;UI&rbrack; Nova configuração na barra de ferramentas contextual para selecionar a pressão da curva: linear, fácil de entrar, fácil de sair
* &lbrack;Tablet&rbrack;&lbrack;UX&rbrack; Add Ctrl+Alt+clique para rolar
* Importar predefinições de pincel do Photoshop (formato ABR)
* &lbrack;ABR&rbrack; Suporte parâmetros de Forma
* &lbrack;ABR&rbrack; Suportar parâmetros de dinâmica da forma
* &lbrack;ABR&rbrack; Suporte Parâmetros de transferência
* &lbrack;ABR&rbrack; Suporte a parâmetros de dispersão
* &lbrack;ABR&rbrack;&lbrack;Traçados dinâmicos&rbrack; Suporte Arredondamento e inversão
* &lbrack;ABR&rbrack;&lbrack;Shelf&rbrack; Expor a estrutura da pasta de pincéis no Editor de Filtros
* &lbrack;Abr&brack;&lbrack;Prateleira&rbrack; Adicionar ícone do Photoshop em miniaturas
* &lbrack;ABR&rbrack;&lbrack;Shelf&rbrack; Adicionar lista de parâmetros não suportados na miniatura detalhada do ABR
* &lbrack;Tool&brack;&lbrack;Traçados dinâmicos&rbrack; Nova configuração de traçado dinâmico para controlar quantas sementes aleatórias gerar
* &lbrack;Tool&brack;&lbrack;UI&rbrack; Adicionar nova distribuição e configurações de eixo para dispersão de tremulação
* &lbrack;Atalho&rbrack; Adicione Ctrl+Shift+B para abrir a janela de Fça bake
* &lbrack;UI&rbrack;&lbrack;Menu&rbrack; Adicionar entrada no menu “Editar” para abrir a janela de Fça bake
* &lbrack;UI&rbrack;&lbrack;Configurações&rbrack; Aprimoramento do alinhamento da lista de atalhos
* &lbrack;UI&rbrack; Substitui ícones de controles de pressão (tamanho e fluxo) por botões de ligar/desligar
* &lbrack;Visor&rbrack; Permitir focalizar o visor 2D e 3D separadamente
* Atualize para QT 5.12.5
* &lbrack;UI&rbrack; Indicar progresso do carregamento da malha
* &lbrack;Substance&rbrack; Adicionar suporte para faixa suave e não fixa com controles deslizantes
* &lbrack;Substance&rbrack; Aumenta a precisão dos parâmetros Substance até 6 decimais
* &lbrack;Substance&rbrack; Leve em consideração a etapa definida por um parâmetro
* &lbrack;Substance&rbrack; Otimizar a geração de Traçado Dinâmico com suporte de condições em userdata
* &lbrack;Substance&rbrack; Permite designar uma saída de gráfico como uma máscara para todos os canais via userdata
* &lbrack;Content&rbrack; Atualizar projeto de amostra &#39;Mat&#39; com topologia amigável ao deslocamento, novo mapa de ID e novas câmeras
* &lbrack;Content&brack; Integrar 3 novos filtros (MatFx): Quadrinhos, Aquarela, Tinta a óleo (inspirado no trabalho de Emrecan Cubukcu)
* &brack;Content&brack; Integra 102 predefinições de pincel Photoshop dos pacotes de Kyle T. Webster
* &lbrack;Content&brack; Integrar 18 novas predefinições de pincel: Seta do rolo de Tinta, Texto de aviso do rolo de Tinta, Carvão fino e muito mais
* &brack;Content&brack; Integrar 9 novas alfas: Rolo de Tinta do Criador de Pincel, Photoshop do Criador de Pincel, Padrões de pincel e muito mais
* &lbrack;Content&brack; Integrar 2 novas predefinições de ferramenta: Guache Dense e Gouache Faded
* &lbrack;Content&brack; Integrar 1 novo gerador : verificador UV (realçar Ilhas UV e emendas)
* &lbrack;Content&brack; Integrar 2 nova predefinição de exportação: Keyshot 9+ e Spark AR Studio
* &lbrack;Content&brack; Integrar 1 novo modelo de projeto : Spark AR Studio (Facebook)

**Corrigido:**

* &preto;Tablet&rbrack; Desfazer traçados da caneta (Ctrl+Z) atrasa mais do que desfazer traçados do mouse
* &lbrack;Tablet&rbrack; A pressão inicial e final não é considerada ao desenhar uma linha reta
* &lbrack;Tablet&rbrack; O primeiro carimbo é desenhado duas vezes ao usar uma linha reta
* &Preenchimento;Tablet&rbrack; Melhorar o suporte para atalhos de tablet Huion
* &lbrack;Tablet&rbrack; Melhorar o suporte para botões de caneta Huion
* &preto;Tablet&rbrack; Deslocamento entre a visualização do pincel e o carimbo desenhado
* &Preenchimento;O uso do tablet&rbrack; atalhos para modificar pincéis com caneta leva a baixo desempenho em casos raros
* &lbrack;Tablet&rbrack; Atraso ao pintar em uma camada específica
* Texturas embaçadas podem ocorrer em casos raros ao alternar entre viewport
* &lbrack;UI&rbrack;&lbrack;Substance&rbrack; As entradas de imagem nem sempre são exibidas
* Limpar não remove as predefinições da prateleira que foram importadas em um projeto
* &lbrack;Tool&rbrack;&lbrack;Dynamic Stroke&rbrack; Problema de desempenho ao ajustar a Contagem Cíclica do Carimbo
* Problemas de atualização ao pintar no modo de visor 3D/2D em casos raros
* Pintar um traçado muito longo pode causar congelamento
* &lbrack;Tool&brack; Problema de desempenho ao pintar com traçados dinâmicos específicos
* &lbrack;UI&rbrack; A barra de ferramentas contextual ainda exibe as propriedades do pincel ao selecionar uma pasta
* Os valores do eixo de simetria não são redefinidos
* A importação de texturas EXR com valores de ponto flutuante é totalmente preta
* Alt+clique em um canal para isolar não funciona para filtro e gerador
* &lbrack;Export&brack; O projeto específico falha na exportação
* &lbrack;Substance&rbrack; Valor padrão incorreto na lista suspensa se o parâmetro estiver oculto por Visível Se
* &lbrack;Sombreador&rbrack; Os canais definidos por meio da Camada de material não são classificados da mesma maneira na interface
* &lbrack;Shelf&rbrack; Os metadados de predefinições não são salvos no disco

**Problemas Conhecidos:**

* &lbrack;Desempacotamento UV&rbrack; O processamento de malhas de alta polarização pode demorar muito tempo
* &lbrack;Desempacotamento UV&rbrack; Vértices nas mesmas coordenadas são mesclados
* &lbrack;Desempacotamento UV&rbrack; A Geração UV pode falhar em algumas partes da malha em alguns casos raros
* &lbrack;UV Unwrapping&rbrack; Proporção de texel não uniforme ou altamente distorcida em uma única Ilha UV em alguns casos
* &lbrack;Desempacotamento UV&rbrack; Proporção de texel não uniforme entre Conjuntos de Textura
* A Ilha UV gerada pelo &lbrack;UV Unwrapping&rbrack; pode ser muito alongada e, em alguns casos, não cabe no espaço UV
* &preto;Desempacotamento UV&rbrack; Faces degeneradas ou faces de malha não triangulares com bordas pequenas ou sobrepostas podem não ter o UV desempacotado
* A amostra do metamat tem alguns problemas com câmeras importadas

### 5.2.3 (2019.2.3)

*(Lançado: 23 de outubro de 2019*)Resumo: **Versão de correção de erros**

**Adicionado:**

* &preto;Textura Definir lista&rbrack; Adicionar botão para ativar/desativar rapidamente o modo de foco
* &lbrack;Log&rbrack; Adicionar o número de versão do Windows 10 no arquivo de log
* Atualize para a versão mais recente do Substance Engine
* &lbrack;MacOS&rbrack; Autenticou o software para seguir os novos requisitos de distribuição do MacOS Catalina

**Corrigido:**

* O código-fonte do plug-in do &lbrack;Plugin&brack; não funciona
* &lbrack;MacOS&rbrack;&lbrack;Sombreador&rbrack; Mac OS 10.14.5 e AMD: a disposição em camadas de material não funciona conforme o esperado

**Problemas Conhecidos:**

* Arquivos Alembic com subdivisões não podem ser importados
* Falhas raras ao importar alguns arquivos Alembic
* A interface não responde temporariamente ao fazer bake com DXR em GPUs Pascal

### 5.2.2 (2019.2.2)

*(Lançado: 20 de setembro de 2019*)Resumo: **Versão de correção**

**Corrigido:**

* A importação de recursos por scripts pode causar uma falha
* &lbrack;Plug-in&rbrack; Baixar material da origem pode levar a um travamento

**Problemas Conhecidos:**

* Arquivos Alembic com subdivisões não podem ser importados
* Falhas raras ao importar alguns arquivos Alembic
* A interface não responde temporariamente ao fazer bake com DXR em GPUs Pascal

### 5.2.1 (2019.2.1)

*(Lançado em: 17 de setembro de 2019*)Resumo: **Versão de correção**

**Corrigido:**

* &lbrack;Mac&rbrack;&lbrack;USD&rbrack; Os arquivos USDZ exportados do MacOS não podem ser abertos
* &lbrack;Conjunto de texturas&rbrack; Não é possível isolar um conjunto de texturas com o modificador ALT
* &preto;Prateleira&rbrack; Predefinições, Materiais inteligentes e Máscaras inteligentes são sempre modificados ao sair do aplicativo
* &lbrack;Pilha de camadas&rbrack; Não é possível selecionar o efeito após excluir outro efeito
* Cintilação ao usar um controle deslizante dentro do painel de propriedades da ferramenta
* Falha ao exportar predefinições para prateleira
* Falha ao exportar uma predefinição com espaço insuficiente
* Falha ao criar uma predefinição com espaço insuficiente

**Problemas Conhecidos:**

* Arquivos Alembic com subdivisões não podem ser importados
* Falhas raras ao importar alguns arquivos Alembic
* A interface não responde temporariamente ao fazer bake com DXR em GPUs Pascal

### 5.2.0 (2019.2.0)

*(Lançado em: 25 de julho de 2019*)Resumo: **Versão principal com atualizações dos baker em termos de desempenho e um novo modo de pré-visualização + novo conteúdo**

**Adicionado:**

* &lbrack;Baker&rbrack; Adicionado suporte para Rastreamento de raios do GPU com DXR e OptiX (Oclusão de ambiente, Thickness)
* &lbrack;Baker&rbrack; Otimizações e acelerações para Rastreamento de raios da CPU
* &lbrack;Baker&rbrack;&lbrack;Modo Vis&rbrack;&lbrack;UI&rbrack; Novo modo de visualização de fça bake no visor
* &lbrack;Baker&rbrack;&lbrack;Preferências&rbrack;&lbrack;IU&rbrack; Nova opção de fça bake para ativar/desativar o Rastreamento de raios do GPU
* &lbrack;Baker&rbrack;&lbrack;UI&rbrack; Retrabalho da caixa de diálogo da barra de progresso
* &lbrack;Baker&rbrack; Aprimoramento de mensagens de aviso e erro
* &lbrack;Baker&rbrack; Permitir cancelamento mais responsivo do processo de fça bake
* &lbrack;Baker&rbrack; Reabrir janela fazer bake após clicar em cancelar
* &lbrack;Proj&rbrack;&lbrack;UX&rbrack; Melhoria da usabilidade do manipulador de rotação
* &lbrack;Settings&brack; Opção para melhorar o desempenho reduzindo a resolução do visor para telas HDPI
* &preto;Script&rbrack; Alterar resolução do conjunto de texturas
* &lbrack;Scripting&brack; Obter conjunto de textura selecionado
* &lbrack;Scripting&brack; Permite que o usuário selecione um conjunto de texturas
* &lbrack;Scripting&rbrack; Função para saber quando a seleção do conjunto de texturas foi alterada
* &lbrack;Prateleira&rbrack; Adicionados 40 novos materiais inteligentes
* &lbrack;Prateleira&rbrack; Adicionadas 20 novas máscaras inteligentes

**Corrigido:**

* &lbrack;Pilha de camadas&rbrack; Congelamento de interface ao selecionar várias camadas
* &lbrack;Pilha de camadas&rbrack; Agrupar muitas camadas congela a interface por mais tempo do que o normal
* &lbrack;Pilha de camadas&rbrack; Uma camada e um efeito podem ser selecionados ao mesmo tempo em alguns casos
* os gráficos de Substance usados nas ferramentas de pintura não são gerados na resolução correta
* &lbrack;Baker&rbrack; o botão “Fazer bake todos os conjuntos de textura” não é desativado quando nenhum baker é selecionado
* &lbrack;MacOS&rbrack; Desativa a mensagem de aviso sobre o mosaico
* A ferramenta de projeção não tem visualização quando usada com uma máscara
* Falha e projetos corrompidos ao tentar salvar com espaço em disco insuficiente
* &lbrack;Shelf&rbrack; Falha ao importar um recurso em disco via prateleira com espaço insuficiente
* &lbrack;Shelf&rbrack; Falha ao restaurar a predefinição de sessão
* &preset;Shelf&rbrack; Importar uma predefinição com um nome que termine com um espaço leva a um travamento
* &lbrack;Shelf&rbrack; Importar um recurso com um prefixo que termine com um espaço vazio leva a um travamento

**Problemas Conhecidos:**

* Arquivos Alembic com subdivisões não podem ser importados
* Falhas raras ao importar alguns arquivos Alembic
* A interface não responde temporariamente ao fazer bake com DXR em GPUs Pascal

### 5.1.3 (2019.1.3)

*(Lançado em: 01 de julho de 2019*)Resumo: **Correção de erro com 2 novos recursos**

**Adicionado:**

* Permite especificar o orçamento VRam com uma linha de comando (por exemplo, —vram-budget 4096)
* &lbrack;QML&rbrack; Expor as propriedades wrapMode e elide dos botões e caixas de verificação QML

**Corrigido:**

* “Seguir caminho” não funciona o tempo todo
* O mapeamento de canal não funciona com SBSAR usado em slots de canal único
* &lbrack;Pilha de camadas&rbrack; Baixo desempenho ao rolar com camadas ocultas
* &lbrack;TextureSet&rbrack; Falha ao clicar entre máscaras
* &lbrack;SVT&rbrack; Deslocamento não exibido corretamente e pisca em alguns casos
* &lbrack;Alembic&rbrack; Falha com malha usando normais de ponto em vez de normais de vértice
* &lbrack;Alembic&rbrack;&lbrack;Log&rbrack; Relatar erro no Log se o arquivo Alembic não for suportado durante a importação

**Problemas Conhecidos:**

* Arquivos Alembic com subdivisões não podem ser importados
* Falhas raras ao importar alguns arquivos Alembic

### 5.1.2 (2019.1.2)

*(Lançado: 21 De maio De 2019*)Resumo: **Hotfix**

**Corrigido:**

* Falha ao selecionar dois recursos com uma entrada de imagem

### 5.1.1 (2019.1.1)

*(Lançado: 20 De maio De 2019*)Resumo: **Hotfix**

**Adicionado:**

* Atualize para a versão mais recente do Substance Engine com a última versão do Substance Designer 2019.1

**Corrigido:**

* &lbrack;Substance&rbrack; Visível Se não for levado em conta para Imagens de Entrada
* &lbrack;SVT&rbrack;&lbrack;Engine&rbrack; Alterar a resolução do conjunto de texturas leva a uma falha em alguns casos
* &lbrack;Engine&rbrack; texturas pretas aleatórias aparecem em alguns casos
* &lbrack;Pilha de camadas&rbrack;&lbrack;UI&rbrack; Alternar uma máscara com SHIFT pode selecionar várias camadas ao mesmo tempo
* &lbrack;Pilha de camadas&rbrack; A opacidade não tem efeito sobre o efeito de Tinta com o modo de mesclagem Passagem
* A entrada do filtro &lbrack;Pilha de camadas&rbrack; Height para Normal não é atualizada corretamente com a pincelada de borracha
* &lbrack;LayersStack&rbrack; Falha ao desfazer o descarte de uma máscara inteligente
* Wireframe piscando com sombras e suavização de borda temporal ativada
* &lbrack;Deslocamento&rbrack; Atraso na AMD com algumas malhas pesadas
* &lbrack;Windows&rbrack; Falha ao abrir alguns projetos através do explorador de arquivos
* &lbrack;Histograma&rbrack; Falha ao remover a máscara com o ponto de ancoragem em alguns casos
* Falha na geração de visualização em alguns casos raros
* &lbrack;Crash&rbrack; Não é possível reabrir um projeto usando muitas ferramentas de clonar e borrar
* Nenhuma malha exibida no modo de material após salvar em alguns casos
* &lbrack;Scripting&brack; alg.mapexport.documentStructure() retorna valores incorretos para pastas

**Problemas Conhecidos:**

* Clicar duas vezes no nome do conjunto de texturas o selecionará antes de entrar no modo de renomeação

### 5.1.0 (2019.1.0)

*(Lançado: 23 de abril de 2019*)Resumo: **Traço dinâmico com novo conteúdo dedicado, Deslocamento e mosaico em tempo real e Iray, efeito Comparar máscara, simetria radial, Planar e Projeção esférica**

**Adicionado:**

* &lbrack;Tool&brack; Traço dinâmico: variação de Substance ao lado de uma pincelada
* &preto;Traço dinâmico&rbrack; Expor novo parâmetro de índice de carimbo com opções
* &preto;Traço dinâmico&rbrack; Leve em consideração o parâmetro $time
* &preto;Traço dinâmico&rbrack; Gerar novo parâmetro $randomseed por traço e por carimbo
* &preto;Traço dinâmico&rbrack; Inicia um índice de traçado dinâmico a partir de um número aleatório
* &lbrack;Traço dinâmico&rbrack;&lbrack;Prateleira&rbrack; Ajuda para encontrar um recurso de traço dinâmico com um novo ícone dedicado
* Deslocamento e mosaico em viewport em tempo real
* Deslocamento e mosaico em Irlanda
* &lbrack;configurações de Sombreador&rbrack;&lbrack;UI&rbrack; Nova guia para controlar deslocamento e mosaico
* &lbrack;Pilha de camadas&rbrack; Novo efeito CompararMáscara: gerar uma máscara comparando dois canais
* &lbrack;Pilha de camadas&rbrack;&lbrack;UI&rbrack; Nova entrada no menu do botão direito do mouse “Adicionar máscara com combinação de height” para inserir um efeito CompararMáscara
* &lbrack;Simetria&rbrack; Novo modo de simetria: pintura radial
* &preto;Configurações de Simetria&rbrack; Expande as duas seções “Configurações” e “Exibição”
* &lbrack;configurações de Simetria&rbrack;&lbrack;IU&rbrack; Visualizar para pintura radial
* Exponha dois novos modos de projeção: planar e esférico
* &lbrack;Proj&rbrack; Novo modo de corte de forma para todas as projeções
* &lbrack;Proj&rbrack; modo Planar com nova manipulador: ferramenta Superfície
* &lbrack;Proj&rbrack;&lbrack;Atalho&rbrack; Atalho SHIFT+W para a ferramenta Superfície
* &lbrack;Proj&rbrack; máscara de projeção Planar com remoção de seleções de profundidade e backface
* &lbrack;Manipulador&rbrack; Melhoria do manipulador de rotação em todos os três eixos para triplanar
* &lbrack;Tool&rbrack;&lbrack;UX&rbrack; clicar com a tecla Alt pressionada em um canal focaliza esse canal (ativa ou desativa todos os outros)
* &lbrack;Engine&rbrack; Atualiza para a versão mais recente do Substance Engine
* &preto;Conjunto de texturas&rbrack; Seleção múltipla e alterar resolução
* &lbrack;Conjunto de texturas&rbrack; Ativação e desativação rápidas dos conjuntos de texturas
* &preto;Conjunto de texturas&rbrack; Combina solo e todas as opções em um novo menu
* &lbrack;Conjunto de texturas&rbrack;&lbrack;Pilha de camadas&rbrack; Novo ícone para ativação e desativação
* &lbrack;Pilha de camadas&rbrack;&lbrack;UX&rbrack; Inserir efeitos acima dos já selecionados
* &lbrack;Pilha de camadas&rbrack;&lbrack;UI&rbrack; Retrabalhar estilo de seleção de exibição de pilha de camadas
* O modo de mesclagem &lbrack;Pilha de camadas&rbrack; para camadas instanciadas agora está no modo Passagem por padrão
* &lbrack;Export&brack; Opção para ativar e desativar o pontilhamento
* &lbrack;Plug-in&rbrack; Suporte ao modificador de precisão para controles deslizantes (SHIFT)
* &lbrack;Plug-in&rbrack;&lbrack;UI&rbrack; Novo ícone para salvamento automático
* &lbrack;Scripting&brack; Lista o conteúdo de uma pasta
* &lbrack;Scripting&brack; Permitir exclusão de arquivos
* &lbrack;Scripting&rbrack; Ler todas as informações da pilha, incluindo os recursos usados
* &lbrack;Conteúdo&rbrack;&lbrack;Traço dinâmico&rbrack; Novas ferramentas e predefinições de pincel
* &lbrack;Content&rbrack;&lbrack;Traço dinâmico&rbrack; Dois novos gradientes processuais: Matiz de gradiente e Construtor de gradiente
* &lbrack;Content&rbrack; 11 novos filtros: Tinta de descascamento MatFx, gotas de água MatFx e muito mais
* &lbrack;Content&rbrack; 7 novos geradores: Auto Stitcher, Cor aleatória UV, Densidade de texel UV e muito mais
* &lbrack;Content&brack; 93 novas alfas: novos textos, setas e várias outras formas
* &lbrack;Content&brack; 2 novos procedimentos: Matiz de Gradiente, Construtor de Gradiente e muito mais
* &lbrack;Content&brack; 21 novas predefinições de ferramenta e pincel para Traçados dinâmicos: Pebbles, Footprints, Spray e muito mais
* &lbrack;Content&rbrack; 2 Novos HDRis: Canopus Ground e Floresta de outono
* &lbrack;Content&rbrack; Atualizar conteúdo com curadoria de semente aleatória na prateleira
* &lbrack;Content&brack; Novo ícone com parâmetro de semente aleatório exposto na prateleira

**Corrigido:**

* &preto;Pilha de camadas&rbrack; a Pilha de camadas continua arrastando para sempre
* &lbrack;Mac&rbrack; “Mostrar no Finder” pode levar ao congelamento
* &lbrack;Scripting&rbrack; As configurações salvas pela interface do usuário personalizada são perdidas se o arquivo de sombreador for movido
* O número da versão da API do &brack;Scripting&brack; está incorreto e não está atualizado
* O conteúdo do Histograma do &Preenchimento;Efeito&Preenchimento; não é exibido corretamente
* O efeito do Histograma do &preto;Efeito&rbrack; não é atualizado em alguns casos
* &lbrack;Prateleira&rbrack; Os pontos não estão alinhados corretamente no material “Pirâmide de tecido plástico”

**Problemas Conhecidos:**

* Clicar duas vezes no nome do conjunto de texturas o selecionará antes de entrar no modo de renomeação
* &lbrack;Pilha de camadas&rbrack;&lbrack;UI&rbrack; Alternar uma máscara com SHIFT pode selecionar várias camadas ao mesmo tempo

## Versão 4

### 4.3.3 (2018.3.3)

*(Lançado em: 07 de março de 2019*)Resumo: **correção de erros**

**Adicionado:**

* &lbrack;Content&brack; Integrar novo modelo de projeto: “PBR - Aspereza metálica Alpha-blend”
* A ordem de pesquisa da biblioteca dinâmica Linux foi alterada para priorizar as bibliotecas no diretório de instalação antes do que está instalado no sistema

**Corrigido:**

* A malha às vezes desaparece da viewport 3D (pressione F para redefinir a câmera)
* Atualize o carregador do Substance Painter Sketchfab com os novos tipos de licença do Sketchfab
* &lbrack;Import&rbrack;&lbrack;glTF&rbrack; Manipulação incorreta da modulação de textura de entrada conforme definido nos arquivos glTF
* &lbrack;Import&rbrack;&lbrack;glTF&rbrack; O plano horizontal é exibido incorretamente com a importação de glTF em alguns casos
* &lbrack;Export&rbrack;&lbrack;USD&rbrack; A opacidade não funciona no Arkit
* &lbrack;Export&rbrack;&lbrack;USD&rbrack; falhas de exportação em USDz em alguns casos
* &lbrack;Export&rbrack;&lbrack;USD&rbrack; Exportar para USD sem salvar leva a um erro fatal
* &lbrack;Export&rbrack;&lbrack;USD&rbrack; Modo de divisão em blocos gráficos incorreto para textura, modo de subdivisão para malhas e tipos de saída para sombreadores
* &lbrack;Export&rbrack;&lbrack;USD&rbrack; Exportações esparsas de apenas alguns conjuntos de texturas com toda a geometria
* &lbrack;Instância&rbrack; Falha ao tentar excluir uma camada de instância quebrada
* &lbrack;Regressão&rbrack;&lbrack;Exportar&rbrack; Alguns mapas não são exportados na profundidade de bits escolhida
* &lbrack;Linux&rbrack; Problema com a biblioteca libtbb.so.2

**Problemas Conhecidos:**

* O congelamento da computação em alguns casos em GPUs AMD VEGA
* Problema do tablet Huion com atalhos no sistema operacional Windows

### 4.3.2 (2018.3.2)

*(Lançado: 24 de janeiro de 2019*)Resumo: **Hotfix com novos recursos (exportação USDZ e filtragem de Textura no visor)**

**Adicionado:**

* &preto;Exportar&rbrack; Permitir exportação para USDZ
* &lbrack;Visor&rbrack; Permite controlar a qualidade da textura nas Configurações de exibição
* &lbrack;Viewport&rbrack; Adicionada configuração de polarização mip nas Configurações de Exibição
* &lbrack;Visor&rbrack; Adicionado filtro anisotrópico em Configurações de exibição
* &lbrack;plugins&rbrack; Atualize os plug-ins oficiais para usar o estilo do Substance Painter 2018
* &lbrack;Licença&rbrack; Instalar licença por padrão em uma pasta do usuário

**Corrigido:**

* Falha vinculada à descompactação
* Adicionar TAA em material solo
* Ruído com sombra, TAA e sombreador de teste alfa com pontilhamento
* Remover pontilhamento de specular para todos os sombreadores PBR clássicos
* Falha nas configurações de sombreador em alguns casos
* A ativação de dispersão não está sincronizada entre as renderizações OpenGL e Iray
* As ferramentas Borrar e Clonar não funcionam mais em malhas específicas
* Alguns conjuntos de texturas não podem aparecer na renderização Iray
* Os conjuntos de texturas renomeados não são salvos após o fechamento do projeto
* Artefatos de wireframe ao arrastar e soltar materiais em mapas de ID
* &lbrack;Criação do caminho do arquivo &rbrack; não forçada ao salvar um projeto
* &lbrack;Scripting&brack; O retorno de chamada “onProjectAboutToSave()” não funciona mais
* Links do fórum quebrados na janela de erro do relatório

**Problemas Conhecidos:**

* O congelamento da computação em alguns casos em GPUs AMD VEGA
* Problema do tablet Huion com atalhos no sistema operacional Windows

### 4.3.1 (2018.3.1)

*(Lançado Em: 06 De dezembro De 2018*)Resumo: **Hotfix**

**Adicionado:**

* &lbrack;Simetria&rbrack;&lbrack;Visor&rbrack; Simetria pintura na Visualização 2D de volta e agora apresenta uma visualização do pincel de clone corrigida

**Corrigido:**

* &lbrack;Exportar&rbrack; Visualização 2D gera uma textura preta em alguns casos
* &lbrack;Iray&rbrack; As informações normais se tornam incorretas no Iray após instanciar uma camada de material
* Conjuntos de textura não quadrada podem levar, em alguns casos, a falhas
* &lbrack;Undo&rbrack; Vários Ctrl+Z podem aleatoriamente levar, em alguns casos, a falhas
* &lbrack;QML&rbrack; AlgScrollView pode criar um aviso no registro em alguns casos (loops de vinculação)

**Problemas Conhecidos:**

* O congelamento da computação em alguns casos em GPUs AMD VEGA
* Problema do tablet Huion com atalhos no sistema operacional Windows
* A suavização de borda e as sombras quando ativas em conjunto podem gerar resultados inesperados

### 4.3.0 (2018.3.0)

*(Lançado em: 20 de novembro de 2018*)Resumo: **Atualizações de viewport, exportação adequada, novos auxiliares de interface, uma ferramenta de simetria aprimorada, novo conteúdo e um enorme aumento no desempenho**

**Adicionado:**

* &lbrack;Suavização de borda&rbrack;&lbrack;Visor&rbrack; Nova filtragem de suavizações temporais para visor 3D (via Configurações de exibição)
* &lbrack;Export&brack; Exporta o conteúdo do visor 2D como uma única textura
* &lbrack;Exportar&rbrack;&lbrack;Pontilhamento&rbrack; Expor pontilhamento na exportação
* &lbrack;Pilha de camadas&rbrack; Cores em camadas e pastas
* &lbrack;Pilha de camadas&rbrack; Ativação e desativação rápidas de várias camadas e efeitos
* &lbrack;Pilha de camadas&rbrack; Navegação mais fácil para modos de mesclagem com teclas para cima e para baixo e rolagem do mouse
* &lbrack;Proj&rbrack;&lbrack;UI&rbrack; manipulador de rotação adicional nos três eixos para triplanar
* &lbrack;Proj&rbrack;&lbrack;Atalhos&rbrack; - e + para alterar o tamanho do manipulador de Projeção UV
* &lbrack;Sombreador&rbrack; Controla os parâmetros da camada revestida com canais no sombreador revestido com PBR
* &lbrack;Substance&rbrack; Expor novas entradas de textura com base em malha para filtros e geradores
* &lbrack;Simetria&rbrack;&lbrack;Visor&rbrack;&lbrack;UI&rbrack; Controlar deslocamento da simetria com manipuladores
* &lbrack;Simetria&rbrack;&lbrack;Barra de ferramentas contextual&rbrack;&lbrack;UI&rbrack; Novo painel de simetria com opções
* &lbrack;Simetria&rbrack; Novo modo de interseção de linha de simetria
* &lbrack;Simetria&rbrack; Novo cursor de clonagem de simetria
* &lbrack;Simetria&rbrack;&lbrack;Atalhos&rbrack; Q para ocultar e -, + para alterar o tamanho e shift para ajustar
* &lbrack;Log&brack; Melhorar as mensagens de erro quando não for possível exportar texturas
* &lbrack;Scripting&rbrack; Permite alterar ou atualizar os recursos em Configurações de exibição
* &lbrack;Scripting&brack; Permite criar ou remover canais em Conjuntos de Textura
* &lbrack;Content&rbrack;&lbrack;Shaders&rbrack; Adicionar suporte para anisotropia com um sombreador dedicado (pbr-metal-rough-anisotropia-angle)
* &lbrack;Conteúdo&rbrack; Atualização da esfera de visualização com anisotropia e ângulo modificado
* &lbrack;Content&rbrack; shutline matFx atualizado
* &lbrack;Content&rbrack; Nova texturização.XYZ varredura de rosto sem emenda
* &lbrack;Content&brack; Novos procedimentos anisotrópicos
* &lbrack;Content&brack; Novo filtro: ambiente de iluminação baked
* &lbrack;Content&brack; Novo mapa de ambiente: estúdio automotivo neutro
* &lbrack;Content&brack; Novo modelo de projeto: PBR - Ângulo de anisotropia de aspereza metálica (com canais de anisotropia)
* &lbrack;Content&brack; Novo modelo de projeto: PBR - aspereza metálica revestida
* &lbrack;SVT&rbrack;&lbrack;Engine&rbrack; Texturas Virtuais Dispersas (SVT)
* &lbrack;SVT&rbrack;&lbrack;Preferências&rbrack;&lbrack;IU&rbrack; SVT hardware support acceleration option
* &lbrack;SVT&rbrack;&lbrack;Log&rbrack; Informações adicionais para o recurso Texturização Virtual Esparsa (por exemplo, tamanho do disco)
* &lbrack;SVT&rbrack;&lbrack;UI&rbrack; Janela de mensagens no início se o tamanho do disco for muito baixo para o cache
* &lbrack;SVT&rbrack;&lbrack;Preferências&rbrack;&lbrack;UI&rbrack; Substance Painter local do cache global
* &lbrack;SVT&rbrack; Nova variável de ambiente para especificar o caminho do cache de Substance Painter
* &lbrack;SVT&rbrack; Nova variável de ambiente para ativar a aceleração de suporte de hardware SVT
* &lbrack;SVT&rbrack; Detectar suporte esparso por hardware
* &lbrack;SVT&rbrack;&lbrack;Hardware Sparse&rbrack; Elevar a versão mínima do driver para a GPU Nvidia
* &lbrack;SVT&rbrack;&lbrack;Sombreador&rbrack;&lbrack;Viewport&rbrack;&lbrack;UI&rbrack; Avisa o usuário se artefatos presentes com Texturização Virtual Esparsa na abertura do projeto

**Corrigido:**

* &preto;Seletor de cores&rbrack; Cursor de pintura que aparece ao tentar escolher uma cor
* A falha ao selecionar ou cancelar a seleção de camadas em uma ordem específica pode causar falha
* Falha ao colar como uma ocorrência uma camada com uma máscara
* &lbrack;User Channel&rbrack;&lbrack;Regressão&rbrack; Falha ao renomear o canal do usuário
* &preto;Canal do usuário&rbrack; visualização do pincel esmaecido
* &lbrack;Alembic&rbrack; Somente uma textura definida de vários materiais após a importação
* &lbrack;Engine&brack; A textura exportada difere da viewport para carimbos de pincel
* &lbrack;Engine&rbrack; Inverter com um efeito de nível não afeta totalmente uma textura
* O seletor de material está aplicando um traçado de pincel ao separar
* Alternar a resolução para 128x128px leva a um travamento
* Os links de mapas de malha não são atualizados corretamente ao reorganizar ou instanciar camadas
* &lbrack;Substance&rbrack; O UserData ColorSpace não funciona no Normal de Malha Feito bake solicitado como entrada
* Incompatibilidade de associação MDL ao usar várias instâncias de sombreadores
* &lbrack;Simetria&rbrack;&lbrack;Camada de preenchimento&rbrack; plano de Simetria e seu manipulador ativo na Camada de preenchimento
* &preto;Visor&rbrack; Ponto dinâmico para tradução nem sempre atualizado após clicar
* &lbrack;UI&rbrack; Ícones fixos e remoção de espaços reservados para monitores HDPI

**Problemas Conhecidos:**

* O congelamento da computação em alguns casos em GPUs AMD VEGA
* Problema do tablet Huion com atalhos no sistema operacional Windows
* A suavização de borda e as sombras quando ativas em conjunto podem gerar resultados inesperados

### 4.2.3 (2018.2.3)

*(Lançado: 25 de setembro de 2018)*

**Corrigido:**

* O &lbrack;Visualização 2D&rbrack; Visualização 2D é quebrado com algumas malhas ao criar um novo projeto
* &lbrack;Crash&rbrack; Alternar de Projeção UV para projeção tri-planar leva a um travamento
* &lbrack;RayCollider&rbrack; Várias falhas devido ao “RayCollider”
* &lbrack;Tool&brack; Alternar camadas perde as propriedades do pincel modificadas
* As configurações do pincel são redefinidas ao alternar para a borracha

**Problemas Conhecidos:**

* Congelamento de computação em GPUs AMD VEGA
* Problema do tablet Huion com atalhos no sistema operacional Windows

### 4.2.2 (2018.2.2)

*(Lançado em: 11 de setembro de 2018*)Resumo: **Hotfix com atualização de conteúdo, novas funcionalidades de script e capacidade de desabilitar a atualização automática**

**Adicionado:**

* &lbrack;Content&rbrack;&lbrack;Shelf&rbrack; Adicionar uma predefinição de prateleira de pele
* &lbrack;Content&rbrack;&lbrack;shelf&rbrack; Conversão de 19 normais de pele em materiais para dispersão subsuperficial
* &lbrack;Scripting&brack; Cria um modelo de projeto a partir de um projeto aberto
* &lbrack;Scripting&brack; Obter/Definir configurações de exportação de um projeto aberto
* &lbrack;Atualizações&rbrack; Consegue desativar o pop-up de atualização automática nas configurações e variáveis de ambiente
* &lbrack;Atualizações&rbrack; Não exibir até a próxima versão no pop-up de manutenção desatualizada

**Corrigido:**

* &lbrack;Camera&brack; Zoom incorreto ao alternar de ortográfica para Perspectiva
* &lbrack;Display&rbrack; Alguns mapas são exibidos de forma linear em vez de sRGB
* O foco da malha do &brack;Viewports&rbrack; não se comporta corretamente
* &lbrack;Visualização 2D&rbrack; Projeto com câmera quebrada tem desaparecendo Shells UVs
* &lbrack;SSS&rbrack;&lbrack;Dica de ferramenta&rbrack; as dicas de ferramentas de dispersão da subsuperfície aparecem no registro
* Alguns projetos não podem ser abertos em 2018.2 e a mensagem de erro não pode salvar um pacote nulo do substance
* A cor da ferramenta de Tinta do &brack;Mask&rbrack; pode ficar presa em alguns casos ao trabalhar em uma máscara
* &lbrack;Material&rbrack; Mapas que não aparecem em situações específicas
* &lbrack;Proj&rbrack;&lbrack;Ferramentas&rbrack; Manipulador ativo com um gerador
* &lbrack;Substance&rbrack; Grupos de Substance de parâmetros ausentes
* &lbrack;Scripting&rbrack; Nome de software incorreto na documentação
* &lbrack;UDIMs&rbrack; Não há informações no log sobre shells UVs em vários blocos UVs

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

*(Lançado em: 2 de agosto de 2018*)Resumo: **Versão de verão, suporte a dispersão de subsuperfície, melhorias de projeção e preenchimento, importação e seleção de câmera, suporte a Alembic e glTF, arrastar e soltar no mapa de ID, suporte aprimorado ao formato de Substance e conteúdo novo**

**Adicionado:**

* &lbrack;SSS&rbrack;&lbrack;Visor&rbrack;&lbrack;Iray&rbrack; Dispersão de subsuperfície genérica
* &lbrack;SSS&rbrack; Sincronizar MDL e parâmetros de dispersão da subsuperfície
* &preto;SSS&rbrack; Adicionado um novo canal em tons de cinza chamado Dispersão
* &lbrack;SSS&rbrack;&lbrack;Configurações de Sombreador&rbrack; Parâmetro de tipo de dispersão para dispersão de subsuperfície (pele ou translúcido)
* &lbrack;SSS&rbrack;&lbrack;Configurações de Sombreador&rbrack; Parâmetro de escala de dispersão para dispersão de subsuperfície
* &lbrack;SSS&rbrack;&lbrack;Configurações de Sombreador&rbrack; Parâmetro de dispersão de cor para dispersão de subsuperfícies
* &lbrack;SSS&rbrack;&lbrack;Configurações de exibição&rbrack; Contagem de amostras de dispersão para dispersão subsuperficial
* &lbrack;Sombreador&rbrack;&lbrack;Iray&rbrack; Integrar MDL de dispersão de subsuperfície para Iray
* &lbrack;Sombreador&rbrack; atualização de Sombreador através do atualizador de recursos
* &lbrack;Sombreador&rbrack; Atualizar a API e a documentação do registro de alterações
* &lbrack;Propriedades da ferramenta&rbrack;&lbrack;Proj&rbrack; Novos parâmetros para a projeção triplanar
* &lbrack;Viewport&rbrack;&lbrack;Proj&rbrack; Controla as propriedades da Camada de preenchimento na exibição 3D diretamente com manipuladores (projeção triplanar)
* &lbrack;Atalhos&rbrack;&lbrack;Proj&rbrack; Novos atalhos Q, W, E, R, T para manipuladores de projeção triplanar
* &lbrack;Viewport&rbrack;&lbrack;Proj&rbrack; Controla as propriedades da Camada de Preenchimento diretamente com manipuladores (Projeção UV)
* &lbrack;Atalhos&rbrack;&lbrack;Proj&rbrack; Novo atalho Q para manipuladores de Projeção UV
* &lbrack;Barra de ferramentas contextual&rbrack;&lbrack;Proj&rbrack; Controla manipuladores de projeção triplanar
* &lbrack;Barra de ferramentas contextual&rbrack;&lbrack;Proj&rbrack; Controlar manipuladores de Projeção UV
* &lbrack;Propriedades da ferramenta&rbrack; Desativar divisão em blocos gráficos por textura com a ferramenta de projeção e estêncil
* &lbrack;Estêncil&rbrack; Usar imagens não quadradas com a ferramenta de projeção/estêncil
* &lbrack;Estêncil&rbrack; Permitir controle do modo lado a lado na janela Propriedades
* &lbrack;Estêncil&rbrack; O Zoom não está centralizado em um estêncil sem revestimento
* &lbrack;Câmeras&rbrack; importar câmeras do Maya, Max, Blender, Modo, DAE
* &lbrack;Câmeras&rbrack;&lbrack;Visor&rbrack; Selecionar e controlar câmeras importadas no visor
* &lbrack;Cameras&brack;&lbrack;Iray&rbrack; Selecionar e controlar câmeras importadas no Iray
* &lbrack;Câmeras&rbrack;&lbrack;UI&rbrack;&lbrack;Novo projeto&rbrack;&lbrack;Configuração do projeto&rbrack; Importar câmeras está marcado por padrão
* &lbrack;Cameras&brack;&lbrack;Atalhos&rbrack; Adicionar atalhos para alternar entre câmeras
* &lbrack;Cameras&brack;&lbrack;Visor&rbrack; Adicionar quadro no visor
* &lbrack;Cameras&brack;&lbrack;Configurações do visor&rbrack; Controle de opacidade de quadro
* &lbrack;Câmeras&rbrack;&lbrack;Configurações da câmera&rbrack; distância focal máxima em 500 mm
* &lbrack;Câmeras&rbrack;&lbrack;Configurações da câmera&rbrack; Taxa de exposição
* &lbrack;Cameras&brack;&lbrack;Configurações da câmera&rbrack; Adicionar uma opção de bloqueio
* &lbrack;Cameras&brack;&lbrack;Configurações da câmera&rbrack; Adicionar uma opção de restauração
* &lbrack;Cameras&brack;&lbrack;Configurações da câmera&rbrack; Adicionar atributo de distância do foco
* &lbrack;glTF&rbrack; Importação de um arquivo glTF
* &lbrack;glTF&rbrack; Importar mapa de oclusão de ambiente
* &lbrack;Alembic&rbrack; Importar quadro Alembic 1 com geometria estática
* &lbrack;Shelf&rbrack; Arraste e solte materiais diretamente na malha usando mapas de ID com um modificador (CTRL/Command)
* &lbrack;Pilha de camadas&rbrack; Criação automática de máscara de ID com arrastar e soltar materiais na malha com mapas de ID
* &lbrack;Pilha de camadas&rbrack; Rolagem automática de camadas com arrastar e soltar pela pilha de camadas
* &lbrack;UI&rbrack;&lbrack;Propriedades da ferramenta&rbrack; Expor predefinição de Substance
* &lbrack;UI&rbrack;&lbrack;Menu Ajuda&rbrack; Aprimoramento do menu Ajuda
* &lbrack;UI&rbrack;&lbrack;Novo Projeto&rbrack;&lbrack;Configuração do Projeto&rbrack; Reorganização da janela
* &lbrack;UI&rbrack;&lbrack;Novo Projeto&rbrack;&lbrack;Configuração do Projeto&rbrack; Substituir termo de Malha por Arquivo
* &lbrack;UI&rbrack;&lbrack;Substance&rbrack; Exibir atributos de Substance na interface do usuário
* &lbrack;Atalhos&rbrack; F4 alterna entre as visualizações 2D e 3D
* &lbrack;Atalhos&rbrack; Novos atalhos para alternar o estêncil N e máscara rápida U
* &lbrack;integração de Substance&rbrack; Leve em consideração as instruções &#39;visible if&#39; nos parâmetros de Substance
* &lbrack;Visor&rbrack; Sombras não forçadas a serem computadas após a movimentação da câmera
* &lbrack;Content&rbrack; Atualizar MeetMat com câmeras importadas
* &lbrack;Content&brack; Adicionar uma amostra com dispersão de subsuperfície ativada - JadeToad
* &lbrack;Content&brack; Adicionar um novo modelo de projeto PBR com dispersão de subsuperfície ativada
* &lbrack;Content&rbrack; Predefinições de exportação atualizadas para adicionar um novo canal de Dispersão
* &lbrack;Content&rbrack;&lbrack;Shelf&rbrack; Suporte a dispersão de subsuperfície adicionado para: pbr-metal-rough, pbr-metal-rough-alpha-test, pbr-coated, pbr-spec-gloss
* &lbrack;Content&rbrack;&lbrack;Shelf&rbrack; Adicionado Canal de dispersão a 5 materiais inteligentes (bolinhas e peles)
* &lbrack;Content&rbrack;&lbrack;Shelf&rbrack; 1 novo Material em jade
* &lbrack;Content&rbrack;&lbrack;Shelf&rbrack; 1 novo material de cera

**Corrigido:**

* &lbrack;CMD&rbrack; Resultados diferentes usando a mesma linha de comando com versões diferentes
* &lbrack;TDR&rbrack; Se o TdrLevel estiver configurado, você não terá erros no seu log
* &lbrack;Baker&rbrack; o mapa de Oclusão de ambiente está invertido
* &lbrack;Mapa de identificações&rbrack; Falha ao selecionar fora do intervalo 0-1
* &lbrack;Iray&rbrack; Falha ao alternar conjuntos de texturas e voltar para o modo de Tinta
* &lbrack;Viewport&rbrack; Sincronizar áreas de soltar entre viewports para arrastar e soltar
* &lbrack;Engine&brack; artefato Moiré ao colocar camadas de preenchimento lado a lado ou pintar um pequeno pincel
* &lbrack;Licença&rbrack; Serviço de licença verificação de versão de software incorreta
* &lbrack;License&rbrack; Trabalhar novamente como lidamos com a autenticação
* &lbrack;API&rbrack; Chame o evento de API de script onNewProjectCreated mesmo ao criar com um modelo
* &lbrack;Sombreador&rbrack; O sombreador compilado não é carregado do cache quando o arquivo de sombreador não é compilado
* &lbrack;Prateleira&rbrack; Exportar o arquivo HDR da prateleira irá gerar um arquivo com valores fixados
* &lbrack;Export&rbrack; EXR exportação grampos valores de cor de RGB entre 0-1
* &lbrack;Content&rbrack; Processual ruído 3D Perlin Fractal está pixelado

**Problemas Conhecidos:**

* Congelamento de computação em GPUs AMD VEGA
* Problema do tablet Huion com atalhos no sistema operacional Windows

### 4.1.3 (2018.1.3)

*(Lançado: 28 de junho de 2018)*

**Adicionado:**

* &lbrack;Preferências&rbrack; Proponha salvar o projeto quando o Painter for reiniciado

**Corrigido:**

* O &lbrack;Plug-in&rbrack; Substance Source de Pesquisa não funciona
* &lbrack;Materiais inteligentes&rbrack; Importar Materiais inteligentes leva a uma falha em alguns casos
* &lbrack;Materiais inteligentes&rbrack; Excluir Materiais inteligentes leva a uma falha em alguns casos
* &lbrack;Salvar&rbrack; salvar leva a uma falha em alguns casos raros
* &lbrack;Shelf&rbrack; Inverter não funciona no Células 2 e no Células 3
* &lbrack;Shelf&rbrack; Erro de ortografia em alguns Alpha
* &lbrack;Shelf&rbrack; Alguns materiais do Substance não são renderizados corretamente

**Problemas Conhecidos:**

* Congelamento de computação em GPUs AMD VEGA

### 4.1.2 (2018.1.2)

*(Lançado: 12 De junho De 2018*)Resumo: **Velocidade De Fça bake Aprimorada, Sistema De Salvamento Aprimorado, Controles Deslizantes Atualizados, API De Plug-In Atualizada, Tradução Para Chinês, Preenchimento Aprimorado Agora Opcional**

**Adicionado:**

* &lbrack;Baker&rbrack; Melhoria de desempenho com a nova versão do baker
* Forçar caixa de diálogo de exibição com GPU incompatível
* &lbrack;Salvar&rbrack; Expor a nova funcionalidade de projeto compacto (modo de salvamento completo/compacto)
* &lbrack;Salvar&rbrack; Informar o usuário em caso de erro ao salvar
* &lbrack;Clean&rbrack; Próxima gravação no modo completo/compacto
* &preto;Controles deslizantes&rrack; Aprimoramento da precisão das barras de cor/escala de cinza e controles deslizantes
* &lbrack;Controles deslizantes&rbrack; Adição de controles de seta para cima/para baixo
* &preto;Controles deslizantes&rbrack; Mesma zona de detecção para controles deslizantes de barra em tons de cinza e coloridos
* &lbrack;Plug-in&rbrack; Salvamento automático sempre em modo incremental
* &lbrack;Plug-in&rbrack; Opção para alternar plug-ins para o novo estilo de interface
* &lbrack;Language&brack; Adicionar tradução para chinês
* &lbrack;Preenchimento&rbrack; Opção para alternar entre o preenchimento do vizinho de espaço UV e 3D por Textura Definida nas Configurações do Conjunto de Textura
* &lbrack;Script&rbrack; Modo de salvamento de exposição: completo/compacto ou incremental
* &lbrack;Script&rbrack; Atualizar documentação de script/QML
* &lbrack;Log&rbrack; Indica o modo de salvamento no log (completo/compacto ou incremental)

**Corrigido:**

* &lbrack;O slot do canal do &rbrack; transforma-se em um slot de material em preenchimentos de canal único
* Falha ao carregar uma malha (FBX) com algumas faces não atribuídas por um material
* Falha na Iray com NVIDIA GRID 5.2 na máquina virtual
* Falha ao desfazer uma exclusão de predefinição de material
* Falha ao carregar alguns projetos
* &lbrack;Linha de comando&rbrack; Nova linha de comando para malhas UDIM divididas por udim
* &lbrack;Barra de ferramentas&rbrack; Redução da barra de ferramentas
* &lbrack;Instanciação&rbrack; Não é possível instanciar bitmaps em vários conjuntos de texturas
* &lbrack;Viewport&rbrack; A atualização não está completa ao pintar na malha com UVs lado a lado
* O Mapa normal &lbrack;Iray&rbrack; é aplicado duas vezes para dielétricos
* &lbrack;Shelf&rbrack; Erros de digitação em alguns parâmetros de Substance (alfas, procedimentos e matfx)
* &lbrack;Shelf&rbrack; Erro de ortografia para o bitmap “Somente Pessoal Autorizado”
* &lbrack;Script&rbrack; A função alg.shaders.materials() não funciona mais

**Problemas Conhecidos:**

* Congelamento de computação em GPUs AMD VEGA

### 4.1.1 (2018.1.1)

*(Lançado em: 3 de abril de 2018)*

**Corrigido:**

* &lbrack;Tablet&rbrack; Problema ao alterar as opções de interação padrão
* &lbrack;Baker&rbrack; Falha com biblioteca Assimp
* &lbrack;Baker&rbrack; Regressão no desempenho com mapa A.O.
* &lbrack;Iray&rbrack; A Distorção de lente não é aplicada ao canal Alfa
* &lbrack;Drivers&rbrack; Atualização dos requisitos mínimos de drivers
* &lbrack;3Dview&rbrack; Normais não gerados corretamente em malhas UDIM sem informações normais
* &lbrack;Intel&rbrack; Falha com o Substance Painter 2018.1.0
* &lbrack;Intel&rbrack;&lbrack;Visor&rbrack; Problema com preenchimento (artefatos pretos)

**Problemas Conhecidos:**

* Congelamento de computação em GPUs AMD VEGA

### 4.1.0 (2018.1.0)

*(Lançado: 15 de março de 2018)*

**Adicionado:**

* Novo estilo geral (ícones, cor, comportamento)
* Novo layout padrão
* &lbrack;Aprimoramento da experiência do usuário do Tablet&rbrack; ao pintar
* &lbrack;Menu principal&rbrack; Primeiro, classificar itens nativos em exibições e barras de ferramentas
* &lbrack;Menu principal&rbrack; Mover ações de máscara rápida na seção do visor
* &lbrack;Menu principal&rbrack; Move ações do botão direito do mouse para a seção do visor
* &lbrack;Menu principal&rbrack; Renomear menu “Exibir” como “Janela”
* &lbrack;Menu rápido&rbrack; Novas propriedades de ferramenta clicando com o botão direito do mouse no visor
* &presilha;Widget de encaixe&rbrack; Nova barra de ferramentas de encaixe para rápida redução/recuperação
* &lbrack;Configurações de exibição&rbrack; Janela de configurações da câmera e do visualizador mesclada
* &lbrack;Pilha de camadas&rbrack; Menu contextual do botão direito
* &lbrack;Pilha de camadas&rbrack; Arraste e solte para mover qualquer efeito dentro da mesma camada
* &lbrack;Barra de ferramentas&rbrack; Reorganização da barra de ferramentas e da nova barra de ferramentas contextual
* &lbrack;Barra de ferramentas Ferramentas&rbrack; Dividir ferramenta de clonagem em duas ferramentas separadas
* &preto;Propriedades das ferramentas&rbrack; Valor em tons de cinza do plano de fundo mais claro na visualização
* &lbrack;Propriedades das ferramentas&rbrack; Organização em guias (preenchimento e ferramentas)
* &preto;Tool&brack; O resultado da pintura corresponde ao estêncil
* &lbrack;Visor&rbrack; Novo cursor para camada de preenchimento
* &lbrack;Visor&rbrack; Navegação e pintura mais suaves (taxa de quadro mais alta)
* &preto;Visor&rbrack; Material/Canal/Mapa seleção caixa de combinação no visor
* &lbrack;Visor&rbrack; Reduzir cintilação ao girar (sombra ativada)
* &lbrack;Shelf&rbrack; Exibir materiais por padrão ao abrir o Painter
* &lbrack;Shelf&rbrack; Melhoria no tempo de carregamento de texturas e materiais (2 a 6 vezes mais rápido)
* &lbrack;Prateleira&rbrack; Reorganizar pastas de materiais para se ajustar à estrutura do Substance Source
* &lbrack;Shelf&rbrack; Arraste e solte materiais diretamente na malha no visor
* &lbrack;Shelf&rbrack; Novos Ruídos 3D (Perlin, Perlin Fractal, Simplex e Worley)
* &lbrack;Prateleira&rbrack; Novo gerador de máscara usando a posição da malha
* &lbrack;Shelf&rbrack; Ruídos base atualizados para suportar o expansão não quadrada
* &lbrack;Shelf&rbrack; Adicionado novo modelo e predefinição de exportação para o Lens Studio (aplicativo Snap)
* &lbrack;Prateleira&rbrack; Materiais inteligentes e Máscaras inteligentes atualizadas para usar a versão mais recente do Editor de máscaras (microdetalhes)
* &lbrack;Shelf&rbrack; Novo projeto de amostra “TilingMaterial” para criar materiais de revestimento perfeitos
* &amp;predefinição;Prateleira&amp;predefinição; Novo pincel (caligrafia, molhado, hachura e assim por diante)
* &preto;Controles deslizantes&rbrack; Novos controles deslizantes e estilo e comportamento de barras de tons de cinza/cores
* &lbrack;Baker&rbrack; Permitir o uso de uma caixa delimitadora de cena completa para calcular o mapa de posição
* &lbrack;Sombreador&rbrack; Remove o parâmetro de força do height dos parâmetros de sombreador padrão
* &lbrack;Mecanismo&rbrack; mecanismo de Substance atualizado
* &lbrack;Engine&brack; Nenhuma ou menos descontinuidades nos blocos UV
* &lbrack;Plugins&rbrack; Importar materiais baixados do Substance Source mais rapidamente
* &lbrack;Plug-ins&rbrack; Atualiza todos os plug-ins para corresponder ao novo estilo geral
* &lbrack;Preferências&rbrack; Visualizar alterações de cor de fundo automaticamente
* &lbrack;Clean&rbrack; Risco reduzido de corrupção do projeto
* &lbrack;Aberto&rbrack; Melhoria na hora de abertura do projeto
* &lbrack;Novo projeto&rbrack; Novo projeto - melhoria no tempo de atualização da malha
* &preto;Salvar&rbrack; Salvando a melhoria do tempo do projeto
* &lbrack;Log&rbrack; Tipo de licença relatado no registro
* &lbrack;TextureSet&rbrack; Renomeie o botão “Fazer bake Texturas” como “Fazer bake Mapas de Malha”
* Renomear “Mapas adicionais” como “Mapas de malha”

**Corrigido:**

* &lbrack;Visor&rbrack; Maus desempenhos com malhas contendo muitos sub-objetos
* &lbrack;Propriedades das ferramentas&rbrack; Canal desativado ao arrastar e soltar uma imagem no slot de material
* &brack;Propriedades das ferramentas&rbrack; A visualização do pincel está quebrada com as ferramentas de borrar e clonar
* &preto;A ordem dos canais do conjunto de texturas &rbrack; está incorreta ao usar modelos
* &lbrack;Shelf&rbrack; Ícone ausente para o gerador de Conversão em escala cinza
* &preto;Shelf&rbrack; Número do Círculo do Sinal alfa está quebrado (fonte ausente)
* Detecção incorreta de GPUs integradas na inicialização
* &lbrack;Falha&rbrack; Arrastar e soltar um recurso importado nomeado com um caractere #
* &lbrack;Engine&rbrack; Problema de detecção de Vram na GPU integrada
* &lbrack;Engine&rbrack; Corrigidas várias falhas no Substance Engine Linker
* &lbrack;Engine&rbrack; Artefatos quadrados ao alterar a resolução
* &lbrack;Pós-efeitos&rbrack; O redimensionamento da interface fica lento quando os pós-efeitos estão ativados
* &lbrack;Baker&rbrack; A unidade de cena não é respeitada corretamente para valores de distância de raio
* &lbrack;Baker&rbrack; O AO da distância do Ocluder de malha é fixado em 1, independentemente do valor de entrada
* &lbrack;Baker&rbrack; Corresponder pelo nome ignora algumas malhas com nomes específicos
* &lbrack;Baker&rbrack; Cor da configuração de malha do Poligrupo e ID de Submalha sempre retorna uma imagem em preto
* &lbrack;Baker&rbrack; O Fça bake de ID falha com malhas FBX binárias do Blender
* &lbrack;Sombreador&rbrack; Ruído no Visualização 2D com brilho dota-2 e não pbr-spec
* &lbrack;Linux&rbrack; Somente um thread de CPU é usado ao fazer bake
* &lbrack;MacOS&rbrack; Falha com o cursor do pincel se movendo sobre o visor

**Problemas Conhecidos:**

* Congelamento de computação em GPUs AMD VEGA
* Pós-processo de distorção não levado em conta ao exportar no IRay (alfa)

## Versão 3

### 3.4.2 (2017.4.2)

*(Lançado: 24 de janeiro de 2018)*

**Adicionado:**

* &lbrack;Export&brack; Obter o status de uma exportação com o progresso da etapa
* &lbrack;Export&brack; Permitir cancelamento de uma exportação
* &lbrack;Export&brack; Exportar texturas para o Sketchfab sem perder a qualidade do mapa normal
* &lbrack;Exportar&rbrack; Exportar no formato binário glTF (glb)
* &lbrack;Export&rbrack; Permitir o redimensionamento de colunas na guia de configuração da janela de exportação
* &lbrack;Sombreador&rbrack; Adicionar um changelog para o API de sombreamento
* &lbrack;Scripting&rbrack; Adicionar funções de retorno de chamada Antes e Depois ao exportar texturas
* &lbrack;Iray&rbrack; Atualização para o SDK 2017.1 (suporte a Volta GPUs)

**Corrigido:**

* Falha ao sair do aplicativo antes que a janela principal seja exibida
* &lbrack;MAC&rbrack; Falha ao carregar mapas em tons de cinza com IRAY
* &lbrack;A detecção do VRAM no MAC&rbrack; não está correta com o novo sistema operacional High Sierra
* &lbrack;Plug-in&rbrack; Baixar ativos do Substance Source não funciona mais
* &lbrack;Scripting&brack; Detecção incorreta da versão mínima do plug-in
* &lbrack;Export&brack; Falha ao salvar predefinição de exportação após exportar texturas
* &lbrack;Instancing&brack; Problema em geradores instanciados em um TextureSet sem Mapas Adicionais
* &lbrack;Viewport&rbrack; O pontilhamento não funciona com resolução superior a 4k
* &lbrack;Visor&rbrack; a exibição de material de Visualização 2D está coberta de ruído
* &amp;predefinição;Prateleira&amp;predefinição; Melhorar tempo de carregamento para predefinições de prateleira
* &lbrack;Engine&brack; Mesclagem incorreta ao pintar sob seleção de cores

### 3.4.1 (2017.4.1)

*(Lançado: 15 de dezembro de 2017)*

**Adicionado:**

* &lbrack;Scripting&brack; Exportar malha pela API de script
* &lbrack;Import&brack; Desativar importação de formato de arquivo de malha não suportado (permitir somente obj, fbx, dae, ply)
* &lbrack;Log&rbrack; Indica com mais precisão o problema de TDR no arquivo de log

**Corrigido:**

* Falha se o aplicativo for fechado antes da conclusão do rastreamento de recursos
* Falha ao abrir projetos com a ferramenta Borrar/Clonar
* Falha ao usar a ação de refazer após uma desfazer de uma alteração de Sombreador nas Configurações do visualizador
* &lbrack;A texturização do Engine&rbrack; difere entre o Painter 2017.2 e 2017.4
* &lbrack;Viewport&rbrack; A separação em um mapa de ID de uma instância obtém a amostra da cor errada
* &lbrack;Export&brack; Falha ao exportar uma textura normal ou de oclusão inválida
* Os arquivos de PSD do &brack;Export&brack; têm seus grupos bloqueados quando abertos no Photoshop CS6
* &lbrack;Plug-in&rbrack; o plug-in do Photoshop ignora a seleção de canais e sempre exporta tudo
* &preto;Camadas&rbrack; As âncoras são rompidas quando copiadas/coladas entre Conjuntos de Texturas
* &lbrack;Camadas&rbrack; Algumas referências de âncora não podem ser restauradas se quebradas
* &lbrack;Sombreador&rbrack; o parâmetro de aspereza secundária revestido com pbr está quebrado
* &lbrack;Steam&brack; O pop-up do verificador de versões não deve estar visível na inicialização

**Problemas Conhecidos:**

* &lbrack;AMD&rbrack; Falha/Congela ao tentar tinta em uma malha. Pode ser corrigido com uma atualização de driver de GPU.

### 3.4.0 (2017.4.0)

*(Lançado: 23 de novembro de 2017)*

**Adicionado:**

* &lbrack;Instancing&brack; Permite criar instâncias de parâmetros entre camadas
* &lbrack;Instancing&brack; Permite saltar entre uma camada de origem e uma instância
* &lbrack;Criação de instância&rbrack; Adicionar uma ação “criar instância entre conjuntos de texturas”
* &lbrack;Instancing&rbrack; Indicar nas instâncias de reentrada de pilha de camadas (ciclos)
* &lbrack;Instancing&brack; Excluir instâncias quando uma origem for removida
* &lbrack;Instancing&brack; Não permitir referências de âncora de fora de uma pasta instanciada
* &lbrack;UI&rbrack; Move a Pilha de Desfazer para sua própria janela chamada “History”
* &lbrack;Plug-in&brack; Plug-in de link dinâmico Integrate DCC
* &lbrack;Engine&brack; Aprimorar o desempenho de pintura com pintura Esparsa
* &lbrack;Export&brack; Adicionar opções de rascunho e de reexportação ao exportador do Sketchfab
* &preto;Prateleira&rbrack; Adicionar “virar” controle para substâncias de fontes
* &lbrack;Shelf&rbrack; Adicionar 20 novos materiais de procedimentos
* &lbrack;Shelf&rbrack; Adicionar 40 novos mapas grunges (baseado em bitmap e processual)
* &lbrack;Visor&rbrack; Ativar colisões de visualização de pincel em outros conjuntos de texturas visíveis
* Atualizar os requisitos mínimos dos drivers de GPU AMD

**Corrigido:**

* Falha ao computar Substance em resoluções muito grandes
* Falha ao pintar fortemente com partículas
* &lbrack;Viewport&rbrack; Reflexo de specular incorreto no Visualização 2D com malhas específicas
* &lbrack;UI&rbrack; Algumas ações indesejadas aparecem na janela Histórico

**Problemas Conhecidos:**

* &lbrack;Camadas&rbrack; Algumas referências de âncora não podem ser restauradas se quebradas
* Falha ao usar a ação de refazer após uma desfazer de uma alteração de Sombreador nas Configurações do visualizador

### 3.3.3 (2017.3.3)

*(Lançado em: 01 de dezembro de 2017)*

**Corrigido:**

* &lbrack;Steam&brack; O pop-up do verificador de versões não deve estar visível na inicialização
* Os arquivos de PSD do &brack;Export&brack; têm seus grupos bloqueados quando abertos no Photoshop CS6

### 3.3.2 (2017.3.2)

*(Lançado: 20 De novembro De 2017)*

**Adicionado:**

* &lbrack;UI&rbrack; Melhorar caixa de diálogo da nova versão e adicionar changelog
* &lbrack;UI&rbrack; Indica se a manutenção expirou na caixa de diálogo de nova versão
* &lbrack;Licença&rbrack; Atualiza o sistema de licenças para lidar com as datas de manutenção
* &lbrack;Export&brack; Renomear Adobe Standard Material para Adobe Dimension

**Corrigido:**

* &preto;A pintura do Mac&rbrack; leva a quadrados pretos e corrupções de textura
* &lbrack;Engine&brack; Cache às vezes pode desaparecer no Visor
* &lbrack;Engine&rbrack; Artefatos de blocos aparecem quando um disparador de compactação de memória
* &lbrack;Fazendo bake&rbrack; Estranhas mensagens de erro ao fazer bake malhas específicas
* &lbrack;Export&brack; PSD foram gravados incorretamente e não são reconhecidos corretamente pelo Photoshop
* &lbrack;Camadas&rbrack; Não deveria ser possível copiar/colar camadas em vários projetos
* &lbrack;Substance&rbrack; O espaço da cor UserData para a entrada Normal é invertido em alguns casos
* &lbrack;Shelf&rbrack; Micro-normal em geradores gera curvatura invertida
* &lbrack;Shelf&rbrack; filtro HSL também afeta o canal alfa
* &lbrack;Linux&rbrack; A instalação em Centos falha devido a dependências ausentes
* O instalador não remove todos os recursos da instalação anterior em certos casos

### 3.3.1 (2017.3.1)

*(Lançado: 26 de outubro de 2017)*

**Adicionado:**

* &lbrack;Export&brack; Permite exportar a malha de um projeto
* &lbrack;Shelf&rbrack; Remover “Sub-Shelf” dos títulos das guias
* Salvar configurações de pós-processamento em modelos
* Tornar a mensagem TDR mais compreensível
* Melhorar a janela Configurações para relatar erros

**Corrigido:**

* Falha ao excluir várias subprateleiras
* Falha ao alternar de um nível para algo diferente durante um cálculo do mecanismo
* &lbrack;Mac&rbrack; Falha na GPU Intel durante cálculos do mecanismo
* &lbrack;Mac&rbrack;&lbrack;Viewport&rbrack; Maus desempenhos quando o pontilhamento está ativado
* &lbrack;O Mac&rbrack; MacOS 10.13 é reconhecido como “Versão desconhecida” no arquivo de registro
* &lbrack;Baker&rbrack; Fazer bake com uma gaiola não funciona mais
* &lbrack;Camadas&rbrack; Ctrl + C atalho (ação de cópia) não funciona mais
* &lbrack;Camadas&rbrack; Colar camadas não atualiza a interface com referências de âncora
* &lbrack;Anchor&rbrack; Duplicar ou Copiar/Colar Camada com Referências quebra os links
* &lbrack;Export&rbrack; A exportação em 8K pode travar ou bloquear o aplicativo em alguns casos
* &lbrack;Export&rbrack; Vários problemas no formato de arquivo glTF gerado
* &lbrack;Import&brack; A reimportação de uma malha com o mesmo nome de arquivo não funciona mais
* &lbrack;Plug-in&rbrack; A janela de salvamento automático sempre aparece acima de tudo
* &lbrack;UI&rbrack; Loop infinito ao pressionar “Escape” na caixa de diálogo TDR
* &lbrack;UI&rbrack; Redefinir interface exibe uma segunda barra de título na janela da prateleira

### 3.3.0 (2017.3.0)

*(Lançado: 28 de setembro de 2017)*

**Adicionado:**

* &lbrack;Export&brack; Permitir a exportação de malha e texturas para o Projeto Adobe Felix
* &lbrack;Export&rbrack; Permitir exportação para o formato de arquivo glTF
* &lbrack;Engine&rbrack; Otimizar o tamanho do textura em VRAM usando compactação de bloco
* &lbrack;Visor&rbrack; Ser capaz de arrastar e soltar uma malha ou projeto no visor
* &lbrack;UI&rbrack; Melhorar mensagem de aviso sobre TDR
* &lbrack;UI&rbrack; O registro deve ser exibido somente mediante solicitação
* &lbrack;UI&rbrack; Permite limpar o conteúdo da janela de registro
* &lbrack;UI&rbrack; Exibir avisos e erros na barra de status
* &lbrack;UI&rbrack; Exibir guias na parte superior como em navegadores da Web
* &lbrack;UI&rbrack; Melhorar contexto e mensagens “não pintáveis”
* &lbrack;UI&rbrack; Adicionar uma ação “salvar como cópia” no menu arquivo
* &lbrack;Camada&rbrack; Define a configuração padrão da divisão em blocos gráficos como 1 por padrão
* &lbrack;Shelf&rbrack; Filtro de gradiente aprimorado para suportar 10 cores dinâmicas
* &lbrack;Shelf&rbrack; Adicionar um espaço na consulta padrão da miniprateleira
* &amp;predefinição;Prateleira&amp;predefinição; Adicionar uma ação “Abrir no explorador” para recursos locais na prateleira
* &brack;Prateleira&rbrack; Adicionar modelo e sombreador para o Adobe Material Standard (Projeto Felix)
* &lbrack;Shelf&rbrack; Aumentar o tamanho máximo da divisão em blocos gráficos para 128 nos sombreadores de camada de material
* &lbrack;Prateleira&rbrack; Curvatura sobel adicionada para microdetalhes de Geradores de máscara
* &lbrack;Plug-in&rbrack; Adicionar plug-in de salvamento automático com intervalo de tempo personalizável
* &lbrack;Scripting&brack; Adicionar uma função “salvar como cópia”

**Corrigido:**

* &lbrack;UI&rbrack; O layout é quebrado na primeira inicialização
* &lbrack;Export&brack; o PSD gerado na exportação apresenta erros de formato
* &lbrack;Export&brack; EXR sempre exporta mapa de altura de 8 bits
* &lbrack;Export&brack; Falha ao exportar mapas adicionais corrompidos
* &lbrack;Import&brack; As arestas sólidas não são preservadas em malhas polidas baixas em alguns casos
* &lbrack;Import&brack; Mensagens de erro aprimoradas ao importar malhas com problemas
* &lbrack;Baker&rbrack; Falha na Faz bake do Mapa de ID com a opção Corresponder pelo nome ativada
* &lbrack;Viewport&rbrack; O espaço tangente não está sincronizado com baker
* &lbrack;Efeito&rbrack; Voltar uma camada não restaura a referência de uma âncora
* &lbrack;Efeito&rbrack; Problema de atualização ao criar um link entre duas Máscaras com âncoras
* &lbrack;Efeito&rbrack; As âncoras de máscaras acima da máscara não devem ser listadas
* &lbrack;Efeito&rbrack; Extrair configuração de Alpha de Âncoras não funciona
* &preto;Motor&rbrack; A máscara se inverte após a primeira pincelada
* &lbrack;Engine&rbrack; Falha ao alternar o Conjunto de texturas em um projeto específico
* &Preset;Shelf&rbrack; Falha ao excluir uma predefinição que está em um projeto
* &lbrack;Shelf&rbrack; Erro de ortografia no filtro Tri-Planar avançado
* &lbrack;Shelf&rbrack; MG Mask Builder O A Escala de ruído do AO não funciona corretamente
* O Construtor de máscaras do MG do &brack;Shelf&rbrack; tem parâmetros de curvatura invertidos
* &lbrack;Shelf&rbrack; Alfas importadas geram uma visualização de esfera de material em vez de uma simples

### 3.2.0 (2017.2.0)

*(Lançado: 27 de julho de 2017)*

**Adicionado:**

* Pontos de ancoragem - Sistema de referência de camada e máscara
* &lbrack;Camadas&rbrack; Capacidade de renomear Efeitos de Preenchimento e Tinta
* &lbrack;Plug-in&rbrack; Plug-in Substance Source atualizado
* &lbrack;Scripting&brack; Permitir consultar a Resolução do Conjunto de Texturas
* &lbrack;Scripting&brack; Permite obter o status do mecanismo de Pintura
* &lbrack;Desempenho&rbrack; Otimizações aprimoradas de carregamento e carimbo de pincel no projeto

**Corrigido:**

* &lbrack;Tool&brack; Problemas de desempenho ao ajustar parâmetros de material
* &lbrack;Engine&brack; Desaparecendo traçados de pincel ao alterar a resolução (4K>2K)
* &lbrack;Visualização 3D&rbrack; O espaço tangente não está sincronizado com baker
* &lbrack;Shelf&rbrack; O caminho da prateleira nos documentos do usuário não é criado automaticamente
* &amp;Predefinição;Prateleira&amp;predefinição; Torna as predefinições compatíveis com versões anteriores após uma atualização
* &lbrack;Sombreador&rbrack; O sombreador não-PBR não funciona mais
* &lbrack;Baker&rbrack; Falha na Faz bake do Mapa de ID com a opção Corresponder pelo nome ativada
* &lbrack;Sample&rbrack; O nome do Conjunto de Texturas do Projeto de Amostra da Reunião está incorreto
* Salvar um projeto antes de criar um modelo retorna erros de permissão de gravação

### 3.1.0 (2017.1.0)

*(Lançado: 20 de junho de 2017)*

**Adicionado:**

* &lbrack;Plug-in&rbrack; Novo plug-in de Substance Source (permite o download de ativos na prateleira)
* &lbrack;Shelf&rbrack; 4 Novas Fontes (Japonês + Chinês Simplificado, Máquina de Escrever, Segmento)
* &lbrack;Prateleira&rbrack; 230 Novos Alpha (Mistura de padrões, pincéis e digitalizações de impressão digital)
* &lbrack;Shelf&rbrack; 50 Novos Procedimentos (Padrões de tecido de roupas medievais e contemporâneas)
* &lbrack;Shelf&rbrack; 2 Novos mapas de ambiente (Mondarrain e Villa Nova Street)
* &lbrack;Shelf&rbrack; 9 Novos filtros (MatFx Detail Edge Wear, Restrinjo, HBAO, etc.)
* &lbrack;Shelf&rbrack; Mapa de ambiente padrão aprimorado do Panorama
* &preto;Prateleira&rbrack; Novo Arnold 5 exportar predefinições
* &lbrack;Scripting&brack; Permitir a importação de recursos para a Prateleira

**Problemas Conhecidos:**

* &preto;Exportar&rbrack; A edição de uma predefinição de exportação é muito lenta

## Versão 2

### 2.6.2

*(Lançado: 20 de outubro de 2017)*

**Adicionado:**

* &lbrack;Conjunto de texturas&rbrack; Permite excluir conjuntos de texturas desativados
* &lbrack;Shelf&rbrack; Permite que vários usuários gravem dentro da mesma pasta de prateleira
* &lbrack;Scripting&brack; Ser capaz de recarregar a pasta de plug-ins
* &lbrack;Scripting&rbrack; Adicione uma versão mínima necessária da API nos metadados do plug-in para garantir a compatibilidade
* &lbrack;IRay&rbrack; Melhorias na caixa de diálogo Exportar imagem

**Corrigido:**

* &lbrack;Engine&rbrack; Problema de traçados que desaparecem, ao alterar a resolução (4K>2K)
* &lbrack;Baker&rbrack; Falha na Faz bake do Mapa de ID com a opção Corresponder pelo nome ativada
* &lbrack;Baker&rbrack; As mensagens de erro não são suficientemente explícitas
* &lbrack;Visualização 3D&rbrack; O espaço tangente não está sincronizado com baker
* &preto;Tool&brack; Artefatos pretos ao usar a ferramenta de borrar
* &lbrack;Sombreador&rbrack; O sombreador não-PBR não funciona mais
* &lbrack;Sombreador&rbrack; “pbr-coated” is broken
* &lbrack;Sombreador&rbrack; A aspereza do revestimento do sombreador “pbr-coated” não tem mais impacto
* &lbrack;Sombreador&rbrack; O sombreador com brilho de especificação não corresponde a Iray e SD
* &lbrack;Shelf&rbrack; Falha ao carregar dois arquivos com o mesmo nome, mas extensões diferentes
* &lbrack;Shelf&rbrack; Não é mais possível editar a predefinição nas prateleiras
* &amp;predefinição;Prateleira&amp;predefinição; Não é possível definir uma visualização personalizada para ativos importados na prateleira
* Os recursos carregados do cache perdem seus usos
* Salvar um projeto antes de criar um modelo retorna erros de permissão de gravação
* Salvar projeto incorreto se o nome do arquivo contiver dois pontos
* Importação de arquivos com vários pontos (.) no nome do arquivo causa problemas

### 2.6.1

*(Lançado: 12 de maio de 2017)*

**Adicionado:**

* &lbrack;TextureSet&rbrack; Não permitir a reatribuição de materiais de malha a nada

**Corrigido:**

* Falha ao alternar o TextureSet após substituir o mapa baked
* Falha ao fazer “Desfazer e Refazer” após alterar o modo de mesclagem da camada
* Falha ou congelamento ao usar o efeito “seleção de cores” com um mapa de ID grande
* &preto;Exportar&rbrack; Os conjuntos de texturas renomeados não são classificados em ordem alfabética na janela de exportação
* &lbrack;TextureSet&rbrack; Redefinir para o nome padrão não verifica a unicidade
* &lbrack;TextureSet&rbrack; O conjunto de texturas renomeado fica desativado após a reabertura do projeto
* &lbrack;Shelf&rbrack; Conteúdo de modelos padrão ausente
* &preto;Prateleira&rbrack; As texturas não quadradas são exibidas como quadradas
* &lbrack;Sombreador&rbrack; Quando um conjunto de texturas é desativado, o sombreador associado é destruído
* &lbrack;Scripting&brack; alg.fazendo bake.definirTexturaDefinirParâmetros() não funciona mais
* &lbrack;Erro de ortografia&rbrack; no tutorial do websocket
* &lbrack;Scripting&brack; Vários problemas em AlgWidgets
* &lbrack;Log&rbrack; Detecção incorreta de memória virtual disponível em alguns casos

### 2.6.0

*(Lançado: 27 de abril de 2017)*

**Adicionado:**

* Adicionar novo projeto de amostra “Meet Mat”
* &lbrack;Plug-in&rbrack; Novo plug-in “Atualizador de recursos”
* &lbrack;TextureSet&rbrack; Permite renomear e adicionar uma descrição aos conjuntos de texturas
* &lbrack;TextureSet&rbrack; Permitir a reatribuição de materiais
* &lbrack;TextureSet&rbrack; Adiciona um botão de configuração na janela da lista do conjunto de texturas
* &lbrack;TextureSet&rbrack; Mostrar conjuntos de texturas “desativados” na parte inferior da lista
* &lbrack;Substance&rbrack; Usar mapas adicionais na resolução atual do conjunto de texturas para melhorar o desempenho
* &lbrack;Scripting&rbrack; Permite atualizar um recurso usado em um projeto (material, gerador, etc.)
* &lbrack;Scripting&brack; Adicionar uma maneira de adicionar/remover uma prateleira
* &lbrack;Scripting&rbrack; Permitir a consulta de informações do recurso em projetos
* &lbrack;Scripting&brack; Permite recuperar uma lista de prateleiras disponíveis
* &lbrack;Scripting&brack; Melhorar tutorial em miniatura do AlgWidget
* &lbrack;Export&rbrack; Desativar/Ativar profundidade de bits com base no suporte ao formato de arquivo
* &lbrack;Log&brack; Adicionar nome de plug-in para imprimir no console
* &lbrack;Log&brack; Remove o erro sobre conjuntos de texturas ocultos
* Atualizar “Tela de boas-vindas” com novos ícones e texto para amostras

**Corrigido:**

* Falha ao atualizar uma malha em projetos específicos
* A cor interna do plano de Simetria do &lbrack;Viewport&rbrack; não está mais visível
* &lbrack;Visor&rbrack; Alguns efeitos pós-processo são ativados ao usar a exibição solo
* A mesclagem de &brack;Shaders&brack; “over_premult” não funciona corretamente
* &lbrack;Sombreadores&rbrack; Aviso sobre o teste alfa com o sombreador padrão
* &lbrack;Prateleira&rbrack; Análise incorreta de tags de Substance
* O &lbrack;Shelf&rbrack; MatFX Ferrugem Weathering não funciona corretamente
* O filtro HSL do &brack;Shelf&rbrack; está habilitado em canais incorretos por padrão
* &lbrack;Shelf&rbrack; A nitidez está habilitada no canal Height/Normal por padrão
* &lbrack;Export&rbrack; As predefinições de exportação variadas não usam um mapa normal OpenGL
* &lbrack;Tool&brack; Problemas de imprecisão com a ferramenta clonar/borrar criam artefatos

### 2.5.3

*(Lançado: 15 de março de 2017)*

**Corrigido:**

* &lbrack;Baker&rbrack; Falha ao fazer bake com malhas específicas

**Problemas Conhecidos:**

* &lbrack;Mac&rbrack; Partículas podem criar corrupção de textura em alguns casos

### 2.5.2

*(Lançado: 14 De março De 2017)*

**Corrigido:**

* &lbrack;Tool&brack; Os tablets Wacom não funcionam no Linux
* &preto;Tool&brack; Artefatos pretos ao usar a ferramenta de borrar
* &lbrack;Baker&rbrack; falha na Faz bake se Corresponder pelo nome for usado com uma caixa
* &lbrack;Baker&rbrack; Oclusão de ambiente interrompida ao fazer bake somente com Mapa normal
* &lbrack;Shelf&rbrack; Os filtros genéricos não tratam o alfa corretamente (Contraste/Luminosidade, Highpass, etc.)
* &lbrack;Viewport&rbrack; Problema de desempenho ao carregar um projeto com sombras ativadas
* &lbrack;Viewport&rbrack; Problema de pontilhamento no Visualização 3D MacOS
* &lbrack;Visor&rbrack; Visualizações de partículas exibidas incorretamente quando o perfil de cores está ativado
* &lbrack;Iray&rbrack; Falha ao alternar o projeto de volta para OpenGL se o Iray não inicializar
* &lbrack;IRay&rbrack; A textura reluzente é ignorada ao renderizar SpecGloss sombreador/mdl
* &lbrack;Sombreador&rbrack; O sombreador de especificação/brilho não corresponde a Iray e SD
* &lbrack;Sombreador&rbrack; sRGB conversão diferente de linear para sRGB LUT conversão
* &lbrack;Sombreador&rbrack; Renderização incorreta ao carregar projeto com sombreadores desatualizados
* &lbrack;Sombreador&rbrack; sombreador “pbr-coated” não funciona mais
* &lbrack;Export&brack; Alguns canais ainda são exportados, mesmo que não estejam presentes no conjunto de texturas
* &lbrack;Camadas&rbrack; O modo de mesclagem “detalhe inverso do mapa normal” não funciona em canais em tons de cinza
* &lbrack;UI&rbrack; Problema em “Janela de seleção de cores” com monitor HDPI e zoom de exibição em 150%

**Problemas Conhecidos:**

* &lbrack;Mac&rbrack; Partículas podem criar corrupção de textura em alguns casos

### 2.5.1

*(Lançado: 27 de fevereiro de 2017)*

**Corrigido:**

* &lbrack;A entrada do tablet Mac&rbrack; Wacom está interrompida em 3D e Visualização 2D
* &lbrack;Baker&rbrack; A correspondência por nome não funciona mais
* &lbrack;Baker&rbrack; A configuração de “Média Normalizada” não funciona mais
* &lbrack;Iray&rbrack; Renderização incorreta sem mapa normal feito bake
* &lbrack;Iray&rbrack; Perfis de cores se comportam de maneira diferente em comparação ao renderizador OpenGL
* &lbrack;Iray&rbrack; Exportar a renderização como bitmap não inclui a correção do perfil de cores
* Os Filtros Materiais do &lbrack;Substance&rbrack; não funcionam mais
* &preto;Tool&brack; A opacidade do traçado não está armazenada em predefinições de pincel
* &lbrack;Tool&brack; O Alinhamento UV do Pincel Clonar não funciona mais
* O canal de Deslocamento do &lbrack;Export&brack; deve ser centralizado em 0,5 ao exportar em números inteiros
* &lbrack;Modelo&rbrack; O caminho absoluto é armazenado em Modelos
* A textura do canal do &brack;TextureSet&rbrack; persiste após remover o canal

**Problemas Conhecidos:**

* As entradas dos tablets &lbrack;Linux&rbrack; Wacom não funcionam em 3D e Visualização 2D
* &lbrack;Mac&rbrack; Partículas podem criar corrupção de textura em alguns casos
* &lbrack;Export&brack; Em casos muito raros, retângulos pretos podem aparecer em GPUs AMD

### 2.5.0

*(Lançado em: 21 de fevereiro de 2017)*

**Adicionado:**

* Adicionar compatibilidade com as GPUs AMD Radeon Pro e AMD FirePro
* &lbrack;Tool&brack; Adicionar suporte para opacidade de traçado
* &lbrack;Tool&brack; Adiciona um modificador que permite continuar a última pincelada
* &lbrack;Iray&rbrack; Atualização para suportar GPUs Pascal
* &preto;Visor&rbrack; Adicionar suporte para perfis de cores (LUT)
* &lbrack;Substance&rbrack; Integrar nova estrutura (mecanismo SD6)
* &lbrack;UI&rbrack; Aumentar lista de tamanhos do “arquivo recente” no menu Arquivo
* &lbrack;Import&brack; Usar categoria de substâncias para preencher o prefixo na caixa de diálogo de importação
* &lbrack;Baker&rbrack; Permitir fazer bake texturas 8K
* &lbrack;Baker&rbrack; Permitir fazer bake resoluções não quadradas
* &lbrack;Baker&rbrack; Melhorar o consumo de memória ao fazer bake malhas pesadas de alta poli
* &preto;Shelf&rbrack; Bloquear prateleiras (e projetos) para proibir a edição simultânea e evitar corrupções
* &lbrack;Shelf&rbrack; Ler categoria e palavras-chave de substâncias para usá-las na filtragem
* &lbrack;Shelf&rbrack; Permite excluir recursos do resultado de uma consulta de pesquisa
* &lbrack;Prateleira&rbrack; Cálculo de tempo de miniaturas aprimorado
* &amp;predefinição;Prateleira&amp;predefinição; Permitir incorporar predefinições em projetos
* &lbrack;Shelf&rbrack; Permite recolher/expandir rapidamente a exibição de árvore com SHIFT
* &lbrack;Shelf&rbrack; Permite salvar miniaturas quando os ativos são somente leitura (cache local)
* &lbrack;Shelf&rbrack; Novo conteúdo : novos filtros (transformo, espelho, tri-planar, etc.)
* &lbrack;Shelf&rbrack; Novo conteúdo: novos perfis de LUTs (clássicos e artísticos, como Film Noir, Vintage etc.)
* &lbrack;Shelf&rbrack; Novo conteúdo: 10 novas Substance de fonte para gerar textos personalizados rapidamente
* &lbrack;Shelf&rbrack; Novos modelos: Unity 5 e Unreal Engine 4
* &lbrack;Shelf&rbrack; Filtro HSL aprimorado para ser mais amigável com artistas
* &lbrack;Sombreador&rbrack; Adicionar suporte para canal de specular level em sombreadores PBR
* &lbrack;Sombreador&rbrack; Adicionar suporte para pontilhamento em sombreador de teste
* &lbrack;Sombreador&rbrack; Adicionar suporte para mapeamento de oclusão de paralaxe em sombreadores PBR
* &lbrack;Sombreador&rbrack; Permite definir interface personalizada para parâmetros de sombreador
* &lbrack;MatLayering&rbrack; Criar novo canal de Máscara para fluxo de trabalho de camada de material
* &lbrack;Scripting&brack; Permite gravar metadados em um projeto SP
* &lbrack;Scripting&brack; Permite exportar com uma predefinição de exportação específica
* &lbrack;Scripting&rbrack; Permite recuperar parâmetros de sombreador como um JSON
* &lbrack;Scripting&brack; Adicionar suporte para conexões WebSocket
* &lbrack;Scripting&brack; Adicionar a possibilidade de carregar instâncias de sombreamento
* &lbrack;Scripting&brack; Adicionar a possibilidade de criar um novo projeto
* &lbrack;Scripting&rbrack; Permite recuperar a url da malha importada em um projeto
* &lbrack;Scripting&rbrack; Permitir fça bake não quadrado
* &lbrack;Scripting&rbrack; Relatar erros ao definir dados por meio da API de script
* &lbrack;Substance&rbrack; Adicionar tag de dados do usuário para especificar o formato de mapa normal

**Corrigido:**

* Falha ao selecionar cor com substâncias
* Falha ao carregar uma imagem não RGBA32f como mapa de ambiente
* Falha relacionada à pintura em GPUs AMD
* A importação de OBJ do &brack;Mesh&brack; não reconhece materiais sem arquivo mtl
* &lbrack;Mesh&rbrack; A geração do nome do conjunto de Textura UDIM pode estar incorreta em algumas malhas
* &lbrack;UI&rbrack; Botão Desfazer/Refazer na Configuração do Visualizador roubar foco e parar a rolagem do mouse
* &lbrack;UI&rbrack; Alguns rótulos são cortados incorretamente em Hi-DPI
* &lbrack;Camada&rbrack; O modo de substituição do efeito de tinta possui um comportamento incorreto na Máscara
* O modo de mesclagem &preto;Camada&rbrack; tem um comportamento incorreto com alfa
* &lbrack;Tool&rbrack; O tamanho do pincel se torna muito grande no Visualização 2D ao pintar nas bordas UV
* &lbrack;Tool&brack; A linha reta encaixada apresenta um comportamento irregular com Hi-DPI
* A resolução do estêncil do &brack;Tool&brack; às vezes está incorreta
* Os valores de &lbrack;Baker&rbrack; “Distância máxima do ocluso” serão bloqueados se “em relação à caixa delimitadora” estiver “Desativado”
* &lbrack;Sombreador&rbrack; As definições de canal de parâmetros automáticos e de pilha não correspondem
* &lbrack;Visualização 3D&rbrack; Exibição inconsistente do canal normal dependendo da configuração do projeto
* &lbrack;Viewport&rbrack; Alguns mapas normais têm valores fixados que aparecem como artefatos
* &lbrack;Viewport&rbrack; O pós-efeito sempre é desativado por padrão
* &lbrack;Exportar&rbrack; A configuração de mixagem normal estará incorreta se o canal normal estiver ausente
* &lbrack;Export&rbrack; Geração de textura incorreta em alguns casos em GPUs AMD
* Os parâmetros de Sombreador do &brack;Export&brack; não são exportados corretamente se localizados dentro de um grupo
* &lbrack;Export&brack; Editar uma predefinição de exportação em uma prateleira personalizada gera um erro de registro
* A filtragem do modo de exibição em árvore do &brack;Shelf&rbrack; não corresponde exatamente ao nome da pasta
* &lbrack;Prateleira&rbrack; Renomear uma predefinição de prateleira é difícil de ler
* &lbrack;O recurso de Sombreador importado na Prateleira não é preservado após a reinicialização
* &amp;Predefinição;Prateleira&amp;predefinição; Conteúdo: A predefinição da ferramenta de solda está ausente
* &lbrack;Shelf&rbrack; Conteúdo : Tile Generator não funciona corretamente
* &lbrack;Shelf&rbrack; Conteúdo: correção de máscara incorreta no material inteligente Sujo de Pneu de Borracha
* &lbrack;Shelf&rbrack; Conteúdo: corrigido o nome incorreto do grupo no material do saco de couro
* &lbrack;Iray&rbrack; Metade das malhas está ausente em Iray
* &lbrack;Linux&rbrack; Falha ao arrastar um recurso acima da Visualização 3D
* &lbrack;Mac&rbrack; As preferências são redefinidas a cada inicialização no Sierra

**Problemas Conhecidos:**

* &lbrack;Export&brack; Em casos muito raros, retângulos pretos podem aparecer em GPUs AMD
* Os perfis de cores do &lbrack;Iray&rbrack; podem se comportar de maneiras ímpares às vezes

### 2.4.1

*(Lançado: 28 de outubro de 2016)*

**Corrigido:**

* Falha ao criar um projeto com um modelo
* Falha ao fechar a caixa de diálogo de exportação durante uma exportação
* &lbrack;Mac&rbrack; Erros ao salvar o projeto (falha ao salvar a predefinição de exportação)
* &preset;Shelf&rbrack; Criar uma nova predefinição a exibirá duas vezes
* &preto;O Shelf&rbrack; Predefinições não podem ser carregadas no modo somente leitura sem direitos administrativos

### 2.4.0

*(Lançado: 27 de outubro de 2016)*

**Adicionado:**

* &lbrack;Shelf&rbrack; Nova interface para procurar recursos (exibição de árvore, filtros e assim por diante)
* &lbrack;Shelf&rbrack; Permitir salvar uma pesquisa como predefinição
* &lbrack;Shelf&rbrack; Permite criar uma nova janela a partir de uma predefinição
* &lbrack;Shelf&rbrack; Nova interface para importar recursos
* &lbrack;Prateleira&rbrack; Não copiar a prateleira alegorítmica padrão na pasta Documentos
* &lbrack;Prateleira&rbrack; Novas predefinições de partículas: Circuito Elétrico, Linhas Elétricas, Rococó, Veias Pequenas
* &lbrack;Shelf&rbrack; Predefinições de partículas mais antigas aprimoradas para serem mais fáceis de usar (como “Rain”)
* &amp;predefinição;Prateleira&amp;predefinição; Adicionar novas informações no menu contextual do recurso
* &lbrack;Viewport&rbrack; Melhorar o desempenho ao carregar mapas do ambiente
* &lbrack;Viewport&rbrack; Adicionar suporte a mapas de ambiente que não sejam potência de dois

**Corrigido:**

* Falha ao remover uma máscara
* Falha ao pintar após salvar uma predefinição
* Falha com desfoque de ambiente em algumas GPUs
* Falha ao atribuir um recurso errado com a miniprateleira
* &Preenchimento;Prateleira&rbrack; Limpar + Salvar remove marcas e metadados de recursos no projeto
* &lbrack;Prateleira&rbrack; importar uma predefinição exibirá seus recursos na prateleira
* O Mapa normal &lbrack;Export&brack; gerado a partir do canal do height tem baixa intensidade
* &lbrack;Export&brack; Normal da malha nem sempre está presente no mapa normal final
* &preto;Exportar&rbrack; Dilatação com transparência às vezes pode resultar sem transparência
* &lbrack;Scripting&brack; “alg.plugin_root_diretory” pode retornar um caminho de rede truncado
* O botão Bloquear &preto;TextureSet&rbrack; é ativado ao reabrir projetos não quadrados

### 2.3.1

*(Lançado em: 07 de outubro de 2016)*

**Adicionado:**

* &lbrack;Plugin&rbrack;&lbrack;Photoshop&rbrack; Permite especificar qual material/pilha/canais exportar
* &lbrack;Scripting&rbrack; Os nomes de função possuem algumas inconsistências

**Corrigido:**

* &lbrack;O Alpha de &amp;exportação pode ser descartado nas predefinições de exportação personalizadas
* &lbrack;Export&rbrack; Alpha obtém conversão incorreta de gama em canais sRGB
* &preto;Exportar&rbrack; Documentos não quadrados são exportados como quadrados
* &lbrack;Export&brack; Impossível exportar mapas adicionais se algum estiver faltando
* &lbrack;Iray&rbrack; Alguns parâmetros (como a Intensidade de emissivo) não têm efeito
* &lbrack;NVIDIA&rbrack; Falha na inicialização com NVIDIA Quadro K2200/GTX 750/760
* &lbrack;AMD&rbrack; Conjunto incorreto de cores para miniaturas e visualizações
* &lbrack;AMD&rbrack; Congela e falha do driver em Novo Arquivo e Abrir Arquivo
* &lbrack;Log&brack; “software-version” está ausente do arquivo de log

### 2.3.0

*(Lançado: 15 de setembro de 2016)*

**Adicionado:**

* &lbrack;Plug-in&rbrack; Novo plug-in “Exportar para o Photoshop” (pilha de camadas completa de exportação)
* &lbrack;Export&brack; Permite especificar a largura do preenchimento (em pixels ou infinito)
* &lbrack;Export&brack; Permite definir o tipo de fundo fora dos UVs
* &lbrack;Prateleira&rbrack; Novo sombreador de camadas de material para mesclar 10 materiais
* &lbrack;Prateleira&rbrack; Novo sombreador de argila para ver detalhes com o canal height/normal
* &lbrack;Shelf&rbrack; Novo filtro de iluminação feito bake com entrada de ambiente
* &lbrack;Shelf&rbrack; Alguns geradores de máscara foram atualizados para adicionar transformações não quadradas
* &preto;Visor&rbrack; Adicionar mapa normal composto (normal+height+faço bake) ao modo solo
* &lbrack;Scripting&brack; Permite exportar mapas adicionais
* &lbrack;Scripting&brack; Permitir a consulta de mapas adicionais disponíveis por conjunto de textura
* &lbrack;Scripting&brack; Permitir a recuperação do formato do canal
* &lbrack;Scripting&brack; Adicionar exemplos na documentação de fça bake
* &lbrack;Scripting&brack; Permite consultar a visibilidade de uma camada
* &lbrack;Scripting&brack; Permitir consultar modo de mesclagem e opacidade da camada
* &lbrack;Scripting&brack; Permite exportar mapas convertidos (mapas normais finais, AO misto, etc.)
* &lbrack;Substance&rbrack; Ler e conectar usos personalizados
* &lbrack;Atalhos&rbrack; Adicionar tecla modificadora (SHIFT) para percorrer o modo solo para trás
* &lbrack;Export&brack; Atualização da predefinição de exportação padrão para desativar a alfa
* &lbrack;UI&rbrack; As miniaturas agora são computadas somente se o mecanismo estiver disponível
* &lbrack;UI&rbrack; Exibir uma menção quando as miniaturas estiverem sendo computadas

**Corrigido:**

* Falha com alguns projetos antigos ao abri-los
* Falha com cache de canais de textura corrompido
* Falha ao mesclar mais de 4 materiais com o fluxo de trabalho de Camada de material
* Os atalhos da ferramenta &lbrack;UI&rbrack; não funcionam se a barra de ferramentas estiver oculta
* &lbrack;UI&rbrack; A barra de ferramentas do Iray está rotulada como “Sem Título” no Menu Exibir
* As barras de ferramentas do plug-in &lbrack;UI&rbrack; são chamadas de “Não Inclinadas” no menu Exibir
* &lbrack;Baker&rbrack; Pressionar Enter enquanto edita uma configuração de faço bake inicia o processo do faço bake
* &lbrack;Baker&rbrack; Intervalos incorretos para alguns parâmetros
* &lbrack;Import&rbrack; Impossível importar malhas OBJ devido a números muito grandes
* &lbrack;Import&rbrack; Alguns arquivos OBJ são importados com muitos sub-objetos
* O plano de fundo do canal do &preto;Export&brack; é preenchido com preto em vez da cor padrão na exportação
* &lbrack;Tool&brack; Partículas não funcionam corretamente se o CDV for muito baixo
* A cor de visualização do pincel do &brack;Tool&brack; está incorreta com máscaras em subpilhas
* &lbrack;Visor&rbrack; Quando o pincel vai para áreas vazias no Visualização 2D ele se torna gigantesco
* &lbrack;Visor&rbrack; Visualização do pincel em branco ao pintar texturas normais
* &lbrack;Scripting&rbrack; Documentação incorreta : “ao” listado em vez de “ambientoclusão”
* &lbrack;Scripting&rbrack; O processo iniciado com subprocess() é finalizado ao fechar o Painter
* &lbrack;Shelf&rbrack; filtro de iluminação Feito bake usa entrada de AO incorreta
* &lbrack;MacOS&rbrack; Projeto de hidrante de incêndio removido (incompatível)
* O projeto padrão é aberto ao carregar um arquivo \*.spt (em vez de \*.spp)

**Problemas Conhecidos:**

* &lbrack;Plug-in&rbrack; Devido ao Photoshop, o height e o canal normal não podem ser traduzidos como estão

### 2.2.0

*(Lançado: 22 de julho de 2016)*

**Adicionado:**

* &lbrack;Shelf&rbrack; Melhorar o sistema de pesquisa e as consultas
* &preto;Prateleira&rbrack; Adicionar campo de pesquisa para miniprateleiras
* &lbrack;Sombreador&rbrack; Permite definir a precisão da etapa para controles deslizantes
* &lbrack;Sombreador&rbrack; Adicionar um botão Desfazer/Refazer para parâmetros de sombreador
* &lbrack;Sombreador&rbrack; Recarregar um sombreador não deve redefinir seus parâmetros
* &lbrack;MatLayering&rbrack; Adicionar suporte para Camadas de material dinâmico e subpilhas
* &lbrack;MatLayering&rbrack; Permite importar arquivo json para definir as configurações de sombreador
* &lbrack;MatLayering&rbrack; Desbloquear limite de amostras de textura (alternar para texturas sem associação)
* &lbrack;Scripting&rbrack; Permite definir configurações de baker e iniciar seus cálculos
* &lbrack;Substance&rbrack; Use “uso” para conexões de entradas/saídas, além de identificadores
* &lbrack;Tool&rbrack; Permite selecionar o canal de visualização no visor para a Ferramenta de Projeção

**Corrigido:**

* Falha durante a inicialização se as substâncias estiverem localizadas na pasta errada
* O relatório de falhas às vezes não funciona devido a um arquivo de log incorreto
* &lbrack;Iray&rbrack; os Pós-efeitos não são atualizados quando o Iray é pausado
* &lbrack;Iray&rbrack; O atalho de foco automático não funciona mais
* &lbrack;Iray&rbrack; O comportamento do controle deslizante de abertura muda dependendo do tamanho do ativo
* &lbrack;Camadas&rbrack; O primeiro canal de material não é ativado por padrão se estiver desativado
* &lbrack;Sombreador&rbrack; Nenhum erro será impresso se um “param auto” estiver incorreto

**Problemas Conhecidos:**

* &lbrack;O limite de amostras de Textura do Mac&rbrack; está bloqueado em 16 (problema no driver de GPU)

### 2.1.1

*(Lançado em: 01 de julho de 2016)*

**Adicionado:**

* &lbrack;Licença&rbrack; Ser capaz de alterar o local do arquivo de licença
* &Preenchimento;Visor&amp;Parâmetro; Adicionar um atalho “B” para alternar entre mapas adicionais
* &lbrack;Import&rbrack; Permite importar FBX 2016/2017 corretamente
* &lbrack;Tool&brack; Remover verificadores ao usar a máscara rápida
* &lbrack;Iray&rbrack; Adicionar informações de dimensões de cena
* &lbrack;Iray&rbrack; Permite aumentar o número máximo de amostras e o tempo de renderização
* &lbrack;UI&rbrack; Atualizar resultado imediatamente ao usar o botão +/- nos controles deslizantes
* &lbrack;UI&rbrack; Permite maior precisão para controles deslizantes em Tons de Cinza
* &lbrack;Export&brack; Não exporte um canal alfa somente para o textura RGB
* &preto;Export&brack; Atualizar predefinição de exportação do Dota 2
* &lbrack;Shelf&rbrack; Novo padrão de “ladrilhos de hexágono”
* &lbrack;Prateleira&rbrack; Nova ferramenta “Solda”
* &lbrack;Shelf&rbrack; Filtros de acabamento atualizados para fornecer controles de direção

**Corrigido:**

* &lbrack;Export&brack; Impossível exportar arquivos de PSD em 8 bits
* &lbrack;Export&rbrack; A exportação em 8K não está disponível em algumas configurações de hardware
* &lbrack;A janela do Sketchfab do Export&rbrack; foi cortada
* &lbrack;Export&brack; Mapa de aspereza incorreto na predefinição de exportação de Especificação/Brilho
* &lbrack;UI&rbrack; A digitação em controles deslizantes em tons de cinza não funciona mais
* &lbrack;UI&rbrack; Impossível colocar filtros nas entradas do substance (como Geradores)
* &lbrack;UI&rbrack; Alguns controles deslizantes têm comportamentos ímpares
* &lbrack;UI&rbrack; DeltaTime +/- passo para partículas é muito grande
* &lbrack;Iray&rbrack; Alguns projetos bloqueiam o aplicativo ao mudar para o Iray
* &lbrack;Iray&rbrack; Falha ao detectar hardware
* A cor de visualização do Pincel no &brack;Tool&brack; está incorreta no modo Máscara
* &lbrack;Tool&brack; O seletor de materiais pode ser usado com ferramentas incompatíveis
* &lbrack;Tool&brack; A visualização da projeção não alterna para a Difusão com o fluxo de trabalho Espec/Gloss
* &lbrack;Prateleira&rbrack; Alterar as quebras de sombreador padrão smart mats/visualizações do máscara inteligente
* &lbrack;Shelf&rbrack; Alguns materiais inteligentes têm nomes incorretos
* &lbrack;Shelf&rbrack; Formas alfa adicionais estão corrompidas e não serão carregadas
* &lbrack;Viewport&rbrack; Alternando para o modo “Mapa adicional” exibe “outro” primeiro
* &lbrack;Visor&rbrack; Visor voltar para “outro” quando não existir um mapa adicional
* &lbrack;Crash&rbrack;&lbrack;Linux&rbrack; O relatório de falhas não funciona no Ubuntu (Steam)
* &lbrack;Crash&rbrack;&lbrack;Links de URL da Web do Linux&rbrack; não funcionam no Ubuntu (Steam)
* &lbrack;Crash&rbrack;&lbrack;Windows&rbrack; Remover “crashwatcher” quando o Substance painter não estiver mais em execução
* &lbrack;Crash&rbrack;&lbrack;O sistema de relatório de falhas do Mac&rbrack; não funciona corretamente
* &lbrack;Falha&rbrack; Importar uma malha enquanto já importa uma malha leva a uma falha
* O atalho de separação do conjunto de textura não é redefinido para nada após uma reinicialização

### 2.1.0

*(Lançado em: 2 de junho de 2016)*

**Adicionado:**

* &lbrack;UDIM&rbrack; Importar ladrilhos UDIM de uma malha como conjuntos de texturas
* &lbrack;Linux&rbrack; Suporte adicionado para CentOS 6.6 e Ubuntu 12.4
* &lbrack;Export&brack; Adicionar resolução 8K (experimental)
* &lbrack;Export&brack; Permite escolher a profundidade de bits durante a exportação
* &lbrack;Baker&rbrack; Permite fazer bake vários conjuntos de texturas de uma vez
* Suporte a monitores de alta resolução (dimensionamento de DPI alto)
* &lbrack;Scripting&rbrack; Definir resolução personalizada e preenchimento por textura na exportação
* &lbrack;Viewport&rbrack; Permite alternar entre conjuntos de textura clicando na malha (via Ctrl+Alt+Clique)
* &preto;Visor&rbrack; Ir onde está o cursor do mouse ao aplicar zoom com a roda do mouse
* &lbrack;UI&rbrack; Atualizar cor de fundo padrão e exibição do mapa de ambiente
* &lbrack;UI&rbrack; Adicionar dicas com nomes originais para canais do usuário
* &lbrack;UI&rbrack; Alterar a cor do plano de fundo dos canais que não podem ser renomeados
* &lbrack;Tool&brack; Remover verificadores ao usar a máscara rápida
* &lbrack;Sombreador&rbrack; Permite definir grupos para parâmetros de sombreador e materiais/máscaras
* &lbrack;Engine&rbrack; Otimização de carimbos de tamanho pequeno
* &lbrack;Estêncil&rbrack; Adicionar “W” como atalho para alternar temporariamente a máscara
* &prego;Prateleira&rcolete; Adicionar um botão de cruz para limpar o campo de pesquisa
* &lbrack;Shelf&rbrack; Carregar Alpha com um único clique
* &lbrack;Shelf&rbrack; Nova predefinição de exportação: Vray UDIM, Arnold UDIM, Spec/Gloss from Metal/Rough
* &lbrack;Shelf&rbrack; Novas alfas: formas geométricas, veias e sinais
* Adicionar nome e versão nas propriedades do executável Substance Painter

**Corrigido:**

* &lbrack;Substance&rbrack; Impossível usar o canal normal e mapa adicional ao mesmo tempo
* &lbrack;Iray&rbrack; a refração MDL e a configuração de absorção não funcionam
* &lbrack;Iray&rbrack; A escala da cena original não é preservada
* &lbrack;Shelf&rbrack; modelo de Specular/Textura Reluzente usar um sombreador incorreto
* &preto;Exportar&rbrack; A predefinição de exportação padrão não exporta alguns mapas (como o AO)
* &lbrack;Viewport&rbrack; O ponto dinâmico não é atualizado ao clicar fora dos UVs na Visualização 2D
* &lbrack;UI&rbrack; Os valores do controle deslizante são arredondados
* &lbrack;UI&rbrack; Às vezes, ao editar os valores dos controles deslizantes, há um espaço livre muito pequeno
* &lbrack;A lista suspensa Novo Projeto&rbrack; Modelo não foi atualizada corretamente (de 1.x para 2.x)
* &lbrack;Scripting&brack; Comportamento “hover” fixo em botões personalizados
* &lbrack;Mac&rbrack; Ao desfazer em um projeto vazio, a câmera fica bloqueada

**Problemas Conhecidos:**

* O relatório de falha não está disponível no Ubuntu
* Alguns botões de URL podem não funcionar. Consulte nossas Perguntas frequentes para obter uma solução alternativa

### 2.0.5

*(Lançado: 29 de abril de 2016)*

**Adicionado:**

* &amp;predefinição de prateleira;Modelo não pbr adicionado/atualizado, sombreador e predefinição de exportação
* &lbrack;Shelf&rbrack; Atualizada a predefinição de exportação UE4 para incluir Oclusão de ambiente

**Corrigido:**

* Falha ao abrir e salvar alguns projetos com recursos corrompidos
* &lbrack;Viewport&rbrack; Wireframe aparece quebrado no Visualização 2D
* &lbrack;Shelf&rbrack; Desempenho aprimorado de alguns mapas de ambiente de estúdio
* &lbrack;Shelf&rbrack; Alguns mapas de ambiente de estúdio estão duplicados
* &lbrack;Shelf&rbrack; “Material de Iluminação Feito bake” Ausente
* &lbrack;Shelf&rbrack; Gerador “conversão em tons de cinza” ausente

### 2.0.4

*(Lançado: 26 de abril de 2016)*

**Adicionado:**

* Melhorar colisões de malha e otimizar a renderização de wireframe
* Melhore o desempenho e o gerenciamento de memória com grandes projetos
* Melhorar a precisão e a revisão do controle deslizante
* &lbrack;UI&rbrack; Atualizar mecanismo somente ao validar um controle deslizante (não ao inserir um valor)
* &lbrack;UI&rbrack; Move a opção Iray para um botão dedicado na barra de ferramentas principal (e altera seu atalho)
* &lbrack;Tool&brack; Adicionar configuração para o comportamento de localização da origem da ferramenta clonar
* &lbrack;Sombreador&rbrack; Permitir a leitura de cores de vértice de malha em sombreadores personalizados
* &lbrack;Scripting&brack; Permite recuperar a lista de conjuntos de texturas, canais e camadas
* &lbrack;Scripting&rbrack; Adicionar funções auxiliares (url para caminho, obter caminho de exportação do projeto)
* &lbrack;Mac&rbrack; Detectar versão “El Capitan” do Sistema Operacional Mac no arquivo de registro

**Corrigido:**

* Falha após a segunda exportação para o Substance share
* Falha ao copiar uma camada entre conjuntos de texturas com dados de Máscara rápida.
* Alguns projetos têm um atualizador muito longo que consome muita memória
* &lbrack;Tool&brack; Falha ao selecionar uma predefinição de partícula com a ferramenta clone/borrar
* &lbrack;Baker&rbrack; Carregar arquivos FBX leva muito tempo para malhas pesadas
* &lbrack;Viewport&rbrack; Mapa de ambiente ampliado em alguns computadores
* &lbrack;Visor&rbrack; Conversão de gama incorreta do alfa do pincel
* O Alpha de &brack;Export&brack; é armazenado como transparência em vez de um canal separado com arquivos Tiff.
* &lbrack;Export&brack; O canal Normal é sempre exportado como OpenGL
* &lbrack;Iray&rbrack; Nomes de controle deslizante ausentes para configurações de Iray
* &lbrack;Iray&rbrack; A renderização é feita em uma resolução incorreta em Retina/High DPI
* &lbrack;Iray&rbrack; Falha ao redimensionar a interface no modo Iray
* &lbrack;Iray&rbrack; Enorme redução de desempenho ao renderizar em algumas resoluções baixas
* &lbrack;Iray&rbrack; A pausa não funciona (o Iray ainda é computado em segundo plano)
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

* &lbrack;Iray&rbrack; Atualize o modelo e o sombreador de Spec/Gloss para que sejam compatíveis com o Iray
* &lbrack;Export&brack; Ser capaz de exportar capturas de tela para o ArtStation
* &lbrack;Script&rbrack; Suporte a execução a partir do diretório de plug-ins
* &lbrack;Scripting&rbrack; Permitir “Salvar como”
* &lbrack;UI&rbrack; Permite clicar duas vezes em um controle deslizante para editar seu valor
* Mover amostra do Vela para o Substance share
* Novo projeto de amostra: Visualização da esfera
* Avisar os usuários sobre conflito de extensão do shell

**Corrigido:**

* Instalação de substituição do instalador do Substance Painter 1.x
* &lbrack;UI&rbrack; O layout da lista de canais está quebrado com filtros
* &lbrack;UI&rbrack; os parâmetros de Sombreador não são exibidos
* &lbrack;UI&rbrack; Redimensionar a janela da camada corta incorretamente o conteúdo
* &lbrack;Tool&brack; O canal de Opacidade nem sempre é usado corretamente
* &lbrack;Tool&brack; Borrar/Clonar não funciona com Simetria
* A opacidade da visualização do Pincel no &brack;Tool&brack; está incorreta em alguns canais
* &lbrack;Iray&rbrack; Falha ao usar o Iray enquanto ele ainda não foi criado
* &lbrack;Iray&rbrack; Não é possível carregar os dados de configuração de iray do projeto
* &lbrack;Iray&rbrack; A Iray não cuida da modificação das configurações após ter sido pausada
* &preto;Prateleira&rbrack; Importar um material para a prateleira não funciona
* O estêncil não funciona com o canal Normal
* Falha ao pintar em alguns projetos
* Falha ao pintar com partículas em alguns projetos
* Falha com o Processador de pixels durante alguns cálculos

### 2.0.0

*(Lançado: 16 de março de 2016)*

**Adicionado:**

* Atalho para armazenamento em Substance na barra de ferramentas principal
* Renderizador Iray com modo de visualização e exportação de captura de tela
* Suporte à criação e ao uso do “Máscara inteligente”
* Suporte para o fluxo de trabalho PBR de Specular/Glossários (com o novo canal difuso)
* Substance de encadeamento (conecta substâncias nas entradas de imagem do substance)
* Suporte a scripts com plug-ins personalizados
* Melhorar a conversão de Height em Normal usando um filtro Sobel
* Alternar resolução de visualização de estêncil/projeção para 2K
* Adicionar canal normal por padrão para novos projetos
* Ler a tag de dados do usuário no nó de saída para ativar/desativar os canais de uma substância por padrão
* Expor mesclagem normal/AO nas configurações do TextureSet
* &lbrack;Tool&brack; Nova ferramenta Borrar para mesclar e espalhar cores
* &lbrack;Tool&rbrack; Nova ferramenta Clonar para copiar parte do textura
* &lbrack;Tool&brack; Permite selecionar canais para as ferramentas Borrar, Clonar e Borracha
* &lbrack;Layer&rbrack; Adicionar nome de Substance para nome do efeito de preenchimento
* &lbrack;Camada&rbrack; Permitir exportação de máscara para área de transferência
* &lbrack;Visor&rbrack; Alternar entre os modos de Perspectiva e ortográfica
* &lbrack;Viewport&rbrack; Permitir controlar o Campo de Visão no modo de Perspectiva
* &lbrack;Visor&rbrack; Permitir definir a Profundidade da distância do campo com CTRL+clique no meio
* &lbrack;Viewport&rbrack; Permite arrastar e soltar mapas de ambiente no Visualização 3D.
* &lbrack;Viewport&rbrack; Feedback aprimorado quando o mecanismo está fazendo cálculos fortes
* &lbrack;Export&brack; Permite exportar parâmetros de sombreador em um arquivo json
* &lbrack;UI&rbrack; Atualizar interface com novos ícones, cores e layout
* &lbrack;UI&rbrack; Adicionar nomes de ativos às miniprateleiras
* &lbrack;UI&rbrack; Recolher “Mapeamento de canais” por padrão
* &lbrack;Sombreador&rbrack; Escolha uma cor personalizada para os parâmetros de textura do sombreador
* &lbrack;Shelf&rbrack; Perguntar onde importar arquivos ao arrastar e soltar recursos
* &lbrack;Shelf&rbrack; Nova esfera de visualização para Materiais inteligentes e Geradores
* &preto;Prateleira&rbrack; Adicionar Specular Brilho sombreador
* &preto;Prateleira&rbrack; Novas formas de Superfície Dura
* &lbrack;Prateleira&rbrack; Novas Alpha textura e formas
* &preto;Prateleira&rbrack; Novas texturas de pele
* &lbrack;Shelf&rbrack; Novos materiais e materiais inteligentes baseados em digitalização
* &lbrack;Shelf&rbrack; Novos materiais inteligentes e suporte a especificações/brilhos de antigos
* &lbrack;Shelf&rbrack; Novos filtros de acabamento para simulação de superfície metálica
* &lbrack;Shelf&rbrack; Novo gerador de máscara poderoso “Editor de máscaras”
* &lbrack;Prateleira&rbrack; Materiais antigos retrabalhados e limpos
* Novo projeto de amostra “Vela”

**Corrigido:**

* &lbrack;Configurações&rbrack; A rotação da câmera e a velocidade de zoom são substituídas pelo projeto
* &lbrack;Viewport&rbrack; O problema de precisão na textura normal padrão leva a reflexos incorretos
* A vinheta do &lbrack;Viewport&rbrack; está ativada por padrão
* &brack;Visor&rbrack; Os artefatos aparecem nas bordas do mapa de ambiente (GPUs Nvidia)
* &lbrack;Viewport&rbrack; A miniatura no modo de projeção/estêncil é muito longa para carregar
* &lbrack;Baker&rbrack; Armazenar texturas feitas bake em inteiros de 16 bits em vez de 32 bits
* &lbrack;Layer&brack; Substâncias desatualizadas são exibidas incorretamente na pilha
* A cor padrão e a profundidade de bits de alguns canais estão incorretas (por exemplo: Specular, Textura reluzente)
* Corrigido o comportamento de borracha para desativar a mesclagem no modo de passagem

**Problemas Conhecidos:**

* A simetria não funciona com as ferramentas Borrar e Clonar
* A exportação do ArtStation está ausente

## Versão 1

### 1.7.3

*(Lançado em: 01 de março de 2016)*

**Adicionado:**

* &lbrack;Export&brack; Adicionar uma opção para desativar o preenchimento
* &lbrack;Prateleira&rbrack; Suporta hierarquia de sub-prateleira dentro de uma pasta de prateleira

**Corrigido:**

* Falha ao salvar sobre arquivo somente leitura anterior
* Falha ao abrir um segundo projeto
* Falha ao carregar algumas miniaturas (prateleira, camadas ou dicas de ferramentas)
* A desativação da opção “Preservar posições de traçados na malha” não funciona
* &lbrack;Export&brack; A ampliação de bitmaps é feita com a filtragem mais próxima
* &lbrack;Shelf&rbrack; A descoberta de recursos é muito lenta
* Os filtros de &amp;predefinição;prateleira&preta; desfoque não são compatíveis com 16 bits
* &lbrack;A Simetria do &amp;Tool&rbrack; não funciona se você carregar uma predefinição de ferramenta antiga
* A caixa de diálogo de cor do canal de Specular não faz uma conversão do espaço de cor

### 1.7.2

*(Lançado: 13 de janeiro de 2016)*

**Adicionado:**

* &lbrack;Camadas&rbrack; Permite especificar a inclinação padrão para camadas de preenchimento

**Corrigido:**

* &lbrack;Export&rbrack; A exportação do Sketchfab não funciona mais
* A filtragem bilinear &preto;Camada&rbrack; é aplicada mesmo no Preenchimento sem nenhuma transformação
* &lbrack;Tool&brack; Baixo desempenho usando o substance com entradas de imagem no modo de projeção
* &lbrack;Tool&brack; O seletor de materiais está danificado

### 1.7.1

*(Lançado: 18 de dezembro de 2015)*

**Corrigido:**

* Falha ao alternar o conjunto de textura
* Desempenho lento ao pintar

### 1.7.0

*(Lançado: 17 de dezembro de 2015)*

**Adicionado:**

* &lbrack;Performances&rbrack; Calcula o conteúdo das camadas e suas miniaturas ao mesmo tempo
* &preto;Exportar&rbrack; Salvar caminho de exportação como relativo quando próximo ao projeto
* &lbrack;Camadas&rbrack; Adicionado novo modo de mesclagem : subtrair e adicionar/sub
* &preto;Camadas&rbrack; Nova filtragem de matriz bilinear para camadas de preenchimento
* &lbrack;Sombreador&rbrack; Defina um sombreador padrão para geração de miniaturas nas preferências.
* &lbrack;Sombreador&rbrack; Permite especificar um sombreador por conjunto de textura
* &lbrack;Sombreador&rbrack; Permite obter amostras de texturas da prateleira
* &lbrack;Tool&brack; Novo comportamento de pincel “em contorno” para pintura
* &lbrack;Tool&brack; Filtragem aprimorada e suavização reduzida ao pintar
* &lbrack;Tool&brack; Qualidade da pintura de subpixels aprimorada
* &lbrack;Tool&brack; Exibição “básica” removida para configurações de pincel e aprimoramento do ícone de abrir/fechar quadro
* &preto;Menu&rbrack; Adicionar ícones de efeitos no menu do botão direito
* Criação de modelo a partir de projetos
* &lbrack;Shelf&rbrack; Novos modelos: PBR, Dota 2
* &preset;Prateleira&rbrack; Nova predefinição de exportação: Dota 2
* &lbrack;Prateleira&rbrack; Novos sombreadores: Dota 2, tinta de carro PBR, PBR Coated, PBR Velvet
* &lbrack;Prateleira&rbrack; Novo material: ferrugem e desgaste de aço, iluminação estilizada
* &lbrack;Shelf&rbrack; Novos filtros : Desfocar iluminação direcional, estilizada
* &lbrack;Shelf&rbrack; Novo pincel: padrão suave e padrão rígido com um novo alfa para um melhor controle de dureza
* &lbrack;Shelf&rbrack; Novos geradores: Distância e Luz 3D
* &lbrack;Prateleira&rbrack; Pincéis atualizados com projeção de quebra e remoção de face de fundo (ativada por padrão)
* &lbrack;Shelf&rbrack; Ruído branco atualizado com a versão do processador de pixels para computação mais rápida

**Corrigido:**

* &lbrack;Tela de boas-vindas&rbrack; Tutorials enviar para vídeos antigos
* &lbrack;Canais&rbrack; Dizendo “não” para preencher a criação de camada com AO ainda cria a camada
* &lbrack;Canais&rbrack; Os nomes dos canais do UserX não se propagam na interface
* &lbrack;Visor&rbrack; A entrada da Máscara está vazia na lista de canais individuais
* &lbrack;Share&brack; Exportar um alfa para Compartilhar a partir do SP cria um arquivo .image ilegível
* &lbrack;License&rbrack; Corrigir ativação de nomes de usuário com caracteres não ASCII
* &lbrack;Sombreador&rbrack; A caixa de diálogo do parâmetro de cor desaparece ao escolher uma cor
* &lbrack;Shelf&rbrack; Miniaturas não são descarregadas da memória quando não usadas
* &preto;Suporte de prateleira; Filtro de gradiente fixo
* &lbrack;A Simetria do &amp;Tool&brack; não funciona com estêncil/projeção
* &lbrack;Tool&brack; Nome incorreto ao criar uma nova predefinição de pincel
* A configuração Preservar traçado permanece desativada mesmo ao reimportar uma malha
* Reinicialização do driver (TDR) ao calcular partículas com tamanho grande.

### 1.6.1

*(Lançado: 09 de novembro de 2015)*

**Corrigido:**

* Falha ao abrir projeto se o Visualização 2D estiver visível
* Falha ao criar nova predefinição de exportação se a prateleira atual não existir
* &lbrack;Tool&brack; O ícone do seletor de materiais pode permanecer exibido
* &lbrack;Tool&brack; O seletor de materiais oculta o cursor do mouse ao pintar ao mesmo tempo
* &lbrack;Shelf&rbrack; Os metadados são gravados no disco após cada saída

### 1.6.0

*(Lançado: 29 de outubro de 2015)*

**Adicionado:**

* Suporte oficial para Windows 10
* &lbrack;Substance&rbrack; Recolher grupos de parâmetros de substância por padrão
* &lbrack;Substance&rbrack; Adicionar nova estrutura (Melhorar o desempenho do Processador de pixels)
* &lbrack;Viewport&rbrack; Permite desativar a exibição do plano de simetria no modo de simetria.
* &preto;Visor&rbrack; Melhorar o desempenho e a renderização das sombras
* &preto;Visor&rbrack; Pausar computação de sombra ao pintar
* &lbrack;Visor&rbrack; Melhorar o desempenho da renderização do wireframe
* &lbrack;Engine&rbrack; Melhorar o gerenciamento de memória Vram para reduzir seu espaço
* &lbrack;Engine&rbrack; Melhorar a atualização de textura em GPUs AMD para melhores desempenhos
* &lbrack;Engine&rbrack; Desabilitar configuração de Otimização encadeada em GPUs NVIDIA para melhor desempenho
* &lbrack;Efeito&rbrack; Adiciona uma marca para solicitar entrada de imagem “preenchida”
* &lbrack;Camada&rbrack; Aumenta a precisão do Deslocamento UV/escala no preenchimento
* &lbrack;Layer&brack; Torna o controle deslizante de escala exponencial no preenchimento
* &lbrack;Layer&brack; Permite arrastar e soltar materiais diretamente na pilha de camadas.
* &lbrack;Layer&brack; Permite arrastar e soltar filtros diretamente na pilha de camadas
* &lbrack;Camada&rbrack; Ajusta a cor do pincel da máscara para a cor de máscara recém-criada
* &lbrack;Sombreador&rbrack; Expor várias texcoords
* &lbrack;Sombreador&rbrack; Expor a função de mapeamento de gama/tons para permitir funções personalizadas
* &lbrack;Baker&rbrack; Alterar configurações padrão do baker de posição para uso TriPlanar
* &lbrack;Tool&brack; Renomear “Decalque de geometria” como “Preenchimento de polígono”
* &lbrack;Prateleira&rbrack; Atualize os geradores para suportar o TriPlanar: MG Metal edge wear, MG Mask builder, MG Fiber glass, MG Dirt
* &lbrack;Prateleira&rbrack; Atualizar materiais com novas configurações e materiais não utilizados removidos
* &lbrack;Shelf&rbrack; 22 novos materiais inteligentes (plástico, ferro, tecido, aço e mais)
* &preto;Prateleira&rbrack; Atualize os filtros de Nitidez, Desfoque e Distorção com entrada de imagem preenchida para evitar emendas
* &lbrack;Shelf&rbrack; Melhorar as configurações de Distorção para facilitar o uso
* &lbrack;Shelf&rbrack; 2 Novos ruídos processuais: ruído 3D Perlin e ruído 3D Worley

**Corrigido:**

* &lbrack;Engine&rbrack; A detecção da quantidade de Vram para a GPU dedicada está incorreta no Mac
* &lbrack;Motor&rbrack; as Texturas mudam para a versão mais escura no visor
* &preto;Engine&brack; Maus desempenhos ao pintar abaixo de várias camadas
* &lbrack;Engine&rbrack; As camadas calculadas ao abrir o projeto diferem da versão armazenada em cache
* &lbrack;Substance&rbrack; Resultados incorretos em 4K no Mac
* Os parâmetros do &lbrack;Substance&rbrack; estão na ordem errada
* &lbrack;Sombreador&rbrack; Os sombreadores de tom e pixelado são totalmente pretos
* &lbrack;Sombreador&rbrack; Os parâmetros desaparecem após alterar o mapa de ambiente
* &lbrack;Shelf&rbrack; Falha ao colocar arquivos png na pasta do gerador
* &lbrack;Shelf&rbrack; Miniaturas são geradas com baixa aspereza
* &lbrack;Tool&brack; Falha ao usar um bitmap na alfa do pincel no Windows
* &lbrack;Export&brack; Mapa adicional exportar predefinição agora exportar um mapa de RGB para a Posição

### 1.5.7

*(Lançado: 24 de setembro de 2015)*

**Corrigido:**

* O relatório de falha não funciona mais

### 1.5.6

*(Lançado: 21 de setembro de 2015)*

**Adicionado:**

* &lbrack;Shelf&rbrack; Melhorar a qualidade da renderização de miniaturas (usar texturas de 1K)

**Corrigido:**

* &lbrack;Share&brack; Impossível assinar com outra conta
* &lbrack;Shelf&rbrack; Miniaturas são muito pesadas no disco
* Os Materiais inteligentes do &brack;Shelf&rbrack; são muito lentos para carregar
* &lbrack;Windows&rbrack; Corrigir a instalação do serviço de licença
* &lbrack;Canais&rbrack; o mapa de Transmissivo é criado como G8 por padrão

### 1.5.5

*(Lançado: 15 de setembro de 2015)*

**Adicionado:**

* &presilha;Prateleira&rcolha; Exportar ativos para o Substance share
* &preto;Shelf&rbrack; Adicionar nova visualização de esfera para Materiais
* &lbrack;Shelf&rbrack; Usar o mapa de ambiente “Pátio envidraçado” para gerar miniaturas
* &lbrack;Prateleira&rbrack; Aumentar a resolução do tamanho da miniatura para 512x512 pixels
* &lbrack;Visualização 3D&rbrack; Expor valor de rotação do ambiente
* &lbrack;Windows&rbrack; Assine o aplicativo

**Corrigido:**

* &lbrack;Baker&rbrack; Resultados incorretos ao fazer bake mapas ao mesmo tempo
* &lbrack;Visualização 3D&rbrack; O mapa de ambiente é exibido quando nenhum projeto está aberto
* &lbrack;Camadas&rbrack; os Geradores de máscara não funcionam no conteúdo da camada
* &lbrack;Camadas&rbrack; Você pode tinta em camadas ocultas
* O ruído do &lbrack;Shelf&rbrack; Dirt_5 e Dirt_6 é idêntico
* &lbrack;Shelf&rbrack; Alguns geradores de máscara estão pixelados ou em baixa qualidade
* &lbrack;Tool&brack; Rotação incorreta do cursor em determinados ângulos.
* &lbrack;Tool&brack; Muitos canais fazem com que os botões do canal sejam cortados
* &lbrack;O atalho Inverter máscara para Máscara rápida não funciona
* &lbrack;Export&brack; Sketchfab: o botão cancelar não foi levado corretamente em consideração
* &lbrack;Licença&rbrack; A ativação falhou quando a licença não pode ser copiada
* O limitador de taxa de quadros não funciona mais na interface do usuário

### 1.5.0

*(Lançado: 20 de agosto de 2015)*

**Adicionado:**

* &lbrack;Sombreador&rbrack; Adicionar número de linha em mensagens de erro de compilação de Sombreador
* &preto;Prateleira&rbrack; Melhorar a qualidade de visualizações de miniaturas
* &lbrack;Shelf&rbrack; Automatizar geração de miniaturas para Materiais inteligentes
* &lbrack;Tool&brack; Atalho para controlar a configuração de dureza na substância
* &preto;Tool&brack; Usar widget de tons de cinza para decalque geométrico quando estiver sobre uma máscara
* &lbrack;Tool&brack; Atalho para inverter a cor da tinta ao pintar em um mapa em tons de cinza
* &lbrack;Viewport&rbrack; Permite exibir o wireframe e alterar sua cor
* &preto;Visor&rbrack; Desfocar o plano de fundo do ambiente
* &preto;Controles&rbrack; Adicionar rotação aos atalhos de mouse do pincel
* &preto;Exportar&rbrack; Exportar para Sketchfab
* &preto;Exportar&rbrack; Criar predefinições de exportação para renderizadores
* &lbrack;Export&brack; Adicionar Reflexo de mapa convertido, F0 e 1/IOR
* &lbrack;UI&rbrack; Adicionar tela de boas-vindas
* &lbrack;UI&rbrack; Atualizar layout padrão
* &lbrack;UI&rbrack; Adiciona dicas de ferramentas ausentes e renomeia algumas entradas do menu
* &lbrack;Camadas&rbrack; Exportar máscara selecionada atualmente como bitmap
* &preto;Camadas&rbrack; Adicionar ação “inverter máscara” no menu do botão direito

**Corrigido:**

* &lbrack;Projeto&rbrack; Se os pivôs das malhas forem diferentes no FBX, as malhas são explodidas na importação
* &lbrack;Substance&rbrack; os Substance usados nas ferramentas de projeção estão bloqueados em 256\*256
* &lbrack;Camadas&rbrack; Falha ao usar limpar máscara
* &lbrack;Export&brack; Conversão de gama incorreta em texturas muito escuras
* &preto;Exportar&rbrack; O mapa de posição só pode ser usado em predefinições de exportação como um mapa em tons de cinza
* &lbrack;Tool&brack; A cor inicial do decalque de geometria é preta quando usada em uma máscara
* O atalho de rotação do &preto;Tool&brack; não funciona se não houver dureza no alfa

### 1.4.2

*(Lançado: 15 de julho de 2015)*

**Corrigido:**

* &lbrack;Tool&brack; Falha ao usar o decalque de geometria com máscara rápida
* A atualização do projeto da versão 1.4.0 para a 1.4.1 consome toda a memória do computador
* Importação incorreta do formato do projeto antigo
* Prateleiras personalizadas analisam toda a hierarquia e duplicam ativos em todos os lugares

### 1.4.1

*(Lançado: 23 de junho de 2015)*

**Adicionado:**

* &Preenchimento;Visor&Preenchimento; Permitir encaixar painéis lado a lado
* &preto;Efeito&rbrack; Adiciona um plano de fundo e uma régua para o efeito de nível
* &lbrack;Efeito&rbrack; Adicionar um efeito de Tinta que permita trabalhar sobre outro efeito

**Corrigido:**

* &lbrack;Shelf&rbrack; A geração de miniaturas é interrompida se nenhum projeto estiver aberto
* &preto;Shelf&rbrack; A visualização predefinida do material não é gerada
* &preto;Shelf&rbrack; As visualizações de material são geradas em uma malha com normais invertidos
* &lbrack;Shelf&rbrack; Miniaturas sempre recalculam por causa de função de hash incorreta
* &lbrack;Shelf&rbrack; Clicar em um material do substance não conecta mapas adicionais
* &lbrack;Tool&brack; Valor incorreto amostrado com seletor de material
* &lbrack;Tool&brack; Seletor de cores selecionar cor do cursor do visor
* &lbrack;Visualização 2D&rbrack; Taxa de quadros/desempenhos muito baixos
* &lbrack;Export&brack; Falha ao abrir a janela de exportação com predefinições de exportação muito recentes.
* &lbrack;Exportar&rbrack; canal de Height para Mapa normal é convertido para o espaço errado
* &lbrack;Mac&rbrack; BaseColor dos efeitos do substance é exibido como Linear
* &lbrack;O widget de linhas retas do Mac&rbrack; foi desenhado incorretamente na Retina
* As linhas retas podem permanecer ativadas mesmo com o atalho liberado.
* O guizmo de linhas retas desaparece após girar o mapa ambiental
* As saídas de oclusão de ambiente de substâncias não são conectadas ao canal AO automaticamente
* Corrigir problema de cópia de licença no Windows com caractere especial no nome de usuário

### 1.4.0

*(Lançado: 10 de junho de 2015)*

**Adicionado:**

* &lbrack;Export&brack; Adiciona mapas adicionais na lista de mapas de entrada disponíveis
* &amp;predefinição;Prateleira&amp;predefinição; Usar materiais sbsar como predefinições de material
* &lbrack;Shelf&rbrack; Permitir o uso de caminhos de Biblioteca personalizados
* &lbrack;Shelf&rbrack; Alterar o tamanho mínimo
* &lbrack;Shelf&rbrack; Novo conteúdo: 20 novos materiais inteligentes
* &lbrack;Shelf&rbrack; Novo conteúdo : nova substância processual (weave, mesh)
* &lbrack;Shelf&rbrack; Filtro de desfoque atualizado
* Desenhar linhas retas usando uma tecla modificadora
* Adicionar canal de Oclusão de ambiente e retrabalhar o comportamento AO/Normal no pilha de camadas
* Ler a cor padrão da Entrada de imagem definida nos dados do usuário Substance
* Permitir a exportação do log a partir do menu Ajuda

**Corrigido:**

* &lbrack;Baker&rbrack;&lbrack;Mac&rbrack; Falha com Normal do baker de malha
* &lbrack;Baker&rbrack; Falha se não houver UVs no arquivo de caixa
* &lbrack;Baker&rbrack; A correspondência por nomes não funciona com OBJ exportado do zBrush
* &lbrack;Baker&rbrack; Fazer bake com uma caixa sobrescreve o faço bake se forem usados vários conjuntos de texturas e UVs sobrepostos
* &lbrack;Baker&rbrack; Arquivos OBJ específicos resultam em texturas pretas
* &lbrack;Shelf&rbrack; Não é possível ler recursos se estiver definido como somente leitura
* &lbrack;Shelf&rbrack; Os arquivos de ativos estão sendo gravados no Painter se tiverem sido usados no projeto.
* &lbrack;Shelf&rbrack; Recarregando substâncias também atualiza a camada
* &lbrack;Export&brack; Tiff exporta imagens de 32 bits que não podem ser lidas corretamente pelo Photoshop ou mecanismos de jogo
* &lbrack;Export&rbrack; Predefinição de canais padrão sempre exportar como RGB
* &lbrack;Material&rbrack; canal de Difusão sobrepõe o mapeamento de BaseColor com substâncias
* &lbrack;Visualização 3D&rbrack; Iluminação incorreta de Difusão com mapas de ambiente específicos
* &lbrack;Tool&brack; Não é possível girar um pincel para um ângulo específico
* O visor obtém o foco quando o mouse é ativado ao digitar em um campo de texto
* Falha com predefinições muito recentes para a versão atual da prateleira
* Falha após substituir a malha
* Falha ao recarregar uma substância com um número diferente de entradas
* Malhas FBX da importação do Cinema4D com nomes de material incorretos

### 1.3.5

*(Lançado: 29 de maio de 2015)*

**Adicionado:**

* &lbrack;Problema de ativação do License&rbrack; quando já existe um arquivo de licença
* &lbrack;Mac&rbrack; Falha ao carregar arquivos FBX específicos
* &lbrack;Mac&rbrack;&lbrack;Visualização 3D&rbrack; Reflexão incorreta para GPU integrada
* A fonte da Máscara rápida do &lbrack;Visualização 3D&rbrack; está quebrada
* &lbrack;Visualização 3D&rbrack; O seletor de materiais torna o visor totalmente preto
* Falha após abrir projetos criados na versão 1.3.3
* A visualização do material fica vazia ao usar sombreadores com alfa
* Pintura para de funcionar em malhas específicas
* O desempenho diminui muito com malhas específicas de OBJ
* Os canais do usuário não são mapeados ao usar efeitos
* As pastas temporárias não são limpas na inicialização

**Corrigido:**

* Melhorias no tempo de computação em projetos extremamente longos para carregar
* Altere a janela “Solução de problemas de GPU” para ser mais compreensível
* &preto;Camadas&rbrack; Salva o status do bloqueio de proporção para camadas de preenchimento e torna-o “Ativado” por padrão
* &lbrack;Baker&rbrack; Correspondência por nome agora usar sufixo como separador

### 1.3.4

*(Lançado: 27 de abril de 2015)*

**Adicionado:**

* &lbrack;Mac&rbrack; Falha com o Mac OS X Yosemite (10.10)
* &lbrack;Mac&rbrack; Impossível sair do modo de tela cheia
* &lbrack;Baker&rbrack; Fazer bake a opção de correspondência por nome não funciona
* &lbrack;Baker&rbrack; O espaço tangente Mikk usado no SP não funciona com UE4
* &lbrack;Baker&rbrack; O baker de ID não pode fazer bake as cores de ID do material
* &lbrack;Visualização 2D; não aparece ao usar a ferramenta de decalque de Geometria
* O canal alfa do Pincel &preto;Tool&brack; é exibido como verificador em vez de transparência com materiais
* &lbrack;Tool&brack; Falha com decalque de geometria
* &lbrack;Camadas&rbrack; O slot de material é recolhido por padrão na camada de preenchimento
* &lbrack;Export&brack; Falha ao exportar em tamanho maior do que a resolução do conjunto de textura
* O canal do specular não é reconhecido nos filtros.
* Limpar e salvar não remove os recursos do arquivo do spp corretamente
* Não armazenar transformação de baixo polígono em arquivo de alta poliuretagem do compartimento
* O arquivo FBX é importado com muitos conjuntos de textura

**Corrigido:**

* Efeitos: o Restrinjo de níveis deve estar ativado por padrão para imitar níveis “clássicos”
* Camadas: alterar a divisão mínima e máxima na ação Preencher
* Camadas: salvar e restaurar o status da pilha
* Baker: Baker AO levar o mapa normal em consideração se nenhum HP for especificado
* Baker: dicas de ferramentas e informações adicionais adicionadas à janela de fça bake
* Criar um arquivo de backup ao salvar um projeto

### 1.3.3

*(Lançado em: 01 de abril de 2015)*

**Adicionado:**

* Adicionar versão de software e nome do projeto na barra de título
* Limpar nomes de TextureSet e nomes de Material inteligente
* Atualizar mecanismo de Substance para V5
* &lbrack;Shelf&rbrack; Adicionar novos mapas de ambiente: Corsica beach, studio 05, Tornoco studio e mais
* &presilha;Prateleira&rbrack; Atualizar MG Construtor de máscaras com novos parâmetros
* &lbrack;Shelf&rbrack; Atualizar e calibrar mapas de ambiente antigos

**Corrigido:**

* Falha ao abrir a janela de exportação
* Não é possível arrastar e soltar no widget da interface do usuário quando desencaixado
* “Verificar atualizações” não está funcionando
* &lbrack;Camadas&rbrack; Não selecione a máscara ao pressionar ALT+clique nela
* &lbrack;Tool&brack; Tri-planar não funciona com o canal Normal
* &lbrack;Visualização 3D; a iluminação da Difusão do mapa de ambiente está incorreta
* O cálculo da exposição do &lbrack;Visualização 3D&rbrack; é diferente do Designer
* &lbrack;Visualização 3D&rbrack; As sombras não devem estar visíveis em uma superfície 100% metálica
* &lbrack;Visualização 3D&rbrack; A malha com UVs espelhados inverteu a tangente/binômios
* &lbrack;Visualização 3D&rbrack; Sombras produzem resultados incorretos em determinadas malhas
* &lbrack;Baker&rbrack; Remove a pasta “.alg_meta” criada por arquivos assbin
* &lbrack;Baker&rbrack; Falha ao fazer bake se o Painter recalcula um TextureSet ao mesmo tempo
* &lbrack;Mac&rbrack; Falha na interface do usuário do White Box ao iniciar o aplicativo

### 1.3.2

*(Lançado: 06 de março de 2015)*

**Corrigido:**

* &lbrack;Visualização 3D&rbrack; Falha ao recarregar um mapa de ambiente salvo com o projeto

### 1.3.1

*(Lançado: 05 de março de 2015)*

**Adicionado:**

* &lbrack;Baker&rbrack; Adicionar uma versão em cache de malhas de alto-polígono para acelerar o cálculo
* &lbrack;Baker&rbrack; Adiciona um ícone de aviso se nenhuma malha de alto polígono estiver carregada
* &lbrack;Baker&rbrack; Se nenhuma malha de alto polígono estiver carregada, use a malha do projeto

**Corrigido:**

* &lbrack;Baker&rbrack; Pressionar “enter” ao editar o valor de um controle deslizante fecha a janela
* &lbrack;Baker&rbrack; Ativar/Desativar um baker também acionará o botão
* &lbrack;Baker&rbrack; Impossível fazer bake se você usar o botão “tudo/nenhum”
* &lbrack;Baker&rbrack; A ordenação dos botões de baker não está na ordem correta
* &lbrack;Baker&rbrack; Caixa de seleção são ignoradas e todos os baker são sempre processados
* &lbrack;Baker&rbrack; Progresso da barra de progresso fixo

### 1.3.0

*(Lançado: 04 de março de 2015)*

**Adicionado:**

* &lbrack;Baker&rbrack;&lbrack;Visualização 3D&rbrack; Usar computação de espaço tangente Mikkt se nenhuma tangente/binormal for encontrado
* &lbrack;Baker&rbrack; Adicionados novos baker: Normal, ID, Oclusão, Curvatura, Thickness, Posição
* &lbrack;Efeitos&rbrack; A pilha de efeitos agora está invertida e exibida de cima para baixo (como camadas)
* &lbrack;Efeitos&rbrack; Adicionar novos ícones na pilha de efeitos
* &lbrack;Efeitos&rbrack; Adicionar modo de mesclagem entre ações de preenchimento na pilha de efeitos
* &lbrack;Efeitos&rbrack; Renomear efeitos (efeito da substância = filtro, etc.)
* Adicionar um arquivo de “bloqueio” durante o processo de salvamento
* &preto;Efeitos&rbrack; Adicionar ação Preenchimento na pilha de efeitos
* Adicionado novo recurso : Materiais inteligentes
* &lbrack;Camadas&rbrack; Permitir a reordenação de efeitos de camada
* &lbrack;Tool&brack; Adicionar projeção tri-Planar
* &lbrack;Visualização 3D&rbrack; Adicionar suporte para sombras
* &lbrack;Visualização 3D&rbrack; Capacidade de definir estados OpenGL necessários em sombreadores personalizados
* &lbrack;Visualização 3D&rbrack; Suporte para alfa através de novos sombreadores
* &lbrack;Visualização 3D&rbrack; Os sombreadores agora possuem versão e foram salvos completamente em um projeto
* &lbrack;Visualização 3D&rbrack; Avisa o usuário se o sombreador não compilar mais

**Corrigido:**

* &lbrack;Camadas&rbrack; corrigir soltar em uma pasta recolhida
* &lbrack;Prateleira&rbrack; Corrigir filtragem de conteúdo em miniprateleiras
* &amp;predefinição;Prateleira&amp;predefinição; Renomear categorias e reorganizar guias

### 1.2.1

*(Lançado em: 12 de fevereiro de 2015)*

**Adicionado:**

* Os arquivos \*.spp agora podem ser abertos com um clique duplo no explorador
* &lbrack;Export&brack; Nova marca “$project” para predefinições de exportação
* &preto;Export&brack; Adicionar lista de mapas (com nomenclatura) abaixo de cada conjunto de textura
* &Preencher;Exportar&preencher; Adicionar um botão Tudo/Nenhum para selecionar os conjuntos de texturas
* &preto;Export&brack; Mapas vazios são descartados durante a exportação

**Corrigido:**

* &lbrack;Export&brack; Unity5 predefinições têm mapas invertidos
* &lbrack;Export&brack; Adicionar uma barra em um nome predefinido criará uma pasta corrompida
* &lbrack;O canal de Height de Exportação&rbrack; exportado em formatos de 32 bits está incorretamente fixado
* A lista do conjunto de texturas &lbrack;Export&brack; não está ordenada como no projeto
* &lbrack;Tool&brack; A remoção da face de fundo não funciona mais
* Salvar não funciona com caracteres especiais no caminho

### 1.2.0

*(Lançado: 28 de janeiro de 2015)*

**Adicionado:**

* Novo canal Normal que permite tinta dados do mapa normal e combinar os resultados
* &lbrack;Export&brack; Nova janela de exportação com a capacidade de criar embalagem personalizada e definir nomes personalizados
* O formato de arquivo do projeto agora é um único arquivo em vez de pastas
* &lbrack;Export&rbrack; Suporte a diferentes formatos Normais (DirectX, OpenGL)
* &lbrack;Export&brack; Criar um arquivo temporário de “bloqueio” durante a exportação
* &lbrack;Camadas&rbrack; Shift+Clique com o botão esquerdo do mouse pode ser usado para alternar uma máscara
* &lbrack;Parâmetros&rbrack; Expor o espaço de cores na parte inferior de uma entrada de imagem
* O &preto;Shelf&rbrack; Efeito “MG Mask Builder” agora tem novas configurações
* &lbrack;Visualização 3D; o mapa de Oclusão de ambiente agora oclui a contribuição difusa, não o specular

**Corrigido:**

* A visualização do material de projeção/estêncil não é exibida corretamente no visor
* &lbrack;Dica de ferramenta do atalho do &amp;Visualização 3D; não exibida ao usar o atalho “S” (estêncil)
* &lbrack;Shelf&rbrack; O efeito “Escala de pele MatFx” agora tem melhores desempenhos em baixa resolução
* &lbrack;Export&brack; as Texturas da exportação são apenas ampliadas ao especificar um tamanho de documento maior

### 1.1.2

*(Lançado: 15 de janeiro de 2015)*

**Adicionado:**

* Adicionado: novas configurações de Traduzir, Girar e Dimensionar na camada Preenchimento
* Filtragem aprimorada para camadas de Pincéis e Preenchimento
* A versão de teste agora está completa em recursos (pode exportar), mas é limitada no tempo.

**Corrigido:**

* Impossibilidade de importar malhas de OBJ com precisão muito pequena
* Problema ao ativar uma licença no Windows 7 e 8
* Falha durante um “Salvar como” de um projeto
* Falha ao excluir o último canal de um conjunto de textura
* Falha ao excluir uma camada em um contexto específico

### 1.1.1

*(Lançado: 25 de dezembro de 2014)*

**Adicionado:**

* &lbrack;Camada&rbrack; Selecione a camada na parte superior ao abrir um conjunto de texturas de projeto/alternância
* Velocidade aprimorada de “Salvar” e “Salvar como” com o novo algoritmo de compactação
* Exibir um erro ao abrir um projeto muito recente para o Painter

**Corrigido:**

* &lbrack;Tool&brack; O decalque geométrico produz corrupções na memória
* &lbrack;Brush&brack; Impossível inserir manualmente valores de flutuação abaixo de 1 para o tamanho do pincel
* &lbrack;Camada&rbrack; Criar um efeito de seleção de cor não o adiciona na pilha de camadas
* &lbrack;Camada&rbrack; Mover o mouse sobre as camadas faz com que o Painter passe rapidamente na barra de tarefas
* &lbrack;Camada&rbrack; Adicionar um bitmap como máscara pode levar a um travamento
* A interface gráfica para o modo solo com o canal de Height está incorreta
* “Salvar projeto” pode falhar e corromper um projeto
* Falha ao abrir um projeto após carregar outro com um sombreador desatualizado

### 1.1.0

*(Lançado: 16 de dezembro de 2014)*

**Adicionado:**

* &preto;Efeito&rbrack; Novo criador de máscara de ID de material
* Nova linha branca/preta pontilhada para o cursor do pincel
* Novo parâmetro de sequência de ângulo
* Novo parâmetro de remoção de tela de fundo
* Novo parâmetro Atraso do mouse
* &lbrack;Camadas&rbrack; Suporte para várias seleções e gerenciamento
* &lbrack;Camadas&rbrack; Copiar e colar de uma textura definida para outra
* &lbrack;Export&brack; formato de PSD do Adobe Photoshop
* &preto;Suporte de prateleira; Nova ferramenta: pele, pontos de metal e zíper
* &preto;Prateleira&rbrack; Novo pincel : molde, lápis, linha afiada e costura
* &preto;Suporte de prateleira; Novo alfa : Ruído gaussiano, linha nítida, molde, caneta, respingo, ponto, zíper
* O desempenho da pintura melhorou atualizando apenas partes das texturas necessárias

**Corrigido:**

* &lbrack;Shelf&rbrack; Impossível carregar uma substância com gráfico com rótulos idênticos
* &lbrack;Camadas&rbrack; O modo de mesclagem Passagem não funciona com máscaras
* &lbrack;A Escala do Estêncil&rbrack; está quebrada no Visualização 2D
* Problemas e falha no Mac OS Yosemite

### 1.0.2

*(Lançado: 09 de novembro de 2014)*

**Adicionado:**

* Desempenho aprimorado na visualização de material com substâncias
* Desempenho aprimorado com visualização de traçado de pincel ao atualizar o documento
* Desempenho aprimorado no visor com menor taxa de atualização para a área não funcional
* &lbrack;Pós-efeitos&rbrack; Interface aprimorada para gerenciar configurações
* &lbrack;Pós-efeitos&rbrack; Redefinir para valores padrão
* efeitos de Substance e operações de camadas no menu do botão direito do mouse
* Apoio a entradas/saídas pré-multiplicadas em substâncias

**Corrigido:**

* &lbrack;Visualização 3D&rbrack; Os parâmetros de sombreador personalizado são separados por um espaço grande
* &lbrack;Export&rbrack; Conversão sRGB ausente para a predefinição Unity4
* Possível falha ao carregar malhas fbx
* Falha às vezes ao carregar malhas obj simples
* A barra de computação permanece bloqueada até 100% no carregamento
* Recarregar uma substância a coloca em todas as categorias
* Chave de DirectX/OpenGL quebrada

### 1.0.1

*(Lançado: 27 de outubro de 2014)*

**Adicionado:**

* &lbrack;Tool&brack; Uso aprimorado de parâmetros de material
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

* Suporte de Sombreador personalizado
* Suporte para resolução 4k
* Projetos de personagem de amostra
* Exibir barra de progresso para longos tempos de computação
* &lbrack;Export&brack; Adicionar uma passagem de dilatação antes do pós-processo de difusão
* Argumentos de linha de comando no SP para operações simples
* Novos materiais e efeitos
* Visualização da ferramenta (visualização de material em tempo real separado e área de teste de traçado)
* Não criar um documento padrão quando o Painter for iniciado
* &preto;Tool&brack; Adiciona a possibilidade de editar manualmente um valor em tons de cinza
* Várias melhorias para os estênceis (Ajustar, Redefinir)
* As partículas agora são subferramentas das ferramentas Pincel, Borracha e Projeção
* &lbrack;Visualização 3D&rbrack; Usar AO feito bake na renderização do visor
* Dividir os controles de estênceis entre a exibição 2D e 3D
* Ajuste pequeno do tamanho do polegar na biblioteca
* Os campos de pesquisa são específicos para cada janela
* Ajustes da interface

**Corrigido:**

* A chave &brack;Substance&brack; não funciona
* &lbrack;Caixa de diálogo de cores&rbrack; Degradê de matiz não atualizado
* Não é possível atualizar uma malha se o nome do arquivo é idêntico
* A ferramenta não fica visível nas exibições quando muito pequena
* A ferramenta de decalque na tela Retina não funciona corretamente
* &lbrack;Substance&rbrack; Int1 são exibidos como float1
* &lbrack;Substance&rbrack; basecolor input/output não são reconhecidos
* Os filtros do &lbrack;Substance&rbrack; não podem ser recarregados
* O widget &preto;Tool&brack; em tons de cinza está sempre recolhido

## Beta

### &#x200B;0. 12. 1- beta

*(Lançado: 18 de setembro de 2014)*

**Adicionado:**

* Predefinição de exportação do Unity 5

**Corrigido:**

* Sombreador PBR, a qualidade da renderização deve melhorar muito
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

* Sombreador dá resultado preto com baixa aspereza
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
* Sombreador dá resultado preto com baixa aspereza
* Os materiais do Substance estão limitados a 256
* A exportação de mapa normal exclui o canal verde

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

* Vários materiais - Agora você pode tinta em vários materiais no mesmo documento
* Simetria pintura
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

* A pintura do mapa de altura não tinta valores negativos.
* A exibição do Seletor de materiais não deve levar em conta o mapa normal de amostra
* Determinismo de partículas quebrado
* Matriz de estêncil no Visualização 2D
* Ngons em arquivos obj
* Várias falhas

### &#x200B;0. 6. 0- beta

*(Lançado em: 04 de junho de 2014)*

**Adicionado:**

* Nova opção de exportação para exportar um mapa de Specular de um composto de aspereza e canais metálicos

**Corrigido:**

* Compatibilidade com o Windows Vista
* O mapa de altura não tinta valores negativos

### &#x200B;0. 5. 0- beta

*(Lançado em: 07 de maio de 2014)*

**Adicionado:**

* 3D/Visualização 2D switches
* Ferramenta Seleção de partes UV
* A ferramenta muda automaticamente ao pintar em máscaras.
* A resolução dos Substance depende da

**Corrigido:**

* Falha na inicialização
* Falha com malhas ASCII
* Matriz de estêncil fixa no Visualização 2D
* Falha com o Borracha

### &#x200B;0. 4. 0- beta

*(Lançado: 17 de abril de 2014)*

**Adicionado:**

* Visualização 2D contínuo
* Máscaras de camada de bitmap
* Controle de exposição do ambiente
* Preencher camadas agora usa a janela Ferramentas para definir suas propriedades
* Os materiais podem ser aplicados a camadas de preenchimento
* Adicionou mais estênceis à biblioteca de estênceis
* Predefinições de partículas atualizadas para uma computação mais rápida
* Otimização do sombreador PBR e melhoria da qualidade para configurações de qualidade mais baixa

**Corrigido:**

* As miniaturas de camadas são vinculadas ao canal atualmente selecionado
* Muitas falhas

### &#x200B;0. 3. 0- beta

*(Lançado: 04 de abril de 2014)*

**Adicionado:**

* Permitir valores negativos no seletor de cores para pintura do mapa de altura
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
* Corrigido: geração incorreta de textura
* Corrigido: falha na inicialização

### &#x200B;0. 2. 0- beta

*(Lançado: 17 de março de 2014)*

**Adicionado:**

* Conta-gotas de material (atalho P)
* Miniaturas na visualização da ferramenta 3D
* Sistema de licenciamento para versões autônomas
* &brack; e &rbrack; atalhos para Tamanho do pincel
* Preenchimento em mapas exportados
* Estilo de Janela de Ferramenta Atualizado
* Estilo atualizado dos controles deslizantes
* Ambiente HDR padrão atualizado

**Corrigido:**

* Estêncil: altere o valor do fluxo nas paradas do Visualização 3D em 52
* Loop infinito no motor ao adicionar teclas de pressão 0 ao traço é fixo
* Ferramenta: a tremulação de ângulo não retorna valores acima de +/- 90%
* Alteração da exibição de Visualização 3D quando uma máscara de camada é selecionada
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
