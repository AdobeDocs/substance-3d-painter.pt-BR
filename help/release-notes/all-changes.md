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
* &amp;preto;Pintura em gaiola&amp;rbrack; Criar interface de Tinta básica em gaiola
* &amp;preto;Pintura em gaiola&amp;rbrack; Novas opções de Visualização em gaiola
* &amp;preto;Pintura em gaiola&amp;rbrack; Editável Ferramenta Selecionar / Preencher
* &amp;preto;Pintura em gaiola&amp;rbrack; Mostrar Modo Combinar na barra de ferramentas
* &amp;preto;Pintura em gaiola&amp;rbrack; Alterações na interface do controle deslizante HDR
* &amp;preto;Pintura de gaiola&amp;rbrack; sombreador de visualização
* &amp;preto;Pintura em gaiola&amp;rbrack; Redefinir opções da pilha
* Melhorias na ferramenta Preenchimento de polígono
* &amp;Preenchimento de polígono&amp;rbrack; Adicionar correção de polígono
* &amp;Preenchimento de polígono&amp;rbrack; Adicionar loop de polígono
* &amp;Preenchimento de polígono&amp;rbrack; suporte para Simetria com Loop/Correção
* &amp;Preenchimento do polígono&amp;rbrack; visualização da borda da Simetria
* &amp;Preenchimento de polígono&amp;rbrack; Remover triângulos com loops e loops parciais
* &amp;preto;Preenchimento de polígono&amp;rbrack; Wireframe visível somente para o Conjunto de texturas ativo
* &amp;preto;Preenchimento de polígono&amp;rbrack; Realce de borda vermelha em triângulos não clicáveis
* &amp;preenchimento;Preenchimento de polígono&amp;rbrack; Não desative as opções do modo de preenchimento
* &amp;Preenchimento de polígono&amp;rbrack; Permitir a definição de todas as propriedades de canal com o Preenchimento de polígono
* &amp;Preenchimento de polígono&amp;rbrack; Retomar traçado anterior funciona com Preenchimento de polígono
* &amp;preto;Preenchimento de polígono&amp;rbrack; Mostrar cursor proibido em conjuntos de texturas não ativos
* &amp;Preenchimento do polígono&amp;rbrack; ALT visualização instantânea
* &amp;Preenchimento de Polígono&amp;rbrack; Atalho para alternar temporariamente para Polyloop (SHIFT+A)
* &amp;preto;Visor&amp;rbrack; Mostrar conjunto de texturas / realce de seleção de Bloco UV
* &amp;lbrack;Visor&amp;rbrack; Adicionar suporte para Transparência Independente da Ordem no visor em tempo real
* &amp;lbrack;Configurações de exibição&amp;rbrack; Reorganizar as configurações de exibição em novos grupos
* &amp;lbrack;Tool&amp;brack; Adicionar suporte para mesclagem aditiva com pinceladas
* &amp;lbrack;Tool&amp;brack; Adicionar suporte para mesclagem aditiva com Preenchimento de Polígono
* &amp;lbrack;USD&amp;rbrack; O USD exportado com mapa de opacidade torna tudo transparente em Arnold
* &amp;lbrack;Nvidia&amp;rbrack; Adicionar aviso sobre os drivers Nvidia mais recentes (616.56 a 617.14)
* Adicionar nova entrada de mapa do mecanismo “mesh_uv_neighbor”
* Atualize os baker para a versão 3.23.0
* Atualize o mecanismo de Substance para a versão 9.6.1

**Corrigido:**

* &amp;lbrack;Fazendo bake&amp;rbrack; A Oclusão de ambiente Ignorar face de fundo pelo nome da malha não funciona
* &amp;lbrack;Fazendo bake&amp;rbrack; &amp;lbrack;AMD&amp;rbrack; Dispositivo perdido ao fazer bake com malhas pesadas de alta espessura
* &amp;lbrack;Desempenho&amp;rbrack; Painter hogs VRAM uso
* &amp;lbrack;Viewport&amp;rbrack; texturas ausentes ao abrir projetos em telas HDPI
* O modo de mesclagem &amp;preto;Tool&amp;rbrack; fica esmaecido ao pintar em uma máscara
* Pastas temporárias não excluídas após a exportação na rede
* &amp;lbrack;USD&amp;rbrack; A geometria USD exportada é dividida ao longo das bordas UV
* &amp;lbrack;USD&amp;rbrack; Congelar ao carregar USDz malformado

### 12.1.5

Data de lançamento: **09/2026/15**

Resumo: **Versão secundária**

**Corrigido:**

* Exportar imagem de prateleira para uma rede não funciona mais
* &amp;lbrack;Gerador&amp;rbrack; Configurar “usar textura” como falso não desativa o uso da entrada de textura
* O visor congela ao salvar enquanto edita a projeção 3D
* A resolução da camada de material é muito baixa

### 12.1.4

Data de lançamento: **9/2026/04**

Resumo: **Versão secundária**

**Corrigido:**

* &amp;lbrack;Falha&amp;rbrack; Falha ao importar ou exportar arquivos cujos nomes de arquivo contenham caracteres não-ASCII

### 12.1.3

Data de lançamento: **2026/08/26**

Resumo: **Versão secundária**

**Adicionado:**

* Atualize o mecanismo de Substance para a versão 9.4.6

**Corrigido:**

* &amp;preto;Seletor de tons de cinza&amp;rbrack; permanece aberto após alterar a ferramenta
* &amp;preto;Inclinar Fazendo bake&amp;rbrack; Inclinar interrupções de correção ao pintar e desfazer
* &amp;lbrack;Ferramenta de Projeção&amp;rbrack; A interação do visor está bloqueada pela ferramenta de projeção
* &amp;preto;Traçado dinâmico&amp;rbrack; Parâmetros de traçado dinâmico ausentes nas propriedades do pincel
* Exportar para uma rede não funciona mais

### 12.1.2

Data de lançamento: **08/2026/03**

Resumo: **Versão secundária**

**Corrigido:**

* &amp;lbrack;Crash&amp;rbrack; Alguns Substance podem levar a uma falha quando renderizados
* &amp;lbrack;Crash&amp;rbrack; Reimportar malha enquanto estiver no modo de fça bake
* &amp;lbrack;Crash&amp;rbrack; A falha ao inicializar a exibição de gráficos pode levar a um travamento
* &amp;lbrack;Falha&amp;rbrack; A exportação de texturas pode falhar em alguns casos ao atualizar o registro
* &amp;lbrack;Falha&amp;rbrack; Falha no modo de fça bake em alguns casos ao carregar/atualizar o mapa de ambiente
* &amp;lbrack;Fazendo bake&amp;rbrack; A reinicialização do faço bake após a modificação do arquivo poly alto pode levar a um congelamento
* &amp;preto;Enviar para o Photoshop&amp;rbrack; Falha ao exportar a máscara da camada
* &amp;lbrack;O resultado do ponto de ancoragem do Engine&amp;brack; não é renderizado entre uma máscara e um canal de cor

### 12.1.1

Data de lançamento: **07/2026/09**

Resumo: versão secundária

Adicionado:

* &amp;preto;Inclinar Fazendo bake&amp;rbrack; Expor Inclinação Base Modo Normal: malha ou por triângulo
* &amp;lbrack;Propriedades&amp;rbrack; Fazer com que as cores uniformes sempre redefinam para o valor padrão de seus canais
* &amp;lbrack;OpenPBR&amp;rbrack; Reagrupar canais por categorias na janela Exportar Texturas para criação de modelos de saída
* Atualize o mecanismo de Substance para a versão 9.4.5

Corrigido:

* &amp;lbrack;Projeto&amp;rbrack; Abrir e salvar alguns projetos pode demorar mais do que o normal
* &amp;lbrack;Crash&amp;rbrack; Recarregar várias malhas pode levar a um travamento
* &amp;lbrack;Crash&amp;rbrack; Excluir um canal enquanto estiver no modo de exibição de máscara leva a um travamento
* &amp;lbrack;Crash&amp;rbrack; Alguns Substance podem levar a uma falha quando renderizados
* &amp;lbrack;Inclinação da Tinta&amp;rbrack; A ferramenta selecionada na inclinação da tinta permanece selecionada após alternar para o Modo de Pintura
* &amp;lbrack;Fazendo bake configurações comuns&amp;rbrack; As configurações de distância da gaiola não atualizam a visualização do wireframe e do sombreador da gaiola
* &amp;lbrack;Engine&amp;rbrack; O preenchimento UV “Vizinho do espaço 3D” não funciona bem em triângulos finos
* &amp;lbrack;O resultado do ponto de ancoragem do Engine&amp;brack; não é renderizado entre uma máscara e um canal de cor

### 12.1.0

Data de lançamento: **2026/06/23**

Resumo: **Esta atualização é uma versão principal. Ela contém melhorias de baker com Novo estado de interface do usuário padrão de fça bake, mapa de inclinação da pintura, retoque automático, nova opção de desencapsulamento automático UV para malhas de superfície dura e OpenPBR. Para obter mais detalhes, consulte as notas de versão completas.**

**Adicionado**:

* &amp;preto;Inclinar fazendo bake&amp;rbrack; Inclinar Ferramentas de Pintura
* &amp;Preencher;Inclinar Fazendo bake&amp;rbrack; Adicionar Inclinar Visualizar sombreador e Inclinar direção Vetor visuais ao pintar mapa de inclinação
* &amp;preto;Inclinar Fazendo bake&amp;rbrack; Adicionar proteção de borda
* &amp;preto;Inclinar fazendo bake&amp;rbrack; Recozimento automático
* &amp;lbrack;Inclinar Fazendo bake&amp;rbrack; Retrabalhar mapa de malha Interface do usuário da lista
* &amp;preto;Inclinar Fazendo bake&amp;rbrack; Dividir mapa de malha / Configurações de Fça bake comuns + Mover configurações comuns para fora da lista de mapas de malha apenas com base em cores ou máscaras
* &amp;preto;Inclinar Fazendo bake&amp;rbrack; Alterar botões da barra de ferramentas do visor
* &amp;preto;Inclinar Fazendo bake&amp;rbrack; Mostrar alternância de Simetria para o pincel na barra de ferramentas superior
* &amp;lbrack;Inclinar Fazendo bake&amp;rbrack; Renomear opções no menu de Sincronização de lista do mapa de malha
* &amp;lbrack;Inclinar Fazendo bake&amp;rbrack; Atualizar Sincronização e Verificado caixas de diálogo de estado
* &amp;preto;Fça bake de inclinação&amp;rbrack; Criar variante do seletor de cores em tons de cinza
* &amp;preto;Inclinar Fazendo bake&amp;rbrack; Atualizar ícone do modo de fça bake
* &amp;lbrack;Desenvolver automaticamente&amp;rbrack; opção Integrar superfície rígida
* &amp;lbrack;OpenPBR&amp;rbrack; Adicionar suporte para OpenPBR 1.1
* &amp;lbrack;OpenPBR&amp;rbrack; Tornar o OpenPBR o fluxo de trabalho e o sombreador padrão
* &amp;lbrack;OpenPBR&amp;rbrack; Importar materiais e texturas de OpenPBR via USD
* &amp;lbrack;OpenPBR&amp;rbrack; Exportar materiais e texturas de OpenPBR via USD
* &amp;lbrack;OpenPBR&amp;rbrack; Janela Atualizar Texturas de Exportação para mostrar a convenção de nomenclatura do OpenPBR
* &amp;lbrack;OpenPBR&amp;rbrack; Adicionar documentação sobre alterações para suportar o OpenPBR
* &amp;lbrack;OpenPBR&amp;rbrack;&amp;lbrack;Iray&amp;rbrack; Adicionar novo MDL para oferecer suporte ao OpenPBR 1.1 no Iray
* Várias melhorias menores nas exportações de USD
* &amp;lbrack;UI&amp;rbrack; Adicionar aviso no visor ao tentar tinta em outro Conjunto de Texturas
* &amp;Preenchimento;Nivelar&amp;Preenchimento; Permite nivelar todas as camadas instanciadas nos Conjuntos de Textura
* &amp;preto;Configurações do conjunto de texturas&amp;rbrack; Permite selecionar vários canais de uma vez através de uma nova janela
* &amp;lbrack;Histórico&amp;rbrack; Atualizar “valor” Desfazer texto de entrada para refletir o nome do parâmetro
* &amp;lbrack;Pilha de camadas&amp;rbrack; Tornar os efeitos de preenchimento em máscaras padrão em branco (1.0)
* &amp;lbrack;Substance&amp;rbrack; Adicionar nova entrada de mapa do mecanismo “mesh_hard_edges_triangle”
* &amp;lbrack;Substance&amp;rbrack; Adicionar nova entrada de mapa de mecanismo “mesh_hard_edges”
* &amp;lbrack;Sombreador&amp;rbrack; Impedir que instâncias de sombreamento compartilhem os mesmos nomes
* &amp;lbrack;Sombreador&amp;rbrack; Usar o sombreador do modelo do projeto ao importar um arquivo USD ou GLTF
* Atualize o Adobe Color Engine para a versão 7.0
* Atualização mínima da versão do MacOSX para a versão 13.0 (Ventura)
* &amp;lbrack;Content&amp;rbrack; Novos modelos de projeto para OpenPBR
* &amp;lbrack;Content&amp;rbrack; Atualiza projetos de amostra para usar o novo sombreador de OpenPBR
* &amp;lbrack;Python&amp;rbrack; Expandir a API da Máscara de Geometria para permitir modos de inclusão e exclusão, como na interface do usuário

**Corrigido**:

* &amp;lbrack;Crash&amp;rbrack;&amp;lbrack;Configurações de mapas de malha&amp;rbrack; Aplicar configurações a outros conjuntos de textura
* &amp;lbrack;Crash&amp;rbrack; Ao fazer bake a curvatura do mapa sem o espaço global normal
* &amp;lbrack;Falha&amp;rbrack;&amp;lbrack;Fazendo bake&amp;rbrack; Fazendo bake com gaiola personalizada ativada, mas nenhum arquivo selecionado falha
* &amp;lbrack;Falha&amp;rbrack; Cancelando fça bake AO
* &amp;lbrack;Caixa Automática&amp;rbrack; Carga infinita quando o caminho do arquivo poli alto é inválido
* &amp;lbrack;Linux&amp;rbrack;&amp;lbrack;Windows&amp;rbrack; O seletor de cores às vezes pode ficar totalmente preto ou não aparecer
* &amp;preto;Ferramenta Preenchimento de polígono&amp;rbrack; A ferramenta não funciona com não-PBR
* &amp;lbrack;&amp;lbrack;Tinta&amp;rbrack; Excluir o canal de cor de base não exclui a cor pintada anteriormente
* As Instâncias de sombreamento do &amp;lbrack;USD&amp;rbrack; não são detectadas corretamente
* &amp;lbrack;Substance&amp;rbrack; Somente o primeiro uso de um nó de entrada/saída é levado em consideração
* A Oclusão de ambiente do &amp;lbrack;Sombreador&amp;rbrack; é aplicada duas vezes com Conjuntos de Texturas usando diferentes métodos de mistura
* &amp;lbrack;Motor&amp;rbrack; texturas normais com canal azul vazio (preto) podem levar a resultados de mesclagem errados
* &amp;lbrack;GLTF Import&amp;rbrack; A mesclagem de alfa está habilitada em todos os conjuntos de texturas
* &amp;lbrack;GLTF Export&amp;rbrack; A mesclagem de alfa está sempre habilitada na exportação
* &amp;lbrack;Export&amp;brack; A geometria de dupla face está sempre desativada ao importar um arquivo GLTF
* &amp;lbrack;Javascript&amp;rbrack; A modificação das configurações de sombreadores não contribui para o histórico de desfazer
* &amp;lbrack;Amostras&amp;rbrack; A dispersão da subsuperfície não está ativada nas Configurações de Exibição do Mat. da Reunião

### 12.0.3

Data de lançamento: **5/2026**

Resumo: **Versão secundária**

**Adicionado:**

* Atualize os baker para a versão 3.22.2
* Atualize o mecanismo de Substance para a versão 9.4.3
* &amp;lbrack;Python&amp;rbrack; Salva uma material inteligente em um local específico

**Corrigido:**

* &amp;lbrack;Ubuntu&amp;rbrack; Falha ao selecionar material
* &amp;lbrack;O pop-up recorrente do Mac&amp;rbrack; aparece para pedir acesso aos dados de outros aplicativos
* &amp;lbrack;Fazendo bake&amp;rbrack; Artefatos podem aparecer no mapa de curvatura
* &amp;lbrack;Fazendo bake&amp;rbrack; Fazendo bake é mais lento em alguns casos
* &amp;preto;Distorcer para geometria&amp;rbrack; A opção Distorcer para geometria fica desativada em alguns casos
* &amp;lbrack;Bloco UV&amp;rbrack; Alfa extraída do ponto de ancoragem ignorada por outras peças
* &amp;lbrack;Python&amp;rbrack;&amp;lbrack;Mac&amp;rbrack; Exceções no console Python com SSL
* &amp;lbrack;Python&amp;rbrack; Painter falha ao sair com widgets Qt restantes

### 12.0.2

Data de lançamento: **04/2026/07**

Resumo: **Versão secundária**

**Adicionado:**

* &amp;lbrack;Gerenciamento de cores&amp;rbrack; Adicionar novo OCIO para especificar o espaço de cores padrão do seletor de cores
* &amp;lbrack;Python&amp;rbrack; Expor configurações de desajuste automático na API Python

**Corrigido:**

* &amp;lbrack;Falha&amp;rbrack; Salvar com espaço em disco insuficiente pode travar ou corromper projetos
* &amp;lbrack;Crash&amp;rbrack; &amp;lbrack;Ribbon&amp;rbrack; Usar a faixa de opções pode causar falhas para alguns projetos
* &amp;lbrack;Falha&amp;rbrack; &amp;lbrack;Fazendo bake&amp;rbrack; falha quando o arquivo .assbin não pode ser gravado na pasta
* &amp;lbrack;Malhas OBJ do Stager podem falhar na criação do projeto
* &amp;lbrack;Import&amp;brack; OBJ tem rosto ausente em alguns casos
* &amp;lbrack;Import&amp;brack; malha USD sem nenhum material atribuído pode falhar na importação
* &amp;lbrack;Caminho preenchido&amp;rbrack; Não afetado pela simetria
* &amp;prec;Estêncil&amp;brack; A visualização tem resolução menor do que o resultado pintado
* &amp;lbrack;UI&amp;rbrack; &#39;uv island&#39; ainda é mencionado na dica de ferramenta de origem de cores do mapa de ID
* &amp;lbrack;Display&amp;brack; As sombras aparecem invertidas
* O transformo de projeção &amp;lbrack;Viewport&amp;rbrack; Warp permanece após alternar para o modo de fça bake
* &amp;lbrack;Distorcer&amp;brack; A grade desaparece quando a escala é definida como 0 no eixo Z com Distorcer para geometria ativado
* &amp;lbrack;Python&amp;rbrack; Erro inesperado ao adicionar um canal com modificação no escopo

### 12.0.1

Data de lançamento: **03/2026/18**

Resumo: **Versão secundária**

**Corrigido:**

* &amp;lbrack;Crash&amp;rbrack;&amp;lbrack;Congelar&amp;rbrack; Exportar de projetos específicos

### 12.0.0

Data de lançamento: **03/2026/09** Resumo: **esta é uma versão principal. Esta versão contém os recursos de camadas achatadas, distorção na geometria, novos pós-efeitos, melhoria na janela do novo projeto e outras melhorias.**

**Adicionado**:

* &amp;Preencher;Nivelar camadas&amp;rbrack; Nivelar camadas dentro da pilha de camadas
* &amp;Preenchimento;Achatar camadas&amp;rbrack; Exportar camadas achatadas para o disco
* &amp;lbrack;Distorcer para geometria&amp;rbrack; Adicionar nova funcionalidade de deformação automática a Distorcer projeções
* &amp;lbrack;Pós-efeitos&amp;rbrack; Substituir pós-efeitos pela adição de novos
* &amp;lbrack;Pós-efeitos&amp;rbrack; Atualizar mapeador de tons
* &amp;lbrack;Pós-efeitos&amp;rbrack; Adicionar novo uso para ativos de Pós-efeitos
* &amp;lbrack;Content&amp;brack;&amp;lbrack;Post-effects&amp;rbrack; Integra os ativos padrão de pós-efeitos na biblioteca
* &amp;lbrack;Novo Projeto&amp;rbrack; Melhorar a interface para a criação de projetos
* &amp;lbrack;Novo projeto&amp;rbrack; Alterações na funcionalidade de malha de reimportação
* &amp;lbrack;Novo projeto&amp;rbrack; Permitir que arquivos \*.geo.usd sejam abertos
* &amp;lbrack;Configuração do projeto&amp;rbrack; Melhorar interface para a configuração do projeto
* Atualizar a biblioteca USD para a versão 25.05
* Atualize o Substance Engine para a versão 9.3.4
* Aumente o mínimo de drivers para 25.3.1/25.Q2 para GPUs AMD
* Atualize o Qt para 6. 8. 6
* &amp;lbrack;Scripting&amp;rbrack; Atualiza a API JavaScript para a versão 1.1.20
* Atualizar Python para a versão 3.13

**Corrigido:**

* &amp;lbrack;Crash&amp;rbrack; Alterar uma saída de canal de material em uma máscara pode travar
* &amp;lbrack;Import&amp;rbrack; As texturas EXR são forçadas para sRGB em vez de lineares ao importar arquivos USD
* &amp;lbrack;Blocos UV&amp;rbrack; A sequência de imagens com uma única imagem também preenche outros Blocos UV
* &amp;lbrack;Fazendo bake&amp;rbrack; O AO é diferente entre o fça bake de CPU e GPU
* &amp;lbrack;Color Management&amp;rbrack;&amp;lbrack;MacOS&amp;rbrack; Viewport BaseColor não corresponde ao selecionador de cores
* &amp;lbrack;USD&amp;rbrack; Valores uniformes não são importados em alguns casos

## Versão 11

### 11.1.3

Data de lançamento: **2026/02/12** Resumo: **versão secundária**

**Corrigido**:

* &amp;lbrack;Tinta&amp;rbrack; Estêncil e simetria não funcionam em alguns casos
* &amp;lbrack;Caminho&amp;rbrack; Nenhuma atualização ao alterar o controle deslizante de opacidade de traçado de borrar
* &amp;lbrack;Projeto&amp;rbrack; Não é possível tinta em alguma geometria
* &amp;lbrack;Ribbon&amp;rbrack; O caminho instanciado desaparece ao alterar a resolução do Conjunto de Texturas
* &amp;lbrack;UI&amp;rbrack; O seletor de cores pode encolher e desaparecer em alguns casos

### 11.1.2

Data de lançamento: **01/2026/13** Resumo: **versão secundária**

**Adicionado**:

* &amp;lbrack;Fazendo bake&amp;rbrack; Melhorar o tempo de fça bake de projetos de Blocos UV com salvamento assíncrono
* &amp;lbrack;Shaders&amp;rbrack; A menção no API de sombreamento muda após a migração Vulkan
* Atualizar OpenEXR para a versão 3.4.4

**Corrigido**:

* &amp;lbrack;Crash&amp;rbrack; Falha durante a inicialização na série Nvidia GTX 10xx
* &amp;lbrack;Crash&amp;rbrack; Usar o seletor de cores em diferentes Conjuntos de texturas pode resultar em uma falha ao sair do aplicativo
* &amp;preto;Desempenho&amp;rbrack; Problema de desempenho ao pintar no projeto com muitas camadas
* &amp;lbrack;Desempenho&amp;rbrack; Atraso ao pintar com caneta eletrônica gráfica
* &amp;lbrack;UI&amp;rbrack; As configurações da câmera permanecem desativadas no modo de renderização (Iray)
* &amp;lbrack;Ribbon&amp;rbrack; O caminho pode se sobrepor inesperadamente após um canto em alguns casos
* &amp;lbrack;Ribbon&amp;rbrack; Problema de desempenho com Blocos UV
* &amp;lbrack;Substance&amp;rbrack;&amp;lbrack;UI&amp;rbrack; As entradas de imagem desaparecem quando recolhidas
* &amp;lbrack;Substance&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Os grupos aninhados podem permanecer mesmo se Visíveis Se os ocultarem
* &amp;lbrack;Fazendo bake&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Não é possível definir o Raio de Amostragem da Curvatura além de 0,01
* &amp;lbrack;Fazendo bake&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Não é possível definir a Distância Máxima do Ocultador além de 1
* &amp;lbrack;Fazendo bake&amp;rbrack; A configuração do AO “Auto-oclusão” é ignorada com vários Conjuntos de Textura e Baixo como Alto fazendo bake
* O mapa de ID do &amp;lbrack;Fazendo bake&amp;rbrack; não faz bake as cores dos vértices do FBX no modo Baixo como Alto
* O filtro &amp;lbrack;Content&amp;brack; Highpass resulta em cores esmaecidas em canais com gerenciamento de cores

### 11.1.1

Data de lançamento: **12/2025/09** Resumo: **versão secundária**

**Adicionado**:

* &amp;lbrack;Desempenho&amp;rbrack; Melhorar o desempenho dos Blocos UV ao calcular texturas parciais
* &amp;lbrack;Baker&amp;rbrack; Atualize para a versão 3.15.4

**Corrigido**:

* &amp;lbrack;Falha&amp;rbrack;&amp;lbrack;MacOS&amp;rbrack; Salvar projeto de versão anterior sempre falha
* &amp;lbrack;Falha&amp;rbrack; Fechar um projeto às vezes pode resultar em uma falha
* &amp;lbrack;Projeto&amp;rbrack; Erro “incompatibilidade na contagem de membros” ao abrir o projeto feito na versão anterior
* Os Blocos UV &amp;lbrack;Fazendo bake&amp;rbrack; não são combinados com resultados de fazes bake anteriores, se presentes
* &amp;lbrack;Fazendo bake&amp;rbrack; Dispositivo perdido mesmo com Rastreamento de raios desativado na série Nvidia GTX 10XX
* &amp;lbrack;Fazendo bake&amp;rbrack; AO com normal tem artefatos nas bordas porque não há preenchimento
* &amp;lbrack;Fazendo bake&amp;rbrack; A configuração do AO “Auto-oclusão” é ignorada com vários Conjuntos de Texturas e “corresponder pelo nome” em
* O Mapa de ID do &amp;lbrack;Fazendo bake&amp;rbrack; é totalmente preto se alguma malha de alto polígono não tiver cores de vértice
* &amp;lbrack;Faixa de opções&amp;rbrack; A dica de ferramenta para o modo de mesclagem Alfa menciona o modo de mesclagem Tela em vez do Subexposição linear
* &amp;lbrack;Caminho&amp;rbrack; Tangentes criam loop inesperado quando o ponto é movido próximo às extremidades do caminho
* &amp;lbrack;Tool&amp;brack; A visualização do material não funciona quando a projeção é usada em uma máscara
* &amp;preto;Engine&amp;brack; Pintar traçados pequenos pode resultar em artefatos em blocos
* &amp;lbrack;Sombreador&amp;rbrack; Se você desfizer a criação da instância de sombreamento, ela não será removida corretamente
* &amp;lbrack;O modo de Alpha de Exportação&amp;rbrack; para exportação de GLTF é sempre definido como MASK
* &amp;lbrack;Python&amp;rbrack; Erro inesperado ao editar a pilha de camadas fora do bloco de modificação com escopo

**Problemas Conhecidos**:

* &amp;lbrack;Ribbon&amp;rbrack; Problema de desempenho com Blocos UV
* &amp;lbrack;Ribbon&amp;rbrack; O caminho pode se sobrepor inesperadamente após um canto em alguns casos
* &amp;lbrack;Crash&amp;rbrack;&amp;lbrack;Ribbon&amp;rbrack; Criar textos muito longos na Faixa de Opções pode falhar
* &amp;lbrack;Gerenciamento de cores&amp;rbrack; As conversões do espaço de cores HDR com ACE no Linux produzem cores fixas
* &amp;lbrack;Regressão&amp;rbrack;&amp;lbrack;UI&amp;rbrack; O menu do botão direito do mouse é muito pequeno em telas HD
* &amp;lbrack;Crash&amp;rbrack;&amp;lbrack;Python&amp;rbrack; Exportação de USD acionada por TextureStateEvent
* &amp;lbrack;Engine&amp;brack; Pintura com ferramenta Clonar nas cores normais de mudança de canal incorretamente
* &amp;lbrack;Python&amp;rbrack; O widget fantasma aparece excluído pelo script ainda em funcionamento

### 11.1.0

Data de lançamento: **2025/11/18** Resumo: **esta atualização é uma versão principal; ela contém a nova ferramenta Faixa de Opções com conteúdo novo dedicado, suporte a simetria para camadas de preenchimento, parâmetro de tamanho físico para deslocamento, desempenho aprimorado através dos baker atualizados, suporte completo a Vulkan para Windows e Linux e outras melhorias.**

**Adicionado**:

* Nova ferramenta da faixa de opções
* &amp;lbrack;Tool&amp;brack; Adicionar nova ferramenta de Faixa de Opções para criar caminhos perfeitos
* &amp;preto;Faixa de opções&amp;rbrack; Adicionar atalhos predefinidos da Faixa de opções na janela Propriedades
* &amp;lbrack;Ribbon&amp;rbrack; Permite alterar a opacidade da Faixa de Opções por vértice no caminho
* &amp;lbrack;Ribbon&amp;rbrack; Permite alterar o tamanho da Faixa por vértice no caminho
* &amp;lbrack;Ribbon&amp;rbrack; Remove o início/fim definido em um Substance quando os caminhos são fechados
* &amp;lbrack;Ribbon&amp;rbrack; Remover Caminho/Visualização de material na janela de propriedades das ferramentas Tinta/Borracha/Borrar caminho
* &amp;lbrack;Ribbon&amp;rbrack; Adicionar modos de mesclagem para o alfa e alguns canais quando autosobrepostos
* Preencher simetria
* &amp;Preencher;Preencher&amp;preencher; Adicionar suporte para simetria em camadas e efeitos de preenchimento
* &amp;lbrack;Preenchimento&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Expor as configurações de simetria na janela de propriedades para a camada de preenchimento e efeitos
* &amp;lbrack;Fill&amp;brack; Interface de configuração de simetria de Retrabalho no menu do visor e na janela de propriedades
* &amp;lbrack;Fill&amp;brack; Reorientar adequadamente as texturas normais ao projetar no modo de distorção
* deslocamento do tamanho físico
* &amp;lbrack;Deslocamento&amp;rbrack; Usar tamanho físico como unidade de deslocamento
* Melhoria de desempenho
* &amp;lbrack;Desempenho&amp;rbrack; Melhorar a renderização de pinceladas pequenas em triângulos grandes
* &amp;lbrack;Desempenho&amp;rbrack; Melhorar o tempo de compilação do Sombreador
* &amp;lbrack;Performance&amp;rbrack; Suporte completo a Vulkan para Windows e Linux
* &amp;lbrack;Desempenho&amp;rbrack; baker atualizados com renderização de GPU mais rápida e suporte ao Rastreamento de raios AMD
* &amp;lbrack;UI&amp;rbrack; Reorganizar as propriedades das ferramentas em grupos e recolher algumas por padrão
* &amp;lbrack;Engine&amp;rbrack; Atualização Substance Engine para a versão 9.2.5
* &amp;lbrack;Substance&amp;rbrack; Expor substituição de resolução para recursos Substance em Ferramentas e Preenchimentos
* &amp;preto;Exportar&amp;rbrack; Atualizar predefinição de exportação de Mapas de Malha para exportar texturas em tons de cinza
* Python
* &amp;lbrack;Fazendo bake&amp;rbrack;&amp;lbrack;Python&amp;rbrack; Indicar em changelog mudanças de quebra após atualização de baker
* &amp;lbrack;Python&amp;rbrack; Expor as configurações de simetria de preenchimento no Python
* Conteúdo e novo conteúdo
* &amp;lbrack;Content&amp;brack; Adicionar 75 novas predefinições de ferramenta para a ferramenta Faixa de Opções
* &amp;lbrack;Content&amp;brack; Atualiza o recurso construtor de gradientes para que seja compatível com a Faixa de Opções

**Corrigido**:

* &amp;lbrack;Falha&amp;rbrack; Carregar outro projeto enquanto o ajuste de caminho está ativado pode falhar
* &amp;lbrack;Falha&amp;rbrack; Clique com o botão direito do mouse no painel Caminho com informações de outra sessão na área de transferência pode falhar
* A interface do &amp;lbrack;UI&amp;rbrack; rola para cima nas propriedades da ferramenta ao criar um caminho
* &amp;lbrack;UI&amp;rbrack; O cursor do mouse desaparece quando a visualização do visor do caminho está oculta
* &amp;lbrack;Caminho&amp;rbrack; Copiar/colar diferentes propriedades de ferramenta no painel Caminho levam a propriedades instáveis
* As predefinições da ferramenta &amp;Preenchimento; Borracha e Borrar nem sempre atualizam a seleção de canal
* &amp;lbrack;Tool&amp;brack; O valor pintado é cinza, mas a interface mostra branco após carregar a predefinição de ferramenta colorida na máscara
* &amp;lbrack;A predefinição &amp;Tool&amp;rbrack; criada a partir da máscara mantém os valores de canais carregados de outra predefinição
* &amp;lbrack;Substance&amp;rbrack; A substituição do espaço de cores normal definida no gráfico não é levada em consideração
* &amp;lbrack;Content&amp;brack; O recurso de forma de pincel padrão usa um Substance desatualizado

**Problemas Conhecidos**:

* Histórico de Instância de sombreamento não controlado corretamente
* &amp;lbrack;Ribbon&amp;rbrack; Problema de desempenho com Blocos UV
* &amp;lbrack;Ribbon&amp;rbrack; O caminho pode se sobrepor inesperadamente após um canto em alguns casos
* &amp;lbrack;Ribbon&amp;rbrack; As tangentes criam um loop indesejado quando o ponto é movido próximo das extremidades do caminho
* &amp;lbrack;Crash&amp;rbrack;&amp;lbrack;Ribbon&amp;rbrack; Criar textos muito longos na Faixa de Opções pode falhar
* &amp;lbrack;Tool&amp;brack; A visualização do material não funciona quando a projeção é usada em uma máscara
* &amp;lbrack;Fazendo bake&amp;rbrack; A configuração do AO “Auto-oclusão” é ignorada com vários Conjuntos de Texturas e a opção “corresponder pelo nome” ativada
* &amp;lbrack;Fazendo bake&amp;rbrack; O AO com normal possui artefatos nas bordas devido à falta de preenchimento
* &amp;lbrack;Gerenciamento de cores&amp;rbrack; As conversões do espaço de cores HDR com ACE no Linux produzem cores fixas
* &amp;lbrack;Regressão&amp;rbrack;&amp;lbrack;UI&amp;rbrack; O menu do botão direito do mouse é muito pequeno em telas HD
* &amp;lbrack;Crash&amp;rbrack;&amp;lbrack;Python&amp;rbrack; Exportação de USD acionada por TextureStateEvent
* &amp;lbrack;Engine&amp;brack; Pintura com ferramenta Clonar nas cores normais de mudança de canal incorretamente
* &amp;lbrack;Python&amp;rbrack; O widget fantasma aparece excluído pelo script ainda em funcionamento

### 11.0.3

Data de lançamento: **08/2025/05** Resumo: **versão secundária**

**Adicionado**:

* &amp;lbrack;Substance 3D Assets&amp;rbrack; Adicionar um ponto de notificação ao painel Ativos 3D
* &amp;lbrack;VFX Platform 2025&amp;rbrack; Adicionar configuração ACE 2.0 nas configurações de gerenciamento de cores
* &amp;lbrack;VFX Platform 2025&amp;rbrack; Atualização do OCIO para a versão 2.4.2
* Atualize o Iray para a versão 2024.10
* &amp;lbrack;Engine&amp;rbrack; Atualização para o Substance Engine v.9.2.3
* &amp;lbrack;Nvidia&amp;rbrack; Eleva a versão mínima dos drivers Nvidia para 572.60 (Win) e 570.169 (Linux)

**Corrigido**:

* &amp;lbrack;Python&amp;rbrack; A Modificação com Escopo não aparece na janela Histórico

**Problemas Conhecidos**:

* &amp;lbrack;Gerenciamento de cores&amp;rbrack; As conversões do espaço de cores HDR com ACE no Linux produzem cores fixas
* &amp;lbrack;Regressão&amp;rbrack;&amp;lbrack;UI&amp;rbrack; O menu do botão direito do mouse é muito pequeno em telas HD
* &amp;lbrack;Crash&amp;rbrack;&amp;lbrack;Python&amp;rbrack; Exportação de USD acionada por TextureStateEvent
* &amp;lbrack;Engine&amp;brack; Pintura com ferramenta Clonar nas cores normais de mudança de canal incorretamente
* &amp;lbrack;Python&amp;rbrack; O widget fantasma aparece excluído pelo script ainda em funcionamento

### 11.0.2

Data de lançamento: **06/2025/10** Resumo: **versão secundária**

**Adicionado**:

* &amp;lbrack;Mac&amp;rbrack; Adicionar aviso sobre a versão específica do sistema operacional levando a artefatos
* &amp;lbrack;Atualização automática&amp;rbrack; Pequenas melhorias de UX no registro de erros de Ativos
* &amp;lbrack;Contornar automaticamente&amp;rbrack; Atualize para a versão 1.3.2 com melhorias de costura
* &amp;lbrack;USD&amp;rbrack;&amp;lbrack;FBX&amp;rbrack; Adicionar suporte para vários conjuntos UV com dados esparsos
* &amp;lbrack;Export&amp;rbrack; As malhas exportadas como FBX não têm seus conjuntos UV adicionais, se houver algum presente na importação

**Corrigido**:

* &amp;lbrack;MacOS&amp;rbrack;&amp;lbrack;Linux&amp;rbrack; Falha ao salvar na unidade de rede
* &amp;lbrack;Win&amp;rbrack;&amp;lbrack;Tablet&amp;rbrack; cintilando ao deslocar
* &amp;lbrack;SpaceMouse&amp;rbrack; Problema ao trabalhar com a ferramenta Caminho
* &amp;lbrack;Caixa automática&amp;rbrack; Não é possível fazer bake após um recarregamento de malha
* &amp;lbrack;Atualização automática&amp;rbrack; A sequência de imagens não é recarregada quando o primeiro bloco está ausente
* &amp;lbrack;Caminho&amp;rbrack; A tangente personalizada pode afetar a outra tangente
* &amp;lbrack;O caminho&amp;rbrack; não aparece no Conjunto de texturas se o primeiro ponto estiver em outro Conjunto de texturas
* &amp;lbrack;UI&amp;rbrack; Alguns menus são sempre desativados após a abertura de um projeto (por exemplo: simetria)
* &amp;lbrack;Propriedades&amp;rbrack; Não é possível usar/carregar predefinições de ferramenta com a ferramenta Caminho preenchido
* &amp;lbrack;USD&amp;rbrack; Vários conjuntos UV não são reconhecidos no sombreador personalizado ao usar arquivos USD
* &amp;brack;USD&amp;rbrack; Câmeras com os mesmos nomes são substituídas
* &amp;preto;Exportar&amp;rbrack; Enviar para o Photoshop resulta em espaço de cor incorreto para os resultados em cores e em tons de cinza
* &amp;preto;Exportar&amp;rbrack; canais em tons de cinza com alfa são exportados como cor em vez de escala de cinza com formato PNG
* &amp;lbrack;Export&amp;brack; Exportar canal em tons de cinza como resultado de PSD em arquivo inválido/truncado
* &amp;lbrack;Content&amp;brack; O filtro Distorcer em modo multidirecional não funciona
* &amp;lbrack;Python&amp;rbrack; Não é possível alocar erros de lista ao rastrear nós de pilha de camadas

**Problemas Conhecidos**:

* &amp;lbrack;Gerenciamento de cores&amp;rbrack; As conversões do espaço de cores HDR com ACE no Linux produzem cores fixas
* &amp;lbrack;Regressão&amp;rbrack;&amp;lbrack;UI&amp;rbrack; O menu do botão direito do mouse é muito pequeno em telas HD
* &amp;lbrack;Crash&amp;rbrack;&amp;lbrack;Python&amp;rbrack; Exportação de USD acionada por TextureStateEvent
* &amp;lbrack;Engine&amp;brack; Pintura com ferramenta Clonar nas cores normais de mudança de canal incorretamente
* &amp;lbrack;Python&amp;rbrack; O widget fantasma aparece excluído pelo script ainda em funcionamento

### 11.0.1

Data de lançamento: **04/2025/10** Resumo: **versão secundária**

Observação: a versão do CCD do **Linux será adiada até 29 de abril**

**Adicionado:**

* Atualize para Qt 6.5.8
* &amp;lbrack;Substance&amp;rbrack; Adicionar mensagem de log para filtros quando várias entradas de imagem compartilham o mesmo uso
* &amp;lbrack;Nvidia&amp;rbrack; Adicionar aviso sobre os drivers Nvidia mais recentes (572.47)

**Corrigido:**

* &amp;lbrack;Crash&amp;rbrack; Ao arrastar e soltar um sbsar com um uso em slots de canal único
* &amp;lbrack;Crash&amp;rbrack;&amp;lbrack;Caminho&amp;rbrack; A opção Alterar tipo de caminho não fica esmaecida quando não se clica em um caminho específico
* &amp;lbrack;Caminho de preenchimento&amp;rbrack; Não deve ser capaz de selecionar o material da substância
* &amp;lbrack;Engine&amp;brack; Artefatos ao longo de pinceladas
* &amp;lbrack;Engine&amp;rbrack; Os caminhos podem ser quebrados com configurações específicas
* Problema com o menu suspenso para o espaço da cor do conta-gotas
* &amp;lbrack;Atualização automática&amp;rbrack; &amp;lbrack;Python&amp;rbrack; Mensagem de erro incorreta ao usar ResourceID sem versão
* &amp;lbrack;Sombreador&amp;rbrack; Falha ao abrir alguns projetos

**Problemas Conhecidos:**

* &amp;lbrack;SpaceMouse&amp;rbrack; Problema ao trabalhar com a ferramenta Caminho
* &amp;lbrack;Gerenciamento de cores&amp;rbrack; As conversões do espaço de cores HDR com ACE no Linux produzem cores fixas
* &amp;lbrack;Regressão&amp;rbrack;&amp;lbrack;UI&amp;rbrack; O menu do botão direito do mouse é muito pequeno em telas HD
* &amp;lbrack;Crash&amp;rbrack;&amp;lbrack;Python&amp;rbrack; Exportação de USD acionada por TextureStateEvent
* &amp;lbrack;Engine&amp;brack; Pintura com ferramenta Clonar nas cores normais de mudança de canal incorretamente
* &amp;lbrack;Python&amp;rbrack; O widget fantasma aparece excluído pelo script ainda em funcionamento

### 11.0.0

Data de lançamento: **03/2025/11** Resumo: **Versão principal, novo recurso de atualização automática, ferramenta de caminho preenchido e outras melhorias no caminho, bem como novos filtros e uma geração experimental de gaiola automática para fça bake**

**Adicionado**:

* Atualização automática
* &amp;lbrack;Atualização automática&amp;rbrack; Atualizar automaticamente os ativos modificados no painel Ativos
* &amp;lbrack;Atualização automática&amp;rbrack; Atualizar automaticamente os ativos modificados em todo o projeto
* &amp;lbrack;Atualização automática&amp;rbrack; Manter a atualização automática desativada por padrão
* &amp;lbrack;Atualização automática&amp;rbrack; Tornar a atualização opcional se os parâmetros de recurso não corresponderem (.sbsar, .glsl, .ai, .svg)
* &amp;lbrack;Atualização automática&amp;rbrack; Adicionar variável de ambiente para desativar o recurso de atualização automática
* &amp;lbrack;Atualização automática&amp;rbrack;&amp;lbrack;SBSAR&amp;rbrack; Tornar a atualização opcional se os parâmetros do recurso não corresponderem
* Caminho preenchido
* &amp;lbrack;Caminho&amp;rbrack;&amp;lbrack;Preenchimento&amp;rbrack; Adicionar nova ferramenta para criar caminhos preenchidos
* Melhorias de caminho
* &amp;lbrack;Caminho&amp;rbrack; Cria um caminho que se ajusta aos polígonos
* &amp;lbrack;Caminho&amp;rbrack; Permitir alternar tipos de caminho
* &amp;lbrack;Caminho&amp;rbrack; Permite copiar e colar dados de vértice de caminho entre conteúdo e máscara
* &amp;lbrack;Caminho&amp;rbrack; Permite restringir o ângulo ao criar um novo ponto
* &amp;lbrack;Caminho&amp;rbrack; Permite restringir a criação de pontos a uma linha
* &amp;lbrack;Path&amp;brack; Fechar forma com um único clique
* &amp;lbrack;Caminho&amp;rbrack; Exibir informações de caminho
* &amp;lbrack;Caminho&amp;rbrack; Permite dimensionar e girar vértices de caminho
* &amp;lbrack;Path&amp;rbrack;&amp;lbrack;UX&amp;rbrack; Facilitar o acesso aos gizmos de transformação
* &amp;lbrack;Caminho&amp;rbrack; Adicionar visualização de caminho
* &amp;lbrack;Caminho&amp;rbrack; Desativar a visualização do caminho com Shift + P
* &amp;lbrack;Caminho&amp;rbrack; Melhorar a edição da tangente na visão lateral
* &amp;lbrack;Caminho&amp;rbrack; Permite focalizar em um caminho 3D
* &amp;lbrack;Caminho&amp;rbrack; Os vértices devem manter o status da seleção ao alternar a interface entre desativada e ativada novamente
* &amp;lbrack;Caminho&amp;rbrack; Permite excluir o Caminho usando o Backspace
* &amp;lbrack;Caminho&amp;rbrack; Mantém a lista de caminhos aberta se o usuário a expandir
* &amp;lbrack;Caminho&amp;rbrack;&amp;lbrack;Pilha de camadas&amp;rbrack; Renomeia duplicatas corretamente ao copiar/colar
* &amp;lbrack;Caminho&amp;rbrack; UI e melhorias na dica de ferramenta
* Desempenho
* &amp;lbrack;Desempenho&amp;rbrack; Melhorar o desempenho do visor ao usar um alto nível de mosaico
* &amp;lbrack;Desempenho&amp;rbrack; Habilita somente o primeiro canal em novas camadas/efeitos de preenchimento
* &amp;lbrack;Desempenho&amp;rbrack; Paralelizar computação de traçado de pincel
* Baking
* &amp;lbrack;Fazendo bake&amp;rbrack; Adicionar nova opção de geração de gaiola totalmente automática para fazer bake com malhas de alto-polietileno (experimental)
* Conteúdo
* &amp;lbrack;Content&amp;rbrack; Adicionar 6 novos filtros: estilização, quantize, kuwahara anisotrópico, suavização de chanfro, distância direcional, conversão em tons de cinza
* &amp;lbrack;Content&amp;rbrack; Atualizar ruídos e grunhidos para a versão mais recente do Designer (com o novo 2D Voronoi)
* &amp;lbrack;Content&amp;brack; Adicionar 3 novos geradores de textura (Telha Aleatória, Triangle Grid, Gerador de Scratches)
* &amp;lbrack;Content&amp;rbrack; Renomear modelo de Mecanismo Irreal e exportar predefinições
* Python
* &amp;lbrack;Shelf&amp;rbrack;&amp;lbrack;Python&amp;rbrack; Salvar material inteligente ou máscara inteligente em disco do Python
* &amp;lbrack;Python&amp;rbrack; Adicionar gaiola automática feita bake à API Python
* &amp;lbrack;Python&amp;rbrack; Permitir a edição de nomes e descrições de Conjuntos/Blocos UV de Textura
* &amp;lbrack;Python&amp;rbrack; Compartilhar configurações de resolução em fontes vetoriais e de fonte
* &amp;lbrack;Atualização automática&amp;rbrack;&amp;lbrack;Python&amp;rbrack; Expor as funcionalidades de atualização automática do projeto em Python
* Diversos
* &amp;brack;Export&amp;brack; Facilite o acesso às opções Enviar para com um novo painel
* &amp;lbrack;Nvidia&amp;rbrack; Adicionar aviso sobre os drivers Nvidia mais recentes (572.16)
* O encaixe de ângulo deve ser afetado pela seleção de espaço Objeto/Mundo
* &amp;preto;Lista do conjunto de texturas&amp;rbrack; Permite adicionar um nome personalizado aos Blocos UV e usá-los na exportação
* Mac
* &amp;lbrack;Mac&amp;rbrack; Usar Metal em vez de OpenGL para renderização gráfica
* &amp;lbrack;Mac&amp;rbrack; Soltar suporte ao Mac Intel

**Corrigido**:

* &amp;lbrack;Crash&amp;brack; Excluir entrada de imagem
* Não é possível adicionar o smart mat através do botão pilha de camadas
* Não é possível encontrar os efeitos do &amp;lbrack;Python&amp;brack; no GroupLayerNode

**Problemas Conhecidos**:

* &amp;lbrack;Gerenciamento de cores&amp;rbrack; As conversões do espaço de cores HDR com ACE no Linux produzem cores fixas
* &amp;lbrack;Regressão&amp;rbrack;&amp;lbrack;UI&amp;rbrack; O menu do botão direito do mouse é muito pequeno em telas HD
* &amp;lbrack;Crash&amp;rbrack;&amp;lbrack;Python&amp;rbrack; Exportação de USD acionada por TextureStateEvent
* &amp;lbrack;MacOS Intel&amp;rbrack; Falha ao importar algumas predefinições
* &amp;lbrack;Engine&amp;brack; Pintura com ferramenta Clonar nas cores normais de mudança de canal incorretamente
* &amp;lbrack;Python&amp;rbrack; O widget fantasma aparece excluído pelo script ainda em funcionamento
* &amp;lbrack;RedHat&amp;rbrack; Problemas no seletor de cores

## Versão 10

### 10.1.2

Data de lançamento: **2024/12/3** Resumo: **versão secundária, correções de erros**

**Corrigido**:

* &amp;lbrack;Crash&amp;brack; Excluir entrada de imagem
* Não é possível adicionar o smart mat através do botão pilha de camadas
* Não é possível encontrar os efeitos do &amp;lbrack;Python&amp;brack; no GroupLayerNode

**Problemas Conhecidos**:

* &amp;lbrack;Gerenciamento de cores&amp;rbrack; As conversões do espaço de cores HDR com ACE no Linux produzem cores fixas
* &amp;lbrack;Regressão&amp;rbrack;&amp;lbrack;UI&amp;rbrack; O menu do botão direito do mouse é muito pequeno em telas HD
* &amp;lbrack;Crash&amp;rbrack;&amp;lbrack;Python&amp;rbrack; Exportação de USD acionada por TextureStateEvent
* &amp;lbrack;MacOS Intel&amp;rbrack; Falha ao importar algumas predefinições
* &amp;lbrack;Engine&amp;brack; Pintura com ferramenta Clonar nas cores normais de mudança de canal incorretamente
* &amp;lbrack;Python&amp;rbrack; O widget fantasma aparece excluído pelo script ainda em funcionamento
* &amp;lbrack;RedHat&amp;rbrack; Problemas no seletor de cores

### 10.1.1

Data de lançamento: **2024/11/5** Resumo: **versão secundária, correções de erros**

**Adicionado**:

* &amp;lbrack;Projeto&amp;rbrack; Mantém o projeto atual aberto até que a seleção do novo projeto seja validada
* &amp;lbrack;Contornar automaticamente&amp;rbrack; A densidade do texel permite dividir melhor as Ilhas UV em UDIMs
* &amp;lbrack;Fazendo bake&amp;rbrack; Corrigir cópia ambígua no menu contextual de Mapas de Malha
* &amp;lbrack;Distorcer&amp;brack; Remover escala no visor para o eixo Z (profundidade)
* &amp;lbrack;Importar/Exportar&amp;rbrack; Remove o suporte de formatos de arquivo de imagem não utilizados
* Atualizar Substance Engine para 9.1.4

**Corrigido**:

* &amp;lbrack;Falha&amp;rbrack; Após realocar recursos em Ativos e salvar projeto
* &amp;lbrack;Crash&amp;rbrack; Problemas com a biblioteca do servidor auxiliar
* &amp;lbrack;Falha&amp;rbrack; falha no servidor Illustrator em alguns casos raros
* &amp;lbrack;Crash&amp;rbrack; Ao sair do aplicativo em alguns casos raros
* Não é possível enviar relatórios de falhas em alguns computadores
* &amp;lbrack;Fazendo bake&amp;rbrack; A cor do vértice não é lida corretamente
* &amp;lbrack;UI&amp;rbrack; A localização das janelas e das Novidades na inicialização é alterada
* &amp;lbrack;Assimp&amp;rbrack; StandardSurface do Maya não reconhecida no fça bake de ID
* &amp;lbrack;Python&amp;rbrack; A biblioteca SSL ausente gera um erro
* &amp;lbrack;Python&amp;rbrack;&amp;lbrack;Win&amp;rbrack; Erro ao chamar QColorConstants.Transparent
* &amp;lbrack;Python&amp;rbrack; As miniaturas de camadas criadas através do Python não são atualizadas até clicar dentro da pilha de camadas
* &amp;lbrack;Sombreador&amp;rbrack; Link quebrado no log de alterações
* &amp;brack;Ativos 3D&amp;rbrack; Usar configurações de proxy do SO ao acessar Ativos 3D

**Problemas Conhecidos**:

* &amp;lbrack;Gerenciamento de cores&amp;rbrack; As conversões do espaço de cores HDR com ACE no Linux produzem cores fixas
* &amp;lbrack;Regressão&amp;rbrack;&amp;lbrack;UI&amp;rbrack; O menu do botão direito do mouse é muito pequeno em telas HD
* &amp;lbrack;Crash&amp;rbrack;&amp;lbrack;Python&amp;rbrack; Exportação de USD acionada por TextureStateEvent
* &amp;lbrack;MacOS Intel&amp;rbrack; Falha ao importar algumas predefinições
* &amp;lbrack;Engine&amp;brack; Pintura com ferramenta Clonar nas cores normais de mudança de canal incorretamente
* &amp;lbrack;Python&amp;rbrack; Widget que parece excluído via script ainda funcionando
* &amp;lbrack;RedHat&amp;rbrack; Problemas no seletor de cores

### 10.1.0

Data de lançamento: **2024/09/17** Resumo: **Versão principal, conteúdo novo: máscara de área de preenchimento/filtro de cor, filtro de decalque de bordado e seis filtros de Substance genéricos, importação de USD com propriedades de material e sombreador, melhoria de desempenho, compatibilidade com a plataforma VFX 2024 e migração para Linux RedHat**

**Adicionado**:

* &amp;preto;Content&amp;brack; Adicionar novo filtro de máscara/cor da área de preenchimento
* &amp;lbrack;Content&amp;brack; Adicionar novo filtro de decalque de bordado
* &amp;lbrack;Content&amp;rbrack; Adicionar 6 novos filtros Substance genéricos (FXAA, pixelate, highpass, posterize, smoothstep, threshold)
* &amp;lbrack;USD&amp;rbrack; Exportar camada de USD com um material ASM definido
* &amp;lbrack;USD&amp;rbrack; Importar USD com propriedades de material e sombreador
* &amp;lbrack;Desempenho&amp;rbrack; Ativar miniaturas de pilha de camadas otimizadas por padrão
* &amp;lbrack;Desempenho&amp;rbrack; Reduz o tempo de abertura do arquivo do projeto e o consumo de memória (decodificação de dados)
* Compatível com a plataforma VFX 2024
* &amp;lbrack;VFX Platform 2024&amp;rbrack; Atualização para Python 3.11
* &amp;lbrack;VFX Platform 2024&amp;rbrack; Atualização para OpenEXR 3.2
* &amp;lbrack;Plataforma VFX 2024&amp;rbrack; &amp;lbrack;USD&amp;rbrack; Atualizar o OpenSubdiv 3.6.0
* &amp;lbrack;VFX Platform 2024&amp;rbrack;&amp;lbrack;Color Management&amp;rbrack; Atualizar para OCIO 2.3.2
* &amp;lbrack;Linux&amp;rbrack; Migração para o Linux RedHat
* &amp;lbrack;Linux&amp;rbrack; Atualize a versão mín do driver Nvidia para 535.171.04
* &amp;lbrack;Import&amp;brack; Adicionar uma opção para inverter o mapa normal ao importar uma malha GLTF
* &amp;lbrack;UI&amp;rbrack; Usar o valor padrão do sistema operacional para a distância de detecção de eventos de arrastar
* &amp;lbrack;Substance Engine&amp;rbrack; Adicionar função de faixa de chamada para remover os símbolos do executável
* &amp;Preenchimento;Tela inicial&amp;rbrack; Atualização para o novo formato de tela inicial
* Atualize o Substance Engine para a versão 9.1.3
* &amp;lbrack;Python&amp;rbrack; Mostrar link para exemplos no menu pilha de camadas documentação
* &amp;lbrack;JavaScript&amp;rbrack; Move plug-ins Javascript para a subpasta javascript/plugins

**Corrigido**:

* &amp;lbrack;Illustrator&amp;rbrack; Falha ao exportar um Bloco UV com gráfico .ai em casos específicos
* &amp;lbrack;Traçados dinâmicos&amp;rbrack;&amp;lbrack;Caminho&amp;rbrack; Aleatório por traçado não funciona em um caminho
* &amp;lbrack;UI&amp;rbrack;&amp;lbrack;Propriedades&amp;rbrack; Bloqueio ativado quando a divisão em blocos gráficos não é uniforme
* O arquivo TXT de depuração é criado ao clicar duas vezes no projeto do Painter
* &amp;lbrack;USD&amp;rbrack;&amp;lbrack;Export&amp;rbrack; Algumas texturas podem estar ausentes
* &amp;lbrack;ASM&amp;rbrack; Dispersão O canal de cores ignora o metal
* O filtro &amp;lbrack;Content&amp;brack; Blur não funciona no espaço de cor “funcionando”
* &amp;lbrack;Content&amp;brack; o filtro Ajustar Height também modifica o alfa da camada

**Problemas Conhecidos**:

* &amp;lbrack;Gerenciamento de cores&amp;rbrack; As conversões do espaço de cores HDR com ACE no Linux produzem cores fixas
* &amp;lbrack;Win&amp;rbrack;&amp;lbrack;Crash&amp;rbrack; &amp;lbrack;ACE&amp;rbrack; Não usar o espaço de cores sRGB ICE para o transformo de exibição
* &amp;lbrack;Regressão&amp;rbrack;&amp;lbrack;UI&amp;rbrack; O menu do botão direito do mouse é muito pequeno em telas HD
* &amp;lbrack;Crash&amp;rbrack;&amp;lbrack;Python&amp;rbrack; Exportação de USD acionada por TextureStateEvent
* &amp;lbrack;MacOS Intel&amp;rbrack; Falha ao importar algumas predefinições
* &amp;lbrack;Crash&amp;rbrack; Realocar recurso e salvar projeto
* &amp;lbrack;Engine&amp;brack; Pintura com ferramenta Clonar nas cores normais de mudança de canal incorretamente
* &amp;lbrack;Python&amp;rbrack; O widget fantasma aparece excluído pelo script ainda em funcionamento
* &amp;lbrack;RedHat&amp;rbrack; Problemas no seletor de cores

### 10.0.1

Data de lançamento: **06/2024/11** Resumo: **versão secundária, correções de erros**

**Adicionado:**

* &amp;lbrack;Library&amp;rbrack; Converte fontes de Substance em arquivos de fonte comuns
* &amp;lbrack;Illustrator&amp;rbrack;&amp;lbrack;SVG&amp;rbrack; Dá às miniaturas na seleção de escopo um fundo cinza claro
* &amp;lbrack;Python&amp;rbrack; Adicionar função na origem do bitmap para listar os espaços de cores disponíveis

**Corrigido**:

* &amp;lbrack;Pilha de camadas&amp;rbrack; Pasta sempre fechada quando movida para dentro ou para fora de outras pastas
* &amp;lbrack;Salvar&amp;rbrack; O arquivo de projeto é perdido quando “salvar como cópia” ou o salvamento automático falha em casos específicos
* &amp;lbrack;Import&amp;brack; Ativos com o mesmo nome, mas com diferentes extensões são substituídos
* &amp;lbrack;Propriedades&amp;rbrack; Configurações ausentes ao usar o ponto de ancoragem nas entradas da imagem
* &amp;lbrack;Illustrator&amp;rbrack; Não é possível importar arquivos do Illustrator após falha no servidor sem reiniciar o Painter
* &amp;lbrack;Python&amp;rbrack; A instância pai não pode ser definida com o tipo “properties”
* &amp;lbrack;Python&amp;rbrack; Configurar o alto poli como um parâmetro de fça bake não carrega o alto poly
* &amp;lbrack;Python&amp;rbrack; A mensagem de erro para set_color_space() é muito genérica
* &amp;lbrack;Python&amp;rbrack; As fontes de referência permitem criar ciclos

**Problemas Conhecidos**:

* &amp;lbrack;Gerenciamento de cores&amp;rbrack; As conversões do espaço de cores HDR com ACE no Linux produzem cores fixas
* &amp;lbrack;Regressão&amp;rbrack;&amp;lbrack;UI&amp;rbrack; O menu do botão direito do mouse é muito pequeno em telas HD
* &amp;lbrack;Crash&amp;rbrack;&amp;lbrack;Python&amp;rbrack; Exportação de USD acionada por TextureStateEvent
* &amp;lbrack;MacOS Intel&amp;rbrack; Falha ao importar algumas predefinições
* &amp;lbrack;Illustrator&amp;rbrack; Falha ao exportar um Bloco UV com gráfico .ai em casos específicos
* &amp;lbrack;Traçados dinâmicos&amp;rbrack;&amp;lbrack;Caminho&amp;rbrack; Aleatório por traçado não funciona em um caminho

### 10.0.0

Data de lançamento: **05/2024/16** Resumo: **Versão principal, edição da pilha de camadas com a API Python, leitura de arquivos nativos do Illustrator, integração de ativos 3D e novo recurso de texto**

**Adicionado**:

* &amp;lbrack;Illustrator&amp;rbrack; Usar arquivos do Illustrator com quadros de arte no Painter
* &amp;lbrack;Illustrator&amp;rbrack;&amp;lbrack;SVG&amp;rbrack; Adicionar visualizações na seleção de escopo
* &amp;lbrack;Substance 3D Assets&amp;rbrack; Procure, selecione e baixe Ativos 3D diretamente no Painter
* &amp;lbrack;Substance 3D Assets&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Novo painel
* &amp;lbrack;Substance 3D Assets&amp;rbrack; Mapas e materiais do ambiente de suporte
* &amp;lbrack;Substance 3D Assets&amp;rbrack; Permitir recarregar, navegar e abrir a pasta do local no novo painel do Substance 3D Assets
* &amp;lbrack;Substance 3D Assets&amp;rbrack; Adição de um gerenciador de downloads
* &amp;lbrack;Recurso de texto&amp;rbrack; Permitir o uso de fontes incorporáveis
* &amp;lbrack;Recurso de texto&amp;rbrack; Permite renderizar uma fonte/texto em uma malha
* &amp;lbrack;Recurso de texto&amp;rbrack; Exibe fontes do usuário e outros caminhos compartilhados no painel Ativos com uma nova categoria
* &amp;lbrack;Recurso de texto&amp;rbrack;&amp;lbrack;Propriedades&amp;rbrack; Adicionar suporte para propriedades avançadas de fontes
* &amp;lbrack;Recurso de texto&amp;rbrack; Permitir pesquisar/exibir fontes em minisprateleiras
* &amp;lbrack;Recurso de texto&amp;rbrack; Adicionar mensagem/caixa de diálogo de erro ao importar uma fonte incompatível
* Diversos
* &amp;lbrack;Preencher projeção&amp;rbrack; Melhorar o comportamento do manipulador de escala ao usar valores pequenos
* &amp;lbrack;Manipuladores&amp;rbrack; Adicionar novo modo preciso ao pressionar o atalho CTRL
* &amp;lbrack;Manipuladores&amp;rbrack; Melhorar a estabilidade do manipulador de superfície ao traduzir
* &amp;lbrack;Export&amp;brack; Adicionar o nome do espaço de cores nas saídas SBSAR
* &amp;lbrack;Desempenho&amp;rbrack; Melhorar o tempo de descoberta de bibliotecas de ativos em disco
* &amp;lbrack;Substance&amp;rbrack; Atualização para o mecanismo de Substance versão 9.1.2
* &amp;lbrack;Arrastar e soltar&amp;rbrack; Alinhar a rotação do decalque à câmera ao soltar no visor
* &amp;lbrack;Python&amp;rbrack; Edição da pilha de camadas
* &amp;lbrack;Python&amp;rbrack; Permite selecionar camada, efeito, máscara, máscara geográfica na interface
* &amp;lbrack;Python&amp;rbrack; Permitir obter/definir modos de mesclagem de camadas
* &amp;lbrack;Python&amp;rbrack; Permitir obter/definir configurações de projeção da camada de preenchimento
* &amp;lbrack;Python&amp;rbrack; Permitir a consulta da cor do material de Substance a partir de uma camada de preenchimento
* &amp;lbrack;Python&amp;rbrack; Permite consultar e definir cores uniformes e recursos em camadas e efeitos
* &amp;lbrack;Python&amp;rbrack; Permite criar e editar recursos de texto na pilha de camadas
* &amp;lbrack;Python&amp;rbrack; Permitir a edição de canais ativos em camadas e efeitos
* &amp;lbrack;Python&amp;rbrack; Permitir que as ações em lote tenham uma única operação de desfazer/refazer
* &amp;lbrack;Python&amp;rbrack; Permitir carregar/editar parâmetros de origem vetorial
* &amp;lbrack;Python&amp;rbrack; Permitir a edição de propriedades de cores de camadas e efeitos com o gerenciamento de cores
* &amp;lbrack;Python&amp;rbrack; Permite consultar e criar camadas instanciadas
* &amp;lbrack;Python&amp;rbrack; Permitir a adição do efeito de seleção de cor
* &amp;lbrack;Python&amp;rbrack; Permitir o controle do gerenciamento de cores de imagens de bitmap
* &amp;lbrack;Python&amp;rbrack; Permitir pausa/cancelamento de pausa do mecanismo
* &amp;lbrack;Python&amp;rbrack; Permite navegar para nós irmãos e pais
* &amp;lbrack;Python&amp;brack; Permitir criar efeito de filtro/gerador
* &amp;lbrack;Python&amp;rbrack; Permitir adicionar efeito de nível
* &amp;lbrack;Python&amp;rbrack; Permite adicionar máscara inteligente em uma camada
* &amp;lbrack;Python&amp;rbrack; Permitir criar/editar pontos de ancoragem
* &amp;lbrack;Python&amp;rbrack; Permitir obter/definir máscara em camadas
* &amp;lbrack;Python&amp;rbrack; Permitir criar efeito de máscara de comparação
* &amp;lbrack;Python&amp;rbrack; Permitir consultar e usar predefinições de recursos Substance
* &amp;lbrack;Python&amp;rbrack; Permite listar predefinições e seus valores por meio da função internal_properties para recursos Substance
* &amp;lbrack;Python&amp;rbrack; Permitir listar predefinições de exportação predefinidas
* &amp;lbrack;Python&amp;rbrack; Permitir listar predefinições de exportação disponíveis na biblioteca
* &amp;lbrack;Python&amp;rbrack; Permite recuperar o conteúdo das predefinições de exportação

**Corrigido**:

* &amp;lbrack;Crash&amp;rbrack; Desfazer “Remover instância de sombreamento” com Ctrl-Z
* &amp;lbrack;Crash&amp;rbrack; Criar uma camada em pilha vazia se a última seleção tiver sido um efeito
* &amp;lbrack;SVG&amp;rbrack; Problema com um valor personalizado da área recortada
* &amp;lbrack;Contornar automaticamente; Recalcular apenas a embalagem sem qualquer alteração na orientação UV resulta em falha
* &amp;lbrack;Arrastar e soltar&amp;rbrack; Atraso devido a recursos externos são pré-carregados várias vezes
* &amp;lbrack;UI&amp;rbrack; Arrastar e soltar a miniatura do recurso pode ocultar a mensagem de aviso na pilha de camadas
* &amp;lbrack;Performance&amp;rbrack; Os blocos UV mascarados ainda são computados
* &amp;lbrack;USD&amp;rbrack; Realce incorreto para seleção de escopo
* &amp;lbrack;Recurso&amp;rbrack; A imagem de bitmap é corrompida após pintar no canal normal e salvar o projeto
* &amp;lbrack;USD&amp;rbrack; Suporte para ordenação de malha de vértice com a mão esquerda
* &amp;lbrack;Substance&amp;rbrack; Redefinir para padrão sempre voltar a zero para widget de ângulo
* &amp;lbrack;Engine&amp;brack; Pintar com um SVG em um estêncil não funciona
* &amp;lbrack;Engine&amp;brack; as pinceladas do Mapa normal se partem após uma ação de desfazer
* &amp;lbrack;O gráfico para o Filtro Material do Content&amp;brack; tem mesclagem alfa e espaço de cores incorretos
* &amp;lbrack;Content&amp;brack; Os modos de mesclagem no Tile Generator não estão funcionando
* O filtro de digitalização do histograma &amp;lbrack;Content&amp;brack; produz faixas em alguns casos
* &amp;lbrack;Conteúdo&amp;rbrack; iluminação Feita bake estilizada não leva em conta o height pintado
* &amp;lbrack;Python&amp;rbrack; Erro inesperado ao recuperar informações de camada da instância após alteração do sombreador
* &amp;lbrack;Salvar&amp;rbrack; O arquivo de projeto é perdido quando “salvar como” falha em casos específicos

**Problemas Conhecidos**:

* &amp;lbrack;Gerenciamento de cores&amp;rbrack; As conversões do espaço de cores HDR com ACE no Linux produzem cores fixas
* &amp;lbrack;Crash&amp;rbrack;&amp;lbrack;Linux&amp;rbrack;&amp;lbrack;AMD&amp;rbrack; Arrastar e soltar recursos em pilha de camadas no Wayland OS
* &amp;lbrack;Regressão&amp;rbrack;&amp;lbrack;UI&amp;rbrack; O Menu do Clique com o Botão Direito é muito pequeno em telas HD
* &amp;lbrack;Crash&amp;rbrack;&amp;lbrack;Python&amp;rbrack; Exportação de USD acionada por TextureStateEvent
* &amp;lbrack;Save&amp;rbrack; O arquivo de projeto Spp é perdido quando “salvar como cópia” falha em casos específicos
* &amp;lbrack;MacOS Intel&amp;rbrack; Falha ao importar algumas predefinições
* &amp;lbrack;Illustrator&amp;rbrack; Não é possível importar arquivos Ai após falha do servidor sem reiniciar o Painter
* &amp;lbrack;Import&amp;brack; Ativos com o mesmo nome, mas com diferentes extensões são substituídos

## Versão 9

### 9.1.2

Data de lançamento: **01/2024/30** Resumo: **versão secundária, correções de erros**

**Adicionado**:

* &amp;lbrack;Desempenho&amp;rbrack; Melhorar o tempo de criação da primeira camada de preenchimento em novos projetos
* &amp;lbrack;Performance&amp;rbrack; Reduz o tempo de carregamento de mapas de ambiente pesado
* &amp;lbrack;Substance&amp;rbrack; Permite salvar/fechar projetos mesmo quando miniaturas estão sendo geradas

**Corrigido**:

* A gravação falha em projetos de versões anteriores quando o visor é modificado
* &amp;lbrack;Crash&amp;rbrack; Reimportando malha ao usar o AO personalizado e o gerenciamento de cores
* &amp;lbrack;Preencher projeção&amp;rbrack; Clicar no manipulador de escala exibe a mensagem “não é possível pintar”
* &amp;lbrack;Pincel&amp;rbrack; Pintar com alinhamento UV causa artefatos
* &amp;lbrack;Pilha de camadas&amp;rbrack; A renomeação da camada é lenta quando a pilha é muito longa
* &amp;lbrack;Pilha de camadas&amp;rbrack; Mensagem de erro incorreta ao usar filtro incompatível na máscara
* &amp;lbrack;Pilha de camadas&amp;rbrack; A seleção volta para a camada superior após a exclusão
* &amp;lbrack;Export&amp;brack; A textura normal gerada está sempre no modo de preenchimento do vizinho de espaço 3D
* &amp;lbrack;A Textura alfa do &amp;rbrack; não é gerada com a predefinição Visualização 2D export
* &amp;lbrack;Export&amp;brack; a exportação de SBSAR tem usos incorretos com mapas convertidos
* &amp;lbrack;Sombreador&amp;rbrack; o registro de alterações do API de sombreamento não está atualizado com as alterações mais recentes do ASM

**Problemas Conhecidos**:

* &amp;lbrack;Gerenciamento de cores&amp;rbrack; As conversões do espaço de cores HDR com ACE no Linux produzem cores fixas
* &amp;lbrack;Crash&amp;rbrack;&amp;lbrack;Linux&amp;rbrack;&amp;lbrack;AMD&amp;rbrack; Arrastar e soltar recursos em pilha de camadas no Wayland OS
* &amp;lbrack;Regressão&amp;rbrack;&amp;lbrack;UI&amp;rbrack; O Menu do Clique com o Botão Direito é muito pequeno em telas HD
* &amp;lbrack;Crash&amp;rbrack;&amp;lbrack;Python&amp;rbrack; Exportação de USD acionada por TextureStateEvent

### 9.1.1

Data de lançamento: **2023/12/05** Resumo: **versão secundária, correções de erros e envio para a funcionalidade do After Effects**

**Adicionado:**

* &amp;lbrack;Interop&amp;rbrack; Permite enviar uma malha texturizada para o After Effects (Ae 24.1)

**Corrigido:**

* &amp;lbrack;Fill&amp;brack; UV definido para projeção de conjunto UV não lê mais de 2 conjuntos UV
* &amp;lbrack;Crash&amp;rbrack; Usando mapa de ambiente de 16K
* &amp;lbrack;Crash&amp;rbrack; Exr usado como entrada de imagem
* &amp;lbrack;Crash&amp;rbrack; Copiar e colar caminhos entre projetos
* &amp;lbrack;QoL&amp;rbrack; Arrastar e soltar o recurso Alpha no modo de decalque cria Projeção UV na máscara
* &amp;lbrack;Caminho&amp;rbrack; Copiar vértices de caminho também renomeia o caminho de destino ao reabrir o projeto
* &amp;lbrack;Linux&amp;rbrack; A escolha de cores pode ser interrompida com várias telas
* &amp;lbrack;Auto Unwrap&amp;brack; problema na interface do usuário para controle de densidade do texel
* O feedback da IU do &amp;lbrack;Color Management&amp;rbrack; é adequado para maiúsculas e minúsculas, mas o mecanismo não
* &amp;lbrack;Gerenciamento de cores&amp;rbrack; Seleção de espaço de cores incorreta na máscara com substituição de dados do usuário

**Problemas Conhecidos:**

* &amp;lbrack;Gerenciamento de cores&amp;rbrack; As conversões do espaço de cores HDR com ACE no Linux produzem cores fixas
* &amp;lbrack;Crash&amp;rbrack;&amp;lbrack;Linux&amp;rbrack; com Linux Wayland no AMD ao arrastar e soltar recursos na Pilha de camadas
* &amp;lbrack;Crash&amp;rbrack;&amp;lbrack;Mac&amp;rbrack; Alterando o valor da filtragem anisotrópica no sistema operacional Monterey
* &amp;lbrack;Regressão&amp;rbrack;&amp;lbrack;UI&amp;rbrack; O menu do botão direito é muito pequeno na tela hd
* &amp;lbrack;Python&amp;rbrack; Falha ao exportar USD acionada por TextureStateEvent

### 9.1.0

Data de lançamento: **2023/11/07** Resumo: **Versão principal que apresenta suporte a SVG e transparência, bem como melhorias na ferramenta de arrastar e soltar e no caminho**

**Adicionado:**

* &amp;lbrack;SVG&amp;rbrack; Permitir importação de arquivos vetoriais (SVG)
* &amp;lbrack;SVG&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Adicionar suporte para propriedades específicas de SVG
* &amp;lbrack;SVG&amp;rbrack; Adicionar uma opção para preservar facilmente as proporções da imagem original
* &amp;lbrack;SVG&amp;rbrack; Permite usar automaticamente alfa de SVG com transparência
* &amp;lbrack;Interop&amp;rbrack; Permite enviar uma malha texturizada para o After Effects (Ae 24.1 beta)
* &amp;lbrack;Interop&amp;rbrack; Adicionar configurações de Enviar para o After Effects
* &amp;lbrack;QoL&amp;rbrack;&amp;lbrack;Assets&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Importar ativo automaticamente ao arrastar e soltar no slot da interface
* &amp;lbrack;QoL&amp;rbrack; Permite arrastar e soltar ativos externos na pilha de camadas
* &amp;lbrack;QoL&amp;rbrack;&amp;lbrack;Pilha de camadas&amp;rbrack; Arraste e solte texturas do painel Ativos para a Pilha de camadas
* &amp;lbrack;QoL&amp;rbrack;&amp;lbrack;Viewport&amp;rbrack; Permitir arrastar e soltar o gerador, filtros na malha
* &amp;lbrack;QoL&amp;rbrack;&amp;lbrack;Viewport&amp;rbrack; Permitir soltar ativos externos na malha
* &amp;lbrack;QoL&amp;rbrack;&amp;lbrack;Projeção&amp;rbrack; Adicionar novo conjunto UV ao modo de projeção do conjunto UV
* &amp;lbrack;QoL&amp;rbrack; Arrastar e soltar Máscaras inteligentes como novas camadas no visor e na Pilha de camadas
* &amp;lbrack;QoL&amp;rbrack; Adicionar seletor para Geradores com múltiplas saídas quando usado em uma máscara
* &amp;lbrack;QoL&amp;rbrack; Permite arrastar e soltar imagens de canal único sobre um efeito de preenchimento
* &amp;lbrack;QoL&amp;rbrack;&amp;lbrack;Pilha de camadas&amp;rbrack; Use modificadores CTRL/ALT com arrastar e soltar para especificar onde/como criar efeitos/camada
* &amp;lbrack;Caminho&amp;rbrack; Alterna a visibilidade dos caminhos individualmente no painel de caminhos
* &amp;lbrack;Caminho&amp;rbrack; Permitir o uso de manipuladores de transformação para pontos de caminho
* &amp;lbrack;Path&amp;brack; Permite controlar manualmente tangentes por vértice
* &amp;lbrack;Caminho&amp;rbrack; Copiar/colar propriedades do caminho
* &amp;lbrack;Caminho&amp;rbrack; Introduzir um atalho vazio para o botão Quebrar tangente
* &amp;lbrack;Sombreador&amp;rbrack; Adicionar suporte para Opacidade e Translucidez no sombreador ASM
* &amp;lbrack;Sombreador&amp;rbrack; Adicionar suporte para canal de Cor de absorção com sombreador ASM
* &amp;lbrack;Sombreador&amp;rbrack; Melhorar dicas de ferramentas de parâmetros de sombreador do ASM
* &amp;lbrack;Sombreador&amp;rbrack; Alterar a cor padrão do canal de Translucidez para preto
* &amp;lbrack;Configurações de exibição&amp;rbrack; Ativar Suavização temporal por padrão
* &amp;preto;Configurações de exibição&amp;rbrack; Ativar configuração de dispersão abaixo da superfície por padrão
* &amp;lbrack;Substance&amp;rbrack; Adicionar suporte para a propriedade ColorSpace a partir da entrada/saída do gráfico
* &amp;lbrack;Substance&amp;rbrack; Atualize o mecanismo de Substance para a versão 9.0.3
* &amp;lbrack;UI&amp;rbrack; Torna o botão contextual da barra de ferramentas acessível mesmo se a janela do aplicativo for pequena
* &amp;preto;Desempacotar automaticamente&amp;rbrack; Controlar o número de Blocos UV com Densidade de texel
* &amp;lbrack;Fazendo bake&amp;rbrack; Desativar Rastreamento de raios do GPU em GPUs AMD por padrão
* &amp;lbrack;Performance&amp;rbrack; Aplicar compactação sem perdas em imagens de 16 bits para reduzir o espaço ocupado pelo projeto
* &amp;lbrack;Python&amp;rbrack; Permite manipular a Câmera padrão no Visualização 3D
* &amp;lbrack;Python&amp;rbrack; Expor a capacidade de exportar malha via script
* &amp;lbrack;Content&amp;rbrack;&amp;lbrack;Amostras&amp;rbrack; Adicionar novo projeto de amostra “Tabela de restaurantes franceses”
* &amp;lbrack;Conteúdo&amp;rbrack; Atualizar o logotipo do Substance alfa para a nova versão
* &amp;lbrack;Content&amp;brack; Adicionar três filtros de material focados em SVG (adesivo personalizado, spray personalizado e gráfico para o material)

**Corrigido:**

* &amp;lbrack;Crash&amp;rbrack; Alterar o tamanho do manipulador quando não estiver usando a ferramenta simetria
* &amp;lbrack;Crash&amp;rbrack; &amp;lbrack;Pilha de camadas&amp;rbrack; Criando camada quando nada estiver selecionado
* &amp;lbrack;Projeto&amp;rbrack; Mapas de malha podem ser corrompidos após a remoção de recursos não utilizados
* &amp;lbrack;Projeto&amp;rbrack; Corrupção de recurso após reimportar ou fazer bake imagem
* &amp;lbrack;Assets&amp;rbrack; Recarregar um ativo o remove de Favoritos
* &amp;lbrack;Import&amp;rbrack; Não é possível importar recursos quando “Nenhum resultado encontrado” no painel de ativos
* &amp;lbrack;UI&amp;rbrack; A seta da barra de ferramentas contextual não aparece em alguns casos
* &amp;lbrack;Substance&amp;rbrack; O botão lado a lado para valores booleanos não é suportado
* &amp;lbrack;Level&amp;rbrack; Rótulo de canal incorreto quando usado na máscara
* &amp;lbrack;Export&amp;rbrack;&amp;lbrack;glTF&amp;rbrack; os arquivos glTF/GLB exportados do Painter não têm uma unidade de tamanho físico
* &amp;lbrack;Content&amp;rbrack; A intensidade do filtro de Desfoque é fixada em 16
* &amp;lbrack;Content&amp;brack; A entrada da imagem do filtro de Correspondência de Cores “cor de destino” não está visível

**Problemas conhecidos:**

* &amp;lbrack;Gerenciamento de cores&amp;rbrack; As conversões do espaço de cores HDR com ACE no Linux produzem cores fixas
* &amp;lbrack;Crash&amp;rbrack;&amp;lbrack;Linux&amp;rbrack; com Linux Wayland no AMD ao arrastar e soltar recursos na Pilha de camadas
* &amp;lbrack;Crash&amp;rbrack;&amp;lbrack;Mac&amp;rbrack; Alterando o valor da filtragem anisotrópica no sistema operacional Monterey
* &amp;lbrack;Crash&amp;rbrack; Exr usado como entrada de imagem
* &amp;lbrack;Crash&amp;rbrack; Usando mapa de ambiente de 16K
* &amp;lbrack;Auto Unwrap&amp;brack; problema na interface do usuário para controle de densidade do texel
* &amp;lbrack;Regressão&amp;rbrack;&amp;lbrack;UI&amp;rbrack; O menu do botão direito é muito pequeno na tela hd
* &amp;lbrack;Python&amp;rbrack; Falha ao exportar USD acionada por TextureStateEvent
* &amp;lbrack;QoL&amp;rbrack; Arrastar e soltar o recurso Alpha no modo de decalque cria Projeção UV na máscara

### 9.0.1

Data de lançamento: **09/2023/19** Resumo: **Versão de correção de bug secundária com várias melhorias**

**Adicionado:**

* &amp;lbrack;Import&amp;rbrack; Definir local de importação padrão na janela de importação
* &amp;lbrack;Modo de Fça bake&amp;rbrack; Permite redefinir parâmetros para seus valores padrão
* &amp;lbrack;Fazendo bake&amp;rbrack; Define o fça bake com resolução de tinta ao criar um projeto
* &amp;lbrack;Simetria&amp;rbrack; Desvincular manipulador específico de simetria do atalho Q
* &amp;lbrack;Menu&amp;rbrack; Adicionar opção “mostrar registro” no menu Ajuda
* &amp;preto;Visor&amp;rbrack; Melhorar a velocidade de renderização da sombra
* &amp;lbrack;Substance&amp;rbrack; Atualize o mecanismo para a versão 9.0.1
* O arquivo de configuração OCIO do &amp;lbrack;Color Management&amp;rbrack; pode ter qualquer tipo de extensão
* &amp;lbrack;Assets&amp;rbrack; O recurso Sbsar com o uso de “decalque” deve ser definido automaticamente para distorcer a projeção
* &amp;lbrack;Caminho&amp;rbrack; Exibir uma mensagem ao tentar interagir com a ferramenta Caminho enquanto a interface do usuário e os Gizmos estiverem ocultos

**Corrigido:**

* &amp;lbrack;Crash&amp;rbrack; Alt + Arrastar no painel Caminho
* &amp;lbrack;Importar Recursos&amp;rbrack; Falha aleatória ao remover recursos para importar
* Falha ao importar um arquivo GLB compactado
* Problema ao pintar em malhas que compartilham UVs
* Flash de malha preto ao recalcular ou carregar cache
* &amp;lbrack;Propriedades&amp;rbrack; O menu do botão direito do mouse para redefinir parâmetros não aparece nas listas suspensas
* &amp;lbrack;Nível&amp;rbrack; Controles deslizantes de entrada bloqueados pelo nível anterior
* &amp;lbrack;AMD&amp;rbrack;&amp;lbrack;Esparsa&amp;rbrack; opção SVT se ativada gera artefatos
* &amp;lbrack;Projeção&amp;rbrack;&amp;lbrack;Distorcer&amp;rbrack; Falha ao clicar duas vezes nos vértices
* &amp;lbrack;Caminho&amp;rbrack; UI e caminho visíveis no modo de fça bake
* &amp;lbrack;AMD&amp;rbrack; Textura perdida ao brincar com a visibilidade
* &amp;lbrack;Sparse&amp;brack; Resolução muito baixa ao girar a malha

**Problemas Conhecidos:**

* &amp;lbrack;Gerenciamento de cores&amp;rbrack; As conversões do espaço de cores HDR com ACE no Linux produzem cores fixas

### 9.0.0

Data de lançamento: **2023/06/20** Resumo: **Versão principal com Tinta ao longo de um caminho que permite curvas 3D, novos materiais de base e limpeza de materiais herdados e novas predefinições para curvas 3D**

**Adicionado:**

* &amp;lbrack;Caminho&amp;rbrack; Adicionar nova Tinta ao longo da ferramenta Caminho
* &amp;lbrack;Caminho&amp;rbrack; Adiciona um atalho vazio para a ferramenta de caminho
* &amp;lbrack;Caminho&amp;rbrack; Permite adicionar novos pontos a um caminho existente
* &amp;lbrack;Caminho&amp;rbrack; Adicionar atalho para sair da criação do caminho atual
* &amp;lbrack;Caminho&amp;rbrack; Permitir a edição de propriedades de pincéis para caminhos
* &amp;lbrack;Caminho&amp;rbrack; Ajusta tangentes automaticamente ao posicionar um ponto
* &amp;lbrack;Caminho&amp;rbrack; Recalcular tangentes quando um ponto for movido
* &amp;lbrack;Caminho&amp;rbrack; Ajustar pontos recém-criados à superfície de uma malha
* &amp;lbrack;Caminho&amp;rbrack; Permite editar a pressão por vértice
* &amp;lbrack;Caminho&amp;rbrack; Ajusta a pressão do ponto recém-criado a partir de pontos vizinhos
* &amp;lbrack;Caminho&amp;rbrack; Permite converter pontos para suavizar/canto (quebra tangente)
* &amp;lbrack;Caminho&amp;rbrack; Permite mover um ponto recém-adicionado imediatamente
* &amp;lbrack;Caminho&amp;rbrack; Permite remover pontos do caminho existente
* &amp;lbrack;Caminho&amp;rbrack; Permite inverter a direção de um caminho
* &amp;lbrack;Caminho&amp;rbrack; Permite selecionar um caminho no visor
* &amp;lbrack;Caminho&amp;rbrack; Permite selecionar pontos do caminho com seleção de letreiro
* &amp;lbrack;Caminho&amp;rbrack; Introduza os atalhos CTRL-A para selecionar todos os pontos de um caminho
* &amp;lbrack;Caminho&amp;rbrack; Permitir fechar caminho
* &amp;lbrack;Caminho&amp;rbrack; Permite especificar o caminho até o eixo em Propriedades
* &amp;lbrack;Caminho&amp;rbrack; Adiciona um menu de controle de vértice à barra de ferramentas contextual
* &amp;lbrack;Caminho&amp;rbrack; Introduzir modos de tinta/apagar/borrar na ferramenta de caminho
* &amp;lbrack;Caminho&amp;rbrack; Criar feedback visual para os caminhos no visor
* &amp;lbrack;Caminho&amp;rbrack; Adicionar um indicador visual para a direção do caminho
* &amp;lbrack;Caminho&amp;rbrack; Adicionar thickness de linha às configurações de exibição do caminho
* &amp;lbrack;Caminho&amp;rbrack; Permitir ocultar caminhos UI
* &amp;lbrack;Caminho&amp;rbrack; Adicionar painel Caminho para listar os caminhos da camada atualmente selecionada
* &amp;lbrack;Caminho&amp;rbrack; Adicionar feedback visual ao passar o mouse sobre um caminho no painel Caminho
* &amp;lbrack;Caminho&amp;rbrack; Exibir painel de caminho sempre que a ferramenta Caminho for selecionada
* &amp;lbrack;Caminho&amp;rbrack; Permite renomear, excluir, copiar, recortar, duplicar caminho no painel Caminho
* &amp;lbrack;Caminho&amp;rbrack; Exibir mensagem ao tentar interagir no visor 2D com a ferramenta Caminho
* &amp;lbrack;Biblioteca&amp;rbrack; Integrar novo conteúdo (ferramentas e materiais de base de caminho)
* &amp;lbrack;Traçados dinâmicos&amp;rbrack; Adicionar propriedade de distância para traçados dinâmicos
* &amp;lbrack;Traçados dinâmicos&amp;rbrack; Adicionar propriedades de tamanho e espaçamento aos traçados dinâmicos
* &amp;lbrack;Traçados dinâmicos&amp;rbrack; Adicionar propriedade início/meio/fim para traçados dinâmicos
* &amp;lbrack;Python&amp;rbrack;&amp;lbrack;USD&amp;rbrack; Expor os parâmetros de configuração do projeto para o formato USD
* &amp;lbrack;Python&amp;rbrack;&amp;lbrack;USD&amp;rbrack; Expor os parâmetros de criação do projeto para o formato USD
* &amp;lbrack;Export&amp;rbrack;&amp;lbrack;USD&amp;rbrack; Adicionar informações de caminho do projeto no arquivo USD exportado
* &amp;lbrack;GLTF&amp;rbrack; Atualiza texturas na biblioteca ao recarregar um arquivo GLTF
* &amp;lbrack;Sombreador&amp;rbrack; Reduzir artefatos de costura para Ilhas UV com orientação diferente
* &amp;lbrack;Engine&amp;rbrack; Atualização para o mecanismo Substance versão 9.0

**Corrigido:**

* &amp;lbrack;Import&amp;rbrack; Algumas GLB com texturas não obtêm texturas no Painter
* &amp;lbrack;AMD&amp;rbrack; Artefatos em bordas para todos os preenchimentos de projeção 3D
* &amp;lbrack;As Texturas do motor&amp;rbrack; são interrompidas ao alternar a visibilidade da camada
* &amp;lbrack;Engine&amp;rbrack; as Texturas estão vazias em alguns locais ao alterar o modo de mesclagem
* &amp;lbrack;Motor&amp;rbrack; Textura/Projeção é um modo de distorção vazio em alguns casos
* &amp;lbrack;Iray&amp;rbrack; a Iteração é redefinida para 0 ao salvar a renderização
* &amp;lbrack;Log&amp;brack; mensagem de erro de USD ao executar Arquivo > Novo

**Problemas Conhecidos:**

* &amp;lbrack;Gerenciamento de cores&amp;rbrack; As conversões do espaço de cores HDR com ACE no Linux produzem cores fixas
* &amp;lbrack;Pilha de camadas&amp;rbrack; Fonte de entrada não salva por camada

## Versão 8

### 8.3.1

Data de lançamento: **2023/04/27**

**Adicionado:**

* &amp;lbrack;Modo de Fça bake&amp;rbrack; Adicionar atalho (vazio) para mostrar/ocultar a visualização do visor
* &amp;lbrack;Modo de Fça bake&amp;rbrack; Sempre mostrar Low Poly ao usar o botão “Ocultar malhas de fça bake”
* &amp;preto;Modo de Fça bake&amp;rbrack; Mostrar sufixo para correspondência por nome com base no conjunto de texturas atual
* &amp;lbrack;Import&amp;rbrack; Adicionar suporte para arquivos binários GLTF (glb)
* &amp;preto;Lista do conjunto de texturas&amp;rbrack; Adicionar menu para selecionar ou criar instâncias de sombreamento
* &amp;preto;Lista do conjunto de texturas&amp;rbrack; Permite alterar rapidamente o conjunto de texturas e a resolução do Bloco UV
* &amp;lbrack;Tamanho físico&amp;rbrack; Melhorar o comportamento do manipulador ao usar tamanho físico na Projeção UV
* &amp;lbrack;UI&amp;rbrack; Trazer de volta &#39;Salvar como&#39; para o menu Arquivo principal
* &amp;lbrack;UI&amp;rbrack; Salvar seleção de visualização (somente 2D, somente 3D, ambos) no layout da interface
* &amp;lbrack;USD&amp;rbrack; Mensagem de erro menos vaga na criação do projeto com formas de USD não suportadas
* &amp;lbrack;Python&amp;rbrack; Adicionar eventos de fça bake para seguir o progresso de Fça bake
* &amp;lbrack;Python&amp;rbrack; Permitir cancelamento de um faço bake
* &amp;lbrack;Python&amp;rbrack; Expor &#39;Baseado no modelo de saída&#39; para Tipo de Arquivo e Profundidade de bits na exportação
* &amp;lbrack;Python&amp;rbrack; Expor tempo de atualização para TextureStateEvent.Update

**Corrigido:**

* &amp;lbrack;Falha&amp;rbrack; Falha rara ao fechar um projeto
* &amp;lbrack;Crash&amp;rbrack; &amp;lbrack;Fazendo bake&amp;rbrack; Ativa a sincronização do mapa de malha com Height ou curvatura em um projeto específico
* &amp;lbrack;Crash&amp;rbrack;&amp;lbrack;Scripting&amp;rbrack; Falha ao adicionar um material após a criação da instância de sombreamento
* &amp;lbrack;Modo de Fça bake&amp;rbrack; A intensidade do AO em material neutro não tem efeito
* &amp;lbrack;Modo de Fça bake&amp;rbrack; Falha ao alternar para o modo de fça bake antes do modelo ser carregado
* &amp;lbrack;Modo de Fça bake&amp;rbrack; Mensagem de erro ausente na guia Processo de Fça bake
* &amp;lbrack;Modo de Fça bake&amp;rbrack; As configurações de materiais neutros não têm efeito após a reimportação de uma malha
* &amp;lbrack;Modo de Fça bake&amp;rbrack; O separador de Janela é salvo globalmente e não por modo
* &amp;lbrack;Modo de Fça bake&amp;rbrack; Problema de visualização: o normal médio não altera a superfície da caixa
* &amp;lbrack;Gerenciamento de cores&amp;rbrack; A configuração de detecção automática de espaço de cores está desativada quando a variável de ambiente OCIO está presente
* &amp;lbrack;O filtro Contorno da Máscara do Content&amp;brack; possui artefato com entrada de height
* O controle deslizante de intensidade do filtro de desfoque de Inclinação do &amp;lbrack;Content&amp;rbrack; está fixado em 1.0
* &amp;lbrack;Interop&amp;rbrack; Não é possível criar projetos com GLTF a partir do Sampler
* &amp;lbrack;Pilha de camadas&amp;rbrack; O valor da divisão em blocos gráficos da projeção não é atualizado corretamente com o manipulador
* &amp;lbrack;Linux&amp;rbrack; Deslocamento entre a caneta eletrônica gráfica e o cursor com HDPI maior que 100%
* &amp;lbrack;Python&amp;rbrack; Falha ao reimportar uma malha após criar um projeto
* &amp;lbrack;Substance&amp;rbrack; os ruídos 3D são quebrados após a reimportação de uma malha
* &amp;lbrack;Blocos UV&amp;rbrack; O deslocamento da Projeção UV é fixado em 1
* O feedback visual em &amp;preto;Visor&amp;rbrack; linhas retas não está mais visível
* &amp;lbrack;WhatsNew&amp;rbrack; Retorno de linha incorreto em títulos de recurso

**Problemas Conhecidos:**

* &amp;lbrack;Import&amp;rbrack; Algumas GLB com texturas não obtêm texturas no Painter

### 8.3.0

*(Lançado: 10 de janeiro de 2023*)Resumo: **Versão principal com novo modo de fça bake, nova importação e exportação de arquivos USD e suporte a tamanho físico para Projeção UV**

**Adicionado:**

* &amp;lbrack;Modo de Fça bake&amp;rbrack; Novo modo de fça bake dedicado ao processo de fça bake

* &amp;lbrack;Modo de Fça bake&amp;rbrack; Define o atalho para alternar para o modo de fça bake para F8

* &amp;lbrack;Modo de Fça bake&amp;rbrack; Adiciona os botões Iniciar e Cancelar fça bake no visor

* &amp;preto;Modo de Fça bake&amp;rbrack; Adicionar seleção de fça bake na lista Conjunto de Texturas

* &amp;lbrack;Modo de Fça bake&amp;rbrack; Adicionar nova janela de Baker do Mapa de Malha para selecionar baker

* &amp;lbrack;Modo de Fça bake&amp;rbrack; Adicionar nova janela Configurações do Mapa de Malha para editar as configurações de fça bake

* &amp;lbrack;Modo de Fça bake&amp;rbrack; Adicionar nova janela de Log de Fça bake para seguir o processo de fça bake

* &amp;lbrack;Modo de Fça bake&amp;rbrack; Adicionar parâmetros de fça bake e desfazer ações na janela de histórico

* &amp;lbrack;Modo de Fça bake&amp;rbrack; Adicionar trilhas nas Configurações do Mapa de Malha

* &amp;lbrack;Modo de Fça bake&amp;rbrack; Adicionar miniaturas de mapas de malha na janela Baker de mapas de malha

* &amp;lbrack;Modo de Fça bake&amp;rbrack; Adicionar menu recolhível de configurações de visualização na janela de visualização 3D

* &amp;lbrack;Modo de Fça bake&amp;rbrack; Adicionar configuração de visualização para mostrar/ocultar a malha de alto polígono

* &amp;lbrack;Modo de Fça bake&amp;rbrack; Adicionar configuração de visualização para mostrar/ocultar a malha do compartimento e o wireframe

* &amp;lbrack;Modo de Fça bake&amp;rbrack; Adicionar configuração de visualização para mostrar/ocultar a malha de baixa poli

* &amp;preto;Modo de Fça bake&amp;rbrack; Adicionar configuração de visualização para mostrar as bordas sólidas sem emendas UV como erros

* &amp;lbrack;Modo de Fça bake&amp;rbrack; Informar no visor sobre a malha e fazer bake erros se o Log de Fça bake não estiver visível

* &amp;preto;Modo de Fça bake&amp;rbrack; Adicionar ação para sincronizar as configurações de baker em todos os Conjuntos de Textura

  Na janela Baker do mapa de malha, cada baker (bem como as configurações comuns) pode ser sincronizado entre os conjuntos de textura clicando no ícone de link ao lado de seu nome. Esta ação abrirá uma janela que permite selecionar quais conjuntos de texturas compartilharão os mesmos parâmetros.

* &amp;preto;Modo de Fça bake&amp;rbrack; Adicionar ações para copiar e colar configurações de baker

  Na janela Baker do Mapa de malha estão disponíveis ações para copiar e colar cada configuração de baker nos Conjuntos de textura por meio do menu dedicado na parte superior da janela ou do menu contextual do botão direito do mouse.

* &amp;lbrack;Modo de Fça bake&amp;rbrack; Adicionar botão ao Fazer bake Log para saltar do erro para as configurações corretas

  Quando um baker falha ou uma malha não é carregada corretamente, uma mensagem de erro aparece no registro de Fça bake. Um botão ao lado da mensagem permite alterar a janela Baker do mapa de malha e Configurações do mapa de malha para mostrar as configurações relacionadas. Isso ajuda a isolar com mais facilidade a origem de um problema para corrigi-lo.

* &amp;Preenchimento;Modo de Fça bake&amp;rbrack; Adiciona menus para gerenciar Conjuntos de Texturas e seleções de Baker

  Tanto na lista “Texture Set” quanto na janela “Mesh Map Baker” foi adicionado um pequeno menu de ação para ajudar a copiar e inverter seleções.

* &amp;lbrack;Modo de Fça bake&amp;rbrack; Dividir lista de seleção de baker por Conjunto de Textura

* &amp;preto;Modo de Fça bake&amp;rbrack; Dividir configurações comuns por Conjunto de Textura

* &amp;lbrack;Modo de Fça bake&amp;rbrack; Carregue malhas de alto-polígono e em gaiola sem congelar a interface

* &amp;lbrack;Modo de Fça bake&amp;rbrack; Use a barra de progresso do visor para mostrar o carregamento da malha

* &amp;lbrack;Modo de Fça bake&amp;rbrack; Adicionar estado de carregamento de malha no Log de Fça bake

* &amp;lbrack;Modo de Fça bake&amp;rbrack; Permite virar a malha no visor durante a faz bake

* &amp;lbrack;Modo de Fça bake&amp;rbrack; Definir ordem de fça bake com base na visibilidade atual do visor da malha

* &amp;lbrack;Modo de Fça bake&amp;rbrack; Exibir gaiola de fça bake implícita no visor

  Se não estiver usando um arquivo de malha de gaiola personalizado, uma malha de gaiola automática será gerada e exibida na janela de visualização. Seu tamanho será baseado no parâmetro Distância frontal máxima das configurações comuns de fça bake. A malha de gaiola é usada para indicar até onde a correspondência entre o poli baixo e alto irá.

* &amp;lbrack;Modo de Fça bake&amp;rbrack; Mostrar lista correspondente de nomes de malha para Correspondência por Nome no Log de Fça bake

* &amp;lbrack;Modo de Fça bake&amp;rbrack; Usar material neutro para exibir modelo 3D no visor

* &amp;lbrack;Modo de Fça bake&amp;rbrack; Desativa o cálculo do motor no modo de fça bake

* &amp;lbrack;Modo de Fça bake&amp;rbrack; Exibir um aviso ao sair do aplicativo enquanto um faço bake estiver em andamento

* &amp;lbrack;Baker&amp;rbrack; Atualizar rótulos de configuração de suavização de serrilhado

  Os valores de configuração de suavização de borda foram renomeados para “Sobreamostragem” e com um número multiplicador explícito para esclarecer seu comportamento.

* &amp;lbrack;Baker&amp;rbrack; Atualize os baker para a versão 2.5.7.

* &amp;lbrack;USD&amp;rbrack; Importar e exportar arquivos de Universal Scene Description (USD)

* &amp;lbrack;USD&amp;rbrack; Adiciona opções de USD à janela Novo Projeto ao selecionar um arquivo USD

* &amp;lbrack;USD&amp;rbrack; Adicionar nova janela de seleção de Escopo e Variantes

  Ao importar um arquivo USD, clicar no botão de alteração na janela Novo projeto ou Configuração do projeto permite selecionar qual parte e variantes de um arquivo USD importar.

* &amp;lbrack;USD&amp;rbrack; Adicionar opções de níveis de subdivisão

  Ao criar um novo projeto com um arquivo de malha USD que contém subdivisões, é possível selecionar o nível de subdivisões usando um controle deslizante. O projeto será criado com a malha subdividida. O nível pode ser modificador por meio da Configuração do projeto.

* &amp;lbrack;USD&amp;rbrack; Importar malhas com pele USD em um quadro específico

  Ao criar um novo projeto com um arquivo de malha USD que contém animação, é possível selecionar a quadro usando um controle deslizante que reflete a sequência de linha do tempo incorporada. O quadro pode ser modificador por meio da Configuração do projeto.

* &amp;lbrack;USD&amp;rbrack;&amp;lbrack;Export&amp;rbrack; Adicionar uma opção para exportar arquivos USD

  Nova caixa de seleção Exportar USD adicionada à janela Exportar textura. Quando marcada, permite exportar arquivos USD, bem como mapas de textura usando qualquer modelo.

* &amp;lbrack;USD&amp;rbrack;&amp;lbrack;Exportar&amp;rbrack; Adicionar formato de arquivo USD à exportação em malha

* &amp;lbrack;USD&amp;rbrack; Renomeie a predefinição de exportação “USD PBR Metal Roughness” existente para ser mais explícita

  O modelo de exportação de USD anteriormente conhecido como &#39;USD PBR Metal Roughness&#39; ainda é acessível por meio de texturas de exportação > Modelo de saída > USDz (Apple AR).

* &amp;presilha;Desenvolver presilha automaticamente&amp;rbrack; Adicionar orientação de bloqueio para embalagem

  Nova opção para configurações de abertura automática que permitem preservar a orientação de Ilhas UV existentes ao usar o recurso de embalagem. Ele pode ser acessado em Novo projeto > Opções de Contornar automaticamente > Orientação da Ilha UV.

* &amp;lbrack;Tamanho físico&amp;rbrack; Adicionar configuração para usar automaticamente Tamanho físico no efeito/camada de preenchimento

  Foi adicionada uma nova opção para alternar automaticamente para a escala de tamanho físico ao usar um material com tamanho físico incorporado. Ele pode ser ativado por projeto por meio de Novo projeto ou de Editar > Configuração do projeto > Tamanho físico > Alternar o dimensionamento da camada de preenchimento para Tamanho físico ao atribuir materiais.

* &amp;lbrack;Tamanho físico&amp;rbrack; Expor tamanho físico para Projeção UV

  O dimensionamento de tamanhos físicos agora está disponível para Projeção UV. Ele ativa o redimensionamento automático de um material com base no tamanho físico de uma malha. Pode ser selecionado por meio de Escala > Tamanho físico na janela Propriedades da camada de preenchimento ou do efeito.

* &amp;lbrack;Scripting&amp;rbrack;&amp;lbrack;Python&amp;rbrack; Permitir consultar a versão do aplicativo

* &amp;lbrack;Scripting&amp;rbrack;&amp;lbrack;JavaScript&amp;rbrack; Atualizar API para corresponder aos novos parâmetros de fça bake

* &amp;lbrack;Scripting&amp;rbrack;&amp;lbrack;Python&amp;rbrack; Fazendo bake módulo: editar parâmetros de fça bake

* &amp;lbrack;Scripting&amp;rbrack;&amp;lbrack;Python&amp;rbrack; Fazendo bake módulo: iniciar/cancelar fça bake

* &amp;lbrack;Scripting&amp;rbrack;&amp;lbrack;Python&amp;rbrack; Fazendo bake módulo: selecione o método de curvatura

* &amp;lbrack;Scripting&amp;rbrack;&amp;lbrack;Python&amp;rbrack; Fazendo bake módulo: seleção de baker/blocos uv

* &amp;lbrack;Scripting&amp;rbrack;&amp;lbrack;Python&amp;rbrack; módulo de Fça bake: sincronizar as configurações de baker em todos os Conjuntos de texturas

* &amp;lbrack;SVT&amp;rbrack; Ativar suporte a hardware esparso em GPUs AMD

  A aceleração de hardware para o sistema de texturas virtuais esparsas agora pode ser ativada com as GPUs da AMD. Essa configuração é ativada automaticamente nas preferências gerais.

* &amp;lbrack;Projeção&amp;rbrack; Renomear parâmetros de projeção cilíndrica

  O parâmetro “Cylinder Cap Culling” foi renomeado para “Backface Culling” para melhor representar sua ação. A dica de ferramenta associada foi ajustada de acordo.

* &amp;lbrack;Projeto&amp;rbrack; Salva a versão do aplicativo no projeto e recupera-a através de scripts

  Desde a versão 8.2, a versão do aplicativo agora é armazenada dentro do arquivo spp ao salvar. Este número de versão pode ser recuperado com a função last_saved_substance_painter_version() no módulo do projeto da API Python. Para projetos feitos antes de 8.2, o valor retornado será nulo.

* &amp;lbrack;Import&amp;brack; Melhorar tempo de importação geral de modelos 3D

  Melhoramos o tempo geral de importação das malhas. Por exemplo, reduzir o tempo de espera ao carregar malhas de alto polígono para fazer bake. Esta otimização aplica-se em particular ao carregamento de arquivos OBJ.

**Corrigido:**

* &amp;lbrack;Crash&amp;rbrack; Alterar canais no filtro com pilha específica

* &amp;lbrack;Mac&amp;rbrack;&amp;lbrack;M1&amp;rbrack; Falha ao criar uma camada de preenchimento e sair da pilha de camadas

  Esse problema pode ser corrigido atualizando para o Mac OS 13 (Ventura).

* &amp;lbrack;Scripting&amp;rbrack;&amp;lbrack;Python&amp;rbrack; Falha ao usar ui.add_dock_widget() com o tipo errado

* &amp;lbrack;Fazendo bake&amp;rbrack; Mensagem de erro incompleta no registro quando um faço bake falha

* &amp;lbrack;Fazendo bake&amp;rbrack; A memória não é liberada quando a faz bake é concluída

* &amp;lbrack;O cache de Textura do Engine&amp;rbrack; não é atualizado ao alterar a visibilidade do efeito

* &amp;lbrack;Exportar&amp;rbrack; Visualização 2D exportações aleatoriamente mapa uniforme

* &amp;lbrack;Projeto&amp;rbrack; Erro de alocação de memória ao salvar o projeto com malha grande

* &amp;lbrack;Viewport&amp;rbrack; TAA causa artefatos ao pintar em alguns casos

**Problemas Conhecidos:**

* &amp;lbrack;Gerenciamento de cores&amp;rbrack; As conversões do espaço de cores HDR com ACE no Linux produzem cores fixas
* &amp;lbrack;Pilha de camadas&amp;rbrack; Fonte de entrada não salva por camada

### 8.2.0

*(Lançado em: 06 de outubro de 2022*)Resumo: **Versão principal com novos painéis de integração (novo painel de boas-vindas e novo painel), exportação para SBSAR, efeitos para pasta, várias melhorias na qualidade de vida e correções de erros.**

**Adicionado:**

* &amp;lbrack;Integração&amp;rbrack; Painel de integração para acolher novos usuários

  Adicionada uma nova tela de boas-vindas quando novos usuários da CC abrem o Painter pela primeira vez.

* &amp;lbrack;Integração&amp;rbrack; Painel de novidades para aprimorar a capacidade de descoberta de novos recursos

  Adicionada uma nova tela Novidades que exibe os novos recursos principais. Ele é exibido automaticamente na primeira vez que o Painter é aberto após uma atualização importante e pode ser acessado novamente em Ajuda > Novidades.

* &amp;lbrack;Integração&amp;rbrack; Renomear antigo Bem-vindo à “Tela inicial”

  A tela de boas-vindas antiga foi renomeada para Tela inicial para evitar confusões com a nova tela de boas-vindas.

* &amp;lbrack;UI&amp;rbrack; Resolver problemas de dimensionamento para telas de DPI alto

  Adaptação aprimorada da interface do Painter em telas de alta definição com dimensionamento de exibição personalizado.

* &amp;lbrack;UI&amp;rbrack; Evitar mensagens de erro persistentes na interface

  As mensagens de erro de projetos anteriores agora são removidas da barra de status inferior.

* &amp;lbrack;UI&amp;rbrack; Menu de salvamento de retrabalho

  Opções adicionais de salvamento agora estão agrupadas em um submenu e algumas são renomeadas para fins de consistência.

* &amp;lbrack;UI&amp;rbrack; Salvar e exportar/compartilhar layouts de interface

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

* &amp;lbrack;Painel de ativos&amp;rbrack; “Fixar” de ativos favoritos para aparecerem sobre o painel de ativos

  Adição de uma nova opção de clicar com o botão direito em ativos da biblioteca que permite fixar-los como favoritos para a parte superior do painel. Você também pode exibir todos os seus ativos favoritos em Pesquisas salvas.

* &amp;lbrack;Painel Ativos&amp;rbrack; Excluir, recarregar e renomear ativos

  Adicionadas as opções do menu de contexto para excluir, recarregar e renomear ativos na biblioteca do usuário. Eles são excluídos diretamente do local da biblioteca no disco e recarregados do local original. Os ativos que fazem parte de um pacote como .abr ou .sbsar não podem ser editados individualmente.

* &amp;preto;Seleção de cores&amp;rbrack; Adicionar modos de mesclagem ao efeito Seleção de cores

* &amp;lbrack;Pilha de camadas&amp;rbrack; Adicionar modo de mesclagem e opacidade em filtros

* &amp;lbrack;Pilha de camadas&amp;rbrack; Permitir valores de divisão em blocos maiores que 128 para camada/efeitos de preenchimento

* &amp;lbrack;Pilha de camadas&amp;rbrack; Tampas de cilindro para projeção cilíndrica em camada/efeito de preenchimento

  A projeção cilíndrica nas propriedades da camada de preenchimento agora tem a opção de remover as tampas dos cilindros.

* &amp;lbrack;Log&amp;brack; Mostra uma mensagem de erro se as partes da malha estiverem em espaço negativo ao tentar criar um projeto de Bloco UV

  Adicionada uma mensagem de erro mais clara ao falhar ao criar um projeto de Bloco UV porque as partes UV são encontradas em espaços negativos.

* &amp;lbrack;Projeto&amp;rbrack; Indica a versão na mensagem de erro “dados muito recentes” ao abrir um projeto

  Ao abrir um projeto que é muito recente para o aplicativo, a mensagem de erro agora indicará a versão do projeto para facilitar a identificação da versão correta do aplicativo.

* &amp;lbrack;Viewport&amp;rbrack; Permitir a iluminação da malha por baixo

  Foi adicionado um novo parâmetro de Alinhamento de ambiente em Configurações de exibição > Câmera > Configurações de ambiente para alinhar a iluminação do mapa de ambiente à câmera quando definida como “Local”.

* &amp;lbrack;Visor&amp;rbrack; Visualizar R, G, B e Alpha no visor (modo de exibição solo)

  Em Configurações de exibição > Configurações do visor > Exibição de canal, há uma nova configuração de Canais de cores que permite exibir apenas o componente R, G, B ou Alpha de um canal quando estiver no modo de exibição única.

* &amp;lbrack;Sombreador&amp;rbrack; Permite definir canais do usuário como RGBA em sombreadores de camadas de material

  Ao definir a configuração dos canais do Conjunto de texturas dentro de um sombreador para camadas de material, agora é possível especificar o formato do canal para se desviar do valor padrão. Isso permite solicitar canais de usuário coloridos em vez de somente tons de cinza.

* &amp;lbrack;Export&amp;brack; Permitir exportação de texturas como SBSAR

  Ao exportar o textura pela janela Arquivo > Exportar Textura, o formato de arquivo SBSAR (Arquivo Substance) pode ser escolhido para reagrupá-los. O conteúdo do SBSAR é orientado pelo modelo de saída usado. O formato de arquivo SBSAR também pode ser definido nas predefinições de exportação. Ao usar configurações híbridas (SBSAR + outro formato), as texturas direcionadas a um SBSAR são agrupadas enquanto o restante é exportado junto com ele.

* &amp;lbrack;Export&amp;brack; Expor opção de 16 bits para o formato de arquivo EXR

  Ao exportar arquivos de textura EXR, agora é possível escolher 16f bits (meia Precisão decimal) ou 32f bits (Precisão decimal) na janela Exportar Textura (para configurações de exportação e predefinições de exportação). Projetos antigos e predefinições de exportação antigas terão o bit 16f como padrão para refletir o comportamento antigo.

* &amp;lbrack;Python&amp;rbrack; Adicionar evento para saber quando os Conjuntos de Texturas são modificados

  O novo “substance_painter.event.TextureStateEvent” permite saber quando um conjunto de texturas foi modificado por causa de um traçado de tinta, um novo canal adicionado ou um canal removido.

* &amp;lbrack;Python&amp;rbrack; Permite obter e definir recursos de Mapa de malha nas configurações do Conjunto de texturas

  Novas funções foram adicionadas ao módulo “substance_painter.project” para obter e definir recursos de mapas de malha. Essas funções podem ser usadas para atualizar os mapas de malha referenciados pelas configurações do Conjunto de texturas.

* &amp;Brack;Plug-ins&amp;rbrack; Remover opção para obter outros plug-ins JS

  Remoção da opção para obter plug-ins JavaScript, pois eles estavam hospedados no site de compartilhamento obsoleto.

* &amp;lbrack;Content&amp;rbrack; Adicionar novo modelo Roblox e exportar predefinição

  Um novo modelo de projeto e predefinição de exportação Roblox “Material Variant” e “Surface Appearance” foram adicionados para facilitar a exportação de texturas PBR para Roblox. O modelo pode ser acessado pela janela Arquivo > Novo projeto.

* Atualize o Substance Engine para a última versão (8.6.3)

* &amp;lbrack;Steam&amp;brack; Compilação otimizada para o chipset Apple Silicon (Apple M1 / M2)

**Corrigido:**

* Falha ao usar exr 16k

* &amp;lbrack;Crash&amp;rbrack; Ctrl Z Depois de excluir uma instância de sombreamento

* &amp;lbrack;Iray&amp;rbrack; IoR está bloqueada em 1 para alguns sombreadores

* &amp;lbrack;Win&amp;rbrack;&amp;lbrack;Fazendo bake&amp;rbrack; Alguns alto-polígonos falham ao carregar

* &amp;lbrack;Gerenciamento de cores&amp;rbrack; Nome do espaço de cores incorreto na interface do usuário com filtros

* &amp;lbrack;Python&amp;rbrack; Os objetos de recursos retornados pela função de importação não têm um tipo

  Ao importar um pacote Substance em Python, a função estava retornando o pacote em vez de seu(s) gráfico(s). O módulo de recursos agora fornece funções e parâmetros para recuperar o(s) gráfico(s) de um pacote de Substance.

**Problemas Conhecidos:**

* &amp;lbrack;Gerenciamento de cores&amp;rbrack; As conversões do espaço de cores HDR com ACE no Linux produzem cores fixas
* &amp;lbrack;Pilha de camadas&amp;rbrack; Fonte de entrada não salva por camada
* &amp;preto;Pintura&amp;rbrack; A suavização temporal causa artefatos ao pintar em alguns casos
* &amp;lbrack;Exportar&amp;rbrack; Visualização 2D exportações aleatoriamente mapa uniforme

### 8.1.3

*(Lançado: 25 de agosto de 2022*)Resumo: **Versão de correção de erro secundária**

**Adicionado:**

* Atualização para o Iray SDK 1.6

**Corrigido:**

* &amp;lbrack;Sombreador&amp;rbrack; Falha com sombreador antigo com defeito
* &amp;lbrack;Camada de material&amp;rbrack; Os materiais podem desaparecer ao reabrir um projeto

**Problemas Conhecidos:**

* &amp;lbrack;Gerenciamento de cores&amp;rbrack; As conversões do espaço de cores HDR com ACE no Linux produzem cores fixas
* &amp;lbrack;Pilha de camadas&amp;rbrack; Fonte de entrada não salva por camada
* &amp;lbrack;Crash&amp;rbrack; Ctrl Z Depois de excluir uma instância de sombreamento
* &amp;lbrack;Iray&amp;rbrack; IoR está bloqueada em 1 para alguns sombreadores

### 8.1.2

*(Lançado em: 19 de julho de 2022*)Resumo: **Versão de correção de erro secundária**

**Adicionado:**

* &amp;lbrack;Auto Unwrap&amp;rbrack; Nova opção “Otimizar para malhas orgânicas” para selecionar o algoritmo de segmentação
* &amp;lbrack;Tamanho físico&amp;rbrack; Expor opções de unidade em Novo Projeto e Configuração de Projeto
* &amp;lbrack;Gerenciamento de cores&amp;rbrack; Usar a tela do monitor por padrão ao usar ACE
* &amp;lbrack;Gerenciamento de cores&amp;rbrack;&amp;lbrack;Python&amp;rbrack; Leve em consideração o arquivo de predefinição ACE env-var ao criar o projeto
* &amp;lbrack;Gerenciamento de cores&amp;rbrack; Redefinir configurações de Gerenciamento de cores na janela Novo projeto quando a configuração mudar
* &amp;lbrack;Gerenciamento de cores&amp;rbrack; Desativar acesso às configurações de OCIO quando env-var estiver presente
* &amp;lbrack;Gerenciamento de cores&amp;rbrack; Atualizar com segurança as configurações de ACE quando um parâmetro não existir mais
* Atualize o Substance Engine para a versão 8.6.0
* &amp;lbrack;Export&amp;brack; Adicionar nova predefinição de exportação de GLTF com suporte para Deslocamento
* &amp;lbrack;Scripting&amp;rbrack;&amp;lbrack;Python&amp;rbrack; Recuperar informações de recursos (incluindo metadados personalizados)
* &amp;lbrack;Scripting&amp;rbrack;&amp;lbrack;Python&amp;rbrack; Adicionar função à lista de consulta de nomes de malha por Conjunto de textura
* &amp;preset;Content&amp;brack; Adicionar novo modelo do Blender e exportar predefinição

**Corrigido:**

* &amp;lbrack;MacOS&amp;rbrack; Falha ao iniciar o Iray em alguns casos
* &amp;lbrack;Miniaturas&amp;rbrack; Miniaturas de prateleira não carregam corretamente
* Vários canais UV são ignorados
* &amp;lbrack;Auto Unwrap&amp;rbrack; Cálculo desnecessário ao dividir ilhas longas
* &amp;lbrack;Auto Unwrap&amp;rbrack; Opção para evitar ilhas alongadas não levadas em consideração
* &amp;lbrack;Desempacotar Automaticamente&amp;rbrack; Perda de dados extras (cores de vértice) ao recompactar UVs
* &amp;lbrack;UI&amp;rbrack; Barra de rolagem horizontal na janela de propriedades quando o Gerenciamento de Cores está habilitado
* &amp;lbrack;Gerenciamento de cores&amp;rbrack; As configurações de OCIO não têm a função substance_3d_painter_standard_srgb
* &amp;lbrack;Generator&amp;rbrack; Uso incorreto de dados do usuário “desabilitado”
* &amp;lbrack;Gerenciamento de cores&amp;rbrack; O menu suspenso Espaço de cores “Não compatível” não deve ser clicável
* &amp;lbrack;Gerenciamento de cores&amp;rbrack;&amp;lbrack;Sombreador&amp;rbrack; sRGB override define não funciona mais
* &amp;lbrack;Generator&amp;rbrack; Uso incorreto de dados do usuário “disable”
* &amp;lbrack;Pilha de camadas&amp;rbrack; Visualizações quebradas com projetos do Bloco UV
* A documentação da API do &amp;lbrack;Sombreador&amp;rbrack; não está totalmente atualizada com o Dobra normal
* &amp;lbrack;Export&amp;brack;&amp;lbrack;Interoperabilidade&amp;rbrack; Não é possível enviar para o Stager com caracteres especiais
* &amp;lbrack;Content&amp;brack; Algumas miniaturas de predefinições de pincel estão vazias ou muito escuras

**Problemas Conhecidos:**

* &amp;lbrack;Gerenciamento de cores&amp;rbrack; As conversões do espaço de cores HDR com ACE no Linux produzem cores fixas
* &amp;lbrack;Pilha de camadas&amp;rbrack; A fonte de entrada não é salva por camada
* &amp;lbrack;Crash&amp;rbrack; Ctrl Z Depois de excluir uma instância de sombreamento
* &amp;lbrack;Iray&amp;rbrack; IoR está bloqueada em 1 para alguns sombreadores
* &amp;lbrack;Sombreador&amp;rbrack; Falha com sombreador antigo com defeito

### 8.1.1

*(Lançado: 28 de junho de 2022*)Resumo: **Hotfix de versão secundária**

**Adicionado:**

* &amp;lbrack;Pilha de camadas&amp;rbrack; Clicar com a tecla Alt pressionada na máscara não desmarca mais os efeitos

**Corrigido:**

* &amp;lbrack;Crash&amp;rbrack; Abrindo projeto antigo salvo no modo de visualização individual
* &amp;lbrack;Crash&amp;brack; Excluir um Gerador nas propriedades
* &amp;lbrack;Configurações do conjunto de texturas&amp;rbrack; A mistura Normal/Oclusão de ambiente e o height para métodos normais estão quebrados
* &amp;brack;Export&amp;brack; Exportar texturas usando o preenchimento de difusão renderiza mapas em preto

**Problemas Conhecidos:**

* &amp;lbrack;MacOS&amp;rbrack; Falha ao iniciar o Iray no Monterey
* &amp;preto;Visualizar miniatura&amp;rbrack; miniaturas simplificadas não são atualizadas quando uma âncora é usada
* &amp;lbrack;Gerenciamento de cores&amp;rbrack; As conversões do espaço de cores HDR com ACE no Linux produzem cores fixas

### 8.1.0

*(Lançado em: 07 de junho de 2022*)Resumo: **Versão principal com suporte ICC, dimensionamento de material com base em dados de tamanho físico, novos baker, melhorias no conta-gotas de cores e uma variedade de conteúdos adicionais**

**Adicionado:**

* &amp;lbrack;Gerenciamento de cores&amp;rbrack; Adicionar suporte para perfis ICC com Adobe Color Engine (ACE)
* &amp;lbrack;Gerenciamento de cores&amp;rbrack; Adicionar suporte para “Adobe 98 RGB” como espaço de cores de trabalho para ICC
* &amp;lbrack;Color Management&amp;rbrack; Permite definir configurações ACE/ICC através de um arquivo de configuração
* &amp;lbrack;Gerenciamento de cores&amp;rbrack; Permitir a entrada de valores de cor lineares no Seletor de Cores com o modo Legado
* &amp;lbrack;Gerenciamento de cores&amp;rbrack; Permite especificar o perfil de cores usado para escolher cores fora da interface
* &amp;lbrack;Gerenciamento de cores&amp;rbrack; Lembrar o último valor de exibição escolhido no visor
* &amp;lbrack;Gerenciamento de cores&amp;rbrack;&amp;lbrack;Substance&amp;rbrack; Faça com que os geradores/filtros funcionem corretamente com o Gerenciamento de cores
* &amp;lbrack;Gerenciamento de cores&amp;rbrack;&amp;lbrack;Substance&amp;rbrack; Adicionar novas palavras-chave de substituição colorspace $working e $standardsrgb
* &amp;lbrack;Tamanho físico&amp;rbrack;&amp;lbrack;Motor&amp;rbrack; Extrair informações de tamanho físico da malha
* &amp;lbrack;Tamanho físico&amp;rbrack;&amp;lbrack;Computação de Tamanho físico do motor&amp;rbrack;
* &amp;lbrack;Tamanho físico&amp;rbrack; Expor opções para usar tamanho físico na interface
* &amp;lbrack;Tamanho físico&amp;rbrack; Adicionar auxiliares visuais no visor
* &amp;lbrack;Fazendo bake&amp;rbrack; Adicionar baker de Height
* &amp;lbrack;Fazendo bake&amp;rbrack; Adicionar baker do Dobra normal
* &amp;preto;Fazendo bake&amp;rbrack; Adicionar baker de Opacidade
* &amp;preto;Conta-gotas&amp;rbrack; Nova visualização de conta-gotas de cor ao lado do mouse e cor gerenciada
* &amp;lbrack;Conta-gotas&amp;rbrack; O painel do seletor de cores reaparece em sua última posição quando reaberto
* &amp;lbrack;Conta-gotas&amp;rbrack; Um novo ícone para o Seletor de materiais
* &amp;lbrack;Conta-gotas&amp;rbrack; Cor gerencia a visualização do canal do seletor de cores
* &amp;preto;Conta-gotas&amp;rbrack; Adicionar a funcionalidade de clicar para selecionar ao conta-gotas
* &amp;lbrack;Conta-gotas&amp;rbrack; O seletor de materiais não ativa mais os canais não ativos
* &amp;preto;Conta-gotas&amp;rbrack; Permitir o uso do conta-gotas com um atalho
* &amp;preto;Conta-gotas&amp;rbrack; O conta-gotas seleciona o canal relevante, quando aplicável
* &amp;preto;Conta-gotas&amp;rbrack; Entrar no modo de seleção de cores desativa todos os atalhos
* &amp;preto;Conta-gotas&amp;rbrack; Remove a seleção automática do campo hexadecimal
* &amp;preto;Conta-gotas&amp;rbrack; Não feche o painel ao usar o seletor de material
* &amp;lbrack;Conta-gotas&amp;rbrack; Novo estado desativado quando o canal não está disponível para seleção
* &amp;lbrack;Export&amp;brack; Adicionar atributo tangente à exportação de glTF
* Atualize o Substance Engine para v8.4
* Atualizar a quebra automática para 0. 9. 0
* Atualize para Qt 5.15.8
* Atualização para o Python 3.9
* &amp;lbrack;Sombreador&amp;rbrack; Adicionar suporte para o Dobra normal sombreamento
* &amp;lbrack;MacOS&amp;rbrack; Suporte ao 3DConnection SpaceMouse
* &amp;lbrack;Python&amp;rbrack; Documenta a versão do Python usada na API
* &amp;lbrack;Content&amp;rbrack; Adicionar 6 novos ruídos 3D com 105 predefinições
* &amp;lbrack;Content&amp;rbrack; 20 novos mapas de desgaste e 2 padrões de dobras de pano
* &amp;lbrack;Content&amp;rbrack; Atualizar predefinição de exportação “Mapas de malha” para usar novos baker
* &amp;lbrack;Content&amp;brack; O filtro de Inclinação e distorção de desfoque depende da resolução do conjunto de texturas
* &amp;lbrack;Content&amp;rbrack; Atualiza projetos de amostra para usar os 3 novos baker

**Corrigido:**

* &amp;lbrack;glTF&amp;rbrack; Não é possível abrir glTF com caractere especial
* &amp;lbrack;Engine&amp;rbrack; Artefatos com anisotropia e SVT desativados
* Os Materiais inteligentes &amp;lbrack;MacOS&amp;rbrack;&amp;lbrack;M1&amp;rbrack; não são exibidos corretamente
* &amp;lbrack;Processamento de malha&amp;rbrack; Não é possível importar malhas do Modeler
* &amp;lbrack;UI&amp;rbrack; Barra de rolagem horizontal na nova janela do projeto com o Gerenciamento de cores ativado
* &amp;lbrack;Gerenciamento de cores&amp;rbrack; Valor do espaço de trabalho ausente no seletor de cores com algumas configurações de OCIO
* &amp;lbrack;Gerenciamento de cores&amp;rbrack; A visualização do pincel no visor não tem gerenciamento de cores
* A Tabela Dinâmica do &amp;SpaceMouse&amp;rbrack; não é atualizada imediatamente com a alteração de foco e às vezes fora do modelo
* &amp;lbrack;Export&amp;rbrack;&amp;lbrack;USD&amp;rbrack; Os arquivos USD exportados têm uma estrutura incorreta
* &amp;lbrack;USD&amp;rbrack; problema de Oclusão de ambiente ao exportar
* &amp;lbrack;Content&amp;rbrack; Atualiza a malha da miniatura para corresponder ao projeto de amostra da Esfera de visualização

**Problemas Conhecidos:**

* Exportar texturas usando o preenchimento de difusão renderiza mapas em preto
* A mistura normal/Oclusão de ambiente está quebrada
* &amp;lbrack;MacOS&amp;rbrack; Falha ao iniciar o Iray em alguns casos raros
* &amp;preto;Visualizar miniatura&amp;rbrack; miniaturas simplificadas não são atualizadas quando uma âncora é usada
* &amp;lbrack;Gerenciamento de cores&amp;rbrack; As conversões do espaço de cores HDR com ACE no Linux produzem cores fixas

## Versão 7

### 7.4.3

*(Lançado em: 11 de abril de 2022*)Resumo: **Correção de erro com suporte para 3Dconnection SpaceMouse em 2D Viewport**

**Adicionado:**

* &amp;lbrack;SpaceMouse&amp;rbrack; Suporte a 3DConnection SpaceMouse em Visor 2D

**Corrigido:**

* &amp;preto;Seletor de cores&amp;rbrack; Não é possível gravar em campo hexadecimal
* &amp;lbrack;Gerenciamento de cores&amp;rbrack; Os recursos usados no modo de projeção não são gerenciados por cores na sobreposição
* &amp;lbrack;Gerenciamento de cores&amp;rbrack; Erros não são relatados no registro
* &amp;lbrack;SpaceMouse&amp;rbrack; Remove uma mensagem de erro genérica se o usuário não tiver um SpaceMouse
* &amp;lbrack;SpaceMouse&amp;rbrack; Ao carregar um projeto, o ponto dinâmico fica sempre oculto
* &amp;lbrack;Baker&amp;rbrack; A configuração de “Média normal” não tem efeito em projetos de Bloco UV
* &amp;lbrack;Bloco UV&amp;rbrack; As sobreposições de blocos uv inativos desaparecem ao recarregar a malha com blocos diferentes
* &amp;lbrack;Scripting&amp;rbrack;&amp;lbrack;Python&amp;rbrack; O script remoto está danificado
* &amp;lbrack;Scripting&amp;rbrack;&amp;lbrack;Python&amp;rbrack; Vários canais não podem ser consultados pela API e isso gera um erro
* &amp;lbrack;Scripting&amp;rbrack;&amp;lbrack;Python&amp;rbrack; Falha ao usar o evento ProjectEditionEntered
* &amp;lbrack;Scripting&amp;rbrack;&amp;lbrack;Python&amp;rbrack; Falha ao chamar get_ative_stack()

**Problemas Conhecidos:**

* Espaço de conexão 3Dsem suporte para mouse no MacOS
* &amp;lbrack;UI&amp;rbrack; Barra de rolagem horizontal com gerenciamento de cores sendo exibida em alguns casos na janela do novo projeto
* &amp;lbrack;Os Materiais inteligentes do Mac M1&amp;rbrack; não são exibidos corretamente

### 7.4.2

*(Lançado: 08 de março de 2022*)Resumo: **Correção de erro com suporte a 3Dconnection SpaceMouse e melhorias no gerenciamento de cores (OCIO)**

**Adicionado:**

* &amp;lbrack;SpaceMouse&amp;rbrack;&amp;lbrack;Windows&amp;rbrack; Suporte ao SpaceMouse 3Dconnection na Janela de Visualização 3D para navegação
* &amp;lbrack;SpaceMouse&amp;rbrack;&amp;lbrack;Windows&amp;rbrack; Atalhos/teclas básicos para modelos Pro e Enterprise SpaceMouse no Visor 3D
* &amp;lbrack;SpaceMouse&amp;rbrack;&amp;lbrack;Windows&amp;rbrack; Ícone do centro de rotação dedicado no Visor 3D
* &amp;lbrack;Gerenciamento de cores&amp;rbrack; Usar funções da configuração do OCIO para alterar as configurações padrão
* &amp;lbrack;Gerenciamento de cores&amp;rbrack; Gerenciamento de cores Gerencia a janela de propriedades dos widgets de cores
* &amp;lbrack;Gerenciamento de cores&amp;rbrack; Cor gerencia a janela de propriedades para visualização do material
* &amp;preto;Gerenciamento de cores&amp;rbrack; Cor gerenciar amostras no seletor de cores
* &amp;lbrack;Gerenciamento de cores&amp;rbrack; Adicionar uma configuração para definir o espaço de cores sRGB padrão
* &amp;lbrack;Gerenciamento de cores&amp;rbrack; Adicionar o espaço de cor sRGB padrão da configuração OCIO na lista de seletores de exibição do seletor de cores
* &amp;preto;Gerenciamento de cores&amp;rbrack; Melhorias para o menu de substituição do espaço de cores
* &amp;lbrack;Gerenciamento de cores&amp;rbrack; Permitir substituição do espaço de cores do mapa de ambiente nas Configurações de exibição
* &amp;preto;Gerenciamento de cores&amp;rbrack; Desenhar gradientes do seletor de cores com base na exibição atual
* &amp;lbrack;Gerenciamento de cores&amp;rbrack; Restringir valores HDR por padrão no editor de cores
* &amp;lbrack;Gerenciamento de cores&amp;rbrack; Usar passagem (sem espaço de cor) para filtros no modo Legado
* &amp;lbrack;Gerenciamento de cores&amp;rbrack; Limitar exibição de gradientes no editor de cores para corresponder ao intervalo do &amp;lbrack;0-1&amp;rbrack;
* &amp;lbrack;Gerenciamento de cores&amp;rbrack; Ocultar seletor de exibição no seletor de cores no modo Legado
* &amp;preto;Gerenciamento de cores&amp;rbrack; Fazer com que o seletor de cores tenha um campo hexadecimal sempre no espaço de cores sRGB
* &amp;lbrack;Gerenciamento de cores&amp;rbrack; Desativar menu suspenso Exibição do seletor de cores para canais de dados
* &amp;lbrack;Otimization&amp;rbrack; A grade de distorção recalcula somente os blocos UV cobertos
* &amp;lbrack;Export&amp;rbrack; Permitir a exportação de projetos do Bloco UV para Sketchfab, USD e glTF
* &amp;lbrack;Scripting&amp;rbrack;&amp;lbrack;Python&amp;rbrack; Permitir alteração da função de mapeamento de tom

**Corrigido:**

* &amp;lbrack;Sketchfab&amp;rbrack; A atualização do modelo existente acaba criando um novo modelo
* &amp;lbrack;Sketchfab&amp;rbrack; Falha ao procurar modelo atualizado anteriormente
* Falha ao exportar para USD
* Falha ao criar uma nova instância de sombreamento em Máscara de geometria ou quando a geometria está oculta
* &amp;Lbrack;Janela Importar Ativo&amp;rbrack; Falha ao alterar o tipo de recursos importados
* Mapas de malha normal são invertidos quando usados em pilha de camadas
* &amp;lbrack;Substance&amp;rbrack; O modo de mesclagem de dados do usuário não é levado em consideração
* &amp;preto;Gerenciamento de cores&amp;rbrack; Bitmaps com espaço de cor no nome do arquivo são importados como sequências de Bloco UV
* &amp;lbrack;Gerenciamento de cores&amp;rbrack; As saídas gerenciadas por cores do gráfico de Substance estão no espaço de cores incorreto
* A ferramenta Preenchimento de polígono do &amp;preto;Gerenciamento de cores&amp;rbrack; exibe a cor errada
* &amp;lbrack;Gerenciamento de cores&amp;rbrack; O mapeador de tons ACE é aplicado aos canais no modo solo
* &amp;lbrack;Gerenciamento de cores&amp;rbrack; A visualização da ferramenta de iluminação da esfera não é gerenciada por cores
* &amp;lbrack;Gerenciamento de cores&amp;rbrack;&amp;lbrack;Exportar&amp;rbrack; Mapas convertidos aplica uma conversão incorreta
* &amp;lbrack;Scripting&amp;rbrack;&amp;lbrack;Python&amp;rbrack;&amp;lbrack;Gerenciamento de cores&amp;rbrack; Os projetos criados com o modelo e a variável de ambiente OCIO estão no modo Legado
* &amp;lbrack;Scripting&amp;rbrack;&amp;lbrack;Python&amp;rbrack; Não é possível usar a função de avaliação do JavaScript na inicialização
* &amp;lbrack;Oferta de Adobe 3D&amp;rbrack; Não é possível iniciar o Painter ao usar configurações regionais com idiomas não suportados por padrão

**Problemas Conhecidos:**

* Espaço de conexão 3Dsem suporte para mouse no MacOS
* &amp;lbrack;UI&amp;rbrack; Barra de rolagem horizontal com gerenciamento de cores sendo exibida em alguns casos na janela do novo projeto
* &amp;lbrack;Baker&amp;rbrack; A configuração de “Média normal” não tem efeito em projetos de Bloco UV
* &amp;lbrack;Os Materiais inteligentes do Mac M1&amp;rbrack; não são exibidos corretamente
* &amp;lbrack;Gerenciamento de cores&amp;rbrack; Os recursos usados no modo de projeção não são gerenciados por cores na sobreposição
* &amp;preto;Seletor de cores&amp;rbrack; Não é possível gravar em campo hexadecimal

### 7.4.1

*(Lançado: 14 de dezembro de 2021*)Resumo: **Correção de erros com melhorias no gerenciamento de cores**

**Adicionado:**

* &amp;preto;Gerenciamento de cores&amp;rbrack; Usar função de dados nos nomes de arquivos exportados
* &amp;preto;Gerenciamento de cores&amp;rbrack; Expande a seção Gerenciamento de cores, por padrão, quando o OCIO for selecionado nas novas janelas de configurações do projeto e do projeto
* &amp;lbrack;Gerenciamento de cores&amp;rbrack; Adicionar mapeador de tons ACE no modo legado
* &amp;preto;Gerenciamento de cores&amp;rbrack; Ajustar as definições de configuração padrão
* &amp;lbrack;Gerenciamento de cores&amp;rbrack;&amp;lbrack;Exportar&amp;rbrack; Preencher $colorSpace nos nomes de arquivos para canais de dados
* &amp;prec;Exportar &amp;prec; Exportar projeto de Bloco UV para o Stager
* &amp;lbrack;Interoperabilidade&amp;rbrack; Não disponível para as edições Steam e Substance
* &amp;lbrack;Interoperabilidade&amp;rbrack; Permitir o envio de um projeto de Bloco UV para o Stager

**Corrigido:**

* &amp;lbrack;MacOS&amp;rbrack;&amp;lbrack;Crash&amp;rbrack; o Painter não começa com o Catalina
* &amp;lbrack;Gerenciamento de cores&amp;rbrack;&amp;lbrack;Falha&amp;rbrack; Falha aleatória ao reproduzir o gerenciamento de cores/tipo de dados no canal do usuário
* &amp;preto;Gerenciamento de cores&amp;rbrack; Recursos usados como tons de cinza no novo menu espaço de cores de exibição de máscara
* &amp;lbrack;Gerenciamento de cores&amp;rbrack; O canal do usuário é mais escuro na viewport no modo legado + visualização individual
* &amp;lbrack;Gerenciamento de cores&amp;rbrack; O mapa de ambiente é sempre linear quando usado no iRay
* &amp;lbrack;Gerenciamento de cores&amp;rbrack; O seletor de cores não seleciona o valor correto para o canal de dados no modo herdado
* &amp;lbrack;Gerenciamento de cores&amp;rbrack; O seletor de cores está quebrado dentro de um Substance no modo herdado
* &amp;lbrack;Gerenciamento de cores&amp;rbrack; Alternar entre exibições de canal individual na viewport não é exibido com o espaço de cor correto ao usar o menu suspenso
* &amp;lbrack;Gerenciamento de cores&amp;rbrack; Exportar aplica a conversão incorreta em canais de usuário com gerenciamento de cores no modo herdado
* Os traçados feitos na máscara de exibição individual não são exibidos ao voltar para a exibição de material
* &amp;preto;Exportar&amp;rbrack; Mapas convertidos não são exportados como canais com gerenciamento de cores
* &amp;lbrack;Textura Set&amp;rbrack; A dica de ferramenta com o nome original está ausente em canais de usuário renomeados
* &amp;lbrack;Steam&amp;brack; Arquivos ausentes ao verificar a integridade do arquivo com o Steam

**Problemas Conhecidos:**

* &amp;lbrack;Os Materiais inteligentes do Mac M1&amp;rbrack; não são exibidos corretamente

### 7.4.0

*(Lançado: 24 De novembro De 2021*)Resumo: **Versão Principal. Introdução da 1ª versão de gerenciamento de cores, desencaixe da exibição 2D ou 3D, nova opção de desencapsulamento automático UV para evitar ilhas alongadas, chame funções JavaScript da API Python e novo conteúdo**

**Adicionado:**

* &amp;lbrack;Gerenciamento de cores&amp;rbrack; Suporte ao gerenciamento de cores OpenColorIO versão 2
* &amp;preto;Gerenciamento de cores&amp;rbrack; Adicionar configurações de gerenciamento de cores às configurações do projeto
* &amp;lbrack;Gerenciamento de cores&amp;rbrack; Janela de aviso sobre as alterações de configuração do Gerenciamento de cores ao abrir um projeto
* &amp;lbrack;Gerenciamento de cores&amp;rbrack; Exibir uma mensagem de erro se um arquivo de configuração OCIO inválido for selecionado
* &amp;lbrack;Gerenciamento de cores&amp;rbrack; Permitir substituir a configuração pela variável de ambiente OCIO
* &amp;lbrack;Gerenciamento de cores&amp;rbrack; Várias configurações de OCIO integradas por padrão com o aplicativo
* &amp;preto;Gerenciamento de cores&amp;rbrack; Extrair o nome do espaço de cores do nome de arquivo bitmap importado
* &amp;lbrack;Color Management&amp;brack; Permite substituir o espaço de cor por um espaço de cor da configuração na janela Propriedades
* &amp;preto;Gerenciamento de cores&amp;rbrack; Adicionar opções de gerenciamento de cores nas Configurações do conjunto de texturas
* &amp;lbrack;Gerenciamento de cores&amp;rbrack;&amp;lbrack;Visor&amp;rbrack; Permitir gerenciamento de cores de exibições 2D e 3D separadamente
* &amp;preto;Gerenciamento de cores&amp;rbrack; Carrega e converte o mapa de ambiente para o espaço de cores de trabalho
* &amp;preto;Gerenciamento de cores&amp;rbrack; Ajustar seletor e editor de cores com o espaço de cores atual
* &amp;lbrack;Color Management&amp;rbrack; Permite selecionar o espaço de cores do transformo de exibição na viewport com um novo menu suspenso
* &amp;lbrack;Gerenciamento de cores&amp;rbrack; Aplicar transformo de exibição com resultados de renderização de matriz
* &amp;preto;Gerenciamento de cores&amp;rbrack; Exportar texturas com espaços de cores diferentes
* &amp;lbrack;Gerenciamento de cores&amp;rbrack;&amp;lbrack;Python&amp;rbrack; Aplicar configurações de gerenciamento de cores da variável de ambiente (OCIO) a novos projetos
* &amp;lbrack;Visor&amp;rbrack; Permitir desencaixar o visor 2D ou 3D
* &amp;lbrack;Auto Unwrap&amp;rbrack; Nova opção para evitar ilhas alongadas
* &amp;lbrack;Script Python&amp;rbrack; Chamar funções JavaScript a partir da API Python
* &amp;preto;Janela Novo projeto&amp;rbrack; Torna a seção de mapas importada flexível
* &amp;lbrack;Projeção&amp;rbrack;&amp;lbrack;Distorcer&amp;rbrack; Permite ocultar normais como uma opção nas configurações de Distorção
* &amp;lbrack;Content&amp;rbrack; 11 novos mapas de desgaste
* &amp;lbrack;Content&amp;brack; 8 novas predefinições de ferramenta (zíper, apertar fio, brilho)
* &amp;lbrack;Content&amp;brack; 8 novos materiais (cicatriz, bolso, ...)
* &amp;lbrack;Content&amp;rbrack; 1 novo gerador (inflar deformação)

**Problemas Conhecidos:**

* &amp;lbrack;Os Materiais inteligentes do Mac M1&amp;rbrack; não são exibidos corretamente
* &amp;lbrack;Gerenciamento de cores&amp;rbrack;&amp;lbrack;Falha&amp;rbrack; Falha aleatória ao reproduzir o gerenciamento de cores/tipo de dados no canal do usuário
* &amp;lbrack;Gerenciamento de cores&amp;rbrack; O seletor de cores não seleciona o valor correto para o canal de dados no modo herdado
* &amp;lbrack;Gerenciamento de cores&amp;rbrack;&amp;lbrack;Iray&amp;rbrack; Salvar a renderização em EXR ou TIFF enquanto o Gerenciamento de cores está ativado na janela de visualização sempre salvará em formato linear
* &amp;preto;Gerenciamento de cores&amp;rbrack; Os recursos usados como tons de cinza na máscara exibem o menu Espaço de cor errado
* &amp;lbrack;Gerenciamento de cores&amp;rbrack;&amp;lbrack;Iray&amp;rbrack; O mapa de ambiente é sempre linear quando usado em Iray
* &amp;lbrack;Gerenciamento de cores&amp;rbrack;&amp;lbrack;Exportar&amp;rbrack; Mapas convertidos não são exportados como canais gerenciados por cores
* &amp;lbrack;Gerenciamento de cores&amp;rbrack;&amp;lbrack;Exportar&amp;rbrack; ignora se o canal do usuário tem gerenciamento de cores ou não com o modo legado

### 7.3.1

*(Lançado: 24 De novembro De 2021*)Resumo: **Correção De Erros**

**Adicionado:**

* &amp;lbrack;Projeção&amp;rbrack; O dimensionamento deve funcionar somente no Espaço do objeto

**Corrigido:**

* &amp;lbrack;O Mac M1&amp;rbrack; Camadas de material não está funcionando
* &amp;lbrack;Mac M1&amp;rbrack;&amp;lbrack;Projeção&amp;rbrack; Warp não funciona
* Os microdetalhes não são exibidos corretamente
* &amp;lbrack;Projeção&amp;rbrack;&amp;lbrack;Falha&amp;rbrack; Alternando para o modo de distorção com uma camada criada com uma versão anterior
* &amp;lbrack;Projeção&amp;rbrack;&amp;lbrack;Distorcer&amp;rbrack; não funciona quando a transformação está definida para o espaço global
* &amp;lbrack;Projection&amp;rbrack;&amp;lbrack;Warp&amp;rbrack; Split option permanece selecionada após a divisão ser feita
* &amp;lbrack;Projeção&amp;rbrack;&amp;lbrack;UV&amp;rbrack; O ponto dinâmico é redefinido ao inverter a projeção
* &amp;lbrack;Filtro&amp;rbrack; Faço bake O ambiente de iluminação está mudando ao recarregar ou alterar um parâmetro
* &amp;lbrack;Interoperabilidade&amp;rbrack; Não disponível para as edições Steam e Substance
* &amp;lbrack;Interoperabilidade&amp;rbrack; O botão “Procurar ativos 3D no Marketplace” deve sempre abrir o CCD na guia Stock e Marketplace 3D

**Problemas Conhecidos:**

* &amp;lbrack;Os Materiais inteligentes do Mac M1&amp;rbrack; não são exibidos corretamente

### 7.3.0

*(Lançado: 13 De outubro De 2021*)Resumo: **Versão Principal. Contém uma nova projeção de distorção 3D, uma nova projeção cilíndrica, melhorias no seletor de cores, novas funções na API Python e correções de erros**

**Adicionado:**

* &amp;lbrack;Projeção&amp;rbrack;&amp;lbrack;Distorcer&amp;rbrack; Expor distorção 3D como um novo modo de projeção
* &amp;lbrack;Projeção&amp;rbrack;&amp;lbrack;Distorcer&amp;rbrack; Permitir modo de decalque para Alpha, Texturas e Procedimentos com arrastar e soltar no visor
* &amp;lbrack;Projeção&amp;rbrack;&amp;lbrack;Distorcer&amp;rbrack; Usar distorcer projeção com atalho de decalque (ALT)
* &amp;lbrack;Projeção&amp;rbrack;&amp;lbrack;Distorcer&amp;rbrack;&amp;lbrack;Barra de ferramentas&amp;rbrack; Transformar distorção como um todo ou por vértices
* &amp;lbrack;Projeção&amp;rbrack;&amp;lbrack;Distorcer&amp;rbrack;&amp;lbrack;Barra de ferramentas&amp;rbrack; Adicionar pontos de grade com distorção dividida nas opções transversal, horizontal ou vertical
* &amp;lbrack;Projeção&amp;rbrack;&amp;lbrack;Distorcer&amp;rbrack;&amp;lbrack;Barra de ferramentas&amp;rbrack; Menu dedicado para ações de redefinição
* &amp;lbrack;Projeção&amp;rbrack;&amp;lbrack;Distorcer&amp;rbrack;&amp;lbrack;Barra de ferramentas&amp;rbrack; Opção para ajustar automaticamente tangentes ao mover pontos
* &amp;lbrack;Projeção&amp;rbrack;&amp;lbrack;Distorção&amp;rbrack;&amp;lbrack;Barra de ferramentas&amp;rbrack; Menu dedicado para edição de grade (tamanho, redefinição, cor e tamanho da alça)
* &amp;lbrack;Projeção&amp;rbrack;&amp;lbrack;Distorção&amp;rbrack; Novo atalho de teclado para alternar o modo de edição de distorção de vértices inteiros (SHIFT+V)
* &amp;lbrack;Projeção&amp;rbrack;&amp;lbrack;Distorcer&amp;rbrack; O clique+Ctrl permite alternar entre a ferramenta de superfície e outras ferramentas
* &amp;lbrack;Projeção&amp;rbrack;&amp;lbrack;Cilíndrico&amp;rbrack; Expor o modo de projeção cilíndrica
* &amp;lbrack;Projeção&amp;rbrack;&amp;lbrack;Barra de ferramentas&amp;rbrack; Configurações do manipulador de grupos (tamanho, etapas da grade, etapas do ângulo)
* &amp;preto;Seletor de cores&amp;rbrack; Nova interface do seletor de cores
* &amp;preto;Seletor de cores&amp;rbrack; Usar valores sRGB nos widgets do seletor de cores
* &amp;preto;Seletor de cores&amp;rbrack; Permite salvar e excluir amostras de cores
* &amp;preto;Seletor de cores&amp;rbrack; Conta-gotas acessível de cor e slots normais
* &amp;lbrack;Seletor de cores&amp;rbrack; Permite editar a cor dinâmica entre 0 e 255 valores
* &amp;preto;Seletor de cores&amp;rbrack; Tornar o estado HSV/RGB comum no aplicativo
* &amp;lbrack;Seletor de Cores&amp;rbrack; A janela do Seletor de Cores é semipersistente
* &amp;preto;Seletor de cores&amp;rbrack; pressionar Esc fecha a janela do seletor de cores
* Melhoria de desempenho para interação de interface e ao pintar
* &amp;lbrack;Engine&amp;rbrack; Atualização para a nova versão do mecanismo de Substance (8.3.0)
* &amp;lbrack;Scripting&amp;rbrack;&amp;lbrack;Python&amp;rbrack; Permitir recarregar a malha do projeto atual
* &amp;lbrack;Scripting&amp;rbrack;&amp;lbrack;Python&amp;rbrack; Permitir atualização de recursos em projetos
* &amp;lbrack;Scripting&amp;rbrack;&amp;lbrack;Python&amp;rbrack; Permite definir e consultar a resolução de Blocos UV
* &amp;lbrack;Interoperabilidade&amp;rbrack; Não disponível para as edições Steam e Substance
* &amp;lbrack;Interoperabilidade&amp;rbrack; Receber vários recursos do Bridge

**Corrigido:**

* O seletor de cores não exibe a cor correta
* &amp;lbrack;Fazendo bake&amp;rbrack; A lista de conjuntos de texturas não está ordenada corretamente
* As transformações dinâmicas de grupo do &amp;lbrack;FBX import&amp;rbrack; 3ds Max não são levadas em consideração
* &amp;lbrack;Substance Engine&amp;rbrack; Falha com importação de SBSAR corrompido
* &amp;lbrack;A opção de configuração do projeto do MacOS&amp;rbrack; em idiomas diferentes não está presente
* Os salvamentos automáticos podem congelar o Painter durante processos longos

**Problemas Conhecidos:**

* &amp;lbrack;Projection&amp;rbrack;&amp;lbrack;Warp&amp;rbrack; Split option permanece selecionada após a divisão ser feita
* &amp;lbrack;Projeção&amp;rbrack;&amp;lbrack;Distorcer&amp;rbrack; não funciona quando a transformação está definida para o espaço global
* &amp;lbrack;Projeção&amp;rbrack;&amp;lbrack;Distorcer&amp;rbrack; Linhas de artefato entre as correções em alguns casos raros
* &amp;lbrack;Projeção&amp;rbrack;&amp;lbrack;UV&amp;rbrack; O ponto dinâmico é redefinido ao inverter a projeção
* &amp;lbrack;Os Materiais inteligentes do Mac M1&amp;rbrack; não são exibidos corretamente
* &amp;lbrack;M1&amp;rbrack;&amp;lbrack;Regressão&amp;rbrack; Camadas de material não funcionam

### 7.2.3

*(Lançado: 24 de agosto de 2021*)Resumo: **Versão secundária, correção de erro**

**Adicionado:**

* &amp;lbrack;Bibliotecas&amp;rbrack; Adicionar uma maneira de impedir que arquivos indesejados sejam rastreados

**Corrigido:**

* &amp;lbrack;Win&amp;rbrack; Vários telas e problemas de suspensão
* &amp;lbrack;MacOS&amp;rbrack;&amp;lbrack;Falha&amp;rbrack; Alternando sombreador ao usar efeitos
* &amp;preto;Visor&amp;rbrack; O modo de visualização completa não mostra mais o cursor do pincel sem alfa
* O widget Ângulo do &amp;lbrack;UI&amp;rbrack; vira da maneira errada
* &amp;lbrack;Pilha de camadas&amp;rbrack; Muitas subpastas criam um congelamento muito longo
* &amp;lbrack;Iray&amp;rbrack; Diferentes vistas em Iray e OpenGL: Visível se não estiver funcionando
* &amp;lbrack;Iray&amp;rbrack; Índice de refração não levado em consideração e não aparece nas propriedades mdl
* &amp;lbrack;JavaScript&amp;rbrack; ShowExportDialog() nunca retorna verdadeiro
* Não é possível ler o mtl do Adobe Stock

### 7.2.2

*(Lançado: 27 de julho de 2021*)Resumo: **Versão secundária, correção de erros**

**Adicionado:**

* Atualizar versão de requisitos de driver AMD

**Corrigido:**

* &amp;lbrack;Mac M1&amp;rbrack; Detecção de memória incorreta
* &amp;lbrack;Export&amp;brack; Os caminhos muito longos não são exibidos corretamente

**Problemas Conhecidos:**

* &amp;lbrack;Content&amp;brack; Sombreadores desatualizados das amostras

### 7.2.1

*(Lançado em: 2 de julho de 2021*)Resumo: **Versão secundária, Hotfix**

**Adicionado:**

* &amp;lbrack;Interop&amp;rbrack; Adicionar dica de ferramenta para informar que o envio de projetos do Bloco UV para o Stager ainda não é suportado
* &amp;lbrack;Plug-in&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Atualização do ícone do Livelink

**Corrigido:**

* &amp;lbrack;A versão do driver Nvidia&amp;rbrack; que começa com 30 é considerada desatualizada
* &amp;lbrack;Bibliotecas&amp;rbrack; O estado do painel Ativos não é salvo, a menos que um projeto esteja aberto
* &amp;lbrack;Bibliotecas&amp;rbrack; A nova pesquisa salva mantém a palavra-chave da pesquisa salva antiga
* &amp;lbrack;Baker&amp;rbrack;&amp;lbrack;UVTiles&amp;rbrack; os mapas de ID por meshID também levam Blocos UV em consideração
* &amp;lbrack;Exportar&amp;rbrack; arquivos gLTF não importam a cor do vértice
* &amp;lbrack;Iray&amp;rbrack; Algumas dicas estão faltando
* O &amp;lbrack;Interop&amp;rbrack; Enviar para o Stager nem sempre é desativado quando o Stager não é detectado
* &amp;lbrack;Atualizador de Recursos&amp;rbrack; O criador de pincéis do Photoshop não pode ser atualizado
* &amp;lbrack;Content&amp;brack; O gerador de desgaste de borda de fibra de vidro está quebrado

### 7.2.0

*(Lançado: 23 de junho de 2021*)Resumo: **Versão principal, fornece uma atualização para o painel de ativos, um novo sombreador com acesso a novos canais e parâmetros, uma atualização geral da interface do usuário, algumas melhorias de desempenho muito solicitadas, suporte a idiomas expandido e muito mais!**

**Adicionado:**

* &amp;lbrack;Bibliotecas&amp;rbrack; Novo painel de ativos para substituir a prateleira
* &amp;lbrack;Bibliotecas&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Novo layout do painel Ativos
* &amp;lbrack;Bibliotecas&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Alterar a orientação e a interface padrão do Painel de ativos
* &amp;lbrack;Bibliotecas&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Introduzir uma opção de exibição em lista para a biblioteca
* &amp;lbrack;Bibliotecas&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Navegação por novas trilhas no Painel de ativos
* &amp;lbrack;Bibliotecas&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Selecione “Todas as bibliotecas” ao selecionar uma pesquisa salva
* &amp;lbrack;Bibliotecas&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Selecione “Todas as bibliotecas” quando todas as pastas estiverem desmarcadas
* &amp;lbrack;Bibliotecas&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Nova marca para pincéis de partícula
* &amp;lbrack;Bibliotecas&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Substituído “prateleira” por “Todas as bibliotecas” no aplicativo
* &amp;lbrack;Bibliotecas&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Permitir ocultar pastas vazias
* &amp;lbrack;Libraries&amp;rbrack;&amp;lbrack;UI&amp;rbrack; A biblioteca padrão do usuário deve estar visível mesmo se estiver vazia
* &amp;lbrack;Bibliotecas&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Novo método de filtragem por meio de ícones de tipo de ativo
* &amp;lbrack;Bibliotecas&amp;rbrack; Atalho “CTRL” para selecionar vários tipos de ativos
* &amp;lbrack;Bibliotecas&amp;rbrack; Nova variável de ambiente para controlar o orçamento de memória de visualização do ativo
* &amp;lbrack;Libraries&amp;rbrack;&amp;lbrack;Content&amp;rbrack; Novos mapas de ambiente
* &amp;lbrack;Bibliotecas&amp;rbrack;&amp;lbrack;Conteúdo&amp;rbrack;&amp;lbrack;IU&amp;rbrack; Renderizar deslocamento em materiais padrão
* &amp;lbrack;Bibliotecas&amp;rbrack;&amp;lbrack;Conteúdo&amp;rbrack; Definir Adobe Standard Material (ASM) sombreador como padrão para a geração de visualizações
* &amp;lbrack;Bibliotecas&amp;rbrack;&amp;lbrack;Conteúdo&amp;rbrack;&amp;lbrack;ASM&amp;rbrack; Novos Modelos de Projeto para o novo sombreador ASM
* &amp;lbrack;Libraries&amp;rbrack;&amp;lbrack;Thumbnail&amp;rbrack; Usar novo mapa de ambiente do Studio 6
* &amp;lbrack;Bibliotecas&amp;rbrack;&amp;lbrack;Miniatura&amp;rbrack; Ler miniatura no recurso em vez de gerá-lo
* &amp;lbrack;Bibliotecas&amp;rbrack;&amp;lbrack;Miniatura&amp;rbrack; Adicionar deslocamento à geração de miniaturas
* &amp;preto;Configurações do conjunto de texturas&amp;rbrack;
* &amp;lbrack;Configurações do conjunto de texturas&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Expor o novo height ao método de conversão normal
* &amp;lbrack;Configurações do conjunto de texturas&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Retrabalho da organização da interface do usuário dos canais
* &amp;lbrack;Configurações do conjunto de texturas&amp;rbrack; Limite dos canais do usuário aumentado para 16 canais
* &amp;lbrack;Configurações do conjunto de texturas&amp;rbrack;&amp;lbrack;IU&amp;rbrack; Indica quais canais são compatíveis com o sombreador selecionado atualmente
* &amp;lbrack;Sombreador&amp;rbrack;&amp;lbrack;ASM&amp;rbrack; Novo sombreador
* &amp;lbrack;Sombreador&amp;rbrack;&amp;lbrack;ASM&amp;rbrack; Suporte adicionado para Anisotropia, Revestimento transparente, Dispersão da subsuperfície, Specular edge color e Brilho
* &amp;lbrack;Sombreador&amp;rbrack;&amp;lbrack;ASM&amp;rbrack; Alterar os valores de cor dos canais padrão
* &amp;lbrack;Sombreador&amp;rbrack;&amp;lbrack;ASM&amp;rbrack;&amp;lbrack;Exportar&amp;rbrack; Modelo de exportação atualizado do Adobe Dimension para o Adobe Substance 3D Stager
* &amp;lbrack;Sombreador&amp;rbrack;&amp;lbrack;ASM&amp;rbrack; Rótulos e dicas de ferramentas adicionados para os parâmetros sombreador e MDL
* &amp;lbrack;Sombreador&amp;rbrack;&amp;lbrack;ASM&amp;rbrack; Torna a cor da Dispersão visível no Visualização 2D, mesmo se o SSS não for suportado
* &amp;lbrack;Sombreador&amp;rbrack;&amp;lbrack;ASM&amp;rbrack;&amp;lbrack;Iray&amp;rbrack; Suporte ao sombreador ASM no Iray com o novo MDL
* &amp;lbrack;Sombreador&amp;rbrack;&amp;lbrack;ASM&amp;rbrack;&amp;lbrack;Iray&amp;rbrack; Atualização da dispersão de subsuperfície no brilho de especificação PBR herdado e revestido
* &amp;lbrack;Sombreador&amp;rbrack;&amp;lbrack;ASM&amp;rbrack;&amp;lbrack;Conteúdo&amp;rbrack; Alterou o tipo padrão de SSS para amostras
* &amp;lbrack;Sombreador&amp;rbrack;&amp;lbrack;ASM&amp;rbrack; Documentação adicionada para API ASM
* &amp;lbrack;Sombreador&amp;rbrack;&amp;lbrack;ASM&amp;rbrack; Otimizar sombreadores para ignorar canais não utilizados
* &amp;lbrack;Sombreador&amp;rbrack; Expor novos canais do Conjunto de Texturas
* &amp;lbrack;Sombreador&amp;rbrack; Dispersão de subsuperfície aprimorada
* &amp;lbrack;Sombreador&amp;rbrack; Novos parâmetros de sombreador ocultos para alguns sombreadores
* &amp;lbrack;Sombreador&amp;rbrack; Visível se para parâmetros de sombreador
* &amp;preto;Desempenho&amp;rbrack;
* &amp;lbrack;Bibliotecas&amp;rbrack; Visualização do recurso carregando melhorias de tempo e desempenho de cálculo
* &amp;lbrack;Mecanismo&amp;rbrack; Melhorias no desempenho da pintura
* &amp;lbrack;Desempacotar automaticamente&amp;rbrack;
* &amp;lbrack;Retirar quebra automática&amp;rbrack; melhorias no desempenho da Embalagem
* &amp;lbrack;Desempacotamento automático&amp;rbrack; Desempacotamento automático compatível com o fluxo de trabalho do Bloco UV
* &amp;lbrack;Contornar automaticamente&amp;rbrack; Nova opção para posicionar UVs de acordo com a orientação da malha
* &amp;prego;Outro&amp;preto;
* &amp;lbrack;Configurações&amp;rbrack; Mudou a direção padrão do zoom
* &amp;lbrack;UI&amp;rbrack; Atualização geral da IU
* &amp;lbrack;UI&amp;rbrack; Retrabalho do Menu Ajuda
* &amp;lbrack;UI&amp;rbrack; Substituir ícone de inversão
* &amp;lbrack;UI&amp;rbrack;&amp;lbrack;Plug-in&amp;rbrack; Ícone Substituir do link dcc do plug-in
* &amp;lbrack;UI&amp;rbrack;&amp;lbrack;AMD&amp;rbrack; Atualizar versão mínima necessária e mensagem pop-up
* &amp;lbrack;Pilha de camadas&amp;rbrack; Cria nova camada dentro da pasta vazia selecionada
* Atualizar Documentação do Python
* &amp;brack;Marca&amp;rbrack;
* &amp;lbrack;Branding&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Nome do aplicativo atualizado para Adobe Substance 3D Painter
* &amp;lbrack;Branding&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Versão autônoma atualizada para &#39;Substance edition&#39;
* &amp;lbrack;Branding&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Nome executável do aplicativo atualizado, caminho de instalação, pacote e ícones
* &amp;lbrack;Branding&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Biblioteca e caminho padrão renomeados
* &amp;lbrack;Marca&amp;rbrack;&amp;lbrack;IU&amp;rbrack; Atualizado Sobre a Janela
* &amp;lbrack;Marca&amp;rbrack;&amp;lbrack;IU&amp;rbrack; Tela de Boas-vindas atualizada
* &amp;lbrack;Marca&amp;rbrack;&amp;lbrack;IU&amp;rbrack; Removido número da versão baseada no ano
* &amp;lbrack;Localização&amp;rbrack; Novas traduções para alemão, francês e chinês simplificado
* &amp;lbrack;Interoperabilidade&amp;rbrack; Não disponível para as edições Steam e Substance
* &amp;lbrack;Interoperabilidade&amp;rbrack; Interoperabilidade com o Ecossistema Adobe: Designer, Sampler, Stager e Bridge
* &amp;lbrack;Interoperabilidade&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Receber e atualizar ativos do Designer
* &amp;lbrack;Interoperabilidade&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Receber ativo do Sampler
* &amp;lbrack;Interoperabilidade&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Enviar ativo para o Stager
* &amp;lbrack;Interoperabilidade&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Mostrar no Adobe Bridge
* &amp;lbrack;Interoperabilidade&amp;rbrack;&amp;lbrack;IU&amp;rbrack; Permitir acesso rápido a Ativos 3D do Adobe
* &amp;lbrack;Interoperabilidade&amp;rbrack; Novas marcas de uso de sbsar
* &amp;lbrack;Interoperabilidade&amp;rbrack; Manipular tipos de ativos recebidos
* &amp;lbrack;Interoperabilidade&amp;rbrack; Os ativos recebidos do Adobe Substance 3D Designer ou Adobe Substance 3D Sampler são armazenados na biblioteca padrão escolhida pelo usuário
* &amp;lbrack;Interoperabilidade&amp;rbrack;&amp;lbrack;IU&amp;rbrack; Novo ícone na barra de ferramentas esquerda para enviar para o Stager ou Photoshop

**Corrigido:**

* &amp;lbrack;Tablet&amp;rbrack; Baixo desempenho ao pintar com pressão
* &amp;lbrack;Problema no tablet com controles deslizantes
* &amp;lbrack;Falha&amp;rbrack; Nome incompatível entre a lista de Conjuntos de Texturas e o Exportador
* &amp;lbrack;Crash&amp;rbrack;&amp;lbrack;Bibliotecas&amp;rbrack; Clique duas vezes em uma subbiblioteca
* &amp;lbrack;Bibliotecas&amp;rbrack; Problema ao Rastrear diretórios de bibliotecas
* &amp;lbrack;Bibliotecas&amp;rbrack; Forçar geração de visualização linha de comando não funciona como esperado
* &amp;lbrack;Bibliotecas&amp;rbrack;&amp;lbrack;Conteúdo&amp;rbrack; O filtro Ambiente de Luz Feito bake é preto por padrão
* &amp;lbrack;Linux&amp;rbrack;&amp;lbrack;MacOS&amp;rbrack;&amp;lbrack;Exportar malha&amp;rbrack; Não é possível importar glTF criado no Linux/MacOS
* &amp;lbrack;Linux&amp;rbrack; Arrastar e soltar um arquivo no Painel de ativos pode causar um travamento
* O &amp;lbrack;Contornar automaticamente&amp;rbrack; Contornar automaticamente disponível mesmo se uma malha não tiver sido selecionada para recarregamento
* &amp;lbrack;Partículas&amp;rbrack; Comportamento de partícula incorreto com a gravidade
* O histograma de nível do &amp;lbrack;Pilha de camadas&amp;rbrack; só pode usar a Luminância com alguns canais
* &amp;preto;Máscara de geometria&amp;rbrack; Menu do botão direito do mouse em uma pasta quando a edição da máscara de geometria não funcionar
* &amp;lbrack;Projeção&amp;rbrack; Costura com projeção esférica e filtragem bilinear
* &amp;lbrack;Blocos UV&amp;rbrack; Exportar máscara para arquivo exporta somente bloco 0, 0
* &amp;preto;Exportar malha&amp;rbrack; A exportação de malha FBX está vazia
* O Mapa normal &amp;lbrack;Iray&amp;rbrack; não é levado em consideração em novos projetos ao renderizar
* &amp;lbrack;Salvar&amp;rbrack; Salvar problemas em unidades compartilhadas
* &amp;lbrack;Fazendo bake&amp;rbrack; Reativar uma malha com parâmetros modificados exibe um aviso
* &amp;lbrack;Fazendo bake&amp;rbrack;&amp;lbrack;Regressão&amp;rbrack; Resultado incorreto quando a caixa delimitadora global de grandes malhas não inclui a origem da cena
* &amp;lbrack;Python&amp;rbrack; As bibliotecas de usuário personalizadas não são levadas em consideração

**Problemas Conhecidos:**

* &amp;lbrack;Bibliotecas&amp;rbrack; Pesquisas salvas não são salvas se nenhum projeto for aberto
* &amp;lbrack;NVIDIA&amp;rbrack; Mensagem para driver desatualizado mesmo se o driver estiver atualizado

### 7.1.1 (2021.1.1)

*(Lançado: 23 de março de 2021*)Resumo: **Versão secundária, correção de erro com possibilidade de inserir valores hexadecimais no seletor de cores**

**Adicionado:**

* &amp;lbrack;Log&amp;rbrack; Avisa os usuários sobre drivers de GPU AMD incompatíveis
* &amp;preto;Seletor de cores&amp;rbrack; Permitir digitar valores hexadecimais

**Corrigido:**

* &amp;lbrack;Baker&amp;rbrack; Queda de desempenho
* &amp;lbrack;Máscara de geometria&amp;rbrack; clicar com a tecla Alt no nome da malha pode levar a um travamento
* &amp;lbrack;Engine&amp;brack; A pintura não atualiza toda a exibição quando necessário
* &amp;lbrack;Pilha de camadas&amp;rbrack; A seleção fica parada após alterar o sombreador
* &amp;lbrack;MacOS&amp;rbrack;&amp;lbrack;Seletor de cores&amp;rbrack; A cor é ligeiramente diferente da escolhida
* &amp;lbrack;Export&amp;rbrack; Usar o formato de arquivo PSD não gera um arquivo por Bloco UV
* &amp;lbrack;Scripting&amp;rbrack;&amp;lbrack;Javascript&amp;rbrack; alg.mapexport.getPathsExportDocumentMaps() não retorna todos os valores
* &amp;lbrack;Scripting&amp;rbrack;&amp;lbrack;Python&amp;rbrack; Os plug-ins desativados são ativados novamente ao reabrir o Painter

### 7.1.0 (2021.1.0)

*(Lançado: 28 de janeiro de 2021*)Resumo: **Versão principal, nova Máscara de Geometria que permite selecionar e tinta partes da geometria, copiar/colar efeitos na pilha de camadas, melhoria do fluxo de trabalho do Bloco UV, atualização do Iray, Baker, Substance Engine e novo conteúdo**

**Adicionado:**

* Nova máscara de geometria e tinta partes selecionadas da geometria
* &amp;preto;Máscara de geometria&amp;rbrack; Permitir a tinta de partes selecionadas da geometria por nomes de malha
* &amp;preto;Máscara de geometria&amp;rbrack; Seleção retangular em ambas as portas de visualização
* &amp;preto;Máscara de geometria&amp;rbrack; Permite ocultar/ignorar a geometria excluída em qualquer camada
* &amp;lbrack;Máscara de geometria&amp;rbrack;&amp;lbrack;Propriedades&amp;rbrack; Seleção rápida de caixas de seleção com clicar e arrastar
* &amp;lbrack;Máscara de geometria&amp;rbrack;&amp;lbrack;Propriedades&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Incluir/Excluir tudo com uma lista suspensa na janela Propriedades
* &amp;lbrack;Máscara de geometria&amp;rbrack;&amp;lbrack;Propriedades&amp;rbrack; Permite selecionar rapidamente um item em uma lista com ALT+CLIQUE ESQUERDO
* &amp;lbrack;Máscara de geometria&amp;rbrack;&amp;lbrack;Propriedades&amp;rbrack; Sobreposição em viewports ao passar o mouse sobre nomes/Blocos UV de malha na janela Propriedades
* &amp;lbrack;Máscara de geometria&amp;rbrack;&amp;lbrack;Pilha de camadas&amp;rbrack; Adicionar opções de copiar/colar à máscara de geometria
* &amp;preto;Máscara de geometria&amp;rbrack; Novo ícone para o botão Ocultar/ignorar geometria excluída
* &amp;preto;Máscara de geometria&amp;rbrack; Nova dica de ferramenta para Ocultar/ignorar geometria excluída
* &amp;lbrack;Máscara de geometria&amp;rbrack; Atalho de teclado ALT+H para ativar/desativar o botão “ocultar ignorar geometria excluída”
* &amp;lbrack;Blocos UV&amp;rbrack;&amp;lbrack;Pilha de camadas&amp;rbrack; Nova miniatura de visualização da esfera da camada de preenchimento para Blocos UV e modo simplificado
* &amp;lbrack;Blocos UV&amp;rbrack;&amp;lbrack;Pilha de camadas&amp;rbrack; Permite sair facilmente da máscara de Bloco UV
* &amp;lbrack;Blocos UV&amp;rbrack;&amp;lbrack;Lista do conjunto de texturas&amp;rbrack; Permitir fornecer uma descrição por Bloco UV
* &amp;lbrack;Blocos UV&amp;rbrack;&amp;lbrack;Configurações do conjunto de textura&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Dois novos títulos de seção no menu suspenso para alterar a resolução do Bloco UV
* &amp;lbrack;Blocos UV&amp;rbrack;&amp;lbrack;Visor&amp;rbrack; Sair da Máscara do Bloco UV ao arrastar um material para o visor
* &amp;preto;Pilha de camadas&amp;rbrack; Adicionar opções de Copiar/Colar para efeitos
* &amp;lbrack;Pilha de camadas&amp;rbrack; Permitir copiar/colar efeitos de um Conjunto de Texturas para outro
* &amp;lbrack;Pilha de camadas&amp;rbrack; Permitir seleção múltipla de efeitos
* &amp;preto;Pilha de camadas&amp;rbrack; Adicionar opções de copiar/colar como atalhos para efeitos de camada
* &amp;lbrack;Pilha de camadas&amp;rbrack; Alterna automaticamente entre máscara e conteúdo ao arrastar efeitos para outra camada
* &amp;lbrack;Pilha de camadas&amp;rbrack; Cria automaticamente uma máscara ao colar uma máscara de outra camada
* &amp;lbrack;Pilha de camadas&amp;rbrack; Adicionar ações de efeito de movimento dentro do menu contextual de clique com o botão direito do mouse dos efeitos
* &amp;lbrack;Pilha de camadas&amp;rbrack; Permite arrastar e soltar efeitos de uma camada para outra
* &amp;lbrack;Pilha de camadas&amp;rbrack; Arrastar itens para uma pasta os coloca na parte superior da pasta
* Atualize o Iray para a versão 2020.1.0
* &amp;lbrack;Baker&amp;rbrack; Atualize os Baker para a versão 2.5.4
* &amp;lbrack;Baker&amp;rbrack; Exibir Blocos UV individuais na janela de progresso de fça bake
* &amp;lbrack;Baker&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Permite fazer bake rapidamente o Conjunto de Texturas atual por um novo botão
* &amp;lbrack;Baker&amp;rbrack; Permite ao usuário selecionar rapidamente um dos baker com ALT+CLIQUE ESQUERDO
* Atualize o Substance Engine para a versão 8.0.8
* &amp;lbrack;Substance Engine&amp;rbrack; Suporte a Cor Padrão em novos arquivos .sbsar
* &amp;lbrack;Desempacotamento Automático&amp;rbrack; Melhoria de desempenho
* &amp;lbrack;Export&amp;brack; Adicionar feedback visual para indicar qual resolução do Bloco UV difere do padrão do projeto
* &amp;lbrack;Export&amp;brack; Adicionar fator de tamanho de cena ao arquivo json de sombreador exportado
* &amp;lbrack;Language&amp;brack; Adicionar tradução para japonês
* &amp;lbrack;UI&amp;rbrack; Atualizar Sobre janela com controle de versão de dependências internas
* &amp;lbrack;Scripting&amp;rbrack;&amp;lbrack;Python&amp;rbrack; Permitir o gerenciamento de recursos de prateleira
* &amp;lbrack;Scripting&amp;rbrack;&amp;lbrack;Python&amp;rbrack; Permite saber quando um projeto está pronto para fazer bake e exportar
* &amp;lbrack;Scripting&amp;rbrack;&amp;lbrack;Python&amp;rbrack; Permitir saber quando uma prateleira terminou de rastrear recursos no disco
* &amp;lbrack;Scripting&amp;rbrack;&amp;lbrack;Python&amp;rbrack; Permitir a consulta da lista de blocos UV por Conjuntos de texturas
* &amp;lbrack;Scripting&amp;rbrack;&amp;lbrack;Python&amp;rbrack; Permitir atribuir visualização personalizada aos recursos de prateleira
* &amp;lbrack;Scripting&amp;rbrack;&amp;lbrack;Python&amp;rbrack; Permitir gerenciar prateleiras personalizadas
* &amp;lbrack;Scripting&amp;rbrack;&amp;lbrack;Python&amp;rbrack; Adicionar um índice de método em cada submódulo na documentação
* &amp;lbrack;Scripting&amp;rbrack;&amp;lbrack;Python&amp;rbrack; Novo estilo para a documentação
* &amp;lbrack;Scripting&amp;rbrack;&amp;lbrack;Python&amp;rbrack; Aprimoramento de recursos e documentação de prateleira
* &amp;lbrack;Content&amp;brack; Três novas predefinições de ferramenta para fazer pontos
* &amp;lbrack;Shelf&amp;rbrack; remove temporariamente “Exportar para o Substance share” durante a transição para a nova plataforma de Substance share

**Corrigido:**

* Falha ao usar monitores com diferentes resoluções
* Falha no Substance Engine com alguns projetos raros
* A atualização do visor falha com a opção Ocultar/Ignorar geometria excluída ao alternar as camadas
* &amp;lbrack;Visualização 2D&amp;rbrack; A Janela de visualização 2D pode estar ausente em alguns projetos
* &amp;lbrack;Fazendo bake&amp;rbrack; “Corresponder pelo nome da malha” ignora partes do objeto
* &amp;lbrack;Pilha de camadas&amp;rbrack; Clicar em um efeito de camada abre a pasta
* O Bloco UV &amp;lbrack;Máscara de geometria&amp;rbrack; ainda é contado na máscara mesmo ao reimportar a malha sem ela
* &amp;lbrack;Máscara de geometria&amp;rbrack; O menu do botão direito no visor não fornece as ferramentas corretas
* &amp;lbrack;Engine&amp;rbrack; Atrasos intensos em projetos específicos
* &amp;lbrack;Scripting&amp;rbrack; Alta latência com solicitações remotas de POST JSON no Windows
* A quantidade de Vram do &amp;lbrack;Linux&amp;rbrack; não é detectada corretamente com GPUs integradas específicas
* &amp;lbrack;Auto desempacotar&amp;rbrack; Trava ou desempacota longamente em alguns projetos

## Versão 6

### 6.2.2 (2020.2.2)

*(Lançado: 28 de setembro de 2020*)Resumo: **Versão secundária, correção de erro com algumas funções na API Python**

**Adicionado:**

* &amp;lbrack;Desempenho&amp;rbrack; Não calcula todos os Blocos UV ao usar a seleção de ID de cor
* &amp;lbrack;Baker&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Exibir descrições do conjunto de texturas
* &amp;lbrack;Baker&amp;rbrack; Permitir salvar configurações do faço bake
* &amp;lbrack;Baker&amp;rbrack; Adicionar recolher tudo/expandir todas as opções para a guia Seleção
* &amp;preto;Lista do conjunto de texturas&amp;rbrack; Ocultar descrição quando vazio
* &amp;lbrack;Blocos UV&amp;rbrack;&amp;lbrack;Lista do conjunto de texturas&amp;rbrack; Clicar no Bloco UV deve expandir/recolher a lista
* &amp;lbrack;Export&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Permitir o redimensionamento horizontal do painel Lista do conjunto de texturas
* &amp;lbrack;Export&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Texto de dica de ferramenta consistente para Blocos UV e fluxo de trabalho do Conjunto de texturas com texturas não selecionadas
* &amp;lbrack;Scripting&amp;rbrack;&amp;lbrack;Python&amp;rbrack; Permitir o uso de predefinições de exportação para exportar texturas
* &amp;lbrack;Scripting&amp;rbrack;&amp;lbrack;Python&amp;rbrack; Adicionar um changelog na documentação
* &amp;lbrack;Scripting&amp;rbrack;&amp;lbrack;Python&amp;rbrack; Permite consultar todos os canais disponíveis em uma determinada pilha
* Melhorias na interface do console do &amp;lbrack;Scripting&amp;rbrack;&amp;lbrack;Python&amp;rbrack;

**Corrigido:**

* &amp;lbrack;AMD&amp;rbrack; Detecção incorreta de versão de driver desatualizada
* Falha ao reimportar uma malha com layout de Blocos UV diferente em alguns casos
* Falha ao usar partículas com UDIMs em malhas muito pesadas
* &amp;lbrack;Blocos UV&amp;rbrack; Falha ao exportar uma malha com informações de deslocamento em alguns casos
* &amp;lbrack;Export&amp;brack;&amp;lbrack;Crash&amp;rbrack; Exportar Visualização 2D no formato psd pode causar um travamento
* Importar imagens como sequências ao criar um projeto não funciona
* Mecanismo travado em um loop infinito
* &amp;brack;Atalho&amp;rbrack; A câmera gira sempre no modo de ajuste ao alterar os atalhos do modo de ajuste
* As malhas são sempre desempacotadas automaticamente quando reimportadas, mesmo que a opção esteja desativada
* &amp;preto;Lista do conjunto de texturas&amp;rbrack; O campo de texto da descrição às vezes não está totalmente visível durante a edição
* &amp;preto;Lista do conjunto de texturas&amp;rbrack; O menu suspenso para ocultar/revelar Conjuntos de texturas não está totalmente visível
* &amp;preto;Lista do conjunto de texturas&amp;rbrack; Clicar no ícone de olho não deve inserir o “Editar nome do conjunto de texturas”
* &amp;preto;Configurações do conjunto de texturas&amp;rbrack; A remoção de um canal também remove o canal abaixo
* &amp;lbrack;Export&amp;rbrack; Incluir tudo e Redefinir tudo não leva Blocos UV em consideração
* &amp;lbrack;Baker&amp;rbrack; Os baker desmarcados aparecem durante o processo de fça bake
* A atualização de resolução não é levada em consideração para mapas baked usados como entrada
* &amp;lbrack;Blocos UV&amp;rbrack;&amp;lbrack;Visor&amp;rbrack; Congelamento do Visor 3D ao adicionar Material inteligente após pasta com a máscara de Bloco UV selecionada
* &amp;lbrack;Blocos UV&amp;rbrack;&amp;lbrack;Visor&amp;rbrack; o Wireframe ainda está visível para ladrilhos ocultos com o modo tinta por
* &amp;lbrack;Export&amp;brack;&amp;lbrack;Sketchfab&amp;rbrack; Problemas com o tipo de assinatura “plus”
* &amp;lbrack;Sketchfab&amp;rbrack; A caixa de seleção “Este ativo é privado” não é exibida após alternar a conta
* &amp;lbrack;Export&amp;brack;&amp;lbrack;Content&amp;rbrack; “Ondulado” predefinições de pincel podem levar a problemas de desempenho
* &amp;lbrack;Plug-in Photoshop&amp;rbrack; Mensagem no registro: não compatível com o fluxo de trabalho do Bloco UV
* &amp;lbrack;Scripting&amp;rbrack;&amp;lbrack;Python&amp;rbrack; PYTHONPATH env var impede que o aplicativo seja iniciado
* &amp;lbrack;Scripting&amp;rbrack;&amp;lbrack;Python&amp;rbrack; Erro de ortografia na documentação do Python

### 6.2.1 (2020.2.1)

*(Lançado Em: 29 De julho De 2020*)Resumo: **Versão Secundária, Hotfix**

**Adicionado:**

* Adicione a variável de ambiente “SUBSTANCE_PAINTER_VRAM_BUDGET” para substituir o valor de VRam da GPU
* &amp;lbrack;Blocos UV&amp;rbrack;&amp;lbrack;Desempenho&amp;rbrack; Não calcular todos os blocos UV ao usar a ferramenta Preenchimento de polígono

**Corrigido:**

* &amp;lbrack;Iray&amp;rbrack; Salvar renderização retorna um erro e resulta em uma imagem em preto
* &amp;lbrack;Linux&amp;rbrack; Falha após a tela inicial no CentOS 7.3
* A quantidade de Vram do &amp;lbrack;Linux&amp;rbrack; não é detectada corretamente com configurações específicas
* &amp;lbrack;Crash&amp;rbrack; Abrindo um projeto com o nome do conjunto de texturas duplicado
* &amp;lbrack;Engine&amp;brack; Problema de invalidação de cache ao modificar uma máscara
* &amp;preto;Lista do conjunto de texturas&amp;rbrack; Efeito de fonte incorreto quando o conjunto de texturas está desativado

**Problemas Conhecidos:**

* &amp;preto;Lista do conjunto de texturas&amp;rbrack; Não é possível ocultar a descrição
* &amp;preto;Lista do conjunto de texturas&amp;rbrack; problemas de interface do usuário
* &amp;lbrack;Iray&amp;rbrack; a renderização de PSD não abre
* &amp;lbrack;Plug-in Photoshop&amp;rbrack; Não compatível com o fluxo de trabalho de Blocos UV

### 6.2.0 (2020.2.0)

*(Lançado em: 23 de julho de 2020*)Resumo: **Versão principal com novo fluxo de trabalho de Blocos UV, tinta entre Blocos UV e melhoria de desempenho**

**Adicionado:**

* Blocos UV (UDIMs)
* &amp;lbrack;Blocos UV&amp;rbrack; Tinta em blocos UV
* &amp;lbrack;Blocos UV&amp;rbrack; Permite escolher entre o fluxo de trabalho novo e herdado para Blocos UV
* &amp;lbrack;Blocos UV&amp;rbrack; Importar sequências de imagens UDIMs/Bloco UV como um recurso
* &amp;lbrack;Blocos UV&amp;rbrack; Adicionar lista de Blocos UV por conjunto de textura na janela Lista de conjuntos de textura
* &amp;lbrack;Blocos UV&amp;rbrack; Permite editar a resolução de vários Blocos UV de uma vez nas Configurações do Conjunto de Texturas
* &amp;lbrack;Blocos UV&amp;rbrack;&amp;lbrack;Visualização 2D&amp;rbrack; Exibir Blocos UV como uma grade
* &amp;lbrack;Blocos UV&amp;rbrack;&amp;lbrack;Visualização 2D&amp;rbrack; Novo botão de visor para exibir ou ocultar informações de Blocos UV
* &amp;lbrack;Blocos UV&amp;rbrack; Alterna a ferramenta de pintura para canal único por padrão para projetos de Bloco UV
* &amp;lbrack;Blocos UV&amp;rbrack; Novo botão na barra de ferramentas contextual para ignorar Blocos UV mascarados ao pintar
* &amp;lbrack;Blocos UV&amp;rbrack;&amp;lbrack;Pilha de camadas&amp;rbrack; Novos ícones de pilha de camadas para melhorar o desempenho
* &amp;lbrack;Blocos UV&amp;rbrack;&amp;lbrack;Pilha de camadas&amp;rbrack; Aprimorar ícones de Tinta e Preenchimento na barra de ferramentas
* &amp;lbrack;Máscara de Bloco UV&amp;rbrack;&amp;lbrack;Visualização 2D&amp;rbrack; Permite incluir ou excluir vários Blocos UV de uma vez (clique com o botão esquerdo, CTRL+clique com o botão esquerdo)
* &amp;preto;Máscara de Bloco UV&amp;rbrack; Nova máscara de Bloco UV a ser incluída, exclui blocos por camada com um novo ícone
* &amp;lbrack;Máscara de Bloco UV&amp;rbrack;&amp;lbrack;Pilha de camadas&amp;rbrack; Exibir o número de Blocos UV no ícone de máscara de Blocos UV quando nem todos estiverem incluídos
* &amp;lbrack;Máscara de Bloco UV&amp;rbrack;&amp;lbrack;2D/Visualização 3D&amp;rbrack; Adicionar efeito hover para visualizar Blocos UV sob o cursor
* &amp;lbrack;Blocos UV&amp;rbrack;&amp;lbrack;Baker&amp;rbrack; Permite selecionar e fazer bake Blocos UV específicos
* &amp;lbrack;Blocos UV&amp;rbrack;&amp;lbrack;Baker&amp;rbrack; Adicionar opções de seleção para Conjuntos/Blocos UV de Textura
* &amp;lbrack;Blocos UV&amp;rbrack;&amp;lbrack;Baker&amp;rbrack; Clique com o botão direito do mouse na opção de menu para selecionar Blocos UV em um Conjunto de Texturas
* &amp;lbrack;Blocos UV&amp;rbrack;&amp;lbrack;Baker&amp;rbrack; Permite a seleção rápida no Conjunto de Texturas/Blocos UV arrastando
* &amp;lbrack;Blocos UV&amp;rbrack;&amp;lbrack;Baker&amp;rbrack; Substituir os botões “Tudo” e “Nenhum” nos Mapas de malha por opções de seleção mais explícitas
* &amp;lbrack;Blocos UV&amp;rbrack;&amp;lbrack;Baker&amp;rbrack; Exibir o número de texturas a serem feitas bake
* &amp;lbrack;Blocos UV&amp;rbrack;&amp;lbrack;Exportar&amp;rbrack; Permite selecionar e exportar Blocos UV específicos
* &amp;lbrack;Blocos UV&amp;rbrack;&amp;lbrack;Exportar&amp;rbrack; Permite a seleção rápida de Blocos UV arrastando
* &amp;lbrack;Blocos UV&amp;rbrack;&amp;lbrack;Exportar&amp;rbrack; Adicionar opções de menu suspenso para Blocos UV
* &amp;lbrack;Blocos UV&amp;rbrack;&amp;lbrack;Exportar&amp;rbrack; Tornar algumas predefinições de exportação indisponíveis se não funcionarem com Blocos UV (Adobe Dimension, Sketchfab, glTF, USD)
* &amp;lbrack;Blocos UV&amp;rbrack;&amp;lbrack;Conteúdo&amp;rbrack; Atualiza as predefinições de exportação para usar a nova tag $udim
* &amp;lbrack;Blocos UV&amp;rbrack; Melhorar o relatório de erros ao importar malhas com Ilhas UV sobrepostas
* &amp;lbrack;Blocos UV&amp;rbrack; Blocos UV compatíveis no Iray
* &amp;lbrack;Blocos UV&amp;rbrack;&amp;lbrack;Scripting&amp;rbrack; Adicionar documentação de exportação de Bloco UV ao documento Python
* Desempenho
* &amp;lbrack;Desempenho&amp;rbrack; Novo botão na barra de ferramentas contextual para pausar o cálculo do mecanismo ao trabalhar (SHIFT+ESC)
* &amp;lbrack;Desempenho&amp;rbrack; Abertura mais rápida do projeto atrasando o cálculo do cache do Conjunto de Texturas
* &amp;lbrack;Performance&amp;brack; Não espere até que os mapas de malha sejam carregados ao abrir o projeto
* &amp;lbrack;Performance&amp;rbrack;&amp;lbrack;2D/Visualização 3D&amp;rbrack; Não calcular o canal da Máscara no visor quando não estiver em uso
* &amp;lbrack;Desempenho&amp;rbrack; Não bloqueia o aplicativo ao carregar mapas de malha exibidos nas viewports
* &amp;lbrack;Desempenho&amp;rbrack; Melhorar a velocidade de salvamento incremental ao salvar um projeto
* &amp;lbrack;Desempenho&amp;rbrack;&amp;lbrack;Baker&amp;rbrack; Alterar configurações de dilatação padrão para melhorar o tempo de salvamento e o tamanho do projeto
* &amp;lbrack;Desempenho&amp;rbrack;&amp;lbrack;Baker&amp;rbrack; Alterne para tons de cinza em Baker específicos para melhorar o tempo de salvamento e o tamanho do projeto
* &amp;lbrack;Performance&amp;rbrack;&amp;lbrack;Export&amp;rbrack; Melhorar o desempenho do mecanismo para exportar texturas mais rapidamente
* &amp;lbrack;Desempenho&amp;rbrack;&amp;lbrack;Exportar&amp;rbrack; Melhorar a capacidade de resposta ao abrir a caixa de diálogo de exportação com muitos Conjuntos de textura
* &amp;lbrack;Performance&amp;rbrack;&amp;lbrack;Export&amp;rbrack; Melhorar o desempenho ao alternar para a guia “Lista de exportações”
* &amp;lbrack;Performance&amp;rbrack;&amp;lbrack;Iray&amp;rbrack; Reduzir tempo de inicialização do Iray
* Outro
* &amp;lbrack;Baker&amp;rbrack; Adicionar opções de seleção para Conjuntos de Textura
* Mover o gerenciamento de instância de sombreamento para as configurações do conjunto de textura
* &amp;lbrack;2D/Visualização 3D&amp;rbrack; Adiciona mensagem na parte inferior do visor para indicar qual tipo de máscara é editado
* &amp;lbrack;Pilha de camadas&amp;rbrack; Nova opção nas configurações para alternar entre miniaturas novas e antigas
* &amp;lbrack;Pilha de camadas&amp;rbrack; Adicionar feedback visual para indicar o estado de carregamento das miniaturas
* &amp;lbrack;Proj&amp;rbrack; Novo modo de projeção “Preenchimento (Corresponder por UV-Tile)” para carregar as sequências de imagens
* &amp;lbrack;Proj&amp;rbrack; Alterar modo de projeção de camadas de preenchimento para “Preenchimento (Corresponder por UV-Tile)” em casos específicos
* &amp;lbrack;Content&amp;brack; Otimizar predefinições do pincel a carvão para melhorar o desempenho
* Atualize o Iray para a versão 2020.0.0
* &amp;lbrack;Export&amp;brack; Desabilitar a guia Lista de Exportações quando nada estiver selecionado
* Desempacotar automaticamente
* &amp;lbrack;Auto Unwrap&amp;rbrack; Melhorar a taxa de sucesso do processo de desencapsulamento automático
* &amp;lbrack;Auto Unwrap&amp;rbrack; Parametrização aprimorada para aumentar a velocidade e estabilidade

**Corrigido:**

* &amp;lbrack;Alembic&amp;rbrack; Facesets são ignoradas ao importar arquivos
* &amp;lbrack;Alembic&amp;rbrack; Tempo de carregamento infinito com arquivos específicos
* &amp;lbrack;Import&amp;rbrack; Sequência de imagem UDIM incorreta é importada quando apenas a extensão do arquivo difere
* &amp;lbrack;Falha&amp;rbrack; Tentar abrir um projeto bloqueado por outro processo leva a uma falha
* &amp;lbrack;Projeção&amp;rbrack; Artefatos em malha duplicada ao usar projeção triplanar
* O canal de Emissivo do &amp;lbrack;Export&amp;rbrack; não é exportado com o formato USD
* &amp;lbrack;Content&amp;brack; Material inteligente “Carvão” contém traços de tinta

**Problemas Conhecidos:**

* &amp;preto;Lista do conjunto de texturas&amp;rbrack; Não é possível ocultar a descrição
* &amp;preto;Lista do conjunto de texturas&amp;rbrack; problemas de interface do usuário

### 6.1.3 (2020.1.3)

*(Lançado: 16 De junho De 2020*)Resumo: **Correção De Erros**

**Adicionado:**

* &amp;lbrack;Export&amp;brack; Adicionar configurações de deslocamento no arquivo json de parâmetros de Sombreador

**Corrigido:**

* &amp;lbrack;Falha&amp;rbrack;&amp;lbrack;Motor&amp;rbrack; Falha ao tentar apagar e substituir canais existentes
* &amp;lbrack;Crash&amp;rbrack; Alterar sombreador após pintar uma máscara em camadas de material
* &amp;lbrack;Crash&amp;rbrack;&amp;lbrack;Engine&amp;rbrack; Falha com alguns projetos pesados
* &amp;lbrack;Baker&amp;rbrack; Corresponder por nome não funciona com OBJ exportado do zBrush
* &amp;lbrack;Deslocamento&amp;rbrack;&amp;lbrack;SVT&amp;rbrack; Texturas não são exibidas na abertura do projeto quando o deslocamento está ativado
* &amp;lbrack;Export&amp;brack; Algumas texturas são exportadas cinza uniforme
* &amp;brack;Exportar&amp;rbrack; Conjuntos de Textura Desativados não devem ser exportados para predefinições de exportação Dimension e Sketchfab
* &amp;lbrack;Scripting&amp;rbrack;&amp;lbrack;JavaScript&amp;rbrack; Falha ao usar a API JavaScript para acessar a configuração de exportação no evento onProjectOpened
* &amp;lbrack;Scripting&amp;rbrack;&amp;lbrack;Javascript&amp;rbrack; onExportFinished() não é chamado após uma exportação

### 6.1.2 (2020.1.2)

*(Lançado: 28 de maio de 2020*)Resumo: **Correção de erros com atualização de Substance Engine e Baker**

**Adicionado:**

* &amp;lbrack;Baker&amp;rbrack; Atualiza para a versão mais recente
* &amp;lbrack;Baker&amp;rbrack; Novo método de amostragem em Oclusão de ambiente, Curvatura, baker de Thickness
* Atualize para a versão mais recente do Substance Engine
* &amp;lbrack;Scripting&amp;rbrack;&amp;lbrack;Python&amp;rbrack; Permitir criação de ResourceID para recursos do projeto
* &amp;lbrack;Scripting&amp;rbrack;&amp;lbrack;Python&amp;rbrack; Permitir consulta de informações de canal
* &amp;lbrack;Scripting&amp;rbrack;&amp;lbrack;Python&amp;rbrack; Adicionar funções dryrun e callback para simular a exportação de textura

**Corrigido:**

* &amp;lbrack;Baker&amp;rbrack; Normais incorretos no baker World Space Normals usando um Mapa normal tangente em casos específicos
* &amp;lbrack;Baker&amp;rbrack; Erro ao fazer bake Oclusão de ambiente com Optix quando não há poli alto
* &amp;lbrack;Traçados dinâmicos&amp;rbrack; Atraso ao carregar um Conjunto de Texturas específico
* &amp;lbrack;Export&amp;brack; Não deve exportar os conjuntos de texturas desativados para USD, glTF
* &amp;lbrack;Scripting&amp;rbrack;&amp;lbrack;JavaScript&amp;rbrack; Não é possível editar as novas configurações de baker de curvatura
* &amp;lbrack;Scripting&amp;rbrack;&amp;lbrack;JavaScript&amp;rbrack; alg.texturesets.addChannel() não retorna um erro em alguns casos
* &amp;lbrack;Scripting&amp;rbrack;&amp;lbrack;JavaScript&amp;rbrack; Erro de ortografia na documentação da API Javascript para setProjectExportOptions()
* &amp;lbrack;Scripting&amp;rbrack;&amp;lbrack;JavaScript&amp;rbrack; Sempre exporta todos os conjuntos de texturas
* &amp;lbrack;Scripting&amp;rbrack;&amp;lbrack;Python&amp;rbrack; sys.executable retorna um caminho para python.exe em vez de Substance Painter
* Cache de textura não compatível com o sistema operacional Mac e Windows/Linux
* &amp;lbrack;Livelink UE4&amp;rbrack; Somente o último material é usado para todos os conjuntos de texturas em uma malha combinada

**Problemas Conhecidos:**

* &amp;lbrack;Export&amp;brack;&amp;lbrack;Dimension&amp;rbrack;&amp;lbrack;Skecthfab&amp;rbrack; Não deve exportar os conjuntos de textura desativados
* &amp;lbrack;Crash&amp;rbrack; Alterar sombreador depois de pintar uma máscara em camadas de material

### 6.1.1 (2020.1.1)

*(Lançado: 05 De maio De 2020*)Resumo: **Hotfix**

**Adicionado:**

* &amp;preto;Exportar&amp;rbrack; Estado substituído de feedback visual no TextureSet

**Corrigido:**

* &amp;lbrack;O tamanho da janela do Exportador Export&amp;brack; é muito grande no monitor de resolução especial e não pode ser redimensionado
* &amp;preto;Opções de exportação&amp;rbrack; não são salvas após a exportação
* &amp;lbrack;Export&amp;brack; Falha ou não é possível exportar com a predefinição de exportação “do cache”
* &amp;lbrack;Export&amp;brack; Cancelar a exportação gera um mapa vazio adicional inesperado
* &amp;preto;Exportar&amp;rbrack; Corrigir configurações de predefinição de exportação virtual
* &amp;lbrack;Python&amp;rbrack; a variável env PYTHONPATH não é levada em consideração
* &amp;lbrack;Python&amp;rbrack;&amp;lbrack;Exportar&amp;rbrack; cancelar a exportação via Python retorna um erro de exceção
* &amp;lbrack;Python&amp;rbrack;&amp;lbrack;Export&amp;rbrack; export_project_textura resultado incorreto com o formato de arquivo psd
* &amp;lbrack;Baker&amp;rbrack; Falha no Linux com Rastreamento de raios do GPU

**Problemas Conhecidos:**

* &amp;lbrack;JavaScript&amp;rbrack; Não é possível editar as novas configurações de baker de curvatura
* &amp;lbrack;JavaScript&amp;rbrack;&amp;lbrack;Exportar&amp;rbrack; Sempre exporta todos os conjuntos de texturas
* &amp;lbrack;Export&amp;rbrack;&amp;lbrack;USD&amp;rbrack; Não deve exportar os conjuntos de texturas desativados
* &amp;lbrack;Crash&amp;rbrack; Alterar sombreador depois de pintar uma máscara em camadas de material

### 6.1.0 (2020.1.0)

*(Lançado: 22 de abril de 2020*)Resumo: **Versão principal com nova textura e exportador de malha (com deslocamento e mosaico), desencapsulamento UV atualizado com mais controles, novos baker, nova API python de script, melhor UX para projeção de decalques e novo conteúdo**

**Adicionado:**

* Nova textura e exportador de malha
* &amp;lbrack;Exportar&amp;rbrack; Nova interface de exportador
* &amp;lbrack;Export&amp;brack;&amp;lbrack;Guia Exportar&amp;rbrack; Permite a seleção dos canais de mapas que são exportados por Conjunto de Textura
* &amp;lbrack;Export&amp;brack;&amp;lbrack;Guia Exportar&amp;rbrack; Permite a modificação do tamanho do Conjunto de Textura para todos os Conjuntos de Textura em uma ação
* &amp;lbrack;Export&amp;brack;&amp;lbrack;Guia Exportar&amp;rbrack; Permite um modelo diferente por Conjunto de Textura (exceto para USD, glTF, Sketchfab e Dimension)
* &amp;lbrack;Export&amp;brack;&amp;lbrack;Guia Exportar&amp;rbrack; Ativação e desativação rápidas de mapas e Conjuntos de texturas
* &amp;lbrack;Export&amp;brack;&amp;lbrack;Guia Exportar&amp;rbrack; A resolução de exportação 8192x8192 não é mais experimental
* &amp;lbrack;Export&amp;brack;&amp;lbrack;Guia Exportar&amp;rbrack; Permite a modificação do formato do arquivo e a profundidade de bits por mapa
* &amp;lbrack;Export&amp;brack;&amp;lbrack;Guia Exportar&amp;rbrack; Permitir redefinição para os valores de parâmetros padrão
* &amp;lbrack;Export&amp;brack;&amp;lbrack;Guia Exportar&amp;rbrack; Permite que as configurações sejam salvas sem exportar
* &amp;lbrack;Exportar&amp;rbrack;&amp;lbrack;guia Modelos de saída&amp;rbrack; Renomeia a guia “Configuração” para a guia “Modelos de saída”
* &amp;lbrack;Export&amp;brack;&amp;lbrack;guia Modelos de saída&amp;rbrack; Permitir definição de formato de arquivo e profundidade de bits por mapa predefinido
* &amp;lbrack;Export&amp;brack;&amp;lbrack;Lista de guias de exportação&amp;rbrack; Nova guia de visualização para resumir e visualizar o processo de exportação
* &amp;lbrack;Importar/Exportar malha&amp;rbrack; Otimização do desempenho do tempo de importação/exportação
* &amp;lbrack;Exportar malha&amp;rbrack; Exportar malha em FBX
* &amp;preto;Exportar malha&amp;rbrack; Exportar malha com deslocamento e mosaico
* &amp;lbrack;Exportar malha&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Novas configurações para recalcular o vértice normal, aplicar triangulação
* &amp;lbrack;Exportar malha&amp;rbrack; Exportar topologia de malha original com novos UVs gerados pelo desencapsulamento automático
* Desencapsulamento automático UV atualizado com mais controles
* &amp;lbrack;Desempacotamento UV&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Adicionar configuração para ativar o desempacotamento UV automático na nova janela do projeto
* &amp;lbrack;UV Unwrapping&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Novas opções para controlar as etapas de abertura (emendas, abertura, embalagem)
* &amp;lbrack;Desempacotamento UV&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Permitir a conservação de emendas/desempacotamento/embalagem de abertura existentes
* &amp;lbrack;Desempacotamento UV&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Novas opções para recalcular totalmente as etapas de desempacotamento
* &amp;lbrack;UV Unwrapping&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Nova Opção para controlar o tamanho da margem (nenhum, pequeno, médio e grande)
* Novos Baker
* &amp;lbrack;Baker&amp;rbrack; Substituir a curvatura antiga pela nova curvatura da malha
* &amp;lbrack;Baker&amp;rbrack; Adicionar a opção corresponder pelo nome para ignorar a face de fundo no baker “Oclusão de ambiente”
* &amp;lbrack;Baker&amp;rbrack; Adicionar opção de plano horizontal no baker “Oclusão de ambiente”
* Nova API de script do Python (3.7.6)
* &amp;lbrack;Python&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Novo menu de scripts para Python
* &amp;lbrack;Python&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Nova documentação em Python no menu Ajuda
* &amp;lbrack;Python&amp;rbrack; Expor módulos Substance Painter python: substance_painter, alg, display, project.setting, project, texturesets, ui
* &amp;lbrack;Python&amp;rbrack; Expor novo módulo Python “substance_painter”
* &amp;lbrack;Python&amp;rbrack; Expor novo submódulo Python: alg, display, log, projeto, recurso, conjuntos de texturas, ui
* &amp;lbrack;Python&amp;rbrack; Ouvinte para alterações no projeto
* &amp;lbrack;Python&amp;rbrack; Novos exemplos na documentação do Python
* &amp;lbrack;JavaScript&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Menu de plug-ins substituído pelo JavaScript
* &amp;lbrack;Viewport&amp;rbrack; Permitir a criação de uma projeção de decalque “arrastando/soltando + ALT” um recurso da prateleira
* Novo conteúdo
* &amp;lbrack;Content&amp;brack; 5 novos materiais de decalque do Substance Source
* &amp;lbrack;Content&amp;brack; Adicionar novos modelos de projeto e exportar predefinições para o renderizador Maxwell
* &amp;lbrack;Content&amp;brack; Adicionar modelo de projeto para exportação do Keyshot 9
* &amp;lbrack;Content&amp;rbrack; Atualizar a predefinição de exportação do Keyshot 9 para suportar deslocamento e emissivo
* &amp;lbrack;Conteúdo&amp;rbrack;&amp;lbrack;Exportador&amp;rbrack; Atualização de todas as predefinições de exportação para corresponder às versões mais recentes dos mecanismos de jogo e renderizadores
* &amp;lbrack;Content&amp;rbrack;&amp;lbrack;Exportador&amp;rbrack; Atualiza arquivos de predefinições de exportação para usar o novo formato e configurações de pontilhamento
* &amp;lbrack;Content&amp;rbrack; Novos modelos e sombreadores para suportar material VRay (VRayMtl)
* &amp;lbrack;Pilha de camadas&amp;rbrack; Permitir exclusão de efeitos de camada usando ícone de lixeira ou atalho de teclado Excluir
* Remover o Substance Source de plug-in (use o iniciador com a funcionalidade “enviar para”)
* &amp;lbrack;Windows&amp;rbrack; Não exibir aviso TDR em GPUs sofisticadas

**Corrigido:**

* Problemas de tradução na caixa de diálogo Novo arquivo de projeto
* &amp;lbrack;Baker&amp;rbrack; Configurar “Salvar arquivo de cena pré-processado” não funciona mais
* &amp;lbrack;Projeção Planar&amp;rbrack; A projeção não funciona em malhas com UVs repetidos
* &amp;lbrack;Decalque&amp;rbrack; Diferença de comportamento no canal normal ao usar modos diferentes de projeção da camada de preenchimento
* &amp;lbrack;Borrar&amp;rbrack;&amp;lbrack;Clonar&amp;rbrack; O artefato pode aparecer ao pintar na máscara
* &amp;lbrack;Engine&amp;brack; Falha com conteúdo de camada específico
* &amp;lbrack;Engine&amp;rbrack; Falha aleatória ao pintar em alguns casos
* &amp;preto;Ponto de ancoragem&amp;rbrack; A referência a uma máscara vazia sempre retorna branco
* &amp;lbrack;Export&amp;brack; Camada não considerada em algumas configurações de pilha específicas
* &amp;lbrack;Exportar malha&amp;rbrack; Não é possível exportar com caminho que contém caracteres especiais
* &amp;lbrack;Exportar malha&amp;rbrack; Não é possível ler arquivos glTF quando exportados do Linux ou MacOS
* &amp;lbrack;Importar malha&amp;rbrack; Reimportar DAE, PLY ou glTF não funciona como pretendido

**Problemas Conhecidos:**

* &amp;lbrack;Scripting&amp;rbrack;&amp;lbrack;JavaScript&amp;rbrack; Não é possível editar as novas configurações de baker de curvatura
* &amp;lbrack;Baker&amp;rbrack; Falha no Linux com Rastreamento de raios do GPU
* &amp;lbrack;Export&amp;rbrack;&amp;lbrack;USD&amp;rbrack; Não deve exportar os conjuntos de texturas desativados
* &amp;lbrack;Crash&amp;rbrack; Alterar sombreador depois de pintar uma máscara em camadas de material

## Versão 5

### 5.3.3 (2019.3.3)

*(Lançado em: 06 de fevereiro de 2020*)Resumo: **Correção de erros com a atualização para o Iray 2019.3**

**Adicionado:**

* Atualização para o Iray 2019.3
* &amp;lbrack;Log&amp;rbrack; Indica bios desatualizado para CPU Ryzen levando a falha durante fça bake
* &amp;lbrack;ABR&amp;rbrack; Extrair ABR alfa para prateleira

**Corrigido:**

* &amp;lbrack;Baker&amp;rbrack; falha na Faz bake se a malha de alto-polígono não tiver UVs
* &amp;lbrack;Linux&amp;rbrack; Os atalhos de mouse personalizados não são salvos
* &amp;lbrack;Pincel&amp;rbrack; O contorno desaparece com algumas formas alfa
* &amp;lbrack;Tablet&amp;rbrack; Detecção incorreta ao mover controles deslizantes
* &amp;lbrack;Atalhos&amp;rbrack; Não é possível configurar nenhum atalho com “Ctrl+Alt+MouseClick”
* &amp;lbrack;Shelf&amp;rbrack; Não é possível ver a dica de ferramenta do recurso ao usar um tablet com caneta
* A predefinição &amp;lbrack;Visualização 2D&amp;rbrack;&amp;lbrack;Export&amp;rbrack; não leva em consideração as informações normais
* Congela ao pintar em alinhamento UV com determinados pincéis
* Pintar sob um filtro cria artefatos no traçado em andamento
* &amp;lbrack;Visor&amp;rbrack; Cache de textura incorreto no visor após a reimportação de uma malha
* &amp;lbrack;Crash&amp;rbrack; Erro ao salvar após exportar para o Photoshop
* &amp;lbrack;Crash&amp;rbrack; Gravando símbolos especiais no prefixo ao importar recursos
* &amp;lbrack;Crash&amp;rbrack; Clique na referência nas Propriedades do Ponto de Ancoragem
* &amp;preto;Pontos de ancoragem&amp;rbrack; O canal não é atualizado quando há um filtro entre o ponto de ancoragem e a referência
* O link de URL do Iray no menu Ajuda não funciona

**Problemas Conhecidos:**

* &amp;lbrack;Desempacotamento UV&amp;rbrack; O processamento de malhas de alta polarização pode demorar muito tempo
* &amp;lbrack;Desempacotamento UV&amp;rbrack; Vértices nas mesmas coordenadas são mesclados
* &amp;lbrack;Desempacotamento UV&amp;rbrack; A Geração UV pode falhar em algumas partes da malha em alguns casos raros
* &amp;lbrack;UV Unwrapping&amp;rbrack; Proporção de texel não uniforme ou altamente distorcida em uma única Ilha UV em alguns casos
* &amp;lbrack;Desempacotamento UV&amp;rbrack; Proporção de texel não uniforme entre Conjuntos de Textura
* A Ilha UV gerada pelo &amp;lbrack;UV Unwrapping&amp;rbrack; pode ser muito alongada e, em alguns casos, não cabe no espaço UV
* &amp;preto;Desempacotamento UV&amp;rbrack; Faces degeneradas ou faces de malha não triangulares com bordas pequenas ou sobrepostas podem não ter o UV desempacotado

### 5.3.2 (2019.3.2)

*(Lançado: 21 De Janeiro De 2020*)Resumo: **Correção De Erros**

**Corrigido:**

* Abrir um projeto que foi salvo no modo de canal individual não exibe a malha
* A janela de visualização nem sempre é atualizada ao pintar sob uma camada usando a ferramenta clone

**Problemas Conhecidos:**

* &amp;lbrack;Baker&amp;rbrack; Falha relacionada a multi-threading em CPUs Ryzen
* &amp;lbrack;Desempacotamento UV&amp;rbrack; O processamento de malhas de alta polarização pode demorar muito tempo
* &amp;lbrack;Desempacotamento UV&amp;rbrack; Vértices nas mesmas coordenadas são mesclados
* &amp;lbrack;Desempacotamento UV&amp;rbrack; A Geração UV pode falhar em algumas partes da malha em alguns casos raros
* &amp;lbrack;UV Unwrapping&amp;rbrack; Proporção de texel não uniforme ou altamente distorcida em uma única Ilha UV em alguns casos
* &amp;lbrack;Desempacotamento UV&amp;rbrack; Proporção de texel não uniforme entre Conjuntos de Textura
* A Ilha UV gerada pelo &amp;lbrack;UV Unwrapping&amp;rbrack; pode ser muito alongada e, em alguns casos, não cabe no espaço UV
* &amp;preto;Desempacotamento UV&amp;rbrack; Faces degeneradas ou faces de malha não triangulares com bordas pequenas ou sobrepostas podem não ter o UV desempacotado

### 5.3.1 (2019.3.1)

*(Lançado: 20 De dezembro De 2019*)Resumo: **Hotfix**

**Corrigido:**

* Falha ao trabalhar em malhas com Projeções UV específicas
* &amp;lbrack;ABR&amp;rbrack; Falha ao alternar entre predefinições Photoshop
* &amp;lbrack;Linux&amp;rbrack; Não é possível iniciar o Substance Painter no CentOS 7.4 devido a um problema de dependência do libGLX
* &amp;lbrack;Baker&amp;rbrack; Falha ao fazer bake após usar Arquivo > Limpar
* &amp;lbrack;Baker&amp;rbrack; Fazendo bake o diálogo de progresso congela após cancelar
* &amp;lbrack;Baker&amp;rbrack; Fazer bake a malha após exportar as texturas não funciona
* &amp;lbrack;Baker&amp;rbrack; Usar “Corresponder por nome” resulta com mapas de malha pretos
* &amp;lbrack;Baker&amp;rbrack; A gaiola não é levada em consideração
* &amp;lbrack;Shelf&amp;rbrack; Importar arquivos de PSD leva a imagens quebradas
* &amp;lbrack;Amostra&amp;rbrack; O projeto de amostra “Mat” possui câmeras quebradas e predefinição de exportação incorreta

**Problemas Conhecidos:**

* &amp;lbrack;Baker&amp;rbrack; Falha relacionada a multi-threading em CPUs Ryzen
* &amp;lbrack;Desempacotamento UV&amp;rbrack; O processamento de malhas de alta polarização pode demorar muito tempo
* &amp;lbrack;Desempacotamento UV&amp;rbrack; Vértices nas mesmas coordenadas são mesclados
* &amp;lbrack;Desempacotamento UV&amp;rbrack; A Geração UV pode falhar em algumas partes da malha em alguns casos raros
* &amp;lbrack;UV Unwrapping&amp;rbrack; Proporção de texel não uniforme ou altamente distorcida em uma única Ilha UV em alguns casos
* &amp;lbrack;Desempacotamento UV&amp;rbrack; Proporção de texel não uniforme entre Conjuntos de Textura
* A Ilha UV gerada pelo &amp;lbrack;UV Unwrapping&amp;rbrack; pode ser muito alongada e, em alguns casos, não cabe no espaço UV
* &amp;preto;Desempacotamento UV&amp;rbrack; Faces degeneradas ou faces de malha não triangulares com bordas pequenas ou sobrepostas podem não ter o UV desempacotado

### 5.3.0 (2019.3.0)

*(Lançado em: 17 de dezembro de 2019*)Resumo: **Versão principal com aprimoramento da experiência do usuário de pintura manual, trabalho com tablets, desencapsulamento UV automático em beta (0.3.0) e conteúdo novo diversificado para pintura manual**

**Adicionado:**

* Integrar a versão 0.3.0 de desenrolamento automático de UV no Substance Painter
* &amp;lbrack;Desencapsulamento UV&amp;rbrack; Desencapsulamento UV automático no Substance Painter quando nenhum UV estiver presente ou UVs parciais
* &amp;lbrack;UV unwrapping&amp;rbrack; Uma configuração global para ativá-lo e desativá-lo
* &amp;lbrack;UV unwrapping&amp;rbrack; Versão relatada no arquivo de registro
* &amp;lbrack;Desempacotamento UV&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Indicar progresso do Desempacotamento UV
* &amp;lbrack;UI&amp;rbrack; Novas configurações na barra de ferramentas contextual para selecionar a visualização do pincel: visualização completa, contorno e mira
* &amp;lbrack;Tool&amp;brack; Novo modo de mesclagem avançado na seção alfa: Clarear (máximo) além de Normal
* &amp;lbrack;Pilha de camadas&amp;rbrack; Opção de correção de gama por camada para alfa ou máscara (menu do botão direito do mouse)
* &amp;lbrack;Pilha de camadas&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Adicionar ícone &#39;i&#39; quando uma camada alfa for corrigida quanto à gama
* &amp;lbrack;Tablet&amp;rbrack;&amp;lbrack;Tool&amp;rbrack; Expor pressão mínima para tamanho e fluxo
* &amp;lbrack;Tablet&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Nova configuração na barra de ferramentas contextual para selecionar a pressão da curva: linear, fácil de entrar, fácil de sair
* &amp;lbrack;Tablet&amp;rbrack;&amp;lbrack;UX&amp;rbrack; Add Ctrl+Alt+clique para rolar
* Importar predefinições de pincel do Photoshop (formato ABR)
* &amp;lbrack;ABR&amp;rbrack; Suporte parâmetros de Forma
* &amp;lbrack;ABR&amp;rbrack; Suportar parâmetros de dinâmica da forma
* &amp;lbrack;ABR&amp;rbrack; Suporte Parâmetros de transferência
* &amp;lbrack;ABR&amp;rbrack; Suporte a parâmetros de dispersão
* &amp;lbrack;ABR&amp;rbrack;&amp;lbrack;Traçados dinâmicos&amp;rbrack; Suporte Arredondamento e inversão
* &amp;lbrack;ABR&amp;rbrack;&amp;lbrack;Shelf&amp;rbrack; Expor a estrutura da pasta de pincéis no Editor de Filtros
* &amp;lbrack;Abr&amp;brack;&amp;lbrack;Prateleira&amp;rbrack; Adicionar ícone do Photoshop em miniaturas
* &amp;lbrack;ABR&amp;rbrack;&amp;lbrack;Shelf&amp;rbrack; Adicionar lista de parâmetros não suportados na miniatura detalhada do ABR
* &amp;lbrack;Tool&amp;brack;&amp;lbrack;Traçados dinâmicos&amp;rbrack; Nova configuração de traçado dinâmico para controlar quantas sementes aleatórias gerar
* &amp;lbrack;Tool&amp;brack;&amp;lbrack;UI&amp;rbrack; Adicionar nova distribuição e configurações de eixo para dispersão de tremulação
* &amp;lbrack;Atalho&amp;rbrack; Adicione Ctrl+Shift+B para abrir a janela de Fça bake
* &amp;lbrack;UI&amp;rbrack;&amp;lbrack;Menu&amp;rbrack; Adicionar entrada no menu “Editar” para abrir a janela de Fça bake
* &amp;lbrack;UI&amp;rbrack;&amp;lbrack;Configurações&amp;rbrack; Aprimoramento do alinhamento da lista de atalhos
* &amp;lbrack;UI&amp;rbrack; Substitui ícones de controles de pressão (tamanho e fluxo) por botões de ligar/desligar
* &amp;lbrack;Visor&amp;rbrack; Permitir focalizar o visor 2D e 3D separadamente
* Atualize para QT 5.12.5
* &amp;lbrack;UI&amp;rbrack; Indicar progresso do carregamento da malha
* &amp;lbrack;Substance&amp;rbrack; Adicionar suporte para faixa suave e não fixa com controles deslizantes
* &amp;lbrack;Substance&amp;rbrack; Aumenta a precisão dos parâmetros Substance até 6 decimais
* &amp;lbrack;Substance&amp;rbrack; Leve em consideração a etapa definida por um parâmetro
* &amp;lbrack;Substance&amp;rbrack; Otimizar a geração de Traçado Dinâmico com suporte de condições em userdata
* &amp;lbrack;Substance&amp;rbrack; Permite designar uma saída de gráfico como uma máscara para todos os canais via userdata
* &amp;lbrack;Content&amp;rbrack; Atualizar projeto de amostra &#39;Mat&#39; com topologia amigável ao deslocamento, novo mapa de ID e novas câmeras
* &amp;lbrack;Content&amp;brack; Integrar 3 novos filtros (MatFx): Quadrinhos, Aquarela, Tinta a óleo (inspirado no trabalho de Emrecan Cubukcu)
* &amp;brack;Content&amp;brack; Integra 102 predefinições de pincel Photoshop dos pacotes de Kyle T. Webster
* &amp;lbrack;Content&amp;brack; Integrar 18 novas predefinições de pincel: Seta do rolo de Tinta, Texto de aviso do rolo de Tinta, Carvão fino e muito mais
* &amp;brack;Content&amp;brack; Integrar 9 novas alfas: Rolo de Tinta do Criador de Pincel, Photoshop do Criador de Pincel, Padrões de pincel e muito mais
* &amp;lbrack;Content&amp;brack; Integrar 2 novas predefinições de ferramenta: Guache Dense e Gouache Faded
* &amp;lbrack;Content&amp;brack; Integrar 1 novo gerador : verificador UV (realçar Ilhas UV e emendas)
* &amp;lbrack;Content&amp;brack; Integrar 2 nova predefinição de exportação: Keyshot 9+ e Spark AR Studio
* &amp;lbrack;Content&amp;brack; Integrar 1 novo modelo de projeto : Spark AR Studio (Facebook)

**Corrigido:**

* &amp;preto;Tablet&amp;rbrack; Desfazer traçados da caneta (Ctrl+Z) atrasa mais do que desfazer traçados do mouse
* &amp;lbrack;Tablet&amp;rbrack; A pressão inicial e final não é considerada ao desenhar uma linha reta
* &amp;lbrack;Tablet&amp;rbrack; O primeiro carimbo é desenhado duas vezes ao usar uma linha reta
* &amp;Preenchimento;Tablet&amp;rbrack; Melhorar o suporte para atalhos de tablet Huion
* &amp;lbrack;Tablet&amp;rbrack; Melhorar o suporte para botões de caneta Huion
* &amp;preto;Tablet&amp;rbrack; Deslocamento entre a visualização do pincel e o carimbo desenhado
* &amp;Preenchimento;O uso do tablet&amp;rbrack; atalhos para modificar pincéis com caneta leva a baixo desempenho em casos raros
* &amp;lbrack;Tablet&amp;rbrack; Atraso ao pintar em uma camada específica
* Texturas embaçadas podem ocorrer em casos raros ao alternar entre viewport
* &amp;lbrack;UI&amp;rbrack;&amp;lbrack;Substance&amp;rbrack; As entradas de imagem nem sempre são exibidas
* Limpar não remove as predefinições da prateleira que foram importadas em um projeto
* &amp;lbrack;Tool&amp;rbrack;&amp;lbrack;Dynamic Stroke&amp;rbrack; Problema de desempenho ao ajustar a Contagem Cíclica do Carimbo
* Problemas de atualização ao pintar no modo de visor 3D/2D em casos raros
* Pintar um traçado muito longo pode causar congelamento
* &amp;lbrack;Tool&amp;brack; Problema de desempenho ao pintar com traçados dinâmicos específicos
* &amp;lbrack;UI&amp;rbrack; A barra de ferramentas contextual ainda exibe as propriedades do pincel ao selecionar uma pasta
* Os valores do eixo de simetria não são redefinidos
* A importação de texturas EXR com valores de ponto flutuante é totalmente preta
* Alt+clique em um canal para isolar não funciona para filtro e gerador
* &amp;lbrack;Export&amp;brack; O projeto específico falha na exportação
* &amp;lbrack;Substance&amp;rbrack; Valor padrão incorreto na lista suspensa se o parâmetro estiver oculto por Visível Se
* &amp;lbrack;Sombreador&amp;rbrack; Os canais definidos por meio da Camada de material não são classificados da mesma maneira na interface
* &amp;lbrack;Shelf&amp;rbrack; Os metadados de predefinições não são salvos no disco

**Problemas Conhecidos:**

* &amp;lbrack;Desempacotamento UV&amp;rbrack; O processamento de malhas de alta polarização pode demorar muito tempo
* &amp;lbrack;Desempacotamento UV&amp;rbrack; Vértices nas mesmas coordenadas são mesclados
* &amp;lbrack;Desempacotamento UV&amp;rbrack; A Geração UV pode falhar em algumas partes da malha em alguns casos raros
* &amp;lbrack;UV Unwrapping&amp;rbrack; Proporção de texel não uniforme ou altamente distorcida em uma única Ilha UV em alguns casos
* &amp;lbrack;Desempacotamento UV&amp;rbrack; Proporção de texel não uniforme entre Conjuntos de Textura
* A Ilha UV gerada pelo &amp;lbrack;UV Unwrapping&amp;rbrack; pode ser muito alongada e, em alguns casos, não cabe no espaço UV
* &amp;preto;Desempacotamento UV&amp;rbrack; Faces degeneradas ou faces de malha não triangulares com bordas pequenas ou sobrepostas podem não ter o UV desempacotado
* A amostra do metamat tem alguns problemas com câmeras importadas

### 5.2.3 (2019.2.3)

*(Lançado: 23 de outubro de 2019*)Resumo: **Versão de correção de erros**

**Adicionado:**

* &amp;preto;Textura Definir lista&amp;rbrack; Adicionar botão para ativar/desativar rapidamente o modo de foco
* &amp;lbrack;Log&amp;rbrack; Adicionar o número de versão do Windows 10 no arquivo de log
* Atualize para a versão mais recente do Substance Engine
* &amp;lbrack;MacOS&amp;rbrack; Autenticou o software para seguir os novos requisitos de distribuição do MacOS Catalina

**Corrigido:**

* O código-fonte do plug-in do &amp;lbrack;Plugin&amp;brack; não funciona
* &amp;lbrack;MacOS&amp;rbrack;&amp;lbrack;Sombreador&amp;rbrack; Mac OS 10.14.5 e AMD: a disposição em camadas de material não funciona conforme o esperado

**Problemas Conhecidos:**

* Arquivos Alembic com subdivisões não podem ser importados
* Falhas raras ao importar alguns arquivos Alembic
* A interface não responde temporariamente ao fazer bake com DXR em GPUs Pascal

### 5.2.2 (2019.2.2)

*(Lançado: 20 de setembro de 2019*)Resumo: **Versão de correção**

**Corrigido:**

* A importação de recursos por scripts pode causar uma falha
* &amp;lbrack;Plug-in&amp;rbrack; Baixar material da origem pode levar a um travamento

**Problemas Conhecidos:**

* Arquivos Alembic com subdivisões não podem ser importados
* Falhas raras ao importar alguns arquivos Alembic
* A interface não responde temporariamente ao fazer bake com DXR em GPUs Pascal

### 5.2.1 (2019.2.1)

*(Lançado em: 17 de setembro de 2019*)Resumo: **Versão de correção**

**Corrigido:**

* &amp;lbrack;Mac&amp;rbrack;&amp;lbrack;USD&amp;rbrack; Os arquivos USDZ exportados do MacOS não podem ser abertos
* &amp;lbrack;Conjunto de texturas&amp;rbrack; Não é possível isolar um conjunto de texturas com o modificador ALT
* &amp;preto;Prateleira&amp;rbrack; Predefinições, Materiais inteligentes e Máscaras inteligentes são sempre modificados ao sair do aplicativo
* &amp;lbrack;Pilha de camadas&amp;rbrack; Não é possível selecionar o efeito após excluir outro efeito
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

* &amp;lbrack;Baker&amp;rbrack; Adicionado suporte para Rastreamento de raios do GPU com DXR e OptiX (Oclusão de ambiente, Thickness)
* &amp;lbrack;Baker&amp;rbrack; Otimizações e acelerações para Rastreamento de raios da CPU
* &amp;lbrack;Baker&amp;rbrack;&amp;lbrack;Modo Vis&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Novo modo de visualização de fça bake no visor
* &amp;lbrack;Baker&amp;rbrack;&amp;lbrack;Preferências&amp;rbrack;&amp;lbrack;IU&amp;rbrack; Nova opção de fça bake para ativar/desativar o Rastreamento de raios do GPU
* &amp;lbrack;Baker&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Retrabalho da caixa de diálogo da barra de progresso
* &amp;lbrack;Baker&amp;rbrack; Aprimoramento de mensagens de aviso e erro
* &amp;lbrack;Baker&amp;rbrack; Permitir cancelamento mais responsivo do processo de fça bake
* &amp;lbrack;Baker&amp;rbrack; Reabrir janela fazer bake após clicar em cancelar
* &amp;lbrack;Proj&amp;rbrack;&amp;lbrack;UX&amp;rbrack; Melhoria da usabilidade do manipulador de rotação
* &amp;lbrack;Settings&amp;brack; Opção para melhorar o desempenho reduzindo a resolução do visor para telas HDPI
* &amp;preto;Script&amp;rbrack; Alterar resolução do conjunto de texturas
* &amp;lbrack;Scripting&amp;brack; Obter conjunto de textura selecionado
* &amp;lbrack;Scripting&amp;brack; Permite que o usuário selecione um conjunto de texturas
* &amp;lbrack;Scripting&amp;rbrack; Função para saber quando a seleção do conjunto de texturas foi alterada
* &amp;lbrack;Prateleira&amp;rbrack; Adicionados 40 novos materiais inteligentes
* &amp;lbrack;Prateleira&amp;rbrack; Adicionadas 20 novas máscaras inteligentes

**Corrigido:**

* &amp;lbrack;Pilha de camadas&amp;rbrack; Congelamento de interface ao selecionar várias camadas
* &amp;lbrack;Pilha de camadas&amp;rbrack; Agrupar muitas camadas congela a interface por mais tempo do que o normal
* &amp;lbrack;Pilha de camadas&amp;rbrack; Uma camada e um efeito podem ser selecionados ao mesmo tempo em alguns casos
* os gráficos de Substance usados nas ferramentas de pintura não são gerados na resolução correta
* &amp;lbrack;Baker&amp;rbrack; o botão “Fazer bake todos os conjuntos de textura” não é desativado quando nenhum baker é selecionado
* &amp;lbrack;MacOS&amp;rbrack; Desativa a mensagem de aviso sobre o mosaico
* A ferramenta de projeção não tem visualização quando usada com uma máscara
* Falha e projetos corrompidos ao tentar salvar com espaço em disco insuficiente
* &amp;lbrack;Shelf&amp;rbrack; Falha ao importar um recurso em disco via prateleira com espaço insuficiente
* &amp;lbrack;Shelf&amp;rbrack; Falha ao restaurar a predefinição de sessão
* &amp;preset;Shelf&amp;rbrack; Importar uma predefinição com um nome que termine com um espaço leva a um travamento
* &amp;lbrack;Shelf&amp;rbrack; Importar um recurso com um prefixo que termine com um espaço vazio leva a um travamento

**Problemas Conhecidos:**

* Arquivos Alembic com subdivisões não podem ser importados
* Falhas raras ao importar alguns arquivos Alembic
* A interface não responde temporariamente ao fazer bake com DXR em GPUs Pascal

### 5.1.3 (2019.1.3)

*(Lançado em: 01 de julho de 2019*)Resumo: **Correção de erro com 2 novos recursos**

**Adicionado:**

* Permite especificar o orçamento VRam com uma linha de comando (por exemplo, —vram-budget 4096)
* &amp;lbrack;QML&amp;rbrack; Expor as propriedades wrapMode e elide dos botões e caixas de verificação QML

**Corrigido:**

* “Seguir caminho” não funciona o tempo todo
* O mapeamento de canal não funciona com SBSAR usado em slots de canal único
* &amp;lbrack;Pilha de camadas&amp;rbrack; Baixo desempenho ao rolar com camadas ocultas
* &amp;lbrack;TextureSet&amp;rbrack; Falha ao clicar entre máscaras
* &amp;lbrack;SVT&amp;rbrack; Deslocamento não exibido corretamente e pisca em alguns casos
* &amp;lbrack;Alembic&amp;rbrack; Falha com malha usando normais de ponto em vez de normais de vértice
* &amp;lbrack;Alembic&amp;rbrack;&amp;lbrack;Log&amp;rbrack; Relatar erro no Log se o arquivo Alembic não for suportado durante a importação

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

* &amp;lbrack;Substance&amp;rbrack; Visível Se não for levado em conta para Imagens de Entrada
* &amp;lbrack;SVT&amp;rbrack;&amp;lbrack;Engine&amp;rbrack; Alterar a resolução do conjunto de texturas leva a uma falha em alguns casos
* &amp;lbrack;Engine&amp;rbrack; texturas pretas aleatórias aparecem em alguns casos
* &amp;lbrack;Pilha de camadas&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Alternar uma máscara com SHIFT pode selecionar várias camadas ao mesmo tempo
* &amp;lbrack;Pilha de camadas&amp;rbrack; A opacidade não tem efeito sobre o efeito de Tinta com o modo de mesclagem Passagem
* A entrada do filtro &amp;lbrack;Pilha de camadas&amp;rbrack; Height para Normal não é atualizada corretamente com a pincelada de borracha
* &amp;lbrack;LayersStack&amp;rbrack; Falha ao desfazer o descarte de uma máscara inteligente
* Wireframe piscando com sombras e suavização de borda temporal ativada
* &amp;lbrack;Deslocamento&amp;rbrack; Atraso na AMD com algumas malhas pesadas
* &amp;lbrack;Windows&amp;rbrack; Falha ao abrir alguns projetos através do explorador de arquivos
* &amp;lbrack;Histograma&amp;rbrack; Falha ao remover a máscara com o ponto de ancoragem em alguns casos
* Falha na geração de visualização em alguns casos raros
* &amp;lbrack;Crash&amp;rbrack; Não é possível reabrir um projeto usando muitas ferramentas de clonar e borrar
* Nenhuma malha exibida no modo de material após salvar em alguns casos
* &amp;lbrack;Scripting&amp;brack; alg.mapexport.documentStructure() retorna valores incorretos para pastas

**Problemas Conhecidos:**

* Clicar duas vezes no nome do conjunto de texturas o selecionará antes de entrar no modo de renomeação

### 5.1.0 (2019.1.0)

*(Lançado: 23 de abril de 2019*)Resumo: **Traço dinâmico com novo conteúdo dedicado, Deslocamento e mosaico em tempo real e Iray, efeito Comparar máscara, simetria radial, Planar e Projeção esférica**

**Adicionado:**

* &amp;lbrack;Tool&amp;brack; Traço dinâmico: variação de Substance ao lado de uma pincelada
* &amp;preto;Traço dinâmico&amp;rbrack; Expor novo parâmetro de índice de carimbo com opções
* &amp;preto;Traço dinâmico&amp;rbrack; Leve em consideração o parâmetro $time
* &amp;preto;Traço dinâmico&amp;rbrack; Gerar novo parâmetro $randomseed por traço e por carimbo
* &amp;preto;Traço dinâmico&amp;rbrack; Inicia um índice de traçado dinâmico a partir de um número aleatório
* &amp;lbrack;Traço dinâmico&amp;rbrack;&amp;lbrack;Prateleira&amp;rbrack; Ajuda para encontrar um recurso de traço dinâmico com um novo ícone dedicado
* Deslocamento e mosaico em viewport em tempo real
* Deslocamento e mosaico em Irlanda
* &amp;lbrack;configurações de Sombreador&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Nova guia para controlar deslocamento e mosaico
* &amp;lbrack;Pilha de camadas&amp;rbrack; Novo efeito CompararMáscara: gerar uma máscara comparando dois canais
* &amp;lbrack;Pilha de camadas&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Nova entrada no menu do botão direito do mouse “Adicionar máscara com combinação de height” para inserir um efeito CompararMáscara
* &amp;lbrack;Simetria&amp;rbrack; Novo modo de simetria: pintura radial
* &amp;preto;Configurações de Simetria&amp;rbrack; Expande as duas seções “Configurações” e “Exibição”
* &amp;lbrack;configurações de Simetria&amp;rbrack;&amp;lbrack;IU&amp;rbrack; Visualizar para pintura radial
* Exponha dois novos modos de projeção: planar e esférico
* &amp;lbrack;Proj&amp;rbrack; Novo modo de corte de forma para todas as projeções
* &amp;lbrack;Proj&amp;rbrack; modo Planar com nova manipulador: ferramenta Superfície
* &amp;lbrack;Proj&amp;rbrack;&amp;lbrack;Atalho&amp;rbrack; Atalho SHIFT+W para a ferramenta Superfície
* &amp;lbrack;Proj&amp;rbrack; máscara de projeção Planar com remoção de seleções de profundidade e backface
* &amp;lbrack;Manipulador&amp;rbrack; Melhoria do manipulador de rotação em todos os três eixos para triplanar
* &amp;lbrack;Tool&amp;rbrack;&amp;lbrack;UX&amp;rbrack; clicar com a tecla Alt pressionada em um canal focaliza esse canal (ativa ou desativa todos os outros)
* &amp;lbrack;Engine&amp;rbrack; Atualiza para a versão mais recente do Substance Engine
* &amp;preto;Conjunto de texturas&amp;rbrack; Seleção múltipla e alterar resolução
* &amp;lbrack;Conjunto de texturas&amp;rbrack; Ativação e desativação rápidas dos conjuntos de texturas
* &amp;preto;Conjunto de texturas&amp;rbrack; Combina solo e todas as opções em um novo menu
* &amp;lbrack;Conjunto de texturas&amp;rbrack;&amp;lbrack;Pilha de camadas&amp;rbrack; Novo ícone para ativação e desativação
* &amp;lbrack;Pilha de camadas&amp;rbrack;&amp;lbrack;UX&amp;rbrack; Inserir efeitos acima dos já selecionados
* &amp;lbrack;Pilha de camadas&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Retrabalhar estilo de seleção de exibição de pilha de camadas
* O modo de mesclagem &amp;lbrack;Pilha de camadas&amp;rbrack; para camadas instanciadas agora está no modo Passagem por padrão
* &amp;lbrack;Export&amp;brack; Opção para ativar e desativar o pontilhamento
* &amp;lbrack;Plug-in&amp;rbrack; Suporte ao modificador de precisão para controles deslizantes (SHIFT)
* &amp;lbrack;Plug-in&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Novo ícone para salvamento automático
* &amp;lbrack;Scripting&amp;brack; Lista o conteúdo de uma pasta
* &amp;lbrack;Scripting&amp;brack; Permitir exclusão de arquivos
* &amp;lbrack;Scripting&amp;rbrack; Ler todas as informações da pilha, incluindo os recursos usados
* &amp;lbrack;Conteúdo&amp;rbrack;&amp;lbrack;Traço dinâmico&amp;rbrack; Novas ferramentas e predefinições de pincel
* &amp;lbrack;Content&amp;rbrack;&amp;lbrack;Traço dinâmico&amp;rbrack; Dois novos gradientes processuais: Matiz de gradiente e Construtor de gradiente
* &amp;lbrack;Content&amp;rbrack; 11 novos filtros: Tinta de descascamento MatFx, gotas de água MatFx e muito mais
* &amp;lbrack;Content&amp;rbrack; 7 novos geradores: Auto Stitcher, Cor aleatória UV, Densidade de texel UV e muito mais
* &amp;lbrack;Content&amp;brack; 93 novas alfas: novos textos, setas e várias outras formas
* &amp;lbrack;Content&amp;brack; 2 novos procedimentos: Matiz de Gradiente, Construtor de Gradiente e muito mais
* &amp;lbrack;Content&amp;brack; 21 novas predefinições de ferramenta e pincel para Traçados dinâmicos: Pebbles, Footprints, Spray e muito mais
* &amp;lbrack;Content&amp;rbrack; 2 Novos HDRis: Canopus Ground e Floresta de outono
* &amp;lbrack;Content&amp;rbrack; Atualizar conteúdo com curadoria de semente aleatória na prateleira
* &amp;lbrack;Content&amp;brack; Novo ícone com parâmetro de semente aleatório exposto na prateleira

**Corrigido:**

* &amp;preto;Pilha de camadas&amp;rbrack; a Pilha de camadas continua arrastando para sempre
* &amp;lbrack;Mac&amp;rbrack; “Mostrar no Finder” pode levar ao congelamento
* &amp;lbrack;Scripting&amp;rbrack; As configurações salvas pela interface do usuário personalizada são perdidas se o arquivo de sombreador for movido
* O número da versão da API do &amp;brack;Scripting&amp;brack; está incorreto e não está atualizado
* O conteúdo do Histograma do &amp;Preenchimento;Efeito&amp;Preenchimento; não é exibido corretamente
* O efeito do Histograma do &amp;preto;Efeito&amp;rbrack; não é atualizado em alguns casos
* &amp;lbrack;Prateleira&amp;rbrack; Os pontos não estão alinhados corretamente no material “Pirâmide de tecido plástico”

**Problemas Conhecidos:**

* Clicar duas vezes no nome do conjunto de texturas o selecionará antes de entrar no modo de renomeação
* &amp;lbrack;Pilha de camadas&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Alternar uma máscara com SHIFT pode selecionar várias camadas ao mesmo tempo

## Versão 4

### 4.3.3 (2018.3.3)

*(Lançado em: 07 de março de 2019*)Resumo: **correção de erros**

**Adicionado:**

* &amp;lbrack;Content&amp;brack; Integrar novo modelo de projeto: “PBR - Aspereza metálica Alpha-blend”
* A ordem de pesquisa da biblioteca dinâmica Linux foi alterada para priorizar as bibliotecas no diretório de instalação antes do que está instalado no sistema

**Corrigido:**

* A malha às vezes desaparece da viewport 3D (pressione F para redefinir a câmera)
* Atualize o carregador do Substance Painter Sketchfab com os novos tipos de licença do Sketchfab
* &amp;lbrack;Import&amp;rbrack;&amp;lbrack;glTF&amp;rbrack; Manipulação incorreta da modulação de textura de entrada conforme definido nos arquivos glTF
* &amp;lbrack;Import&amp;rbrack;&amp;lbrack;glTF&amp;rbrack; O plano horizontal é exibido incorretamente com a importação de glTF em alguns casos
* &amp;lbrack;Export&amp;rbrack;&amp;lbrack;USD&amp;rbrack; A opacidade não funciona no Arkit
* &amp;lbrack;Export&amp;rbrack;&amp;lbrack;USD&amp;rbrack; falhas de exportação em USDz em alguns casos
* &amp;lbrack;Export&amp;rbrack;&amp;lbrack;USD&amp;rbrack; Exportar para USD sem salvar leva a um erro fatal
* &amp;lbrack;Export&amp;rbrack;&amp;lbrack;USD&amp;rbrack; Modo de divisão em blocos gráficos incorreto para textura, modo de subdivisão para malhas e tipos de saída para sombreadores
* &amp;lbrack;Export&amp;rbrack;&amp;lbrack;USD&amp;rbrack; Exportações esparsas de apenas alguns conjuntos de texturas com toda a geometria
* &amp;lbrack;Instância&amp;rbrack; Falha ao tentar excluir uma camada de instância quebrada
* &amp;lbrack;Regressão&amp;rbrack;&amp;lbrack;Exportar&amp;rbrack; Alguns mapas não são exportados na profundidade de bits escolhida
* &amp;lbrack;Linux&amp;rbrack; Problema com a biblioteca libtbb.so.2

**Problemas Conhecidos:**

* O congelamento da computação em alguns casos em GPUs AMD VEGA
* Problema do tablet Huion com atalhos no sistema operacional Windows

### 4.3.2 (2018.3.2)

*(Lançado: 24 de janeiro de 2019*)Resumo: **Hotfix com novos recursos (exportação USDZ e filtragem de Textura no visor)**

**Adicionado:**

* &amp;preto;Exportar&amp;rbrack; Permitir exportação para USDZ
* &amp;lbrack;Visor&amp;rbrack; Permite controlar a qualidade da textura nas Configurações de exibição
* &amp;lbrack;Viewport&amp;rbrack; Adicionada configuração de polarização mip nas Configurações de Exibição
* &amp;lbrack;Visor&amp;rbrack; Adicionado filtro anisotrópico em Configurações de exibição
* &amp;lbrack;plugins&amp;rbrack; Atualize os plug-ins oficiais para usar o estilo do Substance Painter 2018
* &amp;lbrack;Licença&amp;rbrack; Instalar licença por padrão em uma pasta do usuário

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
* &amp;lbrack;Criação do caminho do arquivo &amp;rbrack; não forçada ao salvar um projeto
* &amp;lbrack;Scripting&amp;brack; O retorno de chamada “onProjectAboutToSave()” não funciona mais
* Links do fórum quebrados na janela de erro do relatório

**Problemas Conhecidos:**

* O congelamento da computação em alguns casos em GPUs AMD VEGA
* Problema do tablet Huion com atalhos no sistema operacional Windows

### 4.3.1 (2018.3.1)

*(Lançado Em: 06 De dezembro De 2018*)Resumo: **Hotfix**

**Adicionado:**

* &amp;lbrack;Simetria&amp;rbrack;&amp;lbrack;Visor&amp;rbrack; Simetria pintura na Visualização 2D de volta e agora apresenta uma visualização do pincel de clone corrigida

**Corrigido:**

* &amp;lbrack;Exportar&amp;rbrack; Visualização 2D gera uma textura preta em alguns casos
* &amp;lbrack;Iray&amp;rbrack; As informações normais se tornam incorretas no Iray após instanciar uma camada de material
* Conjuntos de textura não quadrada podem levar, em alguns casos, a falhas
* &amp;lbrack;Undo&amp;rbrack; Vários Ctrl+Z podem aleatoriamente levar, em alguns casos, a falhas
* &amp;lbrack;QML&amp;rbrack; AlgScrollView pode criar um aviso no registro em alguns casos (loops de vinculação)

**Problemas Conhecidos:**

* O congelamento da computação em alguns casos em GPUs AMD VEGA
* Problema do tablet Huion com atalhos no sistema operacional Windows
* A suavização de borda e as sombras quando ativas em conjunto podem gerar resultados inesperados

### 4.3.0 (2018.3.0)

*(Lançado em: 20 de novembro de 2018*)Resumo: **Atualizações de viewport, exportação adequada, novos auxiliares de interface, uma ferramenta de simetria aprimorada, novo conteúdo e um enorme aumento no desempenho**

**Adicionado:**

* &amp;lbrack;Suavização de borda&amp;rbrack;&amp;lbrack;Visor&amp;rbrack; Nova filtragem de suavizações temporais para visor 3D (via Configurações de exibição)
* &amp;lbrack;Export&amp;brack; Exporta o conteúdo do visor 2D como uma única textura
* &amp;lbrack;Exportar&amp;rbrack;&amp;lbrack;Pontilhamento&amp;rbrack; Expor pontilhamento na exportação
* &amp;lbrack;Pilha de camadas&amp;rbrack; Cores em camadas e pastas
* &amp;lbrack;Pilha de camadas&amp;rbrack; Ativação e desativação rápidas de várias camadas e efeitos
* &amp;lbrack;Pilha de camadas&amp;rbrack; Navegação mais fácil para modos de mesclagem com teclas para cima e para baixo e rolagem do mouse
* &amp;lbrack;Proj&amp;rbrack;&amp;lbrack;UI&amp;rbrack; manipulador de rotação adicional nos três eixos para triplanar
* &amp;lbrack;Proj&amp;rbrack;&amp;lbrack;Atalhos&amp;rbrack; - e + para alterar o tamanho do manipulador de Projeção UV
* &amp;lbrack;Sombreador&amp;rbrack; Controla os parâmetros da camada revestida com canais no sombreador revestido com PBR
* &amp;lbrack;Substance&amp;rbrack; Expor novas entradas de textura com base em malha para filtros e geradores
* &amp;lbrack;Simetria&amp;rbrack;&amp;lbrack;Visor&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Controlar deslocamento da simetria com manipuladores
* &amp;lbrack;Simetria&amp;rbrack;&amp;lbrack;Barra de ferramentas contextual&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Novo painel de simetria com opções
* &amp;lbrack;Simetria&amp;rbrack; Novo modo de interseção de linha de simetria
* &amp;lbrack;Simetria&amp;rbrack; Novo cursor de clonagem de simetria
* &amp;lbrack;Simetria&amp;rbrack;&amp;lbrack;Atalhos&amp;rbrack; Q para ocultar e -, + para alterar o tamanho e shift para ajustar
* &amp;lbrack;Log&amp;brack; Melhorar as mensagens de erro quando não for possível exportar texturas
* &amp;lbrack;Scripting&amp;rbrack; Permite alterar ou atualizar os recursos em Configurações de exibição
* &amp;lbrack;Scripting&amp;brack; Permite criar ou remover canais em Conjuntos de Textura
* &amp;lbrack;Content&amp;rbrack;&amp;lbrack;Shaders&amp;rbrack; Adicionar suporte para anisotropia com um sombreador dedicado (pbr-metal-rough-anisotropia-angle)
* &amp;lbrack;Conteúdo&amp;rbrack; Atualização da esfera de visualização com anisotropia e ângulo modificado
* &amp;lbrack;Content&amp;rbrack; shutline matFx atualizado
* &amp;lbrack;Content&amp;rbrack; Nova texturização.XYZ varredura de rosto sem emenda
* &amp;lbrack;Content&amp;brack; Novos procedimentos anisotrópicos
* &amp;lbrack;Content&amp;brack; Novo filtro: ambiente de iluminação baked
* &amp;lbrack;Content&amp;brack; Novo mapa de ambiente: estúdio automotivo neutro
* &amp;lbrack;Content&amp;brack; Novo modelo de projeto: PBR - Ângulo de anisotropia de aspereza metálica (com canais de anisotropia)
* &amp;lbrack;Content&amp;brack; Novo modelo de projeto: PBR - aspereza metálica revestida
* &amp;lbrack;SVT&amp;rbrack;&amp;lbrack;Engine&amp;rbrack; Texturas Virtuais Dispersas (SVT)
* &amp;lbrack;SVT&amp;rbrack;&amp;lbrack;Preferências&amp;rbrack;&amp;lbrack;IU&amp;rbrack; SVT hardware support acceleration option
* &amp;lbrack;SVT&amp;rbrack;&amp;lbrack;Log&amp;rbrack; Informações adicionais para o recurso Texturização Virtual Esparsa (por exemplo, tamanho do disco)
* &amp;lbrack;SVT&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Janela de mensagens no início se o tamanho do disco for muito baixo para o cache
* &amp;lbrack;SVT&amp;rbrack;&amp;lbrack;Preferências&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Substance Painter local do cache global
* &amp;lbrack;SVT&amp;rbrack; Nova variável de ambiente para especificar o caminho do cache de Substance Painter
* &amp;lbrack;SVT&amp;rbrack; Nova variável de ambiente para ativar a aceleração de suporte de hardware SVT
* &amp;lbrack;SVT&amp;rbrack; Detectar suporte esparso por hardware
* &amp;lbrack;SVT&amp;rbrack;&amp;lbrack;Hardware Sparse&amp;rbrack; Elevar a versão mínima do driver para a GPU Nvidia
* &amp;lbrack;SVT&amp;rbrack;&amp;lbrack;Sombreador&amp;rbrack;&amp;lbrack;Viewport&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Avisa o usuário se artefatos presentes com Texturização Virtual Esparsa na abertura do projeto

**Corrigido:**

* &amp;preto;Seletor de cores&amp;rbrack; Cursor de pintura que aparece ao tentar escolher uma cor
* A falha ao selecionar ou cancelar a seleção de camadas em uma ordem específica pode causar falha
* Falha ao colar como uma ocorrência uma camada com uma máscara
* &amp;lbrack;User Channel&amp;rbrack;&amp;lbrack;Regressão&amp;rbrack; Falha ao renomear o canal do usuário
* &amp;preto;Canal do usuário&amp;rbrack; visualização do pincel esmaecido
* &amp;lbrack;Alembic&amp;rbrack; Somente uma textura definida de vários materiais após a importação
* &amp;lbrack;Engine&amp;brack; A textura exportada difere da viewport para carimbos de pincel
* &amp;lbrack;Engine&amp;rbrack; Inverter com um efeito de nível não afeta totalmente uma textura
* O seletor de material está aplicando um traçado de pincel ao separar
* Alternar a resolução para 128x128px leva a um travamento
* Os links de mapas de malha não são atualizados corretamente ao reorganizar ou instanciar camadas
* &amp;lbrack;Substance&amp;rbrack; O UserData ColorSpace não funciona no Normal de Malha Feito bake solicitado como entrada
* Incompatibilidade de associação MDL ao usar várias instâncias de sombreadores
* &amp;lbrack;Simetria&amp;rbrack;&amp;lbrack;Camada de preenchimento&amp;rbrack; plano de Simetria e seu manipulador ativo na Camada de preenchimento
* &amp;preto;Visor&amp;rbrack; Ponto dinâmico para tradução nem sempre atualizado após clicar
* &amp;lbrack;UI&amp;rbrack; Ícones fixos e remoção de espaços reservados para monitores HDPI

**Problemas Conhecidos:**

* O congelamento da computação em alguns casos em GPUs AMD VEGA
* Problema do tablet Huion com atalhos no sistema operacional Windows
* A suavização de borda e as sombras quando ativas em conjunto podem gerar resultados inesperados

### 4.2.3 (2018.2.3)

*(Lançado: 25 de setembro de 2018)*

**Corrigido:**

* O &amp;lbrack;Visualização 2D&amp;rbrack; Visualização 2D é quebrado com algumas malhas ao criar um novo projeto
* &amp;lbrack;Crash&amp;rbrack; Alternar de Projeção UV para projeção tri-planar leva a um travamento
* &amp;lbrack;RayCollider&amp;rbrack; Várias falhas devido ao “RayCollider”
* &amp;lbrack;Tool&amp;brack; Alternar camadas perde as propriedades do pincel modificadas
* As configurações do pincel são redefinidas ao alternar para a borracha

**Problemas Conhecidos:**

* Congelamento de computação em GPUs AMD VEGA
* Problema do tablet Huion com atalhos no sistema operacional Windows

### 4.2.2 (2018.2.2)

*(Lançado em: 11 de setembro de 2018*)Resumo: **Hotfix com atualização de conteúdo, novas funcionalidades de script e capacidade de desabilitar a atualização automática**

**Adicionado:**

* &amp;lbrack;Content&amp;rbrack;&amp;lbrack;Shelf&amp;rbrack; Adicionar uma predefinição de prateleira de pele
* &amp;lbrack;Content&amp;rbrack;&amp;lbrack;shelf&amp;rbrack; Conversão de 19 normais de pele em materiais para dispersão subsuperficial
* &amp;lbrack;Scripting&amp;brack; Cria um modelo de projeto a partir de um projeto aberto
* &amp;lbrack;Scripting&amp;brack; Obter/Definir configurações de exportação de um projeto aberto
* &amp;lbrack;Atualizações&amp;rbrack; Consegue desativar o pop-up de atualização automática nas configurações e variáveis de ambiente
* &amp;lbrack;Atualizações&amp;rbrack; Não exibir até a próxima versão no pop-up de manutenção desatualizada

**Corrigido:**

* &amp;lbrack;Camera&amp;brack; Zoom incorreto ao alternar de ortográfica para Perspectiva
* &amp;lbrack;Display&amp;rbrack; Alguns mapas são exibidos de forma linear em vez de sRGB
* O foco da malha do &amp;brack;Viewports&amp;rbrack; não se comporta corretamente
* &amp;lbrack;Visualização 2D&amp;rbrack; Projeto com câmera quebrada tem desaparecendo Shells UVs
* &amp;lbrack;SSS&amp;rbrack;&amp;lbrack;Dica de ferramenta&amp;rbrack; as dicas de ferramentas de dispersão da subsuperfície aparecem no registro
* Alguns projetos não podem ser abertos em 2018.2 e a mensagem de erro não pode salvar um pacote nulo do substance
* A cor da ferramenta de Tinta do &amp;brack;Mask&amp;rbrack; pode ficar presa em alguns casos ao trabalhar em uma máscara
* &amp;lbrack;Material&amp;rbrack; Mapas que não aparecem em situações específicas
* &amp;lbrack;Proj&amp;rbrack;&amp;lbrack;Ferramentas&amp;rbrack; Manipulador ativo com um gerador
* &amp;lbrack;Substance&amp;rbrack; Grupos de Substance de parâmetros ausentes
* &amp;lbrack;Scripting&amp;rbrack; Nome de software incorreto na documentação
* &amp;lbrack;UDIMs&amp;rbrack; Não há informações no log sobre shells UVs em vários blocos UVs

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

* &amp;lbrack;SSS&amp;rbrack;&amp;lbrack;Visor&amp;rbrack;&amp;lbrack;Iray&amp;rbrack; Dispersão de subsuperfície genérica
* &amp;lbrack;SSS&amp;rbrack; Sincronizar MDL e parâmetros de dispersão da subsuperfície
* &amp;preto;SSS&amp;rbrack; Adicionado um novo canal em tons de cinza chamado Dispersão
* &amp;lbrack;SSS&amp;rbrack;&amp;lbrack;Configurações de Sombreador&amp;rbrack; Parâmetro de tipo de dispersão para dispersão de subsuperfície (pele ou translúcido)
* &amp;lbrack;SSS&amp;rbrack;&amp;lbrack;Configurações de Sombreador&amp;rbrack; Parâmetro de escala de dispersão para dispersão de subsuperfície
* &amp;lbrack;SSS&amp;rbrack;&amp;lbrack;Configurações de Sombreador&amp;rbrack; Parâmetro de dispersão de cor para dispersão de subsuperfícies
* &amp;lbrack;SSS&amp;rbrack;&amp;lbrack;Configurações de exibição&amp;rbrack; Contagem de amostras de dispersão para dispersão subsuperficial
* &amp;lbrack;Sombreador&amp;rbrack;&amp;lbrack;Iray&amp;rbrack; Integrar MDL de dispersão de subsuperfície para Iray
* &amp;lbrack;Sombreador&amp;rbrack; atualização de Sombreador através do atualizador de recursos
* &amp;lbrack;Sombreador&amp;rbrack; Atualizar a API e a documentação do registro de alterações
* &amp;lbrack;Propriedades da ferramenta&amp;rbrack;&amp;lbrack;Proj&amp;rbrack; Novos parâmetros para a projeção triplanar
* &amp;lbrack;Viewport&amp;rbrack;&amp;lbrack;Proj&amp;rbrack; Controla as propriedades da Camada de preenchimento na exibição 3D diretamente com manipuladores (projeção triplanar)
* &amp;lbrack;Atalhos&amp;rbrack;&amp;lbrack;Proj&amp;rbrack; Novos atalhos Q, W, E, R, T para manipuladores de projeção triplanar
* &amp;lbrack;Viewport&amp;rbrack;&amp;lbrack;Proj&amp;rbrack; Controla as propriedades da Camada de Preenchimento diretamente com manipuladores (Projeção UV)
* &amp;lbrack;Atalhos&amp;rbrack;&amp;lbrack;Proj&amp;rbrack; Novo atalho Q para manipuladores de Projeção UV
* &amp;lbrack;Barra de ferramentas contextual&amp;rbrack;&amp;lbrack;Proj&amp;rbrack; Controla manipuladores de projeção triplanar
* &amp;lbrack;Barra de ferramentas contextual&amp;rbrack;&amp;lbrack;Proj&amp;rbrack; Controlar manipuladores de Projeção UV
* &amp;lbrack;Propriedades da ferramenta&amp;rbrack; Desativar divisão em blocos gráficos por textura com a ferramenta de projeção e estêncil
* &amp;lbrack;Estêncil&amp;rbrack; Usar imagens não quadradas com a ferramenta de projeção/estêncil
* &amp;lbrack;Estêncil&amp;rbrack; Permitir controle do modo lado a lado na janela Propriedades
* &amp;lbrack;Estêncil&amp;rbrack; O Zoom não está centralizado em um estêncil sem revestimento
* &amp;lbrack;Câmeras&amp;rbrack; importar câmeras do Maya, Max, Blender, Modo, DAE
* &amp;lbrack;Câmeras&amp;rbrack;&amp;lbrack;Visor&amp;rbrack; Selecionar e controlar câmeras importadas no visor
* &amp;lbrack;Cameras&amp;brack;&amp;lbrack;Iray&amp;rbrack; Selecionar e controlar câmeras importadas no Iray
* &amp;lbrack;Câmeras&amp;rbrack;&amp;lbrack;UI&amp;rbrack;&amp;lbrack;Novo projeto&amp;rbrack;&amp;lbrack;Configuração do projeto&amp;rbrack; Importar câmeras está marcado por padrão
* &amp;lbrack;Cameras&amp;brack;&amp;lbrack;Atalhos&amp;rbrack; Adicionar atalhos para alternar entre câmeras
* &amp;lbrack;Cameras&amp;brack;&amp;lbrack;Visor&amp;rbrack; Adicionar quadro no visor
* &amp;lbrack;Cameras&amp;brack;&amp;lbrack;Configurações do visor&amp;rbrack; Controle de opacidade de quadro
* &amp;lbrack;Câmeras&amp;rbrack;&amp;lbrack;Configurações da câmera&amp;rbrack; distância focal máxima em 500 mm
* &amp;lbrack;Câmeras&amp;rbrack;&amp;lbrack;Configurações da câmera&amp;rbrack; Taxa de exposição
* &amp;lbrack;Cameras&amp;brack;&amp;lbrack;Configurações da câmera&amp;rbrack; Adicionar uma opção de bloqueio
* &amp;lbrack;Cameras&amp;brack;&amp;lbrack;Configurações da câmera&amp;rbrack; Adicionar uma opção de restauração
* &amp;lbrack;Cameras&amp;brack;&amp;lbrack;Configurações da câmera&amp;rbrack; Adicionar atributo de distância do foco
* &amp;lbrack;glTF&amp;rbrack; Importação de um arquivo glTF
* &amp;lbrack;glTF&amp;rbrack; Importar mapa de oclusão de ambiente
* &amp;lbrack;Alembic&amp;rbrack; Importar quadro Alembic 1 com geometria estática
* &amp;lbrack;Shelf&amp;rbrack; Arraste e solte materiais diretamente na malha usando mapas de ID com um modificador (CTRL/Command)
* &amp;lbrack;Pilha de camadas&amp;rbrack; Criação automática de máscara de ID com arrastar e soltar materiais na malha com mapas de ID
* &amp;lbrack;Pilha de camadas&amp;rbrack; Rolagem automática de camadas com arrastar e soltar pela pilha de camadas
* &amp;lbrack;UI&amp;rbrack;&amp;lbrack;Propriedades da ferramenta&amp;rbrack; Expor predefinição de Substance
* &amp;lbrack;UI&amp;rbrack;&amp;lbrack;Menu Ajuda&amp;rbrack; Aprimoramento do menu Ajuda
* &amp;lbrack;UI&amp;rbrack;&amp;lbrack;Novo Projeto&amp;rbrack;&amp;lbrack;Configuração do Projeto&amp;rbrack; Reorganização da janela
* &amp;lbrack;UI&amp;rbrack;&amp;lbrack;Novo Projeto&amp;rbrack;&amp;lbrack;Configuração do Projeto&amp;rbrack; Substituir termo de Malha por Arquivo
* &amp;lbrack;UI&amp;rbrack;&amp;lbrack;Substance&amp;rbrack; Exibir atributos de Substance na interface do usuário
* &amp;lbrack;Atalhos&amp;rbrack; F4 alterna entre as visualizações 2D e 3D
* &amp;lbrack;Atalhos&amp;rbrack; Novos atalhos para alternar o estêncil N e máscara rápida U
* &amp;lbrack;integração de Substance&amp;rbrack; Leve em consideração as instruções &#39;visible if&#39; nos parâmetros de Substance
* &amp;lbrack;Visor&amp;rbrack; Sombras não forçadas a serem computadas após a movimentação da câmera
* &amp;lbrack;Content&amp;rbrack; Atualizar MeetMat com câmeras importadas
* &amp;lbrack;Content&amp;brack; Adicionar uma amostra com dispersão de subsuperfície ativada - JadeToad
* &amp;lbrack;Content&amp;brack; Adicionar um novo modelo de projeto PBR com dispersão de subsuperfície ativada
* &amp;lbrack;Content&amp;rbrack; Predefinições de exportação atualizadas para adicionar um novo canal de Dispersão
* &amp;lbrack;Content&amp;rbrack;&amp;lbrack;Shelf&amp;rbrack; Suporte a dispersão de subsuperfície adicionado para: pbr-metal-rough, pbr-metal-rough-alpha-test, pbr-coated, pbr-spec-gloss
* &amp;lbrack;Content&amp;rbrack;&amp;lbrack;Shelf&amp;rbrack; Adicionado Canal de dispersão a 5 materiais inteligentes (bolinhas e peles)
* &amp;lbrack;Content&amp;rbrack;&amp;lbrack;Shelf&amp;rbrack; 1 novo Material em jade
* &amp;lbrack;Content&amp;rbrack;&amp;lbrack;Shelf&amp;rbrack; 1 novo material de cera

**Corrigido:**

* &amp;lbrack;CMD&amp;rbrack; Resultados diferentes usando a mesma linha de comando com versões diferentes
* &amp;lbrack;TDR&amp;rbrack; Se o TdrLevel estiver configurado, você não terá erros no seu log
* &amp;lbrack;Baker&amp;rbrack; o mapa de Oclusão de ambiente está invertido
* &amp;lbrack;Mapa de identificações&amp;rbrack; Falha ao selecionar fora do intervalo 0-1
* &amp;lbrack;Iray&amp;rbrack; Falha ao alternar conjuntos de texturas e voltar para o modo de Tinta
* &amp;lbrack;Viewport&amp;rbrack; Sincronizar áreas de soltar entre viewports para arrastar e soltar
* &amp;lbrack;Engine&amp;brack; artefato Moiré ao colocar camadas de preenchimento lado a lado ou pintar um pequeno pincel
* &amp;lbrack;Licença&amp;rbrack; Serviço de licença verificação de versão de software incorreta
* &amp;lbrack;License&amp;rbrack; Trabalhar novamente como lidamos com a autenticação
* &amp;lbrack;API&amp;rbrack; Chame o evento de API de script onNewProjectCreated mesmo ao criar com um modelo
* &amp;lbrack;Sombreador&amp;rbrack; O sombreador compilado não é carregado do cache quando o arquivo de sombreador não é compilado
* &amp;lbrack;Prateleira&amp;rbrack; Exportar o arquivo HDR da prateleira irá gerar um arquivo com valores fixados
* &amp;lbrack;Export&amp;rbrack; EXR exportação grampos valores de cor de RGB entre 0-1
* &amp;lbrack;Content&amp;rbrack; Processual ruído 3D Perlin Fractal está pixelado

**Problemas Conhecidos:**

* Congelamento de computação em GPUs AMD VEGA
* Problema do tablet Huion com atalhos no sistema operacional Windows

### 4.1.3 (2018.1.3)

*(Lançado: 28 de junho de 2018)*

**Adicionado:**

* &amp;lbrack;Preferências&amp;rbrack; Proponha salvar o projeto quando o Painter for reiniciado

**Corrigido:**

* O &amp;lbrack;Plug-in&amp;rbrack; Substance Source de Pesquisa não funciona
* &amp;lbrack;Materiais inteligentes&amp;rbrack; Importar Materiais inteligentes leva a uma falha em alguns casos
* &amp;lbrack;Materiais inteligentes&amp;rbrack; Excluir Materiais inteligentes leva a uma falha em alguns casos
* &amp;lbrack;Salvar&amp;rbrack; salvar leva a uma falha em alguns casos raros
* &amp;lbrack;Shelf&amp;rbrack; Inverter não funciona no Células 2 e no Células 3
* &amp;lbrack;Shelf&amp;rbrack; Erro de ortografia em alguns Alpha
* &amp;lbrack;Shelf&amp;rbrack; Alguns materiais do Substance não são renderizados corretamente

**Problemas Conhecidos:**

* Congelamento de computação em GPUs AMD VEGA

### 4.1.2 (2018.1.2)

*(Lançado: 12 De junho De 2018*)Resumo: **Velocidade De Fça bake Aprimorada, Sistema De Salvamento Aprimorado, Controles Deslizantes Atualizados, API De Plug-In Atualizada, Tradução Para Chinês, Preenchimento Aprimorado Agora Opcional**

**Adicionado:**

* &amp;lbrack;Baker&amp;rbrack; Melhoria de desempenho com a nova versão do baker
* Forçar caixa de diálogo de exibição com GPU incompatível
* &amp;lbrack;Salvar&amp;rbrack; Expor a nova funcionalidade de projeto compacto (modo de salvamento completo/compacto)
* &amp;lbrack;Salvar&amp;rbrack; Informar o usuário em caso de erro ao salvar
* &amp;lbrack;Clean&amp;rbrack; Próxima gravação no modo completo/compacto
* &amp;preto;Controles deslizantes&amp;rrack; Aprimoramento da precisão das barras de cor/escala de cinza e controles deslizantes
* &amp;lbrack;Controles deslizantes&amp;rbrack; Adição de controles de seta para cima/para baixo
* &amp;preto;Controles deslizantes&amp;rbrack; Mesma zona de detecção para controles deslizantes de barra em tons de cinza e coloridos
* &amp;lbrack;Plug-in&amp;rbrack; Salvamento automático sempre em modo incremental
* &amp;lbrack;Plug-in&amp;rbrack; Opção para alternar plug-ins para o novo estilo de interface
* &amp;lbrack;Language&amp;brack; Adicionar tradução para chinês
* &amp;lbrack;Preenchimento&amp;rbrack; Opção para alternar entre o preenchimento do vizinho de espaço UV e 3D por Textura Definida nas Configurações do Conjunto de Textura
* &amp;lbrack;Script&amp;rbrack; Modo de salvamento de exposição: completo/compacto ou incremental
* &amp;lbrack;Script&amp;rbrack; Atualizar documentação de script/QML
* &amp;lbrack;Log&amp;rbrack; Indica o modo de salvamento no log (completo/compacto ou incremental)

**Corrigido:**

* &amp;lbrack;O slot do canal do &amp;rbrack; transforma-se em um slot de material em preenchimentos de canal único
* Falha ao carregar uma malha (FBX) com algumas faces não atribuídas por um material
* Falha na Iray com NVIDIA GRID 5.2 na máquina virtual
* Falha ao desfazer uma exclusão de predefinição de material
* Falha ao carregar alguns projetos
* &amp;lbrack;Linha de comando&amp;rbrack; Nova linha de comando para malhas UDIM divididas por udim
* &amp;lbrack;Barra de ferramentas&amp;rbrack; Redução da barra de ferramentas
* &amp;lbrack;Instanciação&amp;rbrack; Não é possível instanciar bitmaps em vários conjuntos de texturas
* &amp;lbrack;Viewport&amp;rbrack; A atualização não está completa ao pintar na malha com UVs lado a lado
* O Mapa normal &amp;lbrack;Iray&amp;rbrack; é aplicado duas vezes para dielétricos
* &amp;lbrack;Shelf&amp;rbrack; Erros de digitação em alguns parâmetros de Substance (alfas, procedimentos e matfx)
* &amp;lbrack;Shelf&amp;rbrack; Erro de ortografia para o bitmap “Somente Pessoal Autorizado”
* &amp;lbrack;Script&amp;rbrack; A função alg.shaders.materials() não funciona mais

**Problemas Conhecidos:**

* Congelamento de computação em GPUs AMD VEGA

### 4.1.1 (2018.1.1)

*(Lançado em: 3 de abril de 2018)*

**Corrigido:**

* &amp;lbrack;Tablet&amp;rbrack; Problema ao alterar as opções de interação padrão
* &amp;lbrack;Baker&amp;rbrack; Falha com biblioteca Assimp
* &amp;lbrack;Baker&amp;rbrack; Regressão no desempenho com mapa A.O.
* &amp;lbrack;Iray&amp;rbrack; A Distorção de lente não é aplicada ao canal Alfa
* &amp;lbrack;Drivers&amp;rbrack; Atualização dos requisitos mínimos de drivers
* &amp;lbrack;3Dview&amp;rbrack; Normais não gerados corretamente em malhas UDIM sem informações normais
* &amp;lbrack;Intel&amp;rbrack; Falha com o Substance Painter 2018.1.0
* &amp;lbrack;Intel&amp;rbrack;&amp;lbrack;Visor&amp;rbrack; Problema com preenchimento (artefatos pretos)

**Problemas Conhecidos:**

* Congelamento de computação em GPUs AMD VEGA

### 4.1.0 (2018.1.0)

*(Lançado: 15 de março de 2018)*

**Adicionado:**

* Novo estilo geral (ícones, cor, comportamento)
* Novo layout padrão
* &amp;lbrack;Aprimoramento da experiência do usuário do Tablet&amp;rbrack; ao pintar
* &amp;lbrack;Menu principal&amp;rbrack; Primeiro, classificar itens nativos em exibições e barras de ferramentas
* &amp;lbrack;Menu principal&amp;rbrack; Mover ações de máscara rápida na seção do visor
* &amp;lbrack;Menu principal&amp;rbrack; Move ações do botão direito do mouse para a seção do visor
* &amp;lbrack;Menu principal&amp;rbrack; Renomear menu “Exibir” como “Janela”
* &amp;lbrack;Menu rápido&amp;rbrack; Novas propriedades de ferramenta clicando com o botão direito do mouse no visor
* &amp;presilha;Widget de encaixe&amp;rbrack; Nova barra de ferramentas de encaixe para rápida redução/recuperação
* &amp;lbrack;Configurações de exibição&amp;rbrack; Janela de configurações da câmera e do visualizador mesclada
* &amp;lbrack;Pilha de camadas&amp;rbrack; Menu contextual do botão direito
* &amp;lbrack;Pilha de camadas&amp;rbrack; Arraste e solte para mover qualquer efeito dentro da mesma camada
* &amp;lbrack;Barra de ferramentas&amp;rbrack; Reorganização da barra de ferramentas e da nova barra de ferramentas contextual
* &amp;lbrack;Barra de ferramentas Ferramentas&amp;rbrack; Dividir ferramenta de clonagem em duas ferramentas separadas
* &amp;preto;Propriedades das ferramentas&amp;rbrack; Valor em tons de cinza do plano de fundo mais claro na visualização
* &amp;lbrack;Propriedades das ferramentas&amp;rbrack; Organização em guias (preenchimento e ferramentas)
* &amp;preto;Tool&amp;brack; O resultado da pintura corresponde ao estêncil
* &amp;lbrack;Visor&amp;rbrack; Novo cursor para camada de preenchimento
* &amp;lbrack;Visor&amp;rbrack; Navegação e pintura mais suaves (taxa de quadro mais alta)
* &amp;preto;Visor&amp;rbrack; Material/Canal/Mapa seleção caixa de combinação no visor
* &amp;lbrack;Visor&amp;rbrack; Reduzir cintilação ao girar (sombra ativada)
* &amp;lbrack;Shelf&amp;rbrack; Exibir materiais por padrão ao abrir o Painter
* &amp;lbrack;Shelf&amp;rbrack; Melhoria no tempo de carregamento de texturas e materiais (2 a 6 vezes mais rápido)
* &amp;lbrack;Prateleira&amp;rbrack; Reorganizar pastas de materiais para se ajustar à estrutura do Substance Source
* &amp;lbrack;Shelf&amp;rbrack; Arraste e solte materiais diretamente na malha no visor
* &amp;lbrack;Shelf&amp;rbrack; Novos Ruídos 3D (Perlin, Perlin Fractal, Simplex e Worley)
* &amp;lbrack;Prateleira&amp;rbrack; Novo gerador de máscara usando a posição da malha
* &amp;lbrack;Shelf&amp;rbrack; Ruídos base atualizados para suportar o expansão não quadrada
* &amp;lbrack;Shelf&amp;rbrack; Adicionado novo modelo e predefinição de exportação para o Lens Studio (aplicativo Snap)
* &amp;lbrack;Prateleira&amp;rbrack; Materiais inteligentes e Máscaras inteligentes atualizadas para usar a versão mais recente do Editor de máscaras (microdetalhes)
* &amp;lbrack;Shelf&amp;rbrack; Novo projeto de amostra “TilingMaterial” para criar materiais de revestimento perfeitos
* &amp;predefinição;Prateleira&amp;predefinição; Novo pincel (caligrafia, molhado, hachura e assim por diante)
* &amp;preto;Controles deslizantes&amp;rbrack; Novos controles deslizantes e estilo e comportamento de barras de tons de cinza/cores
* &amp;lbrack;Baker&amp;rbrack; Permitir o uso de uma caixa delimitadora de cena completa para calcular o mapa de posição
* &amp;lbrack;Sombreador&amp;rbrack; Remove o parâmetro de força do height dos parâmetros de sombreador padrão
* &amp;lbrack;Mecanismo&amp;rbrack; mecanismo de Substance atualizado
* &amp;lbrack;Engine&amp;brack; Nenhuma ou menos descontinuidades nos blocos UV
* &amp;lbrack;Plugins&amp;rbrack; Importar materiais baixados do Substance Source mais rapidamente
* &amp;lbrack;Plug-ins&amp;rbrack; Atualiza todos os plug-ins para corresponder ao novo estilo geral
* &amp;lbrack;Preferências&amp;rbrack; Visualizar alterações de cor de fundo automaticamente
* &amp;lbrack;Clean&amp;rbrack; Risco reduzido de corrupção do projeto
* &amp;lbrack;Aberto&amp;rbrack; Melhoria na hora de abertura do projeto
* &amp;lbrack;Novo projeto&amp;rbrack; Novo projeto - melhoria no tempo de atualização da malha
* &amp;preto;Salvar&amp;rbrack; Salvando a melhoria do tempo do projeto
* &amp;lbrack;Log&amp;rbrack; Tipo de licença relatado no registro
* &amp;lbrack;TextureSet&amp;rbrack; Renomeie o botão “Fazer bake Texturas” como “Fazer bake Mapas de Malha”
* Renomear “Mapas adicionais” como “Mapas de malha”

**Corrigido:**

* &amp;lbrack;Visor&amp;rbrack; Maus desempenhos com malhas contendo muitos sub-objetos
* &amp;lbrack;Propriedades das ferramentas&amp;rbrack; Canal desativado ao arrastar e soltar uma imagem no slot de material
* &amp;brack;Propriedades das ferramentas&amp;rbrack; A visualização do pincel está quebrada com as ferramentas de borrar e clonar
* &amp;preto;A ordem dos canais do conjunto de texturas &amp;rbrack; está incorreta ao usar modelos
* &amp;lbrack;Shelf&amp;rbrack; Ícone ausente para o gerador de Conversão em escala cinza
* &amp;preto;Shelf&amp;rbrack; Número do Círculo do Sinal alfa está quebrado (fonte ausente)
* Detecção incorreta de GPUs integradas na inicialização
* &amp;lbrack;Falha&amp;rbrack; Arrastar e soltar um recurso importado nomeado com um caractere #
* &amp;lbrack;Engine&amp;rbrack; Problema de detecção de Vram na GPU integrada
* &amp;lbrack;Engine&amp;rbrack; Corrigidas várias falhas no Substance Engine Linker
* &amp;lbrack;Engine&amp;rbrack; Artefatos quadrados ao alterar a resolução
* &amp;lbrack;Pós-efeitos&amp;rbrack; O redimensionamento da interface fica lento quando os pós-efeitos estão ativados
* &amp;lbrack;Baker&amp;rbrack; A unidade de cena não é respeitada corretamente para valores de distância de raio
* &amp;lbrack;Baker&amp;rbrack; O AO da distância do Ocluder de malha é fixado em 1, independentemente do valor de entrada
* &amp;lbrack;Baker&amp;rbrack; Corresponder pelo nome ignora algumas malhas com nomes específicos
* &amp;lbrack;Baker&amp;rbrack; Cor da configuração de malha do Poligrupo e ID de Submalha sempre retorna uma imagem em preto
* &amp;lbrack;Baker&amp;rbrack; O Fça bake de ID falha com malhas FBX binárias do Blender
* &amp;lbrack;Sombreador&amp;rbrack; Ruído no Visualização 2D com brilho dota-2 e não pbr-spec
* &amp;lbrack;Linux&amp;rbrack; Somente um thread de CPU é usado ao fazer bake
* &amp;lbrack;MacOS&amp;rbrack; Falha com o cursor do pincel se movendo sobre o visor

**Problemas Conhecidos:**

* Congelamento de computação em GPUs AMD VEGA
* Pós-processo de distorção não levado em conta ao exportar no IRay (alfa)

## Versão 3

### 3.4.2 (2017.4.2)

*(Lançado: 24 de janeiro de 2018)*

**Adicionado:**

* &amp;lbrack;Export&amp;brack; Obter o status de uma exportação com o progresso da etapa
* &amp;lbrack;Export&amp;brack; Permitir cancelamento de uma exportação
* &amp;lbrack;Export&amp;brack; Exportar texturas para o Sketchfab sem perder a qualidade do mapa normal
* &amp;lbrack;Exportar&amp;rbrack; Exportar no formato binário glTF (glb)
* &amp;lbrack;Export&amp;rbrack; Permitir o redimensionamento de colunas na guia de configuração da janela de exportação
* &amp;lbrack;Sombreador&amp;rbrack; Adicionar um changelog para o API de sombreamento
* &amp;lbrack;Scripting&amp;rbrack; Adicionar funções de retorno de chamada Antes e Depois ao exportar texturas
* &amp;lbrack;Iray&amp;rbrack; Atualização para o SDK 2017.1 (suporte a Volta GPUs)

**Corrigido:**

* Falha ao sair do aplicativo antes que a janela principal seja exibida
* &amp;lbrack;MAC&amp;rbrack; Falha ao carregar mapas em tons de cinza com IRAY
* &amp;lbrack;A detecção do VRAM no MAC&amp;rbrack; não está correta com o novo sistema operacional High Sierra
* &amp;lbrack;Plug-in&amp;rbrack; Baixar ativos do Substance Source não funciona mais
* &amp;lbrack;Scripting&amp;brack; Detecção incorreta da versão mínima do plug-in
* &amp;lbrack;Export&amp;brack; Falha ao salvar predefinição de exportação após exportar texturas
* &amp;lbrack;Instancing&amp;brack; Problema em geradores instanciados em um TextureSet sem Mapas Adicionais
* &amp;lbrack;Viewport&amp;rbrack; O pontilhamento não funciona com resolução superior a 4k
* &amp;lbrack;Visor&amp;rbrack; a exibição de material de Visualização 2D está coberta de ruído
* &amp;predefinição;Prateleira&amp;predefinição; Melhorar tempo de carregamento para predefinições de prateleira
* &amp;lbrack;Engine&amp;brack; Mesclagem incorreta ao pintar sob seleção de cores

### 3.4.1 (2017.4.1)

*(Lançado: 15 de dezembro de 2017)*

**Adicionado:**

* &amp;lbrack;Scripting&amp;brack; Exportar malha pela API de script
* &amp;lbrack;Import&amp;brack; Desativar importação de formato de arquivo de malha não suportado (permitir somente obj, fbx, dae, ply)
* &amp;lbrack;Log&amp;rbrack; Indica com mais precisão o problema de TDR no arquivo de log

**Corrigido:**

* Falha se o aplicativo for fechado antes da conclusão do rastreamento de recursos
* Falha ao abrir projetos com a ferramenta Borrar/Clonar
* Falha ao usar a ação de refazer após uma desfazer de uma alteração de Sombreador nas Configurações do visualizador
* &amp;lbrack;A texturização do Engine&amp;rbrack; difere entre o Painter 2017.2 e 2017.4
* &amp;lbrack;Viewport&amp;rbrack; A separação em um mapa de ID de uma instância obtém a amostra da cor errada
* &amp;lbrack;Export&amp;brack; Falha ao exportar uma textura normal ou de oclusão inválida
* Os arquivos de PSD do &amp;brack;Export&amp;brack; têm seus grupos bloqueados quando abertos no Photoshop CS6
* &amp;lbrack;Plug-in&amp;rbrack; o plug-in do Photoshop ignora a seleção de canais e sempre exporta tudo
* &amp;preto;Camadas&amp;rbrack; As âncoras são rompidas quando copiadas/coladas entre Conjuntos de Texturas
* &amp;lbrack;Camadas&amp;rbrack; Algumas referências de âncora não podem ser restauradas se quebradas
* &amp;lbrack;Sombreador&amp;rbrack; o parâmetro de aspereza secundária revestido com pbr está quebrado
* &amp;lbrack;Steam&amp;brack; O pop-up do verificador de versões não deve estar visível na inicialização

**Problemas Conhecidos:**

* &amp;lbrack;AMD&amp;rbrack; Falha/Congela ao tentar tinta em uma malha. Pode ser corrigido com uma atualização de driver de GPU.

### 3.4.0 (2017.4.0)

*(Lançado: 23 de novembro de 2017)*

**Adicionado:**

* &amp;lbrack;Instancing&amp;brack; Permite criar instâncias de parâmetros entre camadas
* &amp;lbrack;Instancing&amp;brack; Permite saltar entre uma camada de origem e uma instância
* &amp;lbrack;Criação de instância&amp;rbrack; Adicionar uma ação “criar instância entre conjuntos de texturas”
* &amp;lbrack;Instancing&amp;rbrack; Indicar nas instâncias de reentrada de pilha de camadas (ciclos)
* &amp;lbrack;Instancing&amp;brack; Excluir instâncias quando uma origem for removida
* &amp;lbrack;Instancing&amp;brack; Não permitir referências de âncora de fora de uma pasta instanciada
* &amp;lbrack;UI&amp;rbrack; Move a Pilha de Desfazer para sua própria janela chamada “History”
* &amp;lbrack;Plug-in&amp;brack; Plug-in de link dinâmico Integrate DCC
* &amp;lbrack;Engine&amp;brack; Aprimorar o desempenho de pintura com pintura Esparsa
* &amp;lbrack;Export&amp;brack; Adicionar opções de rascunho e de reexportação ao exportador do Sketchfab
* &amp;preto;Prateleira&amp;rbrack; Adicionar “virar” controle para substâncias de fontes
* &amp;lbrack;Shelf&amp;rbrack; Adicionar 20 novos materiais de procedimentos
* &amp;lbrack;Shelf&amp;rbrack; Adicionar 40 novos mapas grunges (baseado em bitmap e processual)
* &amp;lbrack;Visor&amp;rbrack; Ativar colisões de visualização de pincel em outros conjuntos de texturas visíveis
* Atualizar os requisitos mínimos dos drivers de GPU AMD

**Corrigido:**

* Falha ao computar Substance em resoluções muito grandes
* Falha ao pintar fortemente com partículas
* &amp;lbrack;Viewport&amp;rbrack; Reflexo de specular incorreto no Visualização 2D com malhas específicas
* &amp;lbrack;UI&amp;rbrack; Algumas ações indesejadas aparecem na janela Histórico

**Problemas Conhecidos:**

* &amp;lbrack;Camadas&amp;rbrack; Algumas referências de âncora não podem ser restauradas se quebradas
* Falha ao usar a ação de refazer após uma desfazer de uma alteração de Sombreador nas Configurações do visualizador

### 3.3.3 (2017.3.3)

*(Lançado em: 01 de dezembro de 2017)*

**Corrigido:**

* &amp;lbrack;Steam&amp;brack; O pop-up do verificador de versões não deve estar visível na inicialização
* Os arquivos de PSD do &amp;brack;Export&amp;brack; têm seus grupos bloqueados quando abertos no Photoshop CS6

### 3.3.2 (2017.3.2)

*(Lançado: 20 De novembro De 2017)*

**Adicionado:**

* &amp;lbrack;UI&amp;rbrack; Melhorar caixa de diálogo da nova versão e adicionar changelog
* &amp;lbrack;UI&amp;rbrack; Indica se a manutenção expirou na caixa de diálogo de nova versão
* &amp;lbrack;Licença&amp;rbrack; Atualiza o sistema de licenças para lidar com as datas de manutenção
* &amp;lbrack;Export&amp;brack; Renomear Adobe Standard Material para Adobe Dimension

**Corrigido:**

* &amp;preto;A pintura do Mac&amp;rbrack; leva a quadrados pretos e corrupções de textura
* &amp;lbrack;Engine&amp;brack; Cache às vezes pode desaparecer no Visor
* &amp;lbrack;Engine&amp;rbrack; Artefatos de blocos aparecem quando um disparador de compactação de memória
* &amp;lbrack;Fazendo bake&amp;rbrack; Estranhas mensagens de erro ao fazer bake malhas específicas
* &amp;lbrack;Export&amp;brack; PSD foram gravados incorretamente e não são reconhecidos corretamente pelo Photoshop
* &amp;lbrack;Camadas&amp;rbrack; Não deveria ser possível copiar/colar camadas em vários projetos
* &amp;lbrack;Substance&amp;rbrack; O espaço da cor UserData para a entrada Normal é invertido em alguns casos
* &amp;lbrack;Shelf&amp;rbrack; Micro-normal em geradores gera curvatura invertida
* &amp;lbrack;Shelf&amp;rbrack; filtro HSL também afeta o canal alfa
* &amp;lbrack;Linux&amp;rbrack; A instalação em Centos falha devido a dependências ausentes
* O instalador não remove todos os recursos da instalação anterior em certos casos

### 3.3.1 (2017.3.1)

*(Lançado: 26 de outubro de 2017)*

**Adicionado:**

* &amp;lbrack;Export&amp;brack; Permite exportar a malha de um projeto
* &amp;lbrack;Shelf&amp;rbrack; Remover “Sub-Shelf” dos títulos das guias
* Salvar configurações de pós-processamento em modelos
* Tornar a mensagem TDR mais compreensível
* Melhorar a janela Configurações para relatar erros

**Corrigido:**

* Falha ao excluir várias subprateleiras
* Falha ao alternar de um nível para algo diferente durante um cálculo do mecanismo
* &amp;lbrack;Mac&amp;rbrack; Falha na GPU Intel durante cálculos do mecanismo
* &amp;lbrack;Mac&amp;rbrack;&amp;lbrack;Viewport&amp;rbrack; Maus desempenhos quando o pontilhamento está ativado
* &amp;lbrack;O Mac&amp;rbrack; MacOS 10.13 é reconhecido como “Versão desconhecida” no arquivo de registro
* &amp;lbrack;Baker&amp;rbrack; Fazer bake com uma gaiola não funciona mais
* &amp;lbrack;Camadas&amp;rbrack; Ctrl + C atalho (ação de cópia) não funciona mais
* &amp;lbrack;Camadas&amp;rbrack; Colar camadas não atualiza a interface com referências de âncora
* &amp;lbrack;Anchor&amp;rbrack; Duplicar ou Copiar/Colar Camada com Referências quebra os links
* &amp;lbrack;Export&amp;rbrack; A exportação em 8K pode travar ou bloquear o aplicativo em alguns casos
* &amp;lbrack;Export&amp;rbrack; Vários problemas no formato de arquivo glTF gerado
* &amp;lbrack;Import&amp;brack; A reimportação de uma malha com o mesmo nome de arquivo não funciona mais
* &amp;lbrack;Plug-in&amp;rbrack; A janela de salvamento automático sempre aparece acima de tudo
* &amp;lbrack;UI&amp;rbrack; Loop infinito ao pressionar “Escape” na caixa de diálogo TDR
* &amp;lbrack;UI&amp;rbrack; Redefinir interface exibe uma segunda barra de título na janela da prateleira

### 3.3.0 (2017.3.0)

*(Lançado: 28 de setembro de 2017)*

**Adicionado:**

* &amp;lbrack;Export&amp;brack; Permitir a exportação de malha e texturas para o Projeto Adobe Felix
* &amp;lbrack;Export&amp;rbrack; Permitir exportação para o formato de arquivo glTF
* &amp;lbrack;Engine&amp;rbrack; Otimizar o tamanho do textura em VRAM usando compactação de bloco
* &amp;lbrack;Visor&amp;rbrack; Ser capaz de arrastar e soltar uma malha ou projeto no visor
* &amp;lbrack;UI&amp;rbrack; Melhorar mensagem de aviso sobre TDR
* &amp;lbrack;UI&amp;rbrack; O registro deve ser exibido somente mediante solicitação
* &amp;lbrack;UI&amp;rbrack; Permite limpar o conteúdo da janela de registro
* &amp;lbrack;UI&amp;rbrack; Exibir avisos e erros na barra de status
* &amp;lbrack;UI&amp;rbrack; Exibir guias na parte superior como em navegadores da Web
* &amp;lbrack;UI&amp;rbrack; Melhorar contexto e mensagens “não pintáveis”
* &amp;lbrack;UI&amp;rbrack; Adicionar uma ação “salvar como cópia” no menu arquivo
* &amp;lbrack;Camada&amp;rbrack; Define a configuração padrão da divisão em blocos gráficos como 1 por padrão
* &amp;lbrack;Shelf&amp;rbrack; Filtro de gradiente aprimorado para suportar 10 cores dinâmicas
* &amp;lbrack;Shelf&amp;rbrack; Adicionar um espaço na consulta padrão da miniprateleira
* &amp;predefinição;Prateleira&amp;predefinição; Adicionar uma ação “Abrir no explorador” para recursos locais na prateleira
* &amp;brack;Prateleira&amp;rbrack; Adicionar modelo e sombreador para o Adobe Material Standard (Projeto Felix)
* &amp;lbrack;Shelf&amp;rbrack; Aumentar o tamanho máximo da divisão em blocos gráficos para 128 nos sombreadores de camada de material
* &amp;lbrack;Prateleira&amp;rbrack; Curvatura sobel adicionada para microdetalhes de Geradores de máscara
* &amp;lbrack;Plug-in&amp;rbrack; Adicionar plug-in de salvamento automático com intervalo de tempo personalizável
* &amp;lbrack;Scripting&amp;brack; Adicionar uma função “salvar como cópia”

**Corrigido:**

* &amp;lbrack;UI&amp;rbrack; O layout é quebrado na primeira inicialização
* &amp;lbrack;Export&amp;brack; o PSD gerado na exportação apresenta erros de formato
* &amp;lbrack;Export&amp;brack; EXR sempre exporta mapa de altura de 8 bits
* &amp;lbrack;Export&amp;brack; Falha ao exportar mapas adicionais corrompidos
* &amp;lbrack;Import&amp;brack; As arestas sólidas não são preservadas em malhas polidas baixas em alguns casos
* &amp;lbrack;Import&amp;brack; Mensagens de erro aprimoradas ao importar malhas com problemas
* &amp;lbrack;Baker&amp;rbrack; Falha na Faz bake do Mapa de ID com a opção Corresponder pelo nome ativada
* &amp;lbrack;Viewport&amp;rbrack; O espaço tangente não está sincronizado com baker
* &amp;lbrack;Efeito&amp;rbrack; Voltar uma camada não restaura a referência de uma âncora
* &amp;lbrack;Efeito&amp;rbrack; Problema de atualização ao criar um link entre duas Máscaras com âncoras
* &amp;lbrack;Efeito&amp;rbrack; As âncoras de máscaras acima da máscara não devem ser listadas
* &amp;lbrack;Efeito&amp;rbrack; Extrair configuração de Alpha de Âncoras não funciona
* &amp;preto;Motor&amp;rbrack; A máscara se inverte após a primeira pincelada
* &amp;lbrack;Engine&amp;rbrack; Falha ao alternar o Conjunto de texturas em um projeto específico
* &amp;Preset;Shelf&amp;rbrack; Falha ao excluir uma predefinição que está em um projeto
* &amp;lbrack;Shelf&amp;rbrack; Erro de ortografia no filtro Tri-Planar avançado
* &amp;lbrack;Shelf&amp;rbrack; MG Mask Builder O A Escala de ruído do AO não funciona corretamente
* O Construtor de máscaras do MG do &amp;brack;Shelf&amp;rbrack; tem parâmetros de curvatura invertidos
* &amp;lbrack;Shelf&amp;rbrack; Alfas importadas geram uma visualização de esfera de material em vez de uma simples

### 3.2.0 (2017.2.0)

*(Lançado: 27 de julho de 2017)*

**Adicionado:**

* Pontos de ancoragem - Sistema de referência de camada e máscara
* &amp;lbrack;Camadas&amp;rbrack; Capacidade de renomear Efeitos de Preenchimento e Tinta
* &amp;lbrack;Plug-in&amp;rbrack; Plug-in Substance Source atualizado
* &amp;lbrack;Scripting&amp;brack; Permitir consultar a Resolução do Conjunto de Texturas
* &amp;lbrack;Scripting&amp;brack; Permite obter o status do mecanismo de Pintura
* &amp;lbrack;Desempenho&amp;rbrack; Otimizações aprimoradas de carregamento e carimbo de pincel no projeto

**Corrigido:**

* &amp;lbrack;Tool&amp;brack; Problemas de desempenho ao ajustar parâmetros de material
* &amp;lbrack;Engine&amp;brack; Desaparecendo traçados de pincel ao alterar a resolução (4K>2K)
* &amp;lbrack;Visualização 3D&amp;rbrack; O espaço tangente não está sincronizado com baker
* &amp;lbrack;Shelf&amp;rbrack; O caminho da prateleira nos documentos do usuário não é criado automaticamente
* &amp;Predefinição;Prateleira&amp;predefinição; Torna as predefinições compatíveis com versões anteriores após uma atualização
* &amp;lbrack;Sombreador&amp;rbrack; O sombreador não-PBR não funciona mais
* &amp;lbrack;Baker&amp;rbrack; Falha na Faz bake do Mapa de ID com a opção Corresponder pelo nome ativada
* &amp;lbrack;Sample&amp;rbrack; O nome do Conjunto de Texturas do Projeto de Amostra da Reunião está incorreto
* Salvar um projeto antes de criar um modelo retorna erros de permissão de gravação

### 3.1.0 (2017.1.0)

*(Lançado: 20 de junho de 2017)*

**Adicionado:**

* &amp;lbrack;Plug-in&amp;rbrack; Novo plug-in de Substance Source (permite o download de ativos na prateleira)
* &amp;lbrack;Shelf&amp;rbrack; 4 Novas Fontes (Japonês + Chinês Simplificado, Máquina de Escrever, Segmento)
* &amp;lbrack;Prateleira&amp;rbrack; 230 Novos Alpha (Mistura de padrões, pincéis e digitalizações de impressão digital)
* &amp;lbrack;Shelf&amp;rbrack; 50 Novos Procedimentos (Padrões de tecido de roupas medievais e contemporâneas)
* &amp;lbrack;Shelf&amp;rbrack; 2 Novos mapas de ambiente (Mondarrain e Villa Nova Street)
* &amp;lbrack;Shelf&amp;rbrack; 9 Novos filtros (MatFx Detail Edge Wear, Restrinjo, HBAO, etc.)
* &amp;lbrack;Shelf&amp;rbrack; Mapa de ambiente padrão aprimorado do Panorama
* &amp;preto;Prateleira&amp;rbrack; Novo Arnold 5 exportar predefinições
* &amp;lbrack;Scripting&amp;brack; Permitir a importação de recursos para a Prateleira

**Problemas Conhecidos:**

* &amp;preto;Exportar&amp;rbrack; A edição de uma predefinição de exportação é muito lenta

## Versão 2

### 2.6.2

*(Lançado: 20 de outubro de 2017)*

**Adicionado:**

* &amp;lbrack;Conjunto de texturas&amp;rbrack; Permite excluir conjuntos de texturas desativados
* &amp;lbrack;Shelf&amp;rbrack; Permite que vários usuários gravem dentro da mesma pasta de prateleira
* &amp;lbrack;Scripting&amp;brack; Ser capaz de recarregar a pasta de plug-ins
* &amp;lbrack;Scripting&amp;rbrack; Adicione uma versão mínima necessária da API nos metadados do plug-in para garantir a compatibilidade
* &amp;lbrack;IRay&amp;rbrack; Melhorias na caixa de diálogo Exportar imagem

**Corrigido:**

* &amp;lbrack;Engine&amp;rbrack; Problema de traçados que desaparecem, ao alterar a resolução (4K>2K)
* &amp;lbrack;Baker&amp;rbrack; Falha na Faz bake do Mapa de ID com a opção Corresponder pelo nome ativada
* &amp;lbrack;Baker&amp;rbrack; As mensagens de erro não são suficientemente explícitas
* &amp;lbrack;Visualização 3D&amp;rbrack; O espaço tangente não está sincronizado com baker
* &amp;preto;Tool&amp;brack; Artefatos pretos ao usar a ferramenta de borrar
* &amp;lbrack;Sombreador&amp;rbrack; O sombreador não-PBR não funciona mais
* &amp;lbrack;Sombreador&amp;rbrack; “pbr-coated” is broken
* &amp;lbrack;Sombreador&amp;rbrack; A aspereza do revestimento do sombreador “pbr-coated” não tem mais impacto
* &amp;lbrack;Sombreador&amp;rbrack; O sombreador com brilho de especificação não corresponde a Iray e SD
* &amp;lbrack;Shelf&amp;rbrack; Falha ao carregar dois arquivos com o mesmo nome, mas extensões diferentes
* &amp;lbrack;Shelf&amp;rbrack; Não é mais possível editar a predefinição nas prateleiras
* &amp;predefinição;Prateleira&amp;predefinição; Não é possível definir uma visualização personalizada para ativos importados na prateleira
* Os recursos carregados do cache perdem seus usos
* Salvar um projeto antes de criar um modelo retorna erros de permissão de gravação
* Salvar projeto incorreto se o nome do arquivo contiver dois pontos
* Importação de arquivos com vários pontos (.) no nome do arquivo causa problemas

### 2.6.1

*(Lançado: 12 de maio de 2017)*

**Adicionado:**

* &amp;lbrack;TextureSet&amp;rbrack; Não permitir a reatribuição de materiais de malha a nada

**Corrigido:**

* Falha ao alternar o TextureSet após substituir o mapa baked
* Falha ao fazer “Desfazer e Refazer” após alterar o modo de mesclagem da camada
* Falha ou congelamento ao usar o efeito “seleção de cores” com um mapa de ID grande
* &amp;preto;Exportar&amp;rbrack; Os conjuntos de texturas renomeados não são classificados em ordem alfabética na janela de exportação
* &amp;lbrack;TextureSet&amp;rbrack; Redefinir para o nome padrão não verifica a unicidade
* &amp;lbrack;TextureSet&amp;rbrack; O conjunto de texturas renomeado fica desativado após a reabertura do projeto
* &amp;lbrack;Shelf&amp;rbrack; Conteúdo de modelos padrão ausente
* &amp;preto;Prateleira&amp;rbrack; As texturas não quadradas são exibidas como quadradas
* &amp;lbrack;Sombreador&amp;rbrack; Quando um conjunto de texturas é desativado, o sombreador associado é destruído
* &amp;lbrack;Scripting&amp;brack; alg.fazendo bake.definirTexturaDefinirParâmetros() não funciona mais
* &amp;lbrack;Erro de ortografia&amp;rbrack; no tutorial do websocket
* &amp;lbrack;Scripting&amp;brack; Vários problemas em AlgWidgets
* &amp;lbrack;Log&amp;rbrack; Detecção incorreta de memória virtual disponível em alguns casos

### 2.6.0

*(Lançado: 27 de abril de 2017)*

**Adicionado:**

* Adicionar novo projeto de amostra “Meet Mat”
* &amp;lbrack;Plug-in&amp;rbrack; Novo plug-in “Atualizador de recursos”
* &amp;lbrack;TextureSet&amp;rbrack; Permite renomear e adicionar uma descrição aos conjuntos de texturas
* &amp;lbrack;TextureSet&amp;rbrack; Permitir a reatribuição de materiais
* &amp;lbrack;TextureSet&amp;rbrack; Adiciona um botão de configuração na janela da lista do conjunto de texturas
* &amp;lbrack;TextureSet&amp;rbrack; Mostrar conjuntos de texturas “desativados” na parte inferior da lista
* &amp;lbrack;Substance&amp;rbrack; Usar mapas adicionais na resolução atual do conjunto de texturas para melhorar o desempenho
* &amp;lbrack;Scripting&amp;rbrack; Permite atualizar um recurso usado em um projeto (material, gerador, etc.)
* &amp;lbrack;Scripting&amp;brack; Adicionar uma maneira de adicionar/remover uma prateleira
* &amp;lbrack;Scripting&amp;rbrack; Permitir a consulta de informações do recurso em projetos
* &amp;lbrack;Scripting&amp;brack; Permite recuperar uma lista de prateleiras disponíveis
* &amp;lbrack;Scripting&amp;brack; Melhorar tutorial em miniatura do AlgWidget
* &amp;lbrack;Export&amp;rbrack; Desativar/Ativar profundidade de bits com base no suporte ao formato de arquivo
* &amp;lbrack;Log&amp;brack; Adicionar nome de plug-in para imprimir no console
* &amp;lbrack;Log&amp;brack; Remove o erro sobre conjuntos de texturas ocultos
* Atualizar “Tela de boas-vindas” com novos ícones e texto para amostras

**Corrigido:**

* Falha ao atualizar uma malha em projetos específicos
* A cor interna do plano de Simetria do &amp;lbrack;Viewport&amp;rbrack; não está mais visível
* &amp;lbrack;Visor&amp;rbrack; Alguns efeitos pós-processo são ativados ao usar a exibição solo
* A mesclagem de &amp;brack;Shaders&amp;brack; “over_premult” não funciona corretamente
* &amp;lbrack;Sombreadores&amp;rbrack; Aviso sobre o teste alfa com o sombreador padrão
* &amp;lbrack;Prateleira&amp;rbrack; Análise incorreta de tags de Substance
* O &amp;lbrack;Shelf&amp;rbrack; MatFX Ferrugem Weathering não funciona corretamente
* O filtro HSL do &amp;brack;Shelf&amp;rbrack; está habilitado em canais incorretos por padrão
* &amp;lbrack;Shelf&amp;rbrack; A nitidez está habilitada no canal Height/Normal por padrão
* &amp;lbrack;Export&amp;rbrack; As predefinições de exportação variadas não usam um mapa normal OpenGL
* &amp;lbrack;Tool&amp;brack; Problemas de imprecisão com a ferramenta clonar/borrar criam artefatos

### 2.5.3

*(Lançado: 15 de março de 2017)*

**Corrigido:**

* &amp;lbrack;Baker&amp;rbrack; Falha ao fazer bake com malhas específicas

**Problemas Conhecidos:**

* &amp;lbrack;Mac&amp;rbrack; Partículas podem criar corrupção de textura em alguns casos

### 2.5.2

*(Lançado: 14 De março De 2017)*

**Corrigido:**

* &amp;lbrack;Tool&amp;brack; Os tablets Wacom não funcionam no Linux
* &amp;preto;Tool&amp;brack; Artefatos pretos ao usar a ferramenta de borrar
* &amp;lbrack;Baker&amp;rbrack; falha na Faz bake se Corresponder pelo nome for usado com uma caixa
* &amp;lbrack;Baker&amp;rbrack; Oclusão de ambiente interrompida ao fazer bake somente com Mapa normal
* &amp;lbrack;Shelf&amp;rbrack; Os filtros genéricos não tratam o alfa corretamente (Contraste/Luminosidade, Highpass, etc.)
* &amp;lbrack;Viewport&amp;rbrack; Problema de desempenho ao carregar um projeto com sombras ativadas
* &amp;lbrack;Viewport&amp;rbrack; Problema de pontilhamento no Visualização 3D MacOS
* &amp;lbrack;Visor&amp;rbrack; Visualizações de partículas exibidas incorretamente quando o perfil de cores está ativado
* &amp;lbrack;Iray&amp;rbrack; Falha ao alternar o projeto de volta para OpenGL se o Iray não inicializar
* &amp;lbrack;IRay&amp;rbrack; A textura reluzente é ignorada ao renderizar SpecGloss sombreador/mdl
* &amp;lbrack;Sombreador&amp;rbrack; O sombreador de especificação/brilho não corresponde a Iray e SD
* &amp;lbrack;Sombreador&amp;rbrack; sRGB conversão diferente de linear para sRGB LUT conversão
* &amp;lbrack;Sombreador&amp;rbrack; Renderização incorreta ao carregar projeto com sombreadores desatualizados
* &amp;lbrack;Sombreador&amp;rbrack; sombreador “pbr-coated” não funciona mais
* &amp;lbrack;Export&amp;brack; Alguns canais ainda são exportados, mesmo que não estejam presentes no conjunto de texturas
* &amp;lbrack;Camadas&amp;rbrack; O modo de mesclagem “detalhe inverso do mapa normal” não funciona em canais em tons de cinza
* &amp;lbrack;UI&amp;rbrack; Problema em “Janela de seleção de cores” com monitor HDPI e zoom de exibição em 150%

**Problemas Conhecidos:**

* &amp;lbrack;Mac&amp;rbrack; Partículas podem criar corrupção de textura em alguns casos

### 2.5.1

*(Lançado: 27 de fevereiro de 2017)*

**Corrigido:**

* &amp;lbrack;A entrada do tablet Mac&amp;rbrack; Wacom está interrompida em 3D e Visualização 2D
* &amp;lbrack;Baker&amp;rbrack; A correspondência por nome não funciona mais
* &amp;lbrack;Baker&amp;rbrack; A configuração de “Média Normalizada” não funciona mais
* &amp;lbrack;Iray&amp;rbrack; Renderização incorreta sem mapa normal feito bake
* &amp;lbrack;Iray&amp;rbrack; Perfis de cores se comportam de maneira diferente em comparação ao renderizador OpenGL
* &amp;lbrack;Iray&amp;rbrack; Exportar a renderização como bitmap não inclui a correção do perfil de cores
* Os Filtros Materiais do &amp;lbrack;Substance&amp;rbrack; não funcionam mais
* &amp;preto;Tool&amp;brack; A opacidade do traçado não está armazenada em predefinições de pincel
* &amp;lbrack;Tool&amp;brack; O Alinhamento UV do Pincel Clonar não funciona mais
* O canal de Deslocamento do &amp;lbrack;Export&amp;brack; deve ser centralizado em 0,5 ao exportar em números inteiros
* &amp;lbrack;Modelo&amp;rbrack; O caminho absoluto é armazenado em Modelos
* A textura do canal do &amp;brack;TextureSet&amp;rbrack; persiste após remover o canal

**Problemas Conhecidos:**

* As entradas dos tablets &amp;lbrack;Linux&amp;rbrack; Wacom não funcionam em 3D e Visualização 2D
* &amp;lbrack;Mac&amp;rbrack; Partículas podem criar corrupção de textura em alguns casos
* &amp;lbrack;Export&amp;brack; Em casos muito raros, retângulos pretos podem aparecer em GPUs AMD

### 2.5.0

*(Lançado em: 21 de fevereiro de 2017)*

**Adicionado:**

* Adicionar compatibilidade com as GPUs AMD Radeon Pro e AMD FirePro
* &amp;lbrack;Tool&amp;brack; Adicionar suporte para opacidade de traçado
* &amp;lbrack;Tool&amp;brack; Adiciona um modificador que permite continuar a última pincelada
* &amp;lbrack;Iray&amp;rbrack; Atualização para suportar GPUs Pascal
* &amp;preto;Visor&amp;rbrack; Adicionar suporte para perfis de cores (LUT)
* &amp;lbrack;Substance&amp;rbrack; Integrar nova estrutura (mecanismo SD6)
* &amp;lbrack;UI&amp;rbrack; Aumentar lista de tamanhos do “arquivo recente” no menu Arquivo
* &amp;lbrack;Import&amp;brack; Usar categoria de substâncias para preencher o prefixo na caixa de diálogo de importação
* &amp;lbrack;Baker&amp;rbrack; Permitir fazer bake texturas 8K
* &amp;lbrack;Baker&amp;rbrack; Permitir fazer bake resoluções não quadradas
* &amp;lbrack;Baker&amp;rbrack; Melhorar o consumo de memória ao fazer bake malhas pesadas de alta poli
* &amp;preto;Shelf&amp;rbrack; Bloquear prateleiras (e projetos) para proibir a edição simultânea e evitar corrupções
* &amp;lbrack;Shelf&amp;rbrack; Ler categoria e palavras-chave de substâncias para usá-las na filtragem
* &amp;lbrack;Shelf&amp;rbrack; Permite excluir recursos do resultado de uma consulta de pesquisa
* &amp;lbrack;Prateleira&amp;rbrack; Cálculo de tempo de miniaturas aprimorado
* &amp;predefinição;Prateleira&amp;predefinição; Permitir incorporar predefinições em projetos
* &amp;lbrack;Shelf&amp;rbrack; Permite recolher/expandir rapidamente a exibição de árvore com SHIFT
* &amp;lbrack;Shelf&amp;rbrack; Permite salvar miniaturas quando os ativos são somente leitura (cache local)
* &amp;lbrack;Shelf&amp;rbrack; Novo conteúdo : novos filtros (transformo, espelho, tri-planar, etc.)
* &amp;lbrack;Shelf&amp;rbrack; Novo conteúdo: novos perfis de LUTs (clássicos e artísticos, como Film Noir, Vintage etc.)
* &amp;lbrack;Shelf&amp;rbrack; Novo conteúdo: 10 novas Substance de fonte para gerar textos personalizados rapidamente
* &amp;lbrack;Shelf&amp;rbrack; Novos modelos: Unity 5 e Unreal Engine 4
* &amp;lbrack;Shelf&amp;rbrack; Filtro HSL aprimorado para ser mais amigável com artistas
* &amp;lbrack;Sombreador&amp;rbrack; Adicionar suporte para canal de specular level em sombreadores PBR
* &amp;lbrack;Sombreador&amp;rbrack; Adicionar suporte para pontilhamento em sombreador de teste
* &amp;lbrack;Sombreador&amp;rbrack; Adicionar suporte para mapeamento de oclusão de paralaxe em sombreadores PBR
* &amp;lbrack;Sombreador&amp;rbrack; Permite definir interface personalizada para parâmetros de sombreador
* &amp;lbrack;MatLayering&amp;rbrack; Criar novo canal de Máscara para fluxo de trabalho de camada de material
* &amp;lbrack;Scripting&amp;brack; Permite gravar metadados em um projeto SP
* &amp;lbrack;Scripting&amp;brack; Permite exportar com uma predefinição de exportação específica
* &amp;lbrack;Scripting&amp;rbrack; Permite recuperar parâmetros de sombreador como um JSON
* &amp;lbrack;Scripting&amp;brack; Adicionar suporte para conexões WebSocket
* &amp;lbrack;Scripting&amp;brack; Adicionar a possibilidade de carregar instâncias de sombreamento
* &amp;lbrack;Scripting&amp;brack; Adicionar a possibilidade de criar um novo projeto
* &amp;lbrack;Scripting&amp;rbrack; Permite recuperar a url da malha importada em um projeto
* &amp;lbrack;Scripting&amp;rbrack; Permitir fça bake não quadrado
* &amp;lbrack;Scripting&amp;rbrack; Relatar erros ao definir dados por meio da API de script
* &amp;lbrack;Substance&amp;rbrack; Adicionar tag de dados do usuário para especificar o formato de mapa normal

**Corrigido:**

* Falha ao selecionar cor com substâncias
* Falha ao carregar uma imagem não RGBA32f como mapa de ambiente
* Falha relacionada à pintura em GPUs AMD
* A importação de OBJ do &amp;brack;Mesh&amp;brack; não reconhece materiais sem arquivo mtl
* &amp;lbrack;Mesh&amp;rbrack; A geração do nome do conjunto de Textura UDIM pode estar incorreta em algumas malhas
* &amp;lbrack;UI&amp;rbrack; Botão Desfazer/Refazer na Configuração do Visualizador roubar foco e parar a rolagem do mouse
* &amp;lbrack;UI&amp;rbrack; Alguns rótulos são cortados incorretamente em Hi-DPI
* &amp;lbrack;Camada&amp;rbrack; O modo de substituição do efeito de tinta possui um comportamento incorreto na Máscara
* O modo de mesclagem &amp;preto;Camada&amp;rbrack; tem um comportamento incorreto com alfa
* &amp;lbrack;Tool&amp;rbrack; O tamanho do pincel se torna muito grande no Visualização 2D ao pintar nas bordas UV
* &amp;lbrack;Tool&amp;brack; A linha reta encaixada apresenta um comportamento irregular com Hi-DPI
* A resolução do estêncil do &amp;brack;Tool&amp;brack; às vezes está incorreta
* Os valores de &amp;lbrack;Baker&amp;rbrack; “Distância máxima do ocluso” serão bloqueados se “em relação à caixa delimitadora” estiver “Desativado”
* &amp;lbrack;Sombreador&amp;rbrack; As definições de canal de parâmetros automáticos e de pilha não correspondem
* &amp;lbrack;Visualização 3D&amp;rbrack; Exibição inconsistente do canal normal dependendo da configuração do projeto
* &amp;lbrack;Viewport&amp;rbrack; Alguns mapas normais têm valores fixados que aparecem como artefatos
* &amp;lbrack;Viewport&amp;rbrack; O pós-efeito sempre é desativado por padrão
* &amp;lbrack;Exportar&amp;rbrack; A configuração de mixagem normal estará incorreta se o canal normal estiver ausente
* &amp;lbrack;Export&amp;rbrack; Geração de textura incorreta em alguns casos em GPUs AMD
* Os parâmetros de Sombreador do &amp;brack;Export&amp;brack; não são exportados corretamente se localizados dentro de um grupo
* &amp;lbrack;Export&amp;brack; Editar uma predefinição de exportação em uma prateleira personalizada gera um erro de registro
* A filtragem do modo de exibição em árvore do &amp;brack;Shelf&amp;rbrack; não corresponde exatamente ao nome da pasta
* &amp;lbrack;Prateleira&amp;rbrack; Renomear uma predefinição de prateleira é difícil de ler
* &amp;lbrack;O recurso de Sombreador importado na Prateleira não é preservado após a reinicialização
* &amp;Predefinição;Prateleira&amp;predefinição; Conteúdo: A predefinição da ferramenta de solda está ausente
* &amp;lbrack;Shelf&amp;rbrack; Conteúdo : Tile Generator não funciona corretamente
* &amp;lbrack;Shelf&amp;rbrack; Conteúdo: correção de máscara incorreta no material inteligente Sujo de Pneu de Borracha
* &amp;lbrack;Shelf&amp;rbrack; Conteúdo: corrigido o nome incorreto do grupo no material do saco de couro
* &amp;lbrack;Iray&amp;rbrack; Metade das malhas está ausente em Iray
* &amp;lbrack;Linux&amp;rbrack; Falha ao arrastar um recurso acima da Visualização 3D
* &amp;lbrack;Mac&amp;rbrack; As preferências são redefinidas a cada inicialização no Sierra

**Problemas Conhecidos:**

* &amp;lbrack;Export&amp;brack; Em casos muito raros, retângulos pretos podem aparecer em GPUs AMD
* Os perfis de cores do &amp;lbrack;Iray&amp;rbrack; podem se comportar de maneiras ímpares às vezes

### 2.4.1

*(Lançado: 28 de outubro de 2016)*

**Corrigido:**

* Falha ao criar um projeto com um modelo
* Falha ao fechar a caixa de diálogo de exportação durante uma exportação
* &amp;lbrack;Mac&amp;rbrack; Erros ao salvar o projeto (falha ao salvar a predefinição de exportação)
* &amp;preset;Shelf&amp;rbrack; Criar uma nova predefinição a exibirá duas vezes
* &amp;preto;O Shelf&amp;rbrack; Predefinições não podem ser carregadas no modo somente leitura sem direitos administrativos

### 2.4.0

*(Lançado: 27 de outubro de 2016)*

**Adicionado:**

* &amp;lbrack;Shelf&amp;rbrack; Nova interface para procurar recursos (exibição de árvore, filtros e assim por diante)
* &amp;lbrack;Shelf&amp;rbrack; Permitir salvar uma pesquisa como predefinição
* &amp;lbrack;Shelf&amp;rbrack; Permite criar uma nova janela a partir de uma predefinição
* &amp;lbrack;Shelf&amp;rbrack; Nova interface para importar recursos
* &amp;lbrack;Prateleira&amp;rbrack; Não copiar a prateleira alegorítmica padrão na pasta Documentos
* &amp;lbrack;Prateleira&amp;rbrack; Novas predefinições de partículas: Circuito Elétrico, Linhas Elétricas, Rococó, Veias Pequenas
* &amp;lbrack;Shelf&amp;rbrack; Predefinições de partículas mais antigas aprimoradas para serem mais fáceis de usar (como “Rain”)
* &amp;predefinição;Prateleira&amp;predefinição; Adicionar novas informações no menu contextual do recurso
* &amp;lbrack;Viewport&amp;rbrack; Melhorar o desempenho ao carregar mapas do ambiente
* &amp;lbrack;Viewport&amp;rbrack; Adicionar suporte a mapas de ambiente que não sejam potência de dois

**Corrigido:**

* Falha ao remover uma máscara
* Falha ao pintar após salvar uma predefinição
* Falha com desfoque de ambiente em algumas GPUs
* Falha ao atribuir um recurso errado com a miniprateleira
* &amp;Preenchimento;Prateleira&amp;rbrack; Limpar + Salvar remove marcas e metadados de recursos no projeto
* &amp;lbrack;Prateleira&amp;rbrack; importar uma predefinição exibirá seus recursos na prateleira
* O Mapa normal &amp;lbrack;Export&amp;brack; gerado a partir do canal do height tem baixa intensidade
* &amp;lbrack;Export&amp;brack; Normal da malha nem sempre está presente no mapa normal final
* &amp;preto;Exportar&amp;rbrack; Dilatação com transparência às vezes pode resultar sem transparência
* &amp;lbrack;Scripting&amp;brack; “alg.plugin_root_diretory” pode retornar um caminho de rede truncado
* O botão Bloquear &amp;preto;TextureSet&amp;rbrack; é ativado ao reabrir projetos não quadrados

### 2.3.1

*(Lançado em: 07 de outubro de 2016)*

**Adicionado:**

* &amp;lbrack;Plugin&amp;rbrack;&amp;lbrack;Photoshop&amp;rbrack; Permite especificar qual material/pilha/canais exportar
* &amp;lbrack;Scripting&amp;rbrack; Os nomes de função possuem algumas inconsistências

**Corrigido:**

* &amp;lbrack;O Alpha de &amp;exportação pode ser descartado nas predefinições de exportação personalizadas
* &amp;lbrack;Export&amp;rbrack; Alpha obtém conversão incorreta de gama em canais sRGB
* &amp;preto;Exportar&amp;rbrack; Documentos não quadrados são exportados como quadrados
* &amp;lbrack;Export&amp;brack; Impossível exportar mapas adicionais se algum estiver faltando
* &amp;lbrack;Iray&amp;rbrack; Alguns parâmetros (como a Intensidade de emissivo) não têm efeito
* &amp;lbrack;NVIDIA&amp;rbrack; Falha na inicialização com NVIDIA Quadro K2200/GTX 750/760
* &amp;lbrack;AMD&amp;rbrack; Conjunto incorreto de cores para miniaturas e visualizações
* &amp;lbrack;AMD&amp;rbrack; Congela e falha do driver em Novo Arquivo e Abrir Arquivo
* &amp;lbrack;Log&amp;brack; “software-version” está ausente do arquivo de log

### 2.3.0

*(Lançado: 15 de setembro de 2016)*

**Adicionado:**

* &amp;lbrack;Plug-in&amp;rbrack; Novo plug-in “Exportar para o Photoshop” (pilha de camadas completa de exportação)
* &amp;lbrack;Export&amp;brack; Permite especificar a largura do preenchimento (em pixels ou infinito)
* &amp;lbrack;Export&amp;brack; Permite definir o tipo de fundo fora dos UVs
* &amp;lbrack;Prateleira&amp;rbrack; Novo sombreador de camadas de material para mesclar 10 materiais
* &amp;lbrack;Prateleira&amp;rbrack; Novo sombreador de argila para ver detalhes com o canal height/normal
* &amp;lbrack;Shelf&amp;rbrack; Novo filtro de iluminação feito bake com entrada de ambiente
* &amp;lbrack;Shelf&amp;rbrack; Alguns geradores de máscara foram atualizados para adicionar transformações não quadradas
* &amp;preto;Visor&amp;rbrack; Adicionar mapa normal composto (normal+height+faço bake) ao modo solo
* &amp;lbrack;Scripting&amp;brack; Permite exportar mapas adicionais
* &amp;lbrack;Scripting&amp;brack; Permitir a consulta de mapas adicionais disponíveis por conjunto de textura
* &amp;lbrack;Scripting&amp;brack; Permitir a recuperação do formato do canal
* &amp;lbrack;Scripting&amp;brack; Adicionar exemplos na documentação de fça bake
* &amp;lbrack;Scripting&amp;brack; Permite consultar a visibilidade de uma camada
* &amp;lbrack;Scripting&amp;brack; Permitir consultar modo de mesclagem e opacidade da camada
* &amp;lbrack;Scripting&amp;brack; Permite exportar mapas convertidos (mapas normais finais, AO misto, etc.)
* &amp;lbrack;Substance&amp;rbrack; Ler e conectar usos personalizados
* &amp;lbrack;Atalhos&amp;rbrack; Adicionar tecla modificadora (SHIFT) para percorrer o modo solo para trás
* &amp;lbrack;Export&amp;brack; Atualização da predefinição de exportação padrão para desativar a alfa
* &amp;lbrack;UI&amp;rbrack; As miniaturas agora são computadas somente se o mecanismo estiver disponível
* &amp;lbrack;UI&amp;rbrack; Exibir uma menção quando as miniaturas estiverem sendo computadas

**Corrigido:**

* Falha com alguns projetos antigos ao abri-los
* Falha com cache de canais de textura corrompido
* Falha ao mesclar mais de 4 materiais com o fluxo de trabalho de Camada de material
* Os atalhos da ferramenta &amp;lbrack;UI&amp;rbrack; não funcionam se a barra de ferramentas estiver oculta
* &amp;lbrack;UI&amp;rbrack; A barra de ferramentas do Iray está rotulada como “Sem Título” no Menu Exibir
* As barras de ferramentas do plug-in &amp;lbrack;UI&amp;rbrack; são chamadas de “Não Inclinadas” no menu Exibir
* &amp;lbrack;Baker&amp;rbrack; Pressionar Enter enquanto edita uma configuração de faço bake inicia o processo do faço bake
* &amp;lbrack;Baker&amp;rbrack; Intervalos incorretos para alguns parâmetros
* &amp;lbrack;Import&amp;rbrack; Impossível importar malhas OBJ devido a números muito grandes
* &amp;lbrack;Import&amp;rbrack; Alguns arquivos OBJ são importados com muitos sub-objetos
* O plano de fundo do canal do &amp;preto;Export&amp;brack; é preenchido com preto em vez da cor padrão na exportação
* &amp;lbrack;Tool&amp;brack; Partículas não funcionam corretamente se o CDV for muito baixo
* A cor de visualização do pincel do &amp;brack;Tool&amp;brack; está incorreta com máscaras em subpilhas
* &amp;lbrack;Visor&amp;rbrack; Quando o pincel vai para áreas vazias no Visualização 2D ele se torna gigantesco
* &amp;lbrack;Visor&amp;rbrack; Visualização do pincel em branco ao pintar texturas normais
* &amp;lbrack;Scripting&amp;rbrack; Documentação incorreta : “ao” listado em vez de “ambientoclusão”
* &amp;lbrack;Scripting&amp;rbrack; O processo iniciado com subprocess() é finalizado ao fechar o Painter
* &amp;lbrack;Shelf&amp;rbrack; filtro de iluminação Feito bake usa entrada de AO incorreta
* &amp;lbrack;MacOS&amp;rbrack; Projeto de hidrante de incêndio removido (incompatível)
* O projeto padrão é aberto ao carregar um arquivo \*.spt (em vez de \*.spp)

**Problemas Conhecidos:**

* &amp;lbrack;Plug-in&amp;rbrack; Devido ao Photoshop, o height e o canal normal não podem ser traduzidos como estão

### 2.2.0

*(Lançado: 22 de julho de 2016)*

**Adicionado:**

* &amp;lbrack;Shelf&amp;rbrack; Melhorar o sistema de pesquisa e as consultas
* &amp;preto;Prateleira&amp;rbrack; Adicionar campo de pesquisa para miniprateleiras
* &amp;lbrack;Sombreador&amp;rbrack; Permite definir a precisão da etapa para controles deslizantes
* &amp;lbrack;Sombreador&amp;rbrack; Adicionar um botão Desfazer/Refazer para parâmetros de sombreador
* &amp;lbrack;Sombreador&amp;rbrack; Recarregar um sombreador não deve redefinir seus parâmetros
* &amp;lbrack;MatLayering&amp;rbrack; Adicionar suporte para Camadas de material dinâmico e subpilhas
* &amp;lbrack;MatLayering&amp;rbrack; Permite importar arquivo json para definir as configurações de sombreador
* &amp;lbrack;MatLayering&amp;rbrack; Desbloquear limite de amostras de textura (alternar para texturas sem associação)
* &amp;lbrack;Scripting&amp;rbrack; Permite definir configurações de baker e iniciar seus cálculos
* &amp;lbrack;Substance&amp;rbrack; Use “uso” para conexões de entradas/saídas, além de identificadores
* &amp;lbrack;Tool&amp;rbrack; Permite selecionar o canal de visualização no visor para a Ferramenta de Projeção

**Corrigido:**

* Falha durante a inicialização se as substâncias estiverem localizadas na pasta errada
* O relatório de falhas às vezes não funciona devido a um arquivo de log incorreto
* &amp;lbrack;Iray&amp;rbrack; os Pós-efeitos não são atualizados quando o Iray é pausado
* &amp;lbrack;Iray&amp;rbrack; O atalho de foco automático não funciona mais
* &amp;lbrack;Iray&amp;rbrack; O comportamento do controle deslizante de abertura muda dependendo do tamanho do ativo
* &amp;lbrack;Camadas&amp;rbrack; O primeiro canal de material não é ativado por padrão se estiver desativado
* &amp;lbrack;Sombreador&amp;rbrack; Nenhum erro será impresso se um “param auto” estiver incorreto

**Problemas Conhecidos:**

* &amp;lbrack;O limite de amostras de Textura do Mac&amp;rbrack; está bloqueado em 16 (problema no driver de GPU)

### 2.1.1

*(Lançado em: 01 de julho de 2016)*

**Adicionado:**

* &amp;lbrack;Licença&amp;rbrack; Ser capaz de alterar o local do arquivo de licença
* &amp;Preenchimento;Visor&amp;Parâmetro; Adicionar um atalho “B” para alternar entre mapas adicionais
* &amp;lbrack;Import&amp;rbrack; Permite importar FBX 2016/2017 corretamente
* &amp;lbrack;Tool&amp;brack; Remover verificadores ao usar a máscara rápida
* &amp;lbrack;Iray&amp;rbrack; Adicionar informações de dimensões de cena
* &amp;lbrack;Iray&amp;rbrack; Permite aumentar o número máximo de amostras e o tempo de renderização
* &amp;lbrack;UI&amp;rbrack; Atualizar resultado imediatamente ao usar o botão +/- nos controles deslizantes
* &amp;lbrack;UI&amp;rbrack; Permite maior precisão para controles deslizantes em Tons de Cinza
* &amp;lbrack;Export&amp;brack; Não exporte um canal alfa somente para o textura RGB
* &amp;preto;Export&amp;brack; Atualizar predefinição de exportação do Dota 2
* &amp;lbrack;Shelf&amp;rbrack; Novo padrão de “ladrilhos de hexágono”
* &amp;lbrack;Prateleira&amp;rbrack; Nova ferramenta “Solda”
* &amp;lbrack;Shelf&amp;rbrack; Filtros de acabamento atualizados para fornecer controles de direção

**Corrigido:**

* &amp;lbrack;Export&amp;brack; Impossível exportar arquivos de PSD em 8 bits
* &amp;lbrack;Export&amp;rbrack; A exportação em 8K não está disponível em algumas configurações de hardware
* &amp;lbrack;A janela do Sketchfab do Export&amp;rbrack; foi cortada
* &amp;lbrack;Export&amp;brack; Mapa de aspereza incorreto na predefinição de exportação de Especificação/Brilho
* &amp;lbrack;UI&amp;rbrack; A digitação em controles deslizantes em tons de cinza não funciona mais
* &amp;lbrack;UI&amp;rbrack; Impossível colocar filtros nas entradas do substance (como Geradores)
* &amp;lbrack;UI&amp;rbrack; Alguns controles deslizantes têm comportamentos ímpares
* &amp;lbrack;UI&amp;rbrack; DeltaTime +/- passo para partículas é muito grande
* &amp;lbrack;Iray&amp;rbrack; Alguns projetos bloqueiam o aplicativo ao mudar para o Iray
* &amp;lbrack;Iray&amp;rbrack; Falha ao detectar hardware
* A cor de visualização do Pincel no &amp;brack;Tool&amp;brack; está incorreta no modo Máscara
* &amp;lbrack;Tool&amp;brack; O seletor de materiais pode ser usado com ferramentas incompatíveis
* &amp;lbrack;Tool&amp;brack; A visualização da projeção não alterna para a Difusão com o fluxo de trabalho Espec/Gloss
* &amp;lbrack;Prateleira&amp;rbrack; Alterar as quebras de sombreador padrão smart mats/visualizações do máscara inteligente
* &amp;lbrack;Shelf&amp;rbrack; Alguns materiais inteligentes têm nomes incorretos
* &amp;lbrack;Shelf&amp;rbrack; Formas alfa adicionais estão corrompidas e não serão carregadas
* &amp;lbrack;Viewport&amp;rbrack; Alternando para o modo “Mapa adicional” exibe “outro” primeiro
* &amp;lbrack;Visor&amp;rbrack; Visor voltar para “outro” quando não existir um mapa adicional
* &amp;lbrack;Crash&amp;rbrack;&amp;lbrack;Linux&amp;rbrack; O relatório de falhas não funciona no Ubuntu (Steam)
* &amp;lbrack;Crash&amp;rbrack;&amp;lbrack;Links de URL da Web do Linux&amp;rbrack; não funcionam no Ubuntu (Steam)
* &amp;lbrack;Crash&amp;rbrack;&amp;lbrack;Windows&amp;rbrack; Remover “crashwatcher” quando o Substance painter não estiver mais em execução
* &amp;lbrack;Crash&amp;rbrack;&amp;lbrack;O sistema de relatório de falhas do Mac&amp;rbrack; não funciona corretamente
* &amp;lbrack;Falha&amp;rbrack; Importar uma malha enquanto já importa uma malha leva a uma falha
* O atalho de separação do conjunto de textura não é redefinido para nada após uma reinicialização

### 2.1.0

*(Lançado em: 2 de junho de 2016)*

**Adicionado:**

* &amp;lbrack;UDIM&amp;rbrack; Importar ladrilhos UDIM de uma malha como conjuntos de texturas
* &amp;lbrack;Linux&amp;rbrack; Suporte adicionado para CentOS 6.6 e Ubuntu 12.4
* &amp;lbrack;Export&amp;brack; Adicionar resolução 8K (experimental)
* &amp;lbrack;Export&amp;brack; Permite escolher a profundidade de bits durante a exportação
* &amp;lbrack;Baker&amp;rbrack; Permite fazer bake vários conjuntos de texturas de uma vez
* Suporte a monitores de alta resolução (dimensionamento de DPI alto)
* &amp;lbrack;Scripting&amp;rbrack; Definir resolução personalizada e preenchimento por textura na exportação
* &amp;lbrack;Viewport&amp;rbrack; Permite alternar entre conjuntos de textura clicando na malha (via Ctrl+Alt+Clique)
* &amp;preto;Visor&amp;rbrack; Ir onde está o cursor do mouse ao aplicar zoom com a roda do mouse
* &amp;lbrack;UI&amp;rbrack; Atualizar cor de fundo padrão e exibição do mapa de ambiente
* &amp;lbrack;UI&amp;rbrack; Adicionar dicas com nomes originais para canais do usuário
* &amp;lbrack;UI&amp;rbrack; Alterar a cor do plano de fundo dos canais que não podem ser renomeados
* &amp;lbrack;Tool&amp;brack; Remover verificadores ao usar a máscara rápida
* &amp;lbrack;Sombreador&amp;rbrack; Permite definir grupos para parâmetros de sombreador e materiais/máscaras
* &amp;lbrack;Engine&amp;rbrack; Otimização de carimbos de tamanho pequeno
* &amp;lbrack;Estêncil&amp;rbrack; Adicionar “W” como atalho para alternar temporariamente a máscara
* &amp;prego;Prateleira&amp;rcolete; Adicionar um botão de cruz para limpar o campo de pesquisa
* &amp;lbrack;Shelf&amp;rbrack; Carregar Alpha com um único clique
* &amp;lbrack;Shelf&amp;rbrack; Nova predefinição de exportação: Vray UDIM, Arnold UDIM, Spec/Gloss from Metal/Rough
* &amp;lbrack;Shelf&amp;rbrack; Novas alfas: formas geométricas, veias e sinais
* Adicionar nome e versão nas propriedades do executável Substance Painter

**Corrigido:**

* &amp;lbrack;Substance&amp;rbrack; Impossível usar o canal normal e mapa adicional ao mesmo tempo
* &amp;lbrack;Iray&amp;rbrack; a refração MDL e a configuração de absorção não funcionam
* &amp;lbrack;Iray&amp;rbrack; A escala da cena original não é preservada
* &amp;lbrack;Shelf&amp;rbrack; modelo de Specular/Textura Reluzente usar um sombreador incorreto
* &amp;preto;Exportar&amp;rbrack; A predefinição de exportação padrão não exporta alguns mapas (como o AO)
* &amp;lbrack;Viewport&amp;rbrack; O ponto dinâmico não é atualizado ao clicar fora dos UVs na Visualização 2D
* &amp;lbrack;UI&amp;rbrack; Os valores do controle deslizante são arredondados
* &amp;lbrack;UI&amp;rbrack; Às vezes, ao editar os valores dos controles deslizantes, há um espaço livre muito pequeno
* &amp;lbrack;A lista suspensa Novo Projeto&amp;rbrack; Modelo não foi atualizada corretamente (de 1.x para 2.x)
* &amp;lbrack;Scripting&amp;brack; Comportamento “hover” fixo em botões personalizados
* &amp;lbrack;Mac&amp;rbrack; Ao desfazer em um projeto vazio, a câmera fica bloqueada

**Problemas Conhecidos:**

* O relatório de falha não está disponível no Ubuntu
* Alguns botões de URL podem não funcionar. Consulte nossas Perguntas frequentes para obter uma solução alternativa

### 2.0.5

*(Lançado: 29 de abril de 2016)*

**Adicionado:**

* &amp;predefinição de prateleira;Modelo não pbr adicionado/atualizado, sombreador e predefinição de exportação
* &amp;lbrack;Shelf&amp;rbrack; Atualizada a predefinição de exportação UE4 para incluir Oclusão de ambiente

**Corrigido:**

* Falha ao abrir e salvar alguns projetos com recursos corrompidos
* &amp;lbrack;Viewport&amp;rbrack; Wireframe aparece quebrado no Visualização 2D
* &amp;lbrack;Shelf&amp;rbrack; Desempenho aprimorado de alguns mapas de ambiente de estúdio
* &amp;lbrack;Shelf&amp;rbrack; Alguns mapas de ambiente de estúdio estão duplicados
* &amp;lbrack;Shelf&amp;rbrack; “Material de Iluminação Feito bake” Ausente
* &amp;lbrack;Shelf&amp;rbrack; Gerador “conversão em tons de cinza” ausente

### 2.0.4

*(Lançado: 26 de abril de 2016)*

**Adicionado:**

* Melhorar colisões de malha e otimizar a renderização de wireframe
* Melhore o desempenho e o gerenciamento de memória com grandes projetos
* Melhorar a precisão e a revisão do controle deslizante
* &amp;lbrack;UI&amp;rbrack; Atualizar mecanismo somente ao validar um controle deslizante (não ao inserir um valor)
* &amp;lbrack;UI&amp;rbrack; Move a opção Iray para um botão dedicado na barra de ferramentas principal (e altera seu atalho)
* &amp;lbrack;Tool&amp;brack; Adicionar configuração para o comportamento de localização da origem da ferramenta clonar
* &amp;lbrack;Sombreador&amp;rbrack; Permitir a leitura de cores de vértice de malha em sombreadores personalizados
* &amp;lbrack;Scripting&amp;brack; Permite recuperar a lista de conjuntos de texturas, canais e camadas
* &amp;lbrack;Scripting&amp;rbrack; Adicionar funções auxiliares (url para caminho, obter caminho de exportação do projeto)
* &amp;lbrack;Mac&amp;rbrack; Detectar versão “El Capitan” do Sistema Operacional Mac no arquivo de registro

**Corrigido:**

* Falha após a segunda exportação para o Substance share
* Falha ao copiar uma camada entre conjuntos de texturas com dados de Máscara rápida.
* Alguns projetos têm um atualizador muito longo que consome muita memória
* &amp;lbrack;Tool&amp;brack; Falha ao selecionar uma predefinição de partícula com a ferramenta clone/borrar
* &amp;lbrack;Baker&amp;rbrack; Carregar arquivos FBX leva muito tempo para malhas pesadas
* &amp;lbrack;Viewport&amp;rbrack; Mapa de ambiente ampliado em alguns computadores
* &amp;lbrack;Visor&amp;rbrack; Conversão de gama incorreta do alfa do pincel
* O Alpha de &amp;brack;Export&amp;brack; é armazenado como transparência em vez de um canal separado com arquivos Tiff.
* &amp;lbrack;Export&amp;brack; O canal Normal é sempre exportado como OpenGL
* &amp;lbrack;Iray&amp;rbrack; Nomes de controle deslizante ausentes para configurações de Iray
* &amp;lbrack;Iray&amp;rbrack; A renderização é feita em uma resolução incorreta em Retina/High DPI
* &amp;lbrack;Iray&amp;rbrack; Falha ao redimensionar a interface no modo Iray
* &amp;lbrack;Iray&amp;rbrack; Enorme redução de desempenho ao renderizar em algumas resoluções baixas
* &amp;lbrack;Iray&amp;rbrack; A pausa não funciona (o Iray ainda é computado em segundo plano)
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

* &amp;lbrack;Iray&amp;rbrack; Atualize o modelo e o sombreador de Spec/Gloss para que sejam compatíveis com o Iray
* &amp;lbrack;Export&amp;brack; Ser capaz de exportar capturas de tela para o ArtStation
* &amp;lbrack;Script&amp;rbrack; Suporte a execução a partir do diretório de plug-ins
* &amp;lbrack;Scripting&amp;rbrack; Permitir “Salvar como”
* &amp;lbrack;UI&amp;rbrack; Permite clicar duas vezes em um controle deslizante para editar seu valor
* Mover amostra do Vela para o Substance share
* Novo projeto de amostra: Visualização da esfera
* Avisar os usuários sobre conflito de extensão do shell

**Corrigido:**

* Instalação de substituição do instalador do Substance Painter 1.x
* &amp;lbrack;UI&amp;rbrack; O layout da lista de canais está quebrado com filtros
* &amp;lbrack;UI&amp;rbrack; os parâmetros de Sombreador não são exibidos
* &amp;lbrack;UI&amp;rbrack; Redimensionar a janela da camada corta incorretamente o conteúdo
* &amp;lbrack;Tool&amp;brack; O canal de Opacidade nem sempre é usado corretamente
* &amp;lbrack;Tool&amp;brack; Borrar/Clonar não funciona com Simetria
* A opacidade da visualização do Pincel no &amp;brack;Tool&amp;brack; está incorreta em alguns canais
* &amp;lbrack;Iray&amp;rbrack; Falha ao usar o Iray enquanto ele ainda não foi criado
* &amp;lbrack;Iray&amp;rbrack; Não é possível carregar os dados de configuração de iray do projeto
* &amp;lbrack;Iray&amp;rbrack; A Iray não cuida da modificação das configurações após ter sido pausada
* &amp;preto;Prateleira&amp;rbrack; Importar um material para a prateleira não funciona
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
* &amp;lbrack;Tool&amp;brack; Nova ferramenta Borrar para mesclar e espalhar cores
* &amp;lbrack;Tool&amp;rbrack; Nova ferramenta Clonar para copiar parte do textura
* &amp;lbrack;Tool&amp;brack; Permite selecionar canais para as ferramentas Borrar, Clonar e Borracha
* &amp;lbrack;Layer&amp;rbrack; Adicionar nome de Substance para nome do efeito de preenchimento
* &amp;lbrack;Camada&amp;rbrack; Permitir exportação de máscara para área de transferência
* &amp;lbrack;Visor&amp;rbrack; Alternar entre os modos de Perspectiva e ortográfica
* &amp;lbrack;Viewport&amp;rbrack; Permitir controlar o Campo de Visão no modo de Perspectiva
* &amp;lbrack;Visor&amp;rbrack; Permitir definir a Profundidade da distância do campo com CTRL+clique no meio
* &amp;lbrack;Viewport&amp;rbrack; Permite arrastar e soltar mapas de ambiente no Visualização 3D.
* &amp;lbrack;Viewport&amp;rbrack; Feedback aprimorado quando o mecanismo está fazendo cálculos fortes
* &amp;lbrack;Export&amp;brack; Permite exportar parâmetros de sombreador em um arquivo json
* &amp;lbrack;UI&amp;rbrack; Atualizar interface com novos ícones, cores e layout
* &amp;lbrack;UI&amp;rbrack; Adicionar nomes de ativos às miniprateleiras
* &amp;lbrack;UI&amp;rbrack; Recolher “Mapeamento de canais” por padrão
* &amp;lbrack;Sombreador&amp;rbrack; Escolha uma cor personalizada para os parâmetros de textura do sombreador
* &amp;lbrack;Shelf&amp;rbrack; Perguntar onde importar arquivos ao arrastar e soltar recursos
* &amp;lbrack;Shelf&amp;rbrack; Nova esfera de visualização para Materiais inteligentes e Geradores
* &amp;preto;Prateleira&amp;rbrack; Adicionar Specular Brilho sombreador
* &amp;preto;Prateleira&amp;rbrack; Novas formas de Superfície Dura
* &amp;lbrack;Prateleira&amp;rbrack; Novas Alpha textura e formas
* &amp;preto;Prateleira&amp;rbrack; Novas texturas de pele
* &amp;lbrack;Shelf&amp;rbrack; Novos materiais e materiais inteligentes baseados em digitalização
* &amp;lbrack;Shelf&amp;rbrack; Novos materiais inteligentes e suporte a especificações/brilhos de antigos
* &amp;lbrack;Shelf&amp;rbrack; Novos filtros de acabamento para simulação de superfície metálica
* &amp;lbrack;Shelf&amp;rbrack; Novo gerador de máscara poderoso “Editor de máscaras”
* &amp;lbrack;Prateleira&amp;rbrack; Materiais antigos retrabalhados e limpos
* Novo projeto de amostra “Vela”

**Corrigido:**

* &amp;lbrack;Configurações&amp;rbrack; A rotação da câmera e a velocidade de zoom são substituídas pelo projeto
* &amp;lbrack;Viewport&amp;rbrack; O problema de precisão na textura normal padrão leva a reflexos incorretos
* A vinheta do &amp;lbrack;Viewport&amp;rbrack; está ativada por padrão
* &amp;brack;Visor&amp;rbrack; Os artefatos aparecem nas bordas do mapa de ambiente (GPUs Nvidia)
* &amp;lbrack;Viewport&amp;rbrack; A miniatura no modo de projeção/estêncil é muito longa para carregar
* &amp;lbrack;Baker&amp;rbrack; Armazenar texturas feitas bake em inteiros de 16 bits em vez de 32 bits
* &amp;lbrack;Layer&amp;brack; Substâncias desatualizadas são exibidas incorretamente na pilha
* A cor padrão e a profundidade de bits de alguns canais estão incorretas (por exemplo: Specular, Textura reluzente)
* Corrigido o comportamento de borracha para desativar a mesclagem no modo de passagem

**Problemas Conhecidos:**

* A simetria não funciona com as ferramentas Borrar e Clonar
* A exportação do ArtStation está ausente

## Versão 1

### 1.7.3

*(Lançado em: 01 de março de 2016)*

**Adicionado:**

* &amp;lbrack;Export&amp;brack; Adicionar uma opção para desativar o preenchimento
* &amp;lbrack;Prateleira&amp;rbrack; Suporta hierarquia de sub-prateleira dentro de uma pasta de prateleira

**Corrigido:**

* Falha ao salvar sobre arquivo somente leitura anterior
* Falha ao abrir um segundo projeto
* Falha ao carregar algumas miniaturas (prateleira, camadas ou dicas de ferramentas)
* A desativação da opção “Preservar posições de traçados na malha” não funciona
* &amp;lbrack;Export&amp;brack; A ampliação de bitmaps é feita com a filtragem mais próxima
* &amp;lbrack;Shelf&amp;rbrack; A descoberta de recursos é muito lenta
* Os filtros de &amp;predefinição;prateleira&amp;preta; desfoque não são compatíveis com 16 bits
* &amp;lbrack;A Simetria do &amp;Tool&amp;rbrack; não funciona se você carregar uma predefinição de ferramenta antiga
* A caixa de diálogo de cor do canal de Specular não faz uma conversão do espaço de cor

### 1.7.2

*(Lançado: 13 de janeiro de 2016)*

**Adicionado:**

* &amp;lbrack;Camadas&amp;rbrack; Permite especificar a inclinação padrão para camadas de preenchimento

**Corrigido:**

* &amp;lbrack;Export&amp;rbrack; A exportação do Sketchfab não funciona mais
* A filtragem bilinear &amp;preto;Camada&amp;rbrack; é aplicada mesmo no Preenchimento sem nenhuma transformação
* &amp;lbrack;Tool&amp;brack; Baixo desempenho usando o substance com entradas de imagem no modo de projeção
* &amp;lbrack;Tool&amp;brack; O seletor de materiais está danificado

### 1.7.1

*(Lançado: 18 de dezembro de 2015)*

**Corrigido:**

* Falha ao alternar o conjunto de textura
* Desempenho lento ao pintar

### 1.7.0

*(Lançado: 17 de dezembro de 2015)*

**Adicionado:**

* &amp;lbrack;Performances&amp;rbrack; Calcula o conteúdo das camadas e suas miniaturas ao mesmo tempo
* &amp;preto;Exportar&amp;rbrack; Salvar caminho de exportação como relativo quando próximo ao projeto
* &amp;lbrack;Camadas&amp;rbrack; Adicionado novo modo de mesclagem : subtrair e adicionar/sub
* &amp;preto;Camadas&amp;rbrack; Nova filtragem de matriz bilinear para camadas de preenchimento
* &amp;lbrack;Sombreador&amp;rbrack; Defina um sombreador padrão para geração de miniaturas nas preferências.
* &amp;lbrack;Sombreador&amp;rbrack; Permite especificar um sombreador por conjunto de textura
* &amp;lbrack;Sombreador&amp;rbrack; Permite obter amostras de texturas da prateleira
* &amp;lbrack;Tool&amp;brack; Novo comportamento de pincel “em contorno” para pintura
* &amp;lbrack;Tool&amp;brack; Filtragem aprimorada e suavização reduzida ao pintar
* &amp;lbrack;Tool&amp;brack; Qualidade da pintura de subpixels aprimorada
* &amp;lbrack;Tool&amp;brack; Exibição “básica” removida para configurações de pincel e aprimoramento do ícone de abrir/fechar quadro
* &amp;preto;Menu&amp;rbrack; Adicionar ícones de efeitos no menu do botão direito
* Criação de modelo a partir de projetos
* &amp;lbrack;Shelf&amp;rbrack; Novos modelos: PBR, Dota 2
* &amp;preset;Prateleira&amp;rbrack; Nova predefinição de exportação: Dota 2
* &amp;lbrack;Prateleira&amp;rbrack; Novos sombreadores: Dota 2, tinta de carro PBR, PBR Coated, PBR Velvet
* &amp;lbrack;Prateleira&amp;rbrack; Novo material: ferrugem e desgaste de aço, iluminação estilizada
* &amp;lbrack;Shelf&amp;rbrack; Novos filtros : Desfocar iluminação direcional, estilizada
* &amp;lbrack;Shelf&amp;rbrack; Novo pincel: padrão suave e padrão rígido com um novo alfa para um melhor controle de dureza
* &amp;lbrack;Shelf&amp;rbrack; Novos geradores: Distância e Luz 3D
* &amp;lbrack;Prateleira&amp;rbrack; Pincéis atualizados com projeção de quebra e remoção de face de fundo (ativada por padrão)
* &amp;lbrack;Shelf&amp;rbrack; Ruído branco atualizado com a versão do processador de pixels para computação mais rápida

**Corrigido:**

* &amp;lbrack;Tela de boas-vindas&amp;rbrack; Tutorials enviar para vídeos antigos
* &amp;lbrack;Canais&amp;rbrack; Dizendo “não” para preencher a criação de camada com AO ainda cria a camada
* &amp;lbrack;Canais&amp;rbrack; Os nomes dos canais do UserX não se propagam na interface
* &amp;lbrack;Visor&amp;rbrack; A entrada da Máscara está vazia na lista de canais individuais
* &amp;lbrack;Share&amp;brack; Exportar um alfa para Compartilhar a partir do SP cria um arquivo .image ilegível
* &amp;lbrack;License&amp;rbrack; Corrigir ativação de nomes de usuário com caracteres não ASCII
* &amp;lbrack;Sombreador&amp;rbrack; A caixa de diálogo do parâmetro de cor desaparece ao escolher uma cor
* &amp;lbrack;Shelf&amp;rbrack; Miniaturas não são descarregadas da memória quando não usadas
* &amp;preto;Suporte de prateleira; Filtro de gradiente fixo
* &amp;lbrack;A Simetria do &amp;Tool&amp;brack; não funciona com estêncil/projeção
* &amp;lbrack;Tool&amp;brack; Nome incorreto ao criar uma nova predefinição de pincel
* A configuração Preservar traçado permanece desativada mesmo ao reimportar uma malha
* Reinicialização do driver (TDR) ao calcular partículas com tamanho grande.

### 1.6.1

*(Lançado: 09 de novembro de 2015)*

**Corrigido:**

* Falha ao abrir projeto se o Visualização 2D estiver visível
* Falha ao criar nova predefinição de exportação se a prateleira atual não existir
* &amp;lbrack;Tool&amp;brack; O ícone do seletor de materiais pode permanecer exibido
* &amp;lbrack;Tool&amp;brack; O seletor de materiais oculta o cursor do mouse ao pintar ao mesmo tempo
* &amp;lbrack;Shelf&amp;rbrack; Os metadados são gravados no disco após cada saída

### 1.6.0

*(Lançado: 29 de outubro de 2015)*

**Adicionado:**

* Suporte oficial para Windows 10
* &amp;lbrack;Substance&amp;rbrack; Recolher grupos de parâmetros de substância por padrão
* &amp;lbrack;Substance&amp;rbrack; Adicionar nova estrutura (Melhorar o desempenho do Processador de pixels)
* &amp;lbrack;Viewport&amp;rbrack; Permite desativar a exibição do plano de simetria no modo de simetria.
* &amp;preto;Visor&amp;rbrack; Melhorar o desempenho e a renderização das sombras
* &amp;preto;Visor&amp;rbrack; Pausar computação de sombra ao pintar
* &amp;lbrack;Visor&amp;rbrack; Melhorar o desempenho da renderização do wireframe
* &amp;lbrack;Engine&amp;rbrack; Melhorar o gerenciamento de memória Vram para reduzir seu espaço
* &amp;lbrack;Engine&amp;rbrack; Melhorar a atualização de textura em GPUs AMD para melhores desempenhos
* &amp;lbrack;Engine&amp;rbrack; Desabilitar configuração de Otimização encadeada em GPUs NVIDIA para melhor desempenho
* &amp;lbrack;Efeito&amp;rbrack; Adiciona uma marca para solicitar entrada de imagem “preenchida”
* &amp;lbrack;Camada&amp;rbrack; Aumenta a precisão do Deslocamento UV/escala no preenchimento
* &amp;lbrack;Layer&amp;brack; Torna o controle deslizante de escala exponencial no preenchimento
* &amp;lbrack;Layer&amp;brack; Permite arrastar e soltar materiais diretamente na pilha de camadas.
* &amp;lbrack;Layer&amp;brack; Permite arrastar e soltar filtros diretamente na pilha de camadas
* &amp;lbrack;Camada&amp;rbrack; Ajusta a cor do pincel da máscara para a cor de máscara recém-criada
* &amp;lbrack;Sombreador&amp;rbrack; Expor várias texcoords
* &amp;lbrack;Sombreador&amp;rbrack; Expor a função de mapeamento de gama/tons para permitir funções personalizadas
* &amp;lbrack;Baker&amp;rbrack; Alterar configurações padrão do baker de posição para uso TriPlanar
* &amp;lbrack;Tool&amp;brack; Renomear “Decalque de geometria” como “Preenchimento de polígono”
* &amp;lbrack;Prateleira&amp;rbrack; Atualize os geradores para suportar o TriPlanar: MG Metal edge wear, MG Mask builder, MG Fiber glass, MG Dirt
* &amp;lbrack;Prateleira&amp;rbrack; Atualizar materiais com novas configurações e materiais não utilizados removidos
* &amp;lbrack;Shelf&amp;rbrack; 22 novos materiais inteligentes (plástico, ferro, tecido, aço e mais)
* &amp;preto;Prateleira&amp;rbrack; Atualize os filtros de Nitidez, Desfoque e Distorção com entrada de imagem preenchida para evitar emendas
* &amp;lbrack;Shelf&amp;rbrack; Melhorar as configurações de Distorção para facilitar o uso
* &amp;lbrack;Shelf&amp;rbrack; 2 Novos ruídos processuais: ruído 3D Perlin e ruído 3D Worley

**Corrigido:**

* &amp;lbrack;Engine&amp;rbrack; A detecção da quantidade de Vram para a GPU dedicada está incorreta no Mac
* &amp;lbrack;Motor&amp;rbrack; as Texturas mudam para a versão mais escura no visor
* &amp;preto;Engine&amp;brack; Maus desempenhos ao pintar abaixo de várias camadas
* &amp;lbrack;Engine&amp;rbrack; As camadas calculadas ao abrir o projeto diferem da versão armazenada em cache
* &amp;lbrack;Substance&amp;rbrack; Resultados incorretos em 4K no Mac
* Os parâmetros do &amp;lbrack;Substance&amp;rbrack; estão na ordem errada
* &amp;lbrack;Sombreador&amp;rbrack; Os sombreadores de tom e pixelado são totalmente pretos
* &amp;lbrack;Sombreador&amp;rbrack; Os parâmetros desaparecem após alterar o mapa de ambiente
* &amp;lbrack;Shelf&amp;rbrack; Falha ao colocar arquivos png na pasta do gerador
* &amp;lbrack;Shelf&amp;rbrack; Miniaturas são geradas com baixa aspereza
* &amp;lbrack;Tool&amp;brack; Falha ao usar um bitmap na alfa do pincel no Windows
* &amp;lbrack;Export&amp;brack; Mapa adicional exportar predefinição agora exportar um mapa de RGB para a Posição

### 1.5.7

*(Lançado: 24 de setembro de 2015)*

**Corrigido:**

* O relatório de falha não funciona mais

### 1.5.6

*(Lançado: 21 de setembro de 2015)*

**Adicionado:**

* &amp;lbrack;Shelf&amp;rbrack; Melhorar a qualidade da renderização de miniaturas (usar texturas de 1K)

**Corrigido:**

* &amp;lbrack;Share&amp;brack; Impossível assinar com outra conta
* &amp;lbrack;Shelf&amp;rbrack; Miniaturas são muito pesadas no disco
* Os Materiais inteligentes do &amp;brack;Shelf&amp;rbrack; são muito lentos para carregar
* &amp;lbrack;Windows&amp;rbrack; Corrigir a instalação do serviço de licença
* &amp;lbrack;Canais&amp;rbrack; o mapa de Transmissivo é criado como G8 por padrão

### 1.5.5

*(Lançado: 15 de setembro de 2015)*

**Adicionado:**

* &amp;presilha;Prateleira&amp;rcolha; Exportar ativos para o Substance share
* &amp;preto;Shelf&amp;rbrack; Adicionar nova visualização de esfera para Materiais
* &amp;lbrack;Shelf&amp;rbrack; Usar o mapa de ambiente “Pátio envidraçado” para gerar miniaturas
* &amp;lbrack;Prateleira&amp;rbrack; Aumentar a resolução do tamanho da miniatura para 512x512 pixels
* &amp;lbrack;Visualização 3D&amp;rbrack; Expor valor de rotação do ambiente
* &amp;lbrack;Windows&amp;rbrack; Assine o aplicativo

**Corrigido:**

* &amp;lbrack;Baker&amp;rbrack; Resultados incorretos ao fazer bake mapas ao mesmo tempo
* &amp;lbrack;Visualização 3D&amp;rbrack; O mapa de ambiente é exibido quando nenhum projeto está aberto
* &amp;lbrack;Camadas&amp;rbrack; os Geradores de máscara não funcionam no conteúdo da camada
* &amp;lbrack;Camadas&amp;rbrack; Você pode tinta em camadas ocultas
* O ruído do &amp;lbrack;Shelf&amp;rbrack; Dirt_5 e Dirt_6 é idêntico
* &amp;lbrack;Shelf&amp;rbrack; Alguns geradores de máscara estão pixelados ou em baixa qualidade
* &amp;lbrack;Tool&amp;brack; Rotação incorreta do cursor em determinados ângulos.
* &amp;lbrack;Tool&amp;brack; Muitos canais fazem com que os botões do canal sejam cortados
* &amp;lbrack;O atalho Inverter máscara para Máscara rápida não funciona
* &amp;lbrack;Export&amp;brack; Sketchfab: o botão cancelar não foi levado corretamente em consideração
* &amp;lbrack;Licença&amp;rbrack; A ativação falhou quando a licença não pode ser copiada
* O limitador de taxa de quadros não funciona mais na interface do usuário

### 1.5.0

*(Lançado: 20 de agosto de 2015)*

**Adicionado:**

* &amp;lbrack;Sombreador&amp;rbrack; Adicionar número de linha em mensagens de erro de compilação de Sombreador
* &amp;preto;Prateleira&amp;rbrack; Melhorar a qualidade de visualizações de miniaturas
* &amp;lbrack;Shelf&amp;rbrack; Automatizar geração de miniaturas para Materiais inteligentes
* &amp;lbrack;Tool&amp;brack; Atalho para controlar a configuração de dureza na substância
* &amp;preto;Tool&amp;brack; Usar widget de tons de cinza para decalque geométrico quando estiver sobre uma máscara
* &amp;lbrack;Tool&amp;brack; Atalho para inverter a cor da tinta ao pintar em um mapa em tons de cinza
* &amp;lbrack;Viewport&amp;rbrack; Permite exibir o wireframe e alterar sua cor
* &amp;preto;Visor&amp;rbrack; Desfocar o plano de fundo do ambiente
* &amp;preto;Controles&amp;rbrack; Adicionar rotação aos atalhos de mouse do pincel
* &amp;preto;Exportar&amp;rbrack; Exportar para Sketchfab
* &amp;preto;Exportar&amp;rbrack; Criar predefinições de exportação para renderizadores
* &amp;lbrack;Export&amp;brack; Adicionar Reflexo de mapa convertido, F0 e 1/IOR
* &amp;lbrack;UI&amp;rbrack; Adicionar tela de boas-vindas
* &amp;lbrack;UI&amp;rbrack; Atualizar layout padrão
* &amp;lbrack;UI&amp;rbrack; Adiciona dicas de ferramentas ausentes e renomeia algumas entradas do menu
* &amp;lbrack;Camadas&amp;rbrack; Exportar máscara selecionada atualmente como bitmap
* &amp;preto;Camadas&amp;rbrack; Adicionar ação “inverter máscara” no menu do botão direito

**Corrigido:**

* &amp;lbrack;Projeto&amp;rbrack; Se os pivôs das malhas forem diferentes no FBX, as malhas são explodidas na importação
* &amp;lbrack;Substance&amp;rbrack; os Substance usados nas ferramentas de projeção estão bloqueados em 256\*256
* &amp;lbrack;Camadas&amp;rbrack; Falha ao usar limpar máscara
* &amp;lbrack;Export&amp;brack; Conversão de gama incorreta em texturas muito escuras
* &amp;preto;Exportar&amp;rbrack; O mapa de posição só pode ser usado em predefinições de exportação como um mapa em tons de cinza
* &amp;lbrack;Tool&amp;brack; A cor inicial do decalque de geometria é preta quando usada em uma máscara
* O atalho de rotação do &amp;preto;Tool&amp;brack; não funciona se não houver dureza no alfa

### 1.4.2

*(Lançado: 15 de julho de 2015)*

**Corrigido:**

* &amp;lbrack;Tool&amp;brack; Falha ao usar o decalque de geometria com máscara rápida
* A atualização do projeto da versão 1.4.0 para a 1.4.1 consome toda a memória do computador
* Importação incorreta do formato do projeto antigo
* Prateleiras personalizadas analisam toda a hierarquia e duplicam ativos em todos os lugares

### 1.4.1

*(Lançado: 23 de junho de 2015)*

**Adicionado:**

* &amp;Preenchimento;Visor&amp;Preenchimento; Permitir encaixar painéis lado a lado
* &amp;preto;Efeito&amp;rbrack; Adiciona um plano de fundo e uma régua para o efeito de nível
* &amp;lbrack;Efeito&amp;rbrack; Adicionar um efeito de Tinta que permita trabalhar sobre outro efeito

**Corrigido:**

* &amp;lbrack;Shelf&amp;rbrack; A geração de miniaturas é interrompida se nenhum projeto estiver aberto
* &amp;preto;Shelf&amp;rbrack; A visualização predefinida do material não é gerada
* &amp;preto;Shelf&amp;rbrack; As visualizações de material são geradas em uma malha com normais invertidos
* &amp;lbrack;Shelf&amp;rbrack; Miniaturas sempre recalculam por causa de função de hash incorreta
* &amp;lbrack;Shelf&amp;rbrack; Clicar em um material do substance não conecta mapas adicionais
* &amp;lbrack;Tool&amp;brack; Valor incorreto amostrado com seletor de material
* &amp;lbrack;Tool&amp;brack; Seletor de cores selecionar cor do cursor do visor
* &amp;lbrack;Visualização 2D&amp;rbrack; Taxa de quadros/desempenhos muito baixos
* &amp;lbrack;Export&amp;brack; Falha ao abrir a janela de exportação com predefinições de exportação muito recentes.
* &amp;lbrack;Exportar&amp;rbrack; canal de Height para Mapa normal é convertido para o espaço errado
* &amp;lbrack;Mac&amp;rbrack; BaseColor dos efeitos do substance é exibido como Linear
* &amp;lbrack;O widget de linhas retas do Mac&amp;rbrack; foi desenhado incorretamente na Retina
* As linhas retas podem permanecer ativadas mesmo com o atalho liberado.
* O guizmo de linhas retas desaparece após girar o mapa ambiental
* As saídas de oclusão de ambiente de substâncias não são conectadas ao canal AO automaticamente
* Corrigir problema de cópia de licença no Windows com caractere especial no nome de usuário

### 1.4.0

*(Lançado: 10 de junho de 2015)*

**Adicionado:**

* &amp;lbrack;Export&amp;brack; Adiciona mapas adicionais na lista de mapas de entrada disponíveis
* &amp;predefinição;Prateleira&amp;predefinição; Usar materiais sbsar como predefinições de material
* &amp;lbrack;Shelf&amp;rbrack; Permitir o uso de caminhos de Biblioteca personalizados
* &amp;lbrack;Shelf&amp;rbrack; Alterar o tamanho mínimo
* &amp;lbrack;Shelf&amp;rbrack; Novo conteúdo: 20 novos materiais inteligentes
* &amp;lbrack;Shelf&amp;rbrack; Novo conteúdo : nova substância processual (weave, mesh)
* &amp;lbrack;Shelf&amp;rbrack; Filtro de desfoque atualizado
* Desenhar linhas retas usando uma tecla modificadora
* Adicionar canal de Oclusão de ambiente e retrabalhar o comportamento AO/Normal no pilha de camadas
* Ler a cor padrão da Entrada de imagem definida nos dados do usuário Substance
* Permitir a exportação do log a partir do menu Ajuda

**Corrigido:**

* &amp;lbrack;Baker&amp;rbrack;&amp;lbrack;Mac&amp;rbrack; Falha com Normal do baker de malha
* &amp;lbrack;Baker&amp;rbrack; Falha se não houver UVs no arquivo de caixa
* &amp;lbrack;Baker&amp;rbrack; A correspondência por nomes não funciona com OBJ exportado do zBrush
* &amp;lbrack;Baker&amp;rbrack; Fazer bake com uma caixa sobrescreve o faço bake se forem usados vários conjuntos de texturas e UVs sobrepostos
* &amp;lbrack;Baker&amp;rbrack; Arquivos OBJ específicos resultam em texturas pretas
* &amp;lbrack;Shelf&amp;rbrack; Não é possível ler recursos se estiver definido como somente leitura
* &amp;lbrack;Shelf&amp;rbrack; Os arquivos de ativos estão sendo gravados no Painter se tiverem sido usados no projeto.
* &amp;lbrack;Shelf&amp;rbrack; Recarregando substâncias também atualiza a camada
* &amp;lbrack;Export&amp;brack; Tiff exporta imagens de 32 bits que não podem ser lidas corretamente pelo Photoshop ou mecanismos de jogo
* &amp;lbrack;Export&amp;rbrack; Predefinição de canais padrão sempre exportar como RGB
* &amp;lbrack;Material&amp;rbrack; canal de Difusão sobrepõe o mapeamento de BaseColor com substâncias
* &amp;lbrack;Visualização 3D&amp;rbrack; Iluminação incorreta de Difusão com mapas de ambiente específicos
* &amp;lbrack;Tool&amp;brack; Não é possível girar um pincel para um ângulo específico
* O visor obtém o foco quando o mouse é ativado ao digitar em um campo de texto
* Falha com predefinições muito recentes para a versão atual da prateleira
* Falha após substituir a malha
* Falha ao recarregar uma substância com um número diferente de entradas
* Malhas FBX da importação do Cinema4D com nomes de material incorretos

### 1.3.5

*(Lançado: 29 de maio de 2015)*

**Adicionado:**

* &amp;lbrack;Problema de ativação do License&amp;rbrack; quando já existe um arquivo de licença
* &amp;lbrack;Mac&amp;rbrack; Falha ao carregar arquivos FBX específicos
* &amp;lbrack;Mac&amp;rbrack;&amp;lbrack;Visualização 3D&amp;rbrack; Reflexão incorreta para GPU integrada
* A fonte da Máscara rápida do &amp;lbrack;Visualização 3D&amp;rbrack; está quebrada
* &amp;lbrack;Visualização 3D&amp;rbrack; O seletor de materiais torna o visor totalmente preto
* Falha após abrir projetos criados na versão 1.3.3
* A visualização do material fica vazia ao usar sombreadores com alfa
* Pintura para de funcionar em malhas específicas
* O desempenho diminui muito com malhas específicas de OBJ
* Os canais do usuário não são mapeados ao usar efeitos
* As pastas temporárias não são limpas na inicialização

**Corrigido:**

* Melhorias no tempo de computação em projetos extremamente longos para carregar
* Altere a janela “Solução de problemas de GPU” para ser mais compreensível
* &amp;preto;Camadas&amp;rbrack; Salva o status do bloqueio de proporção para camadas de preenchimento e torna-o “Ativado” por padrão
* &amp;lbrack;Baker&amp;rbrack; Correspondência por nome agora usar sufixo como separador

### 1.3.4

*(Lançado: 27 de abril de 2015)*

**Adicionado:**

* &amp;lbrack;Mac&amp;rbrack; Falha com o Mac OS X Yosemite (10.10)
* &amp;lbrack;Mac&amp;rbrack; Impossível sair do modo de tela cheia
* &amp;lbrack;Baker&amp;rbrack; Fazer bake a opção de correspondência por nome não funciona
* &amp;lbrack;Baker&amp;rbrack; O espaço tangente Mikk usado no SP não funciona com UE4
* &amp;lbrack;Baker&amp;rbrack; O baker de ID não pode fazer bake as cores de ID do material
* &amp;lbrack;Visualização 2D; não aparece ao usar a ferramenta de decalque de Geometria
* O canal alfa do Pincel &amp;preto;Tool&amp;brack; é exibido como verificador em vez de transparência com materiais
* &amp;lbrack;Tool&amp;brack; Falha com decalque de geometria
* &amp;lbrack;Camadas&amp;rbrack; O slot de material é recolhido por padrão na camada de preenchimento
* &amp;lbrack;Export&amp;brack; Falha ao exportar em tamanho maior do que a resolução do conjunto de textura
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
* &amp;lbrack;Shelf&amp;rbrack; Adicionar novos mapas de ambiente: Corsica beach, studio 05, Tornoco studio e mais
* &amp;presilha;Prateleira&amp;rbrack; Atualizar MG Construtor de máscaras com novos parâmetros
* &amp;lbrack;Shelf&amp;rbrack; Atualizar e calibrar mapas de ambiente antigos

**Corrigido:**

* Falha ao abrir a janela de exportação
* Não é possível arrastar e soltar no widget da interface do usuário quando desencaixado
* “Verificar atualizações” não está funcionando
* &amp;lbrack;Camadas&amp;rbrack; Não selecione a máscara ao pressionar ALT+clique nela
* &amp;lbrack;Tool&amp;brack; Tri-planar não funciona com o canal Normal
* &amp;lbrack;Visualização 3D; a iluminação da Difusão do mapa de ambiente está incorreta
* O cálculo da exposição do &amp;lbrack;Visualização 3D&amp;rbrack; é diferente do Designer
* &amp;lbrack;Visualização 3D&amp;rbrack; As sombras não devem estar visíveis em uma superfície 100% metálica
* &amp;lbrack;Visualização 3D&amp;rbrack; A malha com UVs espelhados inverteu a tangente/binômios
* &amp;lbrack;Visualização 3D&amp;rbrack; Sombras produzem resultados incorretos em determinadas malhas
* &amp;lbrack;Baker&amp;rbrack; Remove a pasta “.alg_meta” criada por arquivos assbin
* &amp;lbrack;Baker&amp;rbrack; Falha ao fazer bake se o Painter recalcula um TextureSet ao mesmo tempo
* &amp;lbrack;Mac&amp;rbrack; Falha na interface do usuário do White Box ao iniciar o aplicativo

### 1.3.2

*(Lançado: 06 de março de 2015)*

**Corrigido:**

* &amp;lbrack;Visualização 3D&amp;rbrack; Falha ao recarregar um mapa de ambiente salvo com o projeto

### 1.3.1

*(Lançado: 05 de março de 2015)*

**Adicionado:**

* &amp;lbrack;Baker&amp;rbrack; Adicionar uma versão em cache de malhas de alto-polígono para acelerar o cálculo
* &amp;lbrack;Baker&amp;rbrack; Adiciona um ícone de aviso se nenhuma malha de alto polígono estiver carregada
* &amp;lbrack;Baker&amp;rbrack; Se nenhuma malha de alto polígono estiver carregada, use a malha do projeto

**Corrigido:**

* &amp;lbrack;Baker&amp;rbrack; Pressionar “enter” ao editar o valor de um controle deslizante fecha a janela
* &amp;lbrack;Baker&amp;rbrack; Ativar/Desativar um baker também acionará o botão
* &amp;lbrack;Baker&amp;rbrack; Impossível fazer bake se você usar o botão “tudo/nenhum”
* &amp;lbrack;Baker&amp;rbrack; A ordenação dos botões de baker não está na ordem correta
* &amp;lbrack;Baker&amp;rbrack; Caixa de seleção são ignoradas e todos os baker são sempre processados
* &amp;lbrack;Baker&amp;rbrack; Progresso da barra de progresso fixo

### 1.3.0

*(Lançado: 04 de março de 2015)*

**Adicionado:**

* &amp;lbrack;Baker&amp;rbrack;&amp;lbrack;Visualização 3D&amp;rbrack; Usar computação de espaço tangente Mikkt se nenhuma tangente/binormal for encontrado
* &amp;lbrack;Baker&amp;rbrack; Adicionados novos baker: Normal, ID, Oclusão, Curvatura, Thickness, Posição
* &amp;lbrack;Efeitos&amp;rbrack; A pilha de efeitos agora está invertida e exibida de cima para baixo (como camadas)
* &amp;lbrack;Efeitos&amp;rbrack; Adicionar novos ícones na pilha de efeitos
* &amp;lbrack;Efeitos&amp;rbrack; Adicionar modo de mesclagem entre ações de preenchimento na pilha de efeitos
* &amp;lbrack;Efeitos&amp;rbrack; Renomear efeitos (efeito da substância = filtro, etc.)
* Adicionar um arquivo de “bloqueio” durante o processo de salvamento
* &amp;preto;Efeitos&amp;rbrack; Adicionar ação Preenchimento na pilha de efeitos
* Adicionado novo recurso : Materiais inteligentes
* &amp;lbrack;Camadas&amp;rbrack; Permitir a reordenação de efeitos de camada
* &amp;lbrack;Tool&amp;brack; Adicionar projeção tri-Planar
* &amp;lbrack;Visualização 3D&amp;rbrack; Adicionar suporte para sombras
* &amp;lbrack;Visualização 3D&amp;rbrack; Capacidade de definir estados OpenGL necessários em sombreadores personalizados
* &amp;lbrack;Visualização 3D&amp;rbrack; Suporte para alfa através de novos sombreadores
* &amp;lbrack;Visualização 3D&amp;rbrack; Os sombreadores agora possuem versão e foram salvos completamente em um projeto
* &amp;lbrack;Visualização 3D&amp;rbrack; Avisa o usuário se o sombreador não compilar mais

**Corrigido:**

* &amp;lbrack;Camadas&amp;rbrack; corrigir soltar em uma pasta recolhida
* &amp;lbrack;Prateleira&amp;rbrack; Corrigir filtragem de conteúdo em miniprateleiras
* &amp;predefinição;Prateleira&amp;predefinição; Renomear categorias e reorganizar guias

### 1.2.1

*(Lançado em: 12 de fevereiro de 2015)*

**Adicionado:**

* Os arquivos \*.spp agora podem ser abertos com um clique duplo no explorador
* &amp;lbrack;Export&amp;brack; Nova marca “$project” para predefinições de exportação
* &amp;preto;Export&amp;brack; Adicionar lista de mapas (com nomenclatura) abaixo de cada conjunto de textura
* &amp;Preencher;Exportar&amp;preencher; Adicionar um botão Tudo/Nenhum para selecionar os conjuntos de texturas
* &amp;preto;Export&amp;brack; Mapas vazios são descartados durante a exportação

**Corrigido:**

* &amp;lbrack;Export&amp;brack; Unity5 predefinições têm mapas invertidos
* &amp;lbrack;Export&amp;brack; Adicionar uma barra em um nome predefinido criará uma pasta corrompida
* &amp;lbrack;O canal de Height de Exportação&amp;rbrack; exportado em formatos de 32 bits está incorretamente fixado
* A lista do conjunto de texturas &amp;lbrack;Export&amp;brack; não está ordenada como no projeto
* &amp;lbrack;Tool&amp;brack; A remoção da face de fundo não funciona mais
* Salvar não funciona com caracteres especiais no caminho

### 1.2.0

*(Lançado: 28 de janeiro de 2015)*

**Adicionado:**

* Novo canal Normal que permite tinta dados do mapa normal e combinar os resultados
* &amp;lbrack;Export&amp;brack; Nova janela de exportação com a capacidade de criar embalagem personalizada e definir nomes personalizados
* O formato de arquivo do projeto agora é um único arquivo em vez de pastas
* &amp;lbrack;Export&amp;rbrack; Suporte a diferentes formatos Normais (DirectX, OpenGL)
* &amp;lbrack;Export&amp;brack; Criar um arquivo temporário de “bloqueio” durante a exportação
* &amp;lbrack;Camadas&amp;rbrack; Shift+Clique com o botão esquerdo do mouse pode ser usado para alternar uma máscara
* &amp;lbrack;Parâmetros&amp;rbrack; Expor o espaço de cores na parte inferior de uma entrada de imagem
* O &amp;preto;Shelf&amp;rbrack; Efeito “MG Mask Builder” agora tem novas configurações
* &amp;lbrack;Visualização 3D; o mapa de Oclusão de ambiente agora oclui a contribuição difusa, não o specular

**Corrigido:**

* A visualização do material de projeção/estêncil não é exibida corretamente no visor
* &amp;lbrack;Dica de ferramenta do atalho do &amp;Visualização 3D; não exibida ao usar o atalho “S” (estêncil)
* &amp;lbrack;Shelf&amp;rbrack; O efeito “Escala de pele MatFx” agora tem melhores desempenhos em baixa resolução
* &amp;lbrack;Export&amp;brack; as Texturas da exportação são apenas ampliadas ao especificar um tamanho de documento maior

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

* &amp;lbrack;Camada&amp;rbrack; Selecione a camada na parte superior ao abrir um conjunto de texturas de projeto/alternância
* Velocidade aprimorada de “Salvar” e “Salvar como” com o novo algoritmo de compactação
* Exibir um erro ao abrir um projeto muito recente para o Painter

**Corrigido:**

* &amp;lbrack;Tool&amp;brack; O decalque geométrico produz corrupções na memória
* &amp;lbrack;Brush&amp;brack; Impossível inserir manualmente valores de flutuação abaixo de 1 para o tamanho do pincel
* &amp;lbrack;Camada&amp;rbrack; Criar um efeito de seleção de cor não o adiciona na pilha de camadas
* &amp;lbrack;Camada&amp;rbrack; Mover o mouse sobre as camadas faz com que o Painter passe rapidamente na barra de tarefas
* &amp;lbrack;Camada&amp;rbrack; Adicionar um bitmap como máscara pode levar a um travamento
* A interface gráfica para o modo solo com o canal de Height está incorreta
* “Salvar projeto” pode falhar e corromper um projeto
* Falha ao abrir um projeto após carregar outro com um sombreador desatualizado

### 1.1.0

*(Lançado: 16 de dezembro de 2014)*

**Adicionado:**

* &amp;preto;Efeito&amp;rbrack; Novo criador de máscara de ID de material
* Nova linha branca/preta pontilhada para o cursor do pincel
* Novo parâmetro de sequência de ângulo
* Novo parâmetro de remoção de tela de fundo
* Novo parâmetro Atraso do mouse
* &amp;lbrack;Camadas&amp;rbrack; Suporte para várias seleções e gerenciamento
* &amp;lbrack;Camadas&amp;rbrack; Copiar e colar de uma textura definida para outra
* &amp;lbrack;Export&amp;brack; formato de PSD do Adobe Photoshop
* &amp;preto;Suporte de prateleira; Nova ferramenta: pele, pontos de metal e zíper
* &amp;preto;Prateleira&amp;rbrack; Novo pincel : molde, lápis, linha afiada e costura
* &amp;preto;Suporte de prateleira; Novo alfa : Ruído gaussiano, linha nítida, molde, caneta, respingo, ponto, zíper
* O desempenho da pintura melhorou atualizando apenas partes das texturas necessárias

**Corrigido:**

* &amp;lbrack;Shelf&amp;rbrack; Impossível carregar uma substância com gráfico com rótulos idênticos
* &amp;lbrack;Camadas&amp;rbrack; O modo de mesclagem Passagem não funciona com máscaras
* &amp;lbrack;A Escala do Estêncil&amp;rbrack; está quebrada no Visualização 2D
* Problemas e falha no Mac OS Yosemite

### 1.0.2

*(Lançado: 09 de novembro de 2014)*

**Adicionado:**

* Desempenho aprimorado na visualização de material com substâncias
* Desempenho aprimorado com visualização de traçado de pincel ao atualizar o documento
* Desempenho aprimorado no visor com menor taxa de atualização para a área não funcional
* &amp;lbrack;Pós-efeitos&amp;rbrack; Interface aprimorada para gerenciar configurações
* &amp;lbrack;Pós-efeitos&amp;rbrack; Redefinir para valores padrão
* efeitos de Substance e operações de camadas no menu do botão direito do mouse
* Apoio a entradas/saídas pré-multiplicadas em substâncias

**Corrigido:**

* &amp;lbrack;Visualização 3D&amp;rbrack; Os parâmetros de sombreador personalizado são separados por um espaço grande
* &amp;lbrack;Export&amp;rbrack; Conversão sRGB ausente para a predefinição Unity4
* Possível falha ao carregar malhas fbx
* Falha às vezes ao carregar malhas obj simples
* A barra de computação permanece bloqueada até 100% no carregamento
* Recarregar uma substância a coloca em todas as categorias
* Chave de DirectX/OpenGL quebrada

### 1.0.1

*(Lançado: 27 de outubro de 2014)*

**Adicionado:**

* &amp;lbrack;Tool&amp;brack; Uso aprimorado de parâmetros de material
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
* &amp;lbrack;Export&amp;brack; Adicionar uma passagem de dilatação antes do pós-processo de difusão
* Argumentos de linha de comando no SP para operações simples
* Novos materiais e efeitos
* Visualização da ferramenta (visualização de material em tempo real separado e área de teste de traçado)
* Não criar um documento padrão quando o Painter for iniciado
* &amp;preto;Tool&amp;brack; Adiciona a possibilidade de editar manualmente um valor em tons de cinza
* Várias melhorias para os estênceis (Ajustar, Redefinir)
* As partículas agora são subferramentas das ferramentas Pincel, Borracha e Projeção
* &amp;lbrack;Visualização 3D&amp;rbrack; Usar AO feito bake na renderização do visor
* Dividir os controles de estênceis entre a exibição 2D e 3D
* Ajuste pequeno do tamanho do polegar na biblioteca
* Os campos de pesquisa são específicos para cada janela
* Ajustes da interface

**Corrigido:**

* A chave &amp;brack;Substance&amp;brack; não funciona
* &amp;lbrack;Caixa de diálogo de cores&amp;rbrack; Degradê de matiz não atualizado
* Não é possível atualizar uma malha se o nome do arquivo é idêntico
* A ferramenta não fica visível nas exibições quando muito pequena
* A ferramenta de decalque na tela Retina não funciona corretamente
* &amp;lbrack;Substance&amp;rbrack; Int1 são exibidos como float1
* &amp;lbrack;Substance&amp;rbrack; basecolor input/output não são reconhecidos
* Os filtros do &amp;lbrack;Substance&amp;rbrack; não podem ser recarregados
* O widget &amp;preto;Tool&amp;brack; em tons de cinza está sempre recolhido

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
* &amp;brack; e &amp;rbrack; atalhos para Tamanho do pincel
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
