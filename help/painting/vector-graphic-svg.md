---
helpx_url: "https://helpx.adobe.com/br/substance-3d-painter/painting/vector-graphic-svg.html"
breadcrumb-title: ''
description: Saiba como usar gráficos vetoriais (arquivos SVG e AI) no Substance 3D Painter para adicionar arte vetorial dimensionável a texturas.
helpx_creative_field: ""
helpx_description: Substance 3D Painter
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Gráfico vetorial (SVG)
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '522'
ht-degree: 1%

---


# Gráfico vetorial (.svg &amp; .ai)

![Imagem mostrando um arquivo svg projetado em uma malha próximo a uma lista de parâmetros](../assets/svg_overview.png)

Arquivos gráficos vetoriais (<b>.svg</b> e Illustrator <b>.ai</b>) podem ser importados como imagens regulares dentro do Painter. Algumas configurações estão disponíveis para ajustar a aparência do gráfico e ajustá-lo melhor ao restante da texturização.

* Para obter mais informações sobre arquivos SVG, [veja esta página](https://www.adobe.com/creativecloud/file-types/image/vector/svg-file.html).
* Para obter mais informações sobre arquivos AI, [consulte esta página](https://www.adobe.com/ie/creativecloud/file-types/image/vector/ai-file.html).

Os arquivos de SVG e AI são automaticamente convertidos em imagens em pixels quando usados dentro da [Pilha de camadas](../interface/layer-stack/layer-stack.md) (dependendo da configuração selecionada). Esse é um processo não destrutivo. Alterar a resolução ou atualizar o arquivo de origem atualizará o resultado final de acordo.

## Propriedades

Depois de importar um arquivo vetorial e carregá-lo dentro de uma camada ou propriedades de ferramenta, um conjunto de parâmetros estará disponível:

| Seção | Configuração | Descrição |
| --- | --- | --- |
| <b>Prancheta</b> | <b>Prancheta</b> | Selecione qual prancheta incluída no arquivo é usada.  **Observação:** esta configuração só está disponível com arquivos Illustrator (.ai). |
| <b>Resolução</b> | Resolução | Defina o tamanho em que o svg será convertido em uma imagem bitmap (pixels) quando usado para texturização dentro da Pilha de camadas.   Valores possíveis:<ul data-preserve-html="true"> <li data-preserve-html="true"><b>Automático</b>: a resolução é determinada pela resolução do Conjunto de Textura atual (quando usado na camada/efeito de preenchimento) ou para 512 pixels quando usado em uma ferramenta de pincel.<br/> </li> <li data-preserve-html="true"><b>Ativo</b>: a resolução é determinada pelo tamanho de pixel definido no próprio arquivo SVG.<br/> </li> <li data-preserve-html="true"><b>Personalizada</b>: a resolução é determinada pela configuração de resolução imediatamente abaixo na interface.</li> </ul>  <div><img alt="configuração de resolução svg" class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_table_row-ad42696-column-7212622_image" src="../assets/svg_resolution_custom.png" title="configuração de resolução svg"/></div> |
|  |  |  |
| <b>Área de corte</b> | Cortar para | Defina como as formas de SVG serão limitadas à área renderizada.   Valores possíveis:<ul data-preserve-html="true"> <li data-preserve-html="true"><b>Limites do ativo</b>: a área é definida pelos limites definidos no arquivo SVG.</li> <li data-preserve-html="true"><b>Personalizado</b>: a área é definida por valores explícitos através das configurações da interface logo abaixo.<br/> </li> </ul> |
|  | Proporção quadrada | Se a área de corte for definida por <b>Limites do ativo</b>, essa configuração garante que a proporção original seja preservada, evitando qualquer amplificação incorreta ao renderizar o SVG como uma imagem quadrada.   Esta configuração pode tornar alguns elementos inesperadamente visíveis. Para evitar esse problema, desative essa configuração e, em vez disso, ajuste as configurações UV manualmente quando estiver dentro de uma camada/efeito de preenchimento. |
|  | Superior esquerdo inferior direito | Se o corte estiver definido como Área personalizada, essas configurações permitirão definir a área manualmente, especificando os cantos superior esquerdo e inferior direito. |
|  |  |  |
| <b>Escopo</b> | Escopo | Defina quais elementos dentro do arquivo SVG são incluídos antes de renderizá-lo.   O padrão é <b>Documento</b>, o que significa que todo o conteúdo do arquivo SVG é usado. Use o botão <b>Alterar</b> para ajustar os elementos a serem incluídos. |

### Janela Escopo

Ao editar o escopo de um gráfico vetorial (consulte a configuração acima), uma janela será exibida com uma lista de elementos a serem selecionados para especificar o que incluir ou excluir da imagem renderizada final.

Use a caixa de seleção <b>Mostrar miniaturas</b> para exibir uma imagem de cada elemento.

![](../assets/v10_ai_thumbs.jpg)
