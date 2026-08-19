---
helpx_url: "https://helpx.adobe.com/br/substance-3d-painter/technical-support/performances-guidelines/mesh-and-uv-setup.html"
breadcrumb-title: ''
description: Saiba mais sobre as práticas recomendadas para configuração de malha e UV no Substance 3D Painter para otimizar o desempenho e a qualidade da textura.
helpx_creative_field: ""
helpx_description: Painter > Technical support > Performances guidelines > Mesh and UV setup
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Configuração de malha e UV
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '432'
ht-degree: 0%

---


# Configuração de malha e UV

Reservar alguns minutos para preparar a malha para o Painter pode tornar o processo de texturização mais rápido e fácil.

+++Modelos de alto contador
Não há um benchmark específico para o policount que o Painter possa manipular, pois ele depende muito das especificações da máquina, da atribuição do conjunto de texturas e das propriedades da pilha de camadas. No entanto, menos de 10 milhões de poliys devem ser manipulados adequadamente se as otimizações da pilha de camadas forem levadas em consideração.

+++

+++Modelos de baixo policontagem
Existe uma coisa tão baixa quanto o poli. Isso ocorre porque o mecanismo de textura usa os Polígonos para saber qual parte da malha deve ser renderizada para calcular os traçados do pincel. Malhas com um Polycount muito baixo podem ser totalmente renderizadas mesmo com pinceladas pequenas que podem sobrecarregar a GPU desnecessariamente.

Por exemplo, se estiver texturizando um único plano quádruplo, é melhor subdividir a malha, especialmente ao pintar à mão com muitos traçados, pois as informações são espalhadas por mais vértices.

+++

+++Dividir texturas em vários conjuntos de texturas
É melhor dividir malhas maiores com atribuições de material mais complexas em vários conjuntos de texturas. Os conjuntos de textura permitem atribuir diferentes configurações por conjunto de textura, como propriedades de resolução e sombreador. Por exemplo, se apenas uma parte da malha usar translucidez ou SSS, é melhor atribuir outro Conjunto de texturas e uma ocorrência de sombreador diferente a essa parte. Assim, essas propriedades mais complexas não precisam ser calculadas onde não são utilizadas.

+++

+++Mantenha as Ilhas UV próximas
Tente manter próximas as Ilhas UV que são vizinhas no espaço 3D. Isso se aplica ao layout UDIM e ao layout de espaço UV clássico. Se eles tiverem traçados de tinta ou texturização compartilhados, será mais fácil calculá-los quando estiverem amontoados na mesma área do espaço UV, em vez de se estiverem em extremidades opostas.

O mecanismo de textura trabalha dividindo uma textura em blocos menores para acelerar o cálculo. Isso significa que cada traçado atualiza apenas os blocos que precisam ser alterados, em vez de atualizar a textura inteira com cada traçado. Ao manter as Ilhas UV vizinhas próximas umas das outras, minimiza o número de blocos que serão afetados por um único traçado.

+++

+++Evite ter muitos objetos
O desempenho deve permanecer confortável ao importar uma malha com menos de 8.000 subobjetos. Ultrapassar esse limite pode afetar o desempenho da viewport e da pintura. Se esse limite for atingido, recomendamos mesclar os objetos para reduzir a sobrecarga de renderização.

+++
