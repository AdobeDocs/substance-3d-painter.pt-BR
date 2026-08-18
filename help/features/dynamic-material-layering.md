---
helpx_url: "https://helpx.adobe.com/br/substance-3d-painter/features/dynamic-material-layering.html"
breadcrumb-title: ''
description: Saiba como usar o camadas de material dinâmico no Substance 3D Painter para mesclar e combinar materiais com máscaras de procedimento.
helpx_creative_field: ""
helpx_description: Painter > Features > Dynamic Material Layering
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Camadas de material dinâmico
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '594'
ht-degree: 0%

---


# Camadas de material dinâmico

![](../assets/dynamic-material-blending-materials.jpg){width="450px"}

**Camadas de material dinâmico** é um fluxo de trabalho específico em que materiais genéricos são misturados dentro de um sombreador em vez de em uma única textura. A principal vantagem desse fluxo de trabalho é que a mesclagem é dinâmica e permite controlar e preservar um certo nível de qualidade, inclinando materiais genéricos dentro do sombreador. Embora os materiais sejam genéricos, as máscaras usadas para mesclá-los são específicas para malha e, portanto, não se repetem.

![](../assets/tilling-mat-layer.gif){width="400px"}

Para habilitar o fluxo de trabalho de camada de material, é necessário um sombreador específico.\
O sombreador &quot; **pbr-material-layering** &quot; enviado por padrão com o Substance 3D Painter permite mesclar 4 materiais com 3 máscaras.

## Pilhas de subcamadas

Nessa camada, as subpilhas do sombreador podem ser definidas e amostradas diretamente pelo sombreador. Exemplo com o sombreador “pbr-material-layering” fornecido com o Substance 3D Painter:

```
//: stacks [ 

//:   { 

//:     "id": "Mask", 

//:     "channels": [ 

//:   {"id": "opacity"} 

//:  ] 

//:   }, 

[...] 

//: ]
```


![](../assets/sub-stacks.png) Neste exemplo, o sombreador criará três subpilhas em um determinado conjunto de texturas com um canal de “opacidade” em cada uma. As subpilhas podem ser acessadas na janela de lista do TextureSet:

Como os **canais** das pilhas de subcamadas estão definidos **no sombreador**, é impossível adicionar novos canais nas configurações do conjunto de texturas. Para adicionar ou remover um canal, é necessário atualizar o arquivo de sombreador.

O número máximo de canais suportados é definido pelo número total de amostradores suportados pelo hardware.\
Embora o Substance 3D Painter ofereça suporte a texturas sem associação (e, portanto, quantidade ilimitada de texturas) para materiais carregados como parâmetros, os canais fornecidos pelo mecanismo para as pilhas de camadas são limitados a 32 (no Windows). Esse limite também inclui outras texturas, como a Oclusão Normal e a Ambient assadas na malha do projeto.

## Entradas de materiais

Embora seja possível configurar subpilhas para definir materiais além de máscaras, muitas vezes é mais prático apenas definir entradas de materiais no sombreador e usar materiais diretamente da prateleira. Na maioria das vezes, esses materiais também existem na aplicação final, como Unity ou Unreal Engine 4. A convenção de nomenclatura para declarar materiais é parecida com a seguinte no sombreador “pbr-material-layering”:

```
//: materials [ 

//:   { 

//:      "id": "Material1", 

//:      "label": "Material 1", 

//:      "default": "", 

//:      "size": 1024, 

//:      "default_color": [0.5, 0.5, 0.5] 

//:   }, 

[...] 

//: ]
```


![](../assets/materials.png) Este é o resultado quando alguns materiais (materiais do substance ou predefinições de material) foram carregados:

A resolução do material pode ser definida com o parâmetro “size”. Também é possível carregar materiais por padrão quando o sombreador é criado com o parâmetro “padrão” (usando o nome/rótulo do recurso que precisa ser carregado).

Para acessar os materiais e a máscara no próprio sombreador, basta conectá-los com a palavra-chave “param auto” :

```
//: param auto Material1.channel_basecolor 

uniform sampler2D color1; 

 

//: param auto Mask.channel_opacity 

uniform sampler2D mask;
```


Nesse fluxo de trabalho específico, a parte mais importante é a máscara e os parâmetros de sombreador. Portanto, na janela de exportação do Substance 3D Painter, é recomendável habilitar a configuração &quot; **Exportar parâmetros de sombreadores** “. Isso criará um arquivo **JSON** no disco, próximo às texturas, que conterá informações sobre a configuração das subpilhas, os materiais usados, os sombreadores e seus parâmetros. Exportação e importação de parâmetros

No momento, a embalagem de máscaras em uma única textura não é suportada durante a exportação. No entanto, uma solução alternativa simples para isso seria usar os recursos de script e chamar as ferramentas de lote de Substance para fazer a embalagem com um Substance.

![](../assets/export-window-shader.png)

Esse arquivo JSON pode ser usado para configurar as pilhas de camadas e os sombreadores de um projeto.\
Isso permite alternar entre vários aplicativos facilmente compartilhando parâmetros comuns.

![](../assets/import-jsons.png)
