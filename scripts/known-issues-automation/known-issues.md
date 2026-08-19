---
helpx_url: "https://helpx.adobe.com/br/substance-3d-painter/release-notes/know-issues.html"
breadcrumb-title: ''
description: Analise os problemas conhecidos do Substance 3D Painter para se manter informado sobre as limitações atuais e as soluções alternativas da versão mais recente.
helpx_creative_field: ""
helpx_description: Substance 3D Painter
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Problemas conhecidos
user-guide-description: ''
user-guide-title: ''
source-git-commit: 99ba6e8d891dab9cebbf6035a6850bab331e7472
workflow-type: tm+mt
source-wordcount: '905'
ht-degree: 0%

---


# Problemas conhecidos

Esta página lista todos os problemas conhecidos ativos presentes na v12.1.0 do Substance 3D Painter:

* `[Engine]` Erro ao usar materiais inteligentes se o Conjunto de texturas não tiver bloco 1001
* `[Engine]` Pintura com a ferramenta Clonar em cores normais de deslocamento de canal incorretamente
* A máscara de geometria `[Engine]` mostra artefatos em bordas UV com camadas instanciadas
* `[Engine]` O preenchimento UV do modo “Vizinho do Espaço 3D” não funciona bem em triângulos finos
* O resultado do ponto de ancoragem `[Engine]` não é renderizado entre uma máscara e um canal de cor

* `[Baking]` AO incorreto em cubos simples
* `[Baking]` Correspondência por interpretação de sufixo de nome incorreta
* `[Baking]` emendas Uv não aparecem após a reimportação de mes
* `[Baking]` artefatos tipo grade com algumas configurações

* `[Substance]` Vários erros ortográficos nos recursos
* `[Substance]` Espaço em branco interrompe a condição de visibilidade
* `[Substance]` Predefinições para alguns materiais levam muito tempo para carregar
* `[Substance]` Não é possível importar o recurso com usos mistos

* `[Color Management]` Associações incompatíveis com gerador não usadas na máscara
* A saída do filtro `[Color Management]` não foi considerada corretamente
* `[Color Management]` conversões de espaço de cores HDR com ACE no Linux produzem cores vivas

* Os recursos `[Shelf]` obtêm o uso incorreto se colocados em uma pasta com um nome específico
* `[Shelf]` `[Substance]` Dados do usuário não levados em conta para geração de miniatura de prateleira

* O parâmetro “camera_vp_matrix_inverse” `[Shader]` não é reconhecido
* O canal `[Shader]` user0 não pode sempre ser lido como sRGB com sombreador específico

* `[Scripting]` Erro de digitação `[Javascript]` “Desabilitado” ao especificar o parâmetro de pontilhamento em funções de exportação
* `[Scripting]` `[Python]` Vários erros de digitação no módulo substance_painter.project

* O projeto `[Single Channel View]` salvo na exibição de cor base parece mais escuro após a atualização da versão do Painter
* O projeto `[Single Channel View]` salvo na exibição de cor base parece mais escuro após a atualização da versão do Painter

* `[gltf]` Não é possível abrir arquivos exportados pelo Babylon Exporter
* `[Displacement]` Falha ao pintar
* `[Polygon Fill Tool]` Seleção incorreta com simetria
* `[2D view]` Os traços às vezes não aparecem ao pintar
* `[Console]` Símbolos associados ao atalho não podem ser gravados
* `[LOG]` A mensagem de erro está errada ao falhar a exportação
* O estêncil `[3D View]` não funciona em objetos duplicados
* `[Resource updater]` Recursos diferentes na prateleira com o mesmo nome são lidos como um recurso
* `[Sample]` Câmera quebrada na amostra de Visualização
* `[Instancing]` `[Projection]` Ao selecionar uma instância em um projeto planar, outro projeto planar é selecionado em outro conjunto de texturas
* `[Slider]` entradas numéricas são desmarcadas quando o cursor sai da janela
* `[Anchor point]` referências quebradas ao copiar e colar conteúdo da máscara
* `[Mesh export]` Não considera novos nomes de conjuntos de texturas
* `[Anchor Points]` Cor incorreta quando usada no gerador
* O padeiro do Mapa de Identificação do `[Bakers]` não leva em consideração o Material Físico do 3ds Max 2021
* `[UV Tiles]` Nenhuma mensagem de erro ao sobrepor espaços UV com uma malha específica
* `[GLTF]` `[Crash]` Criar um projeto com arquivo gltf compactado causa uma falha
* `[UV Tile sequence]` mapas de posição não foram importados corretamente
* A máscara de combinação de Height `[UVTiles]` não está atualizada com a Máscara de bloco UV
* `[Import]` Não é possível importar o arquivo obj com valores “nan”
* `[Export]` exportações de GLTF no tamanho incorreto
* O nome `[Texture Set]` pode estar vazio
* `[Layer stack]` Copiar para alternar máscara para modo de material
* `[UI]` Erro de ortografia nas configurações do criador de pincel
* `[Texture Set Settings]` Nome de instância de sombreador incorreto após renomeação
* `[Blending]` O modo de mesclagem de cor e saturação também altera o brilho
* `[Librairies]` A largura das janelas Pesquisas salvas e filtrar por caminho não é salva quando alterada
* `[Geometry mask]` Problema ao reimportar a malha e a camada de instância
* `[Color management]` Espaço de cores não encontrado quando o bloco 1001 está ausente
* `[Export mesh]` Deslocamento não exportado com blocos UV específicos configurados
* `[RedHat]` problemas no seletor de cores
* `[Regression]` `[UI]` O Menu do Clique com o Botão Direito é muito pequeno na tela hd
* `[Resources]` mapas de malha importados são ignorados pela atualização automática
* A visualização do espaço de mistura de cores `[User Channels]` está incorreta
* A seleção de geometria `[Mask]` ainda está ativa após alternar para o modo empilhado
* `[Sonoma]` Ícones não aparecem nos menus
* `[Path]` a mesclagem de Height de vários caminhos pode causar artefatos
* `[USD]` Atribuição usda incorreta em alguns casos
* `[Polygon Fill]` A alteração do espaço de cores da cor base não atualiza o seletor de cores
* `[Paint Skew]` A ferramenta selecionada na inclinação de pintura permanece selecionada após alternar para o Modo de Pintura
* O seletor `[Color Picker]` permanece aberto após a alteração da ferramenta
* `[UV Padding]` artefatos ao aumentar a textura de 4k para 8k na exportação
* `[Baking Common Settings]` As configurações de Distância da Gaiola não atualizam a visualização do wireframe e do sombreador da gaiola
* `[Send to Photoshop]` Falha ao exportar a máscara da camada
* `[Skew Baking]` A correção de inclinação é interrompida ao pintar e desfazer
* A interação do visor `[Projection Tool]` foi bloqueada pela ferramenta de projeção
* Os recursos não quadrados são esticados quando usados nos slots do canal de pincel
* Falha ao decodificar a substância
* UVs não perfeitamente sobrepostos podem criar artefatos
* Normais de malha inválidas com algum fbx
* A visualização não é atualizada ao mudar o canal afetado por um nível
* Projetos com um conjunto de texturas são reabertos no modo Base Color solo
* A interface do botão de canal nas propriedades de material/pintura pode ser quebrada
* A ordem dos canais em Propriedades pode ser quebrada
* Os traçados feitos em L16F e RBG16F podem exibir artefatos
* O comportamento do botão Restaurar não interage com a tecla de bloqueio nas configurações da câmera
* A exportação do Photoshop ignora a seleção da máscara de geometria
* O filtro de Inclinação e distorção de desfoque depende da resolução do conjunto de texturas
* Mapas sem nomes são criados fora da pasta de exportação
* O estêncil não é atualizado ao alterar a predefinição de pincel
* Problema com transparência em arquivos PSD
* As modificações dos parâmetros de pincel na barra de ferramentas contextual não aparecem no histórico
* Não é possível renomear ou excluir predefinições de exportação se você já as excluiu e recriou nesta sessão
* O mapeamento de canal não funciona para a visualização da ferramenta de projeção em alguns casos
* Abrir e salvar alguns projetos pode demorar mais do que o normal

## Estabilidade

* `[Crash]` Clicar na lista de Texturas Definidas após falha na criação do projeto causa uma falha
* `[Crash]` Falha de erro crítico quando o mesmo projeto está aberto duas vezes
* `[Crash]` Selecione “Exportar malha” quando a malha falhar ao carregar
* `[Crash]` Clicando em “Iniciar pintura” após tentar abrir um projeto antigo
* `[Crash]` A criação de textos muito longos na Faixa de Opções pode falhar
* `[Crash]` Retornando ao modo de pintura após a perda do dispositivo na cozedura
* `[Crash]` Sair do Painter após cancelar a exportação de mapas
* `[Crash]` Exportando malha com alguns símbolos especiais no nome da câmera
* `[Crash]` A exclusão de um canal no modo de exibição de máscara leva a uma falha
* `[Crash]` Alguns Substance podem levar a uma falha quando renderizados
* `[Crash]` Reimportar malha enquanto estiver no modo de cozimento
* `[Crash]` Recarregar várias malhas pode levar a uma falha
