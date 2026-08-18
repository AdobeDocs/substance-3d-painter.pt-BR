---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/getting-started/glossary.html"
breadcrumb-title: ''
description: Acesse o glossário da Substance 3D Painter para entender termos e conceitos importantes usados em toda a documentação.
helpx_creative_field: ""
helpx_description: Painter > Getting Started > Glossary
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Glossário
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '2131'
ht-degree: 6%

---


# Glossário

O Substance 3D Painter é um aplicativo 3D que depende de muitas técnicas e palavras-chave técnicas que podem ser difíceis de entender no início.\
Esta página lista as palavras-chave mais comuns usadas pelo aplicativo com uma breve explicação do conceito por trás delas.

| *Palavra-chave* | *Definição* |
| --- | --- |
| **Alinhamento** | O alinhamento é como um pincel será orientado em direção à malha 3D ao pintar. |
| **Alpha** | Um alfa é uma máscara que pode ser usada para pintar detalhes ou formas complexas, como um código de barras ou um logotipo. |
| **Assar** | Cozimento (ou cozimento) refere-se à ação de computação de informações de uma malha 3D e salvá-las em uma textura com base nas informações UV de uma malha. |
| **Profundidade de bits** | A profundidade de bits é a quantidade de informação que pode ser armazenada em uma textura (por cor). Quanto maior o número, melhor a precisão da informação. Entretanto, o desempenho diminui com números altos ao realizar cálculos. |
| **Pincel** | Um pincel é uma ferramenta para pintar em uma malha. Um pincel é definido por vários parâmetros que controlam seu comportamento (como tamanho e opacidade). |
| **Câmera** | A câmera é o objeto que permite controlar a posição e a direção de onde você olha em um visor 3D ou 2D. |
| **Canal** | Um canal é uma textura com um comportamento específico. Alguns canais são usados para definir a cor de um material, outros canais são usados para controlar a luz de comportamento sobre uma superfície. |
| **Clonar** | O clone é uma ferramenta usada para replicar parte da pintura/textura em outro local. |
| **Conteúdo/Máscara** | O conteúdo e a máscara se referem às duas propriedades principais de uma camada. O conteúdo é a pintura real armazenada nos canais que estão contidos em uma camada, enquanto a máscara é usada para exibir/ocultar o conteúdo. Uma máscara preta é igual a um conteúdo invisível. |
| **Difusão** | A difusão é uma maneira de gerar informações fora da Ilha UV de uma malha. Funciona sangrando os últimos pixels perto da borda de uma ilha UV, criando cores desfocadas. |
| **Dilatação/Preenchimento** | Na mesma ideia da difusão, a dilatação é uma forma de gerar informações fora da Ilha UV, estendendo as cores dos pixels. |
| **Efeito** | Um efeito é um elemento que pode ser adicionado a uma camada, no conteúdo ou na máscara. O Substance 3D Painter é compatível com vários tipos de efeitos, como filtros. |
| **Ambiente** | Um ambiente é uma imagem usada para calcular a iluminação de uma cena, geralmente uma textura HDR que representa uma ampla variedade de informações de cores. |
| **Exportar** | A ação de exportar é a forma de gerar texturas achatadas a partir da pintura realizada dentro do aplicativo. As texturas criadas a partir da exportação podem ser usadas em outro aplicativo. |
| **CDV/Campo de Exibição** | O CDV é a extensão do mundo observável pela Câmera. |
| **Preencher** | O Preenchimento é uma ação (que pode ser um efeito ou uma camada) que pode carregar uma cor, uma textura ou até mesmo um material sobre toda a Malha 3D. |
| **Filtro** | Um filtro é um efeito de Substance que pode modificar as informações anteriores. Por exemplo, um filtro de desfoque suavizará uma imagem anterior. Os filtros também podem ser mais complexos e modificar um material completo. |
| **Filtragem** | A filtragem se refere à maneira como a textura é exibida em uma viewport 3D. As mais comuns são as mais próximas (os pixels são lidos como estão, fazendo com que uma imagem pareça estar achatada de perto) e bilineares (os pixels são interpolados, fazendo com que uma imagem pareça embaçada de perto). |
| **GPU** | A GPU (unidade de processamento gráfico) é a parte de um computador que executa uma computação rápida para produzir imagens. |
| **Gerador** | Um Gerador é um Substance que gera novas informações/imagens geralmente com base em texturas adicionais. Por exemplo, alguns geradores de máscara usam textura assada para criar máscaras complexas. |
| **Histograma** | Um histograma é uma representação gráfica da distribuição de valores de cores. É usado para visualizar como as cores são equilibradas dentro de uma imagem entre sombras, tons médios e realces. |
| **Iray** | O Iray é um renderizador de rastreamento de caminho criado pela NVIDIA, usado para projetar uma iluminação realista sobre a malha 3D. Como é um renderizador avançado, ele é destinado à criação de imagens bonitas e não ao trabalho em tempo real. |
| **Tremulação** | A tremulação é uma propriedade do pincel para produzir um comportamento aleatório ao pintar. |
| **Camada** | Uma camada é um elemento que contém vários canais com propriedade adicional, como um modo de mesclagem e uma opacidade. |
| **Pilha de camadas** | Uma pilha de camadas é um local onde as camadas podem ser gerenciadas e organizadas. As camadas são organizadas de baixo para cima. A camada inferior será desenhada primeiro e, em seguida, cada camada acima será adicionada uma por uma sobre a outra. |
| **Mouse Preguiçoso** | O mouse preguiçoso é um comportamento da ferramenta Pincel. Diminui o caminho do pincel para melhorar a precisão ao pintar, criando um atraso/deslocamento entre o cursor do mouse e a pintura real. |
| **Nível** | Um nível é um efeito que permite controlar um intervalo ou informações de cor/escala de cinza por meio de um histograma. Pode ser usado para inverter a cor ou escurecer/clarear a cor, por exemplo. |
| **Log** | Um log é um arquivo de texto no qual são gravadas informações do software, geralmente relacionadas ao computador que executa o aplicativo. |
| **Malha de poli baixa/alta** | Uma malha baixa e uma alta são ambas malha 3D, uma é com uma baixa densidade de polígonos enquanto a outra é com uma quantidade maior de policontagem (muitas vezes 100 vezes maior). Normalmente, as informações de malha alta são transferidas para a malha baixa. |
| **Material** | Um material define as propriedades para representar um assunto específico. Em uma malha 3D, o material também é usado para definir grupos de faces poligonais. |
| **Malha** | Uma malha é um objeto 3D definido por várias informações. No Substance 3D Painter, uma malha é definida por polígonos (geralmente triângulos). Uma malha pode ser criada em um aplicativo de modelagem 3D, como o **Blender** ou o **Autodesk Maya** . |
| **Mapa de malha** | Um mapa de malha é um mapa cozido de uma malha que contém informações relativas à malha. Pode ser uma informação de posição ou uma informação de oclusão, por exemplo. |
| **Mapa De Mip** | Um mip-map é uma textura pré-computada, geralmente presente como uma sequência de imagens cada vez em uma resolução mais baixa do que a textura original. |
| **Modo** | Um modo se refere à configuração da interface que dá acesso a um conjunto específico de ferramentas e controles, dependendo do modo. |
| **Ruído** | Um ruído é uma imagem de procedimento e aleatória, que geralmente representa formas orgânicas e valores de cor/escala de cinza. |
| **Normal** | Um normal é uma textura especial que deforma a maneira como uma luz se comporta na superfície de uma malha 3D para simular detalhes que não existem na geometria. |
| **OpenGL/DirectX** | OpenGL e DirectX são uma interface de programação de aplicativo (API) usada para renderizar informações 2D e 3D. Eles também definem o formato de mapa normal. |
| **Ortográfico** | Uma projeção ortográfica é um meio de representar objetos tridimensionais em duas dimensões em que todas as linhas de projeção são ortogonais ao plano de projeção. |
| **PBR/PBS** | A renderização baseada em física (PBR) ou Sombreamento baseado em física (PBS) é um modelo em computação gráfica que procura renderizar gráficos de uma maneira que modela com mais precisão o fluxo de luz no mundo real. |
| **Embalagem** | Embalagem é a ação de armazenar várias imagens em uma textura. Como as texturas são compostas de canais vermelhos, verdes e azuis separados, elas podem armazenar informações diferentes que podem ser lidas de forma independente em outro aplicativo. |
| **Partículas** | As partículas são um tipo de ferramenta que gera traçados de pincel com base em propriedades físicas ou outros comportamentos complexos. |
| **Perspectiva** | Perspectiva é uma representação aproximada de um objeto ou cena vista pelo olho humano em uma superfície plana (como uma tela). É uma simulação de profundidade e escala. |
| **Pixel/Texel** | Um pixel é um ponto em uma imagem. É o menor elemento possível que contém informações de cores. Quanto maior a resolução, mais pixels estarão disponíveis, permitindo uma melhor definição e mais detalhes. Os texels são pixels dentro de uma textura. |
| **Plug-in** | Plug-ins são funções de programação (muitas vezes expressas por script) que podem ser adicionadas ao software, estendendo as possibilidades do aplicativo. |
| **Pós-processo** | Um pós-processo é um efeito visual aplicado na tela depois que a imagem 3D é renderizada, geralmente para simular um comportamento especial, como a correção de cores ou o desabrochar. |
| **Procedimento** | Procedural é um termo para descrever processos gerados por um computador com base em uma série de parâmetros. Pode ser simplesmente resultados matemáticos, como números ou imagens complexas. |
| **Projeção** | Uma projeção é a ação de aplicar de um ponto de vista específico (como a Câmera) uma imagem/objeto na superfície da Malha 3D. |
| **Resolução (Potência de 2)** | A resolução define o tamanho de uma textura nos eixos X e Y (ou largura e height). Muitas vezes em uma potência de 2 escala (2, 4, 8, 16... 512, 1024, 2048...) porque ele é otimizado para cálculos em uma GPU. |
| **Script** | Script é o ato ou o uso de um comando específico por meio de um formato de arquivo baseado em texto para executar comportamentos específicos. |
| **Sombreador** | Um sombreador define o comportamento de um material quando ele recebe informações de iluminação. Alguns sombreadores podem ser simples (como um sombreamento de tom) ou mais avançados (como um sombreamento de pele que simula a absorção de luz em uma superfície). |
| **Prateleira** | Uma prateleira é o local no aplicativo onde recursos de vários tipos são organizados. Pode ir de imagens simples a ferramentas mais complexas. |
| **Máscara inteligente** | As Máscaras inteligentes se comportam como materiais inteligentes, mas, em vez de serem camadas, são efeitos definidos para gerar máscara somente com base na Malha 3D atual. |
| **Material inteligente** | Um material inteligente é um grupo de camadas salvas como um arquivo. O material inteligente pode se adaptar a cada projeto no Substance 3D Painter, permitindo criar materiais que mudarão dependendo da malha 3D atual. |
| **Borrar** | A Borrar é uma ferramenta para sangrar, espalhar ou misturar cores. É frequentemente usado para suavizar pixels. |
| **Estêncil** | Um estêncil é uma imagem alinhada à tela e usada com uma projeção de câmera para pintar na Malha 3D. |
| **Substance** | Um Substance é um formato de arquivo que permite gerar textura com base em um conjunto de parâmetros (que envolvem cálculos de procedimento). Esses parâmetros podem ser modificados para criar variações. |
| **Simetria** | A simetria é uma opção de uma ferramenta que permite pintar em dois lugares ao mesmo tempo no espelho. |
| **Modelo** | Um modelo é um conjunto de opções predefinidas usadas ao criar um novo projeto. Ele pode definir a resolução padrão ou a configuração de cozimento padrão, por exemplo. |
| **Taxa de texel** | A proporção de texel é a regra que compara o tamanho de uma Ilha UV (2D) com a geometria da malha 3D relacionada a ela. Uma boa proporção de texel significa um desdobramento uniforme da geometria em 2D. Isso é importante para manter a aparência e a qualidade da pintura/texturização consistentes na Malha 3D. |
| **Textura** | Uma textura é um arquivo que contém pixels em duas dimensões definidas por uma resolução. Os pixels podem ser coloridos ou em tons de cinza. Quando coloridos, os pixels podem ter uma informação de transparência (se compatíveis com o formato do arquivo). |
| **Conjunto de Texturas** | No Substance 3D Painter, um conjunto de texturas representa uma parte de uma malha que tem UVs específicos para serem pintados. O Conjunto de texturas é criado de acordo com o material exclusivo detectado ao importar uma malha 3D. |
| **Cobrança** | O revestimento é a repetição de uma textura onde as costuras não são visíveis nas bordas, ele é feito para simular um plano infinito. Exemplo: grama ou pavimentos. |
| **Ferramenta** | Uma ferramenta se refere a uma ação que permite interagir com a Malha 3D, geralmente para pintar ou aplicar efeitos. |
| **Barra de ferramentas** | A barra de ferramentas é o local onde todos os atalhos de ícone para as ferramentas estão disponíveis. |
| **UDIM** | O UDIM é uma maneira de dividir os UVs de uma malha 3D em vários intervalos para aumentar a resolução da textura geral. |
| **UV** | UV são informações definidas em uma malha 3D que indicam como ela pode ser desdobrada para se tornar uma forma plana. Essas informações são usadas para projetar uma textura em uma Malha 3D. O Substance 3D Painter permite pintar somente no intervalo 0-1, que representa o tamanho de uma textura. Outros intervalos só são aceitos pelo sistema UDIM. |
| **VRam** | A VRam é a memória da GPU (placa gráfica), usada para armazenar informações e texturas ao realizar cálculos. Quanto mais VRam, melhor para trabalhar com o Substance 3D Painter. |
| **Visor** | A janela de visualização é o local onde a cena 3D ou 2D é exibida na tela. Nela também é possível interagir com as ferramentas e com a Malha 3D controlando a câmera. |
