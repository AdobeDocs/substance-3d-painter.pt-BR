---
helpx_url: 'https://helpx.adobe.com/substance-3d-painter/baking/mesh-map-settings.html'
breadcrumb-title: ''
description: Saiba como definir as configurações do mapa de malha no Substance 3D Painter para controlar os parâmetros de cozimento e a qualidade da saída.
helpx_creative_field: ''
helpx_description: Substance 3D Painter
helpx_experience_level: ''
helpx_learn_topic: ''
helpx_tags: ''
title: Configurações do mapa de malha
user-guide-description: ''
user-guide-title: ''
source-git-commit: 7b5f6e6c9623cb51253b6e49c8dbcbb22856418c
workflow-type: tm+mt
source-wordcount: '1348'
ht-degree: 10%

---


# Configurações do mapa de malha

<b>O painel de configurações do Mapa de malha</b> está disponível no modo de cozimento e tem controles para preparar a malha para cozimento. Para ajustar as configurações de mapa de malha de um determinado mapa, selecione o mapa no <b>painel Preparadores de mapa de malha</b>. Cada mapa de malha pode ter diferentes configurações disponíveis. Uma coleção de <b>Configurações comuns </b>compartilhadas por todos os mapas de malha está disponível na parte superior do painel Preparadores de mapas de malha.

Todas as configurações compartilhadas entre mapas de malha serão exibidas na página Configurações comuns, em vez de em cada mapa de malha individual.

## Configurações comuns

A página Configurações comuns contém controles que afetam o modo como todos os mapas de malha são preparados.

### Configurações de saída

| Configuração | Função |
| --- | --- |
| Tamanho da saída | Defina a resolução X e Y dos mapas de malha gerados. Clique no cadeado para permitir resoluções não quadradas. |
| Largura de dilatação | Ajuste o quanto as informações preparadas se estendem além dos limites das Ilhas UV. |
| Aplicar difusão | Habilite esta caixa para aplicar a difusão às bordas das informações geradas. |

### Parâmetros de alta poligonalidade

| Configuração | Função |
| --- | --- |
| Usar malha Low poly como malha high poly | Ative esta configuração para preparar mapas com base na malha do seu projeto. |
| Malhas de alta definição | Adicione malhas polinomiais altas ao seu projeto para fazer a partir de uma malha polinomial alta até a malha polinomial baixa em seu projeto. Várias malhas podem ser importadas. |
| Gaiola | Determine como a assadeira é gerada.<ul data-preserve-html="true"> <li data-preserve-html="true">Distância com base: infle os vértices fora da malha a uma distância uniforme pelo modelo para criar uma caixa.</li> <li data-preserve-html="true">Automático (experimental): o Painter analisará sua malha e gerará uma gaiola automaticamente, tentando mantê-la próxima à superfície sem criar interseções para obter melhores resultados.</li> <li data-preserve-html="true">Arquivo personalizado: importe um arquivo que você criou para usar como o compartimento. Observe que os arquivos importados devem ter o mesmo número de vértices que a malha base para funcionar corretamente.</li> </ul> |
| Ignorar Face traseira | Se marcada, as faces traseiras são ignoradas durante a cozedura. Isso pode ajudar a reduzir artefatos, mas também pode causar erros em alguns casos extremos. |
| Correspondência | Mude como o Padeiro determina se os objetos devem ser incluídos durante a cozimento:<ul data-preserve-html="true"> <li data-preserve-html="true">Sempre: Inclua todas as malhas de poli alto que são atingidas dentro da gaiola enquanto assando.</li> <li data-preserve-html="true">Por nome de malha: para cada gaiola, assar apenas malhas com o sufixo de malha correspondente.</li> </ul> |
| Sufixo de malha de poli baixa | Ao usar o nome da malha Corresponder por, use esse sufixo para definir malhas poligonais baixas. |
| Sufixo de malha de poli alta | Ao usar Corresponder pelo nome da malha, use esse sufixo para definir malhas de poli alto e correspondê-las à malha de poli baixo correspondente. |
| Suavização de borda | Ajuste a quantidade de suavização de borda nos mapas gerados. |

#### Correção de distorção

| Configuração | Descrição |
| --- | --- |
| **Correção de inclinação de pintura** | Entre no modo de pintura de correção de inclinação. |
| **Proteção de borda** | Alterne a proteção de aresta para mascarar valores de correção de inclinação pintados próximos às arestas sólidas. |
| **Distância da borda** | Controla o quanto a proteção de aresta se estende das arestas sólidas |
| **Contraste de borda** | Controle a nitidez da transição do gradiente da proteção de borda da proteção total para nenhuma proteção. |

## Configurações do mapa de IDs

| Configuração | Função |
| --- | --- |
| Origem da cor | Altere como as cores de cozimento do mapa de ID são determinadas:<ul data-preserve-html="true"> <li data-preserve-html="true">Cor do vértice</li> <li data-preserve-html="true">Cor do material</li> <li data-preserve-html="true">ID do arquivo</li> <li data-preserve-html="true">Identificação/Poligrupo de malha</li> </ul> |
| Gerador de cores | Ao usar a ID do arquivo ou a ID/Polygroup de malha como a origem da cor, determine como as cores são geradas:<ul data-preserve-html="true"> <li data-preserve-html="true">Aleatória</li> <li data-preserve-html="true">Alteração de matiz</li> <li data-preserve-html="true">Tons de cinza</li> </ul> |

## Configurações do mapa de oclusão do ambiente

| Configuração | Função |
| --- | --- |
| Raios secundários | Altere o número de raios secundários. Mais raios podem produzir melhores resultados em detrimento do maior tempo de processamento. |
| Distância mínima do oclusor | Ajuste a distância mínima para que os raios viajem para atingir a alta geometria poli e impactar o mapa de AO resultante. |
| Distância máxima do oclusor | Os raios que se estendem para além dessa distância sem atingir a malha alta do poli são considerados como não sendo ocultados e não afetarão o mapa do AO. |
| Referente à caixa delimitadora | Quando esta caixa está marcada, outras configurações que se referem à distância se baseiam na caixa delimitadora da malha do projeto. Portanto, uma distância de 1 é igual ao tamanho da caixa delimitadora. |
| Ângulo de propagação | Ajuste o intervalo de angular dos raios gerados. Um ângulo de propagação mais alto permite que uma superfície seja ocultada mais facilmente por geometria que não está posicionada perpendicularmente longe da superfície. |
| Distribuição | Selecione como os raios são distribuídos. |
| Ignorar Face traseira | Altere se as faces traseiras são consideradas para ocultar objetos. |
| Auto-oclusão | Selecione quais malhas devem afetar a oclusão ambiente da malha atual. |
| Atenuação | Alterar como a oclusão é atenuada pela distância do oclusor. |
| Plano do solo | Habilite isto para criar um plano terrestre que atue como um oclusor. |
| Deslocamento do plano do solo | Alterar a posição do plano do solo. |

## Configurações do mapa de curvatura

| Configuração | Função |
| --- | --- |
| Método | Escolha como gerar o mapa de curvatura. |
| Raios secundários | Ajuste quantos raios secundários são usados para gerar o mapa de curvatura. Mais raios secundários podem produzir melhores resultados, ao custo de um maior tempo de processamento. |
| Raio de amostragem | Ajuste o quanto o padeiro busca para calcular a curvatura do ponto atual. |
| Em relação à caixa delimitadora | Quando esta opção está marcada, todas as distâncias são baseadas no tamanho da caixa delimitadora de malha. |
| Auto-interseção | Escolha quais objetos serão considerados ao determinar a curvatura. |
| Mapeamento de tons automáticos (por bloco UV) | Deixe essa opção marcada para ajustar automaticamente os mapas de curvatura do mapa de tons por bloco UV. |
| Mapeamento de tons mínimo | Se o mapeamento automático de tons estiver desativado, ajuste o valor mínimo para o mapeamento de tons. |
| Mapeamento de tons máximo | Se o mapeamento automático de tons estiver desativado, ajuste o valor máximo para o mapeamento de tons. |

## Configurações do mapa de posições

| Configuração | Função |
| --- | --- |
| Modo | Selecione se deseja gerar um mapa de posição de todos os eixos ou calcular somente a posição para um eixo selecionado. |
| Eixo | Se o modo Eixo único estiver selecionado, use essa configuração para escolher qual eixo calcular. |
| Tipo de normalização | Altere como os valores de posição são normalizados, seja com uma Caixa delimitadora, uma Esfera delimitadora ou desative a normalização. |
| Escala de normalização | Altere o que é considerado o limite máximo do espaço de posição. |

## Configurações do mapa de thicknesss

| Configuração | Função |
| --- | --- |
| Raios secundários | Altere o número de raios secundários. Mais raios podem produzir melhores resultados em detrimento do maior tempo de processamento. |
| Distância mínima do oclusor | Ajuste a distância mínima para que os raios viajem para atingir a alta geometria poli e impactar o mapa de thickness resultante. |
| Distância máxima do oclusor | Os raios que se estendem para além dessa distância sem atingir a malha alta de poli são considerados como não estando ocultos e não afetarão o mapa de thickness. |
| Referente à caixa delimitadora | Quando esta caixa está marcada, outras configurações que se referem à distância se baseiam na caixa delimitadora da malha do projeto. Portanto, uma distância de 1 é igual ao tamanho da caixa delimitadora. |
| Ângulo de propagação | Ajuste o intervalo de angular dos raios gerados. Um ângulo de propagação mais alto permite que uma superfície seja ocultada mais facilmente por geometria que não está posicionada perpendicularmente longe da superfície. |
| Distribuição | Selecione como os raios são distribuídos. |
| Auto-oclusão | Selecione quais malhas devem afetar o thickness da malha atual. |
| Normalização | Altere como os valores de thickness são normalizados. |

## Configurações do mapa de heights

| Configuração | Função |
| --- | --- |
| Normalização | Altere como os valores de height são normalizados. |
| Divisor de escala | Se a Normalização estiver definida como Manual, use esse controle deslizante para ajustar o divisor de escala e a normalização do mapa de height. |

## Configurações do mapa de curvas normais

| Configuração | Função |
| --- | --- |
| Raios secundários | Altere o número de raios secundários. Mais raios podem produzir melhores resultados em detrimento do maior tempo de processamento. |
| Distância mínima do oclusor | Ajuste a distância mínima para que os raios viajem para atingir a alta geometria poli e impactar o mapa de curvas normais resultante. |
| Distância máxima do oclusor | Os raios que se estendem para além dessa distância sem atingir a malha alta de poli são considerados não ocluídos e não afetarão o mapa de curvas normais. |
| Referente à caixa delimitadora | Quando esta caixa está marcada, outras configurações que se referem à distância se baseiam na caixa delimitadora da malha do projeto. Portanto, uma distância de 1 é igual ao tamanho da caixa delimitadora. |
| Ângulo de propagação | Ajuste o intervalo de angular dos raios gerados. Um ângulo de propagação mais alto permite que uma superfície seja ocultada mais facilmente por geometria que não está posicionada perpendicularmente longe da superfície. |
| Distribuição | Selecione como os raios são distribuídos. |
| Ignorar Face traseira | Escolha se as faces traseiras devem ser tratadas como oclusivas. |
| Auto-oclusão | Selecione quais malhas devem afetar os normais de curvatura para a malha atual. |
