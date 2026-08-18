---
helpx_url: "https://helpx.adobe.com/br/substance-3d-painter/technical-support/performances-guidelines/layer-management.html"
breadcrumb-title: ''
description: Aprenda as práticas recomendadas para o gerenciamento de camadas no Substance 3D Painter para otimizar o desempenho e manter projetos organizados.
helpx_creative_field: ""
helpx_description: Painter > Technical support > Performances guidelines > Layer management
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Gerenciamento de camadas
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '677'
ht-degree: 0%

---


# Gerenciamento de camadas

O Painter calcula a pilha de camadas de baixo para cima. Portanto, se você fizer alterações na camada superior da pilha, o Painter só precisará calcular as alterações dessa camada. No entanto, se você fizer uma alteração em uma camada na parte inferior da pilha, o Painter precisará calcular todas as camadas acima dessa camada para calcular o resultado final.

Há várias opções que você pode usar para reduzir o custo de desempenho de fazer alterações em camadas mais baixas na pilha:

+++Usar máscaras de geometria
As máscaras de geometria são a sua melhor ferramenta de otimização. Sempre que puder isolar uma parte da malha para trabalhar, faça isso, mascarando camadas ou pastas. As máscaras de geometria funcionam isolando-as pelo UDIM ou pela parte da malha para que as áreas que não estão na máscara não sejam processadas, melhorando o desempenho. Como bônus, você também pode isolar essas partes visualmente na viewport para facilitar a texturização.

Você pode [saber mais sobre máscaras de geometria com este tutorial](https://www.youtube.com/watch?v=TGASuIGSUns) ou [consultando a documentação](../../interface/layer-stack/geometry-mask.md).

+++

+++Ocultar camadas
Para evitar lentidão ao fazer alterações em um nível inferior na pilha de camadas, você pode ocultar camadas acima da camada editada até terminar de fazer os ajustes. O Painter não processa camadas ocultas, portanto, se todas as camadas acima delas estiverem ocultas, será como se você estivesse editando a camada superior da pilha. Dessa forma, as camadas acima serão computadas apenas uma vez, quando você as reexibir, em vez de após cada alteração feita.

+++

+++Desativar camadas
Assim como as camadas ocultas, o modo de mesclagem desativado impedirá o cálculo das camadas. Pode ser útil definir camadas de baixo impacto para desativar o modo de mesclagem ao modificar áreas em que não são importantes.

+++

+++Usar pastas
Tente agrupar camadas sempre que possível, pois as pastas funcionam como um ponto de cache invisível. Se você estiver fazendo alterações abaixo ou acima de uma determinada pasta, as camadas dentro da pasta não serão recalculadas individualmente, mas o resultado do grupo será recalculado.

+++

+++Limitar o uso de filtros próximos ao topo da pilha de camadas
Os filtros podem ser caros. Se for necessário usar um filtro próximo ao topo da pilha de camadas, use máscaras de geometria para reduzir o custo de desempenho.

+++

+++Limitar o uso do modo de mistura passagem
A passagem é frequentemente usada com filtros ou camadas de traçado de pincel. É um modo de mesclagem dispendioso porque examina todas as camadas subjacentes e transforma o resultado, em vez de substituir o resultado como o modo de mesclagem normal. Sempre que usar a passagem, tente combiná-la com máscaras e pastas de geometria para minimizar o impacto no desempenho.

+++

+++Manter a profundidade de projeção pequena
Com qualquer ferramenta ou modo que tenha uma configuração de profundidade de projeção (distorção, plano, caminho etc.), mantenha o valor de profundidade de projeção o menor possível. Quanto mais a profundidade de projeção se estende, menos desempenho ela é.

+++

+++Tenha cuidado com pincéis que têm traçados dinâmicos
Pincéis e ferramentas com uma tag laranja têm um parâmetro dinâmico. Esse parâmetro dinâmico pode ser definido como “Ilimitado”, o que significa que cada carimbo em um traçado será exclusivo. Isso pode afetar bastante o desempenho ao usar centenas ou milhares de traçados. Na maioria dos casos, é difícil perceber a diferença após 16-32 variações, de modo geral, ir além disso não é susceptível de ter muito impacto visual.

[Saiba mais sobre traçados dinâmicos na documentação.](../../painting/dynamic-strokes/dynamic-strokes.md)

+++

+++Trabalhar com uma resolução de textura mais baixa
Diminuir a resolução do documento é a maneira mais rápida de melhorar o desempenho. Dobrar a resolução significa um mapa quatro vezes maior, de modo que passar de 1k para 2k significa um aumento de até 4 vezes no custo de desempenho. Como resultado, geralmente é útil trabalhar com uma resolução mais baixa pelo maior tempo possível.

+++

+++Definir decalques para o modo de projeção planar
O modo de decalque padrão é Distorcer, mas, a menos que você esteja deformando o decalque movendo seus pontos, alterná-lo para o modo Planar é muito menos dispendioso.

+++
