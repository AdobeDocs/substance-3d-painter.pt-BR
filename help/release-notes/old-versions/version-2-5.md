---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/release-notes/old-versions/version-2-5.html"
breadcrumb-title: ''
description: Consulte as notas de versão do Substance 3D Painter versão 2.5 para saber mais sobre novos recursos, aprimoramentos e correções de erros.
helpx_creative_field: ""
helpx_description: Painter > Release notes > Old versions > Version 2.5
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Versão 2.5
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '1699'
ht-degree: 0%

---


# Versão 2.5

O **Substance Painter 2.5** apresenta muitos recursos novos: desde o suporte à opacidade nas configurações do pincel (além do fluxo) até a capacidade de assar mapas adicionais em 8K e muito mais.

Data de lançamento: *21 de fevereiro de 2017*

## Principais recursos

### Nova opacidade do pincel

![](../../assets/brush-combined.gif){width="650px"}

Agora há uma nova configuração nos **parâmetros do pincel** ao Pintar no Substance Painter, que é a **opacidade**.\
A **opacidade** controla a **intensidade geral de um traçado de pincel**, diferentemente da configuração de **fluxo** que controla a intensidade de **cada carimbo individual** dentro de um traçado de pincel. Isso significa que agora é possível pintar e repintar uma mesma área **sem criar valores sobrepostos**. Para fazer isso, defina o fluxo como 100 e o valor de opacidade com a intensidade que preferir. Como a opacidade funciona, não é possível vinculá-la à pressão da caneta. Para esse tipo de controle, o fluxo ainda é a melhor escolha.

Também adicionamos um **novo modificador** junto com este novo parâmetro que está na chave **”A”** por padrão. Pressionar esta tecla permitirá que **continue o traçado anterior do pincel** em vez de criar um novo. Isso significa que você pode pintar uma cor uniforme com a opacidade desejada, mantendo a possibilidade de mover a câmera, por exemplo. Outro exemplo seria continuar a cópia que você estava fazendo com a ferramenta clone.

![](../../assets/stroke-opacity-parameter.png)

### Novo cozimento em 8K e resoluções não quadradas

![](../../assets/baking-250-8k.png)

O padeiro foi aprimorado para suportar resoluções de até **8192x8192** (8K mais suavização de borda), o que significa que agora você pode exportar em 8K com proporção de 1:1 com os mapas adicionais.\
Também adicionamos suporte para resoluções **não quadradas**. Agora é possível assar uma textura de **4096x2048**, por exemplo. Para isso, basta clicar no ícone de “**cadeado**” ao lado do menu suspenso para selecionar a resolução.

### Nova compatibilidade com o Perfil de cor no visor

![](../../assets/lut-example.jpg)

Adicionamos o suporte de **LUT** (texturas) para controlar a renderização do **visor** em Substance Painter. Para aplicar um perfil, basta habilitar a configuração “**Perfil de Cor**” na janela “**Configurações de exibição**” e carregar o LUT no slot dedicado. Ele funciona com o visor do **OpenGL** (pintura) e o renderizador **IRay**. Alguns exemplos estão disponíveis por padrão, de **Predefinições de câmera** comuns a mais **Efeitos artísticos**. Para obter mais informações, consulte a página dedicada da documentação: [Perfil de Cores](../../features/post-processing/color-profile.md)

### Novo mecanismo de Substance compatível com o Substance Designer 6

![](../../assets/font-shelf.png)

Adicionamos o suporte para **Substance Designer 6**, o que significa que os recursos criados com o **SD6** podem ser abertos e usados no **Substance Painter 2.5**!\
Um bom exemplo é a capacidade de usar o **novo nó de texto** do SD6 e integrá-lo a uma substância. Dessa forma, é possível criar **texto dinâmico** e pintá-lo diretamente sem a necessidade de sair do aplicativo. **Incluímos 10 fontes** com cada uma de um estilo diferente por padrão para cobrir o uso mais comum. Você pode encontrá-los na seção “**procedure**” da **prateleira**.

![](../../assets/text-sp250-optim.gif){width="400px"}

### Novo conteúdo na prateleira

![](../../assets/new-filters.jpg)

Juntamente com algumas correções e melhorias na nova prateleira, também adicionamos vários **novos filtros** para melhorar a pintura e a texturização. Também **melhoramos** o comportamento do filtro já existente (como o “**HSL**”). Também adicionamos novos **modelos** ao criar **novos projetos** (como o **Unity 5** e o **Unreal Engine 4**).

### Novas melhorias de script com suporte para interface de usuário de sombreador personalizada

![](../../assets/ui-shader.jpg)

Com esta versão, adicionamos uma maneira de **script e controlar** os **parâmetros de sombreador**. Também adicionamos o suporte para usar uma **interface personalizada** em vez da padrão, abrindo muitas novas possibilidades, como o **sombreador animado**.\
Para obter mais detalhes, consulte a documentação de scripting disponível no menu Ajuda do aplicativo.

## Tutorial

Os novos recursos principais são abordados na mais recente transmissão do Twitch:

## Notas de versão

### 2.5.3

(Lançado em 15 de março de 2017)

**Corrigido:**

* [Baker] Falha ao assar com malhas específicas

**Problema Conhecido:**

* [Mac] As partículas podem criar corrupção de textura em alguns casos

### 2.5.2

(Lançado em 14 de março de 2017)

**Corrigido:**

* [Ferramenta] O tablet Wacom não funciona no Linux
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

**Problema Conhecido:**

* [Mac] As partículas podem criar corrupção de textura em alguns casos

### 2.5.1

(Lançado em 27 de fevereiro de 2017)

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

**Problema Conhecido:**

* [Linux] A entrada do tablet Wacom não funciona na exibição 3D e 2D
* [Mac] As partículas podem criar corrupção de textura em alguns casos
* [Exportar] Em casos muito raros, retângulos pretos podem aparecer em GPUs da AMD

### 2.5.0

(Lançado em 21 de fevereiro de 2017)

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

**Problema Conhecido:**

* [Exportar] Em casos muito raros, retângulos pretos podem aparecer em GPUs da AMD
* [Iray] Os perfis de cores podem se comportar de maneiras ímpares às vezes
