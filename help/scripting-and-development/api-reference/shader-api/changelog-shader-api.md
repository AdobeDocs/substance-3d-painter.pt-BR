---
helpx_url: "https://helpx.adobe.com/br/substance-3d-painter/scripting-and-development/api-reference/shader-api/changelog-shader-api.html"
breadcrumb-title: ''
description: Revise o log de alterações do Substance 3D Painter API de sombreamento para acompanhar atualizações, novos recursos e alterações ao longo do tempo.
helpx_creative_field: ""
helpx_description: Painter > Scripting and development > API Reference > Shader API > Changelog - Shader API
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Changelog - API de sombreamento
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '837'
ht-degree: 3%

---


# Changelog - API de sombreamento

## Changelog

## 2018.3.2

* [lib-sparse.glsl](libraries-shader-api/lib-sparse-shader-api.md): as funções de amostragem usam derivados de textura em vez de nível do mipmap simples. É um requisito para o suporte de amostragem de anisotropia. As assinaturas das funções de amostragem não são modificadas.
* [lib-pom.glsl](libraries-shader-api/lib-pom-shader-api.md): a assinatura da função *getParallaxOffset* foi alterada para usar derivados de textura

## 2018.3.0

* Adicione uma nova biblioteca [lib-pbr-aniso.glsl](libraries-shader-api/lib-pbr-aniso-shader-api.md) para ajudar a visualizar o destaque de specular anisotrópico
* Adicione uma nova biblioteca [lib-sparse.glsl](libraries-shader-api/lib-sparse-shader-api.md) para ajudar na amostragem de canais, cuidando da disponibilidade de mipmaps
* Atualize as interfaces das bibliotecas do sombreador para cuidar desta amostragem segura
* **Descontinuação**: as funções anteriores baseadas nas coordenadas de textura vec2 e no amostrador de textura foram descontinuadas (use novas assinaturas)
* [lib-pom.glsl](libraries-shader-api/lib-pom-shader-api.md): adicione uma função *applyParallaxOffset* para simplificar o uso do efeito de oclusão de paralaxe
* [lib-random.glsl](libraries-shader-api/lib-random-shader-api.md): adicionar um gerador de valor aleatório de Ruído Azul e alternativas temporais
* [lib-sampler.glsl](libraries-shader-api/lib-sampler-shader-api.md): divida todos os auxiliares de amostragem de canal para ter ambos os auxiliares de interpretação de valor e amostragem

## 2018.2.0

* **Alteração de API de sombreamento de superfície**: a assinatura da função *sombra* foi alterada, consulte [surface-shader.glsl](shaders-shader-api/surface-shader-shader-api.md)
* A função *shadeShadow* não é mais usada e pode ser removida com segurança de sombreadores de superfície personalizados
* Adicione suporte para dispersão de subsuperfície; consulte [surface-shader.glsl](shaders-shader-api/surface-shader-shader-api.md) e [lib-sss.glsl](libraries-shader-api/lib-sss-shader-api.md) para obter detalhes
* [lib-pbr.glsl](libraries-shader-api/lib-pbr-shader-api.md): a função *pbrComputeBRDF* foi removida. Veja o exemplo de [pbr-metal-rough.glsl](shaders-shader-api/pbr-metal-rough-shader-api.md) para saber como usar a biblioteca agora
* Novos parâmetros de mecanismo foram adicionados: *textura\_azul\_noise*, *aspecto\_razão*, *camera\_vp\_matrix\_inverse*, *ambiente\_exposição*, *ambiente\_rotação*, *fovy*, *principal\_luz* e *tela\_tamanho*. Consulte [all-engine-params.glsl](parameters-shader-api/all-engine-params-shader-api.md) para obter detalhes
* Adicionar os metadados de *descrição* para fornecer dicas de ferramentas para parâmetros de sombreador personalizados

## 2017.4.2

* Corrigir sombreadores ausentes em amostras de documentação (sombreadores pixelados e toon)
* Corrigir pontilhamento para alta resolução
  * [lib-bayer.glsl](libraries-shader-api/lib-bayer-shader-api.md): **bayerMatrix8()** retorna valores válidos para coordenadas > 4k

## 2017.4.1

* Corrigir sombreador revestido com pbr
  * [lib-vetors.glsl](libraries-shader-api/lib-vectors-shader-api.md): **tangentSpaceToWorldSpace()** e **worldSpaceToTangentSpace()** as saídas agora estão normalizadas

## 2017.4.0

* Reflexo de specular incorreto na exibição 2D para determinadas malhas

## 2017.3.1

* Pontilhamento mais barato

## 2017.2.0

* Remova a normalização interpolada de tbn para corresponder ao comportamento de Substance Designer e padeiros
* [Visor] Substituir a tabela Hammersley por uma espiral de Fibonacci

## 2.6.0

* Corrigir os modos de mesclagem e eliminação de sombreadores
* Retrabalhe o pontilhamento. Agora, se tivermos uma renderização em linear, a aplicaremos após o perfil de cores

## 2.5.0

* Adicionar suporte para perfis de cor (LUT) em viewports (conversão sRGB opcional)
* Adicionar pontilhamento à opacidade em sombreadores
* Adicionar mapeamento de oclusão de paralaxe a sombreadores PBR
* Adicionar uma maneira de ocultar parâmetros personalizados da interface do usuário do sombreador padrão
* Adicionar um link para a lista de tags de canal na documentação do sombreador de camadas
* Substituir a tag &#39;channel\_ao&#39; por &#39;channel\_ambientocclusion&#39;
* [Janela de visualização] Alguns mapas normais têm valores fixados que aparecem como artefatos
* Corrigir canais disponíveis no documento shaders
* Permitir a definição de uma interface de usuário de sombreador personalizada
* Adicionar uma interface de usuário de sombreador personalizada padrão para sombreadores de camadas de material
* Os arquivos de interface personalizada agora são pesquisados em relação a uma pasta shaders/custom-ui nas prateleiras (como o mdl)
* Usar o canal de specular level em sombreadores padrão
* Exemplo de parâmetros de sombreador Fix vec3
* Atualizar o Painter para o perfil principal do OpenGL

## 2.4.0

* Corrija a diferença no mapa normal combinado exportado e aquele exibido no visor

## 2.2.0

* Adicionar suporte para texturas sem associação em material genérico para texturas que não sejam do Documento
* Atualizar a documentação de controles deslizantes de sombreador personalizados
* Permitir a definição da precisão da etapa para controles deslizantes
* Documentação do camadas de material dinâmico

## 2.1.1

* Adicionar uma função &#39;RGB2Gray&#39; em lib-utils

## 2.1.0

* Permitir a definição de grupos para parâmetros de sombreador e materiais/máscaras
* Adicionar canais ausentes na documentação (&#39;ao&#39;, &#39;diffuse&#39;, &#39;specularlevel&#39;)

## 2.0.4

* Função de descompactação normal incorreta com valores alfa baixos
* Permitir a leitura de cores de vértice de malha no sombreador personalizado
* [Visor] Mapa de ambiente ampliado em alguns computadores

## 2.0.0

* Permitir a substituição de mapas adicionais de Normal/AO por canal dedicado
* Altere a função Height2Normal para usar o método Sobel
* Adicionar a possibilidade de definir um mdl por sombreador
* Adicionar uma nova pasta mdl na prateleira
* Adicionar predefinições de canal difuso e de specular level
* Atualização da documentação para mapeamento de tom
* Corrigir reflexos no modo ortográfico
* Correção de uma falha vertical branca que aparecia em um local específico no mapa de ambiente
* Permitir a definição de &#39;default\_color&#39; para parâmetros de textura

## 1.7.0

* Permitir a amostragem de texturas externas (da prateleira)

## 1.6.0

* Exponha a função de mapeamento de gama/tons para permitir que eles sejam substituídos
* Expor várias palavras de texto

## 1.5.0

* Adicionar número de linha e nome de arquivo no relatório de erros do sombreador

## 1.4.1

* Todas as conversões sRGB seguem o padrão sRGB, exceto aquelas feitas nos sombreadores que possuem uma aproximação aproximada
* O canal de height para o Mapa normal é convertido no espaço de cores incorreto

## 1.4.0

* Adicionar canal de oclusão de ambiente
* Adicionar novo fluxo de trabalho para a edição normal
* Adicionar sintaxe de expressão &#39;or&#39; para parâmetros automáticos relacionados à textura
* Corrigir pbr shader para GPU Intel no OSX

## 1.3.4

* Permitir a interpolação de binormais no sombreador de fragmentos
* Corrigir espaço tangente Mikkt

## 1.3.3

* Corrigir harmônicos esféricos produzindo intensidade de luz negativa
* O cálculo da exposição é diferente do controle deslizante Substance Designer (e corrigir a exposição)
* As sombras não devem ser visíveis em uma superfície 100% metálica

## 1.3.0

* Adicionar função de sombra
* Adicionar suporte para opacidade (&#39;alpha\_test&#39; e &#39;alpha\_blend&#39;)

## 1.2.0

* Capacidade de definir estados necessários de OpenGL em sombreadores personalizados
* Corrigir bitangents invertidos
* Adicionar suporte para canal normal

## 1.0

* Adicionar suporte para sombreadores personalizados
