---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/release-notes/old-versions/version-2017-3.html"
breadcrumb-title: ''
description: Revise as notas de versão do Substance 3D Painter versão 2017.3 para saber mais sobre novos recursos, aprimoramentos e correções de erros.
helpx_creative_field: ""
helpx_description: Painter > Release notes > Old versions > Version 2017.3
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Versão 2017.3
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '1588'
ht-degree: 0%

---


# Versão 2017.3

O **Substance Painter 2017.3** concentra-se na nova predefinição de exportação avançada com o suporte do **Adobe Project Felix** e o formato aberto **glTF**. Esta nova versão também se concentra na experiência do usuário, aprimorando a interface e adicionando um plug-in de salvamento automático.

Data de lançamento: *28 de setembro de 2017*

## Principais recursos

### Predefinição de exportação de material padrão da Adobe

![](../../assets/adobe-dimension-meetmat.jpg)

Um dos novos exportadores que incluímos nesta versão é o suporte ao Material padrão da Adobe a ser usado com o Adobe Dimension (anteriormente Adobe Project Felix). Permitimos que você exporte a malha de cena e suas texturas para serem importadas para o Projeto Felix em um clique. Para acessá-lo, basta escolher “**Material padrão da Adobe**” na janela de texturas de exportação. Para obter mais informações, consulte: [http://www.adobe.com/products/dimension.html](https://www.adobe.com/products/dimension.html)

Você também pode conferir nossa postagem sobre isso no blog: <https://www.allegorithmic.com/blog/new-dimension-substance-ecosystem>

### predefinição de exportação de glTF 2.0

![](../../assets/gltf-export.jpg)

Também adicionamos suporte para o formato de arquivo **glTF**, com a exportação da **malha de cena** e das **texturas PBR** (metálico/rugosidade). Para acessá-la, basta escolher “**glTF PBR Metal Roughness**” na janela de exportação de texturas. **glTF** é um formato de arquivo de código aberto dirigido pelo grupo Khronos. Você pode exibir o arquivo glTF no **Windows 10** ou usar um visualizador WebGL, como o [**Babylon**](http://sandbox.babylonjs.com/).

Para obter mais informações, consulte: <https://github.com/KhronosGroup/glTF>

### Plug-in de salvamento automático

![](../../assets/autosave-details.png)

Nesta versão, também incluímos um novo plug-in que tem a possibilidade de **criar backups** do projeto aberto no momento. Cria um arquivo de backup no lado do projeto aberto atualmente.\
Por isso, também adicionamos uma entrada “**Salvar como cópia**” no menu Arquivo. O **salvamento automático** pode ser interrompido ao desabilitar o próprio plug-in. Suas **configurações** podem ser acessadas **por meio do painel de configuração**. Quando o atraso do tempo de aviso for atingido, uma **barra de progresso** aparecerá abaixo do botão na barra de ferramentas principal, permitindo adiá-la por alguns minutos, se necessário (útil se você quiser concluir algo antes do backup).

Se um backup for criado, mas o projeto não tiver sido salvo (também conhecido como Não Inclinado), o backup será armazenado na pasta **Documents/Allegorithmic/Substance Painter/autosave**. Caso contrário, o backup será feito ao lado do próprio projeto (a menos que o caminho seja substituído pelo painel de configuração).

### Filtro de gradiente aprimorado

![](../../assets/gradient-rust.jpg)

O **filtro de gradiente** foi completamente renovado. Agir de forma muito mais semelhante ao nó **mapa de degradê** disponível em **Substance Designer**. Agora ele suporta até **10 cores diferentes**, com a possibilidade de especificar **onde a cor está localizada dentro do** gradiente ****, abrindo muitas portas novas. Isso permite criar mais **padrões de cores avançados**, mas também **remapear mapas de altura**e criar **novas formas**.

O controle deslizante principal (quantidade de cores) define o número de cores totais que são usadas para criar o gradiente. O botão logo abaixo define o modo de mesclagem de cores (sRGB ou Linear). Isso é importante se você quiser ter uma mistura adequada entre as cores. Por exemplo, mesclar um vermelho puro e um verde puro deve produzir um amarelo agradável no meio. Isso não acontecerá se o botão estiver desativado (ele exibirá um marrom escuro como alternativa). Ao remapear a height ou qualquer outro canal de tons de cinza, esse botão deve ser desativado para evitar a conversão da gama.

O botão na parte superior permite substituir o resultado do filtro pelo próprio gradiente, para visualizar o gradiente na visualização 2D.

![](../../assets/gradient-height-demo.jpg)

### Melhorias de interface e comportamento

![](../../assets/tabs-top.png)

Nesta versão, as **guias** das diferentes docking stations do aplicativo agora estão localizadas **na parte superior em vez da parte inferior** das respectivas janelas. Esta escolha foi feita para ajudar a legibilidade da interface, mas também para ser mais consistente com outros aplicativos. Após essa alteração, é apresentada a **pequena cruz** ao lado do título da guia para **fechá-la facilmente**. Também é possível **clicar com o botão direito** na guia para trazer um **menu de contexto** (que permite fechar ou desencaixar a janela). Um atalho para desencaixar a janela é simplesmente arrastar e soltar a guia fora da área da janela.

Agora também é possível **abrir projetos** simplesmente arrastando-os e soltando-os **na viewport** do explorador de arquivos. Isso também funciona com arquivos de **malha**: arrastar e soltar um arquivo de malha em um **visor vazio** abrirá a **nova janela de projeto**, mas fazê-lo em um **projeto já aberto** abrirá a **caixa de diálogo de configuração de projeto**, permitindo **atualizar rapidamente uma malha**.

**Observação**: se você tiver problemas ao arrastar e soltar, verifique as [Perguntas frequentes sobre o assunto](../../technical-support/technical-issues/miscellaneous-issues/impossible-to-drag-and-drop-files-into-the-shelf.md).

### Melhorias de desempenho

Esta versão do Substance Painter também inclui uma nova e forte melhoria de desempenho em relação à maneira como gerenciamos a memória de GPU (VRam). Cores uniformes (como camadas de preenchimento) agora são compactadas em texturas menores, acelerando a transferência entre a memória principal e a memória de GPU, mas também reduzindo o espaço físico da memória e o tempo de computação. Isso deve ser especialmente visível ao abrir projetos grandes e ao atingir os limites da memória de GPU.

## Notas de versão

### 2017.3.3

(Lançado em 01 de dezembro de 2017)

**Corrigido:**

* [Steam] O pop-up do verificador de versão não deve estar visível na inicialização
* [Exportar] Os arquivos de PSD têm seus grupos bloqueados quando abertos no Photoshop CS6

### 2017.3.2

(Lançado em 20 de novembro de 2017)

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

### 2017.3.1

(Lançado em 26 de outubro de 2017)

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

### 2017.3

(Lançado em 28 de setembro de 2017)

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
* [Prateleira] Adicionar uma ação &#39;Abrir no explorador&#39; para recursos locais na prateleira
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
