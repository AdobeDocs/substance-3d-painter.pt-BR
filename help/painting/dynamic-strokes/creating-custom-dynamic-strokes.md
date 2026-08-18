---
helpx_url: "https://helpx.adobe.com/br/substance-3d-painter/painting/dynamic-strokes/creating-custom-dynamic-strokes.html"
breadcrumb-title: ''
description: Saiba como criar traçados dinâmicos personalizados no Substance 3D Painter para criar comportamentos e efeitos exclusivos no traçado de pincel.
helpx_creative_field: ""
helpx_description: Painter > Painting > Dynamic strokes > Creating Custom Dynamic Strokes
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Criação de Traçados dinâmicos personalizados
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '471'
ht-degree: 0%

---


# Criação de Traçados dinâmicos personalizados

Para criar Traçados dinâmicos personalizados, duas opções estão disponíveis:

* Uso de um recurso de Substance existente para criar uma nova predefinição de pincel/ferramenta
* Crie um novo recurso Substance do zero (requer o [Substance 3D Designer](https://substance3d.adobe.com/display/SDDOC/Substance+Designer) ).

Também é recomendável ler os [Desempenhos de traçado dinâmico](dynamic-stroke-performances.md) antes de criar arquivos de Substance personalizados para evitar culpados.

## Reutilizando recurso existente

Criar novos Traçados dinâmicos do zero pode ser difícil. Usar recursos existentes, ajustá-los e salvá-los como novas predefinições pode ser um bom ponto de partida.

Encontre recursos compatíveis na Prateleira que atendam às suas necessidades e confira nossa página sobre [Predefinições](../presets/presets.md).

## Criação de arquivos de Substance personalizados para Traçados dinâmicos

Abaixo há uma lista dos parâmetros suportados para Traçados dinâmicos em gráficos de Substance.

| Identificador de Variável | Descrição |
| --- | --- |
| <b>Propagação Aleatória</b> | Se um arquivo de Substance for preparado com a Distribuição aleatória exposta, ele poderá ser controlado com o recurso Traçado dinâmico. |
| <b>índiceDeCarimbo</b> | <b>Inteiro1</b> será alimentado pelo Substance 3D Painter ao pintar o traçado do pincel. Os valores mínimo e máximo não têm efeito, o Substance 3D Painter os ignora. |
| <b>stampCycleCount</b> | <b>Inteiro1</b> O Painter lerá os valores padrão, mínimo e máximo do parâmetro para expor o parâmetro de Contagem Cíclica de Carimbo. Esse parâmetro controla quantas variações de Substance exclusivas serão criadas. |
| <b>$time</b> | <b>Flutuante1</b> será alimentado pelo Substance 3D Painter ao pintar o traçado de pincel com base no tempo de pintura decorrido (por traçado). Essa propriedade pode gerar muitas variações de Substance e, portanto, afetar o desempenho. |
| <b>strokeSpacing</b> | <b>float1</b> O valor de espaçamento atual para o traçado inteiro pintado. |
| <b>strokeSize</b> | <b>float1</b> O valor do tamanho atual para o traçado inteiro pintado. |
| <b>stampStrokePosition</b> | <b>integer1</b> Usado para especificar o início/início de um traçado. O valor final está disponível apenas no traçado de caminho, não por meio de pintura manual. Valor possível:<ul data-preserve-html="true"> <li data-preserve-html="true">0 = médio</li> <li data-preserve-html="true">1 = início</li> <li data-preserve-html="true">2 = fim</li> </ul>Pode ser desativado usando a tag de usuário isstrokepositionative. |
| <b>distanceAlongCurve</b> | <b>float1</b> A distância atual no carimbo fornecido ao longo de um Caminho. Essa propriedade pode gerar muitas variações de Substance e, portanto, afetar o desempenho. Pode ser desabilitado com a marca de usuário <b>iscurvedistanceactive</b>. |
| <b>distanceMaxCurve</b> | <b>float1</b> O comprimento total de um Caminho criado com a ferramenta de caminho. Pode ser desabilitado com a marca de usuário <b>iscurvedistanceactive</b>. |
| <b>pathCorner</b> | <b>integer1</b> Indique que tipo de canto que uma Faixa de Opções está usando. Valor possível:<ul data-preserve-html="true"> <li data-preserve-html="true">0 = Sem canto</li> <li data-preserve-html="true">1 = Canto esquerdo</li> <li data-preserve-html="true">2 = Canto direito</li> </ul> |
| <b>pathCornerAngle</b> | <b>flutuar</b> ângulo (em radiano) do canto em uma Caminho da faixa. Pode ser usado para compensar ou ajustar a aparência de um canto com base em um valor de ângulo preciso. |
| <b>patchLengthOnCurve</b> | <b>flutuar</b> Tamanho de uma seção (correção) em um Caminho da faixa. Combinado com <b>distanceAlongCurve</b> e <b>distanceMaxCurve</b>, ele pode ser usado para normalizar o tamanho de um patch, por exemplo. |
