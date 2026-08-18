---
helpx_url: "https://helpx.adobe.com/br/substance-3d-painter/painting/dynamic-strokes/dynamic-stroke-performances.html"
breadcrumb-title: ''
description: Saiba mais sobre as considerações sobre o desempenho do traçado dinâmico no Substance 3D Painter para otimizar a renderização e a capacidade de resposta do traçado de pincel.
helpx_creative_field: ""
helpx_description: Painter > Painting > Dynamic strokes > Dynamic Stroke Performances
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Desempenho de traçado dinâmico
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '995'
ht-degree: 0%

---


# Desempenho de traçado dinâmico

Para Traçados dinâmicos, as performances do gráfico de Substance importam muito porque o Substance pode ser regenerado muitas vezes em um período muito curto. Se um cálculo de Substance for muito pesado, ele pode criar latência e, portanto, gaguejar e congelar ao pintar. Tudo isso pode acabar criando uma experiência de pintura ruim. Esta página agrupa informações e recomendações sobre o uso do recurso Traçado dinâmico.

## A computação de traçados dinâmicos pode ser pesada

Também é importante saber que a computação pode ter um impacto em diferentes contextos:

* **Ao pintar**: o Traçado Dinâmico é gerado (dependendo de suas configurações) durante a pintura. Uma configuração incorreta pode tornar a pintura lenta e demorada.
* **Ao reabrir um projeto**: mesmo que o processo de pintura tenha corrido bem, ainda há uma possibilidade de que o cálculo pare ao abrir um projeto, tornando os projetos muito mais longos do que o normal para serem abertos. Isso ocorre porque o processo de pintura inicial correu bem porque a computação foi espalhada ao longo do tempo, no entanto, acontece quase tudo de uma vez ao abrir um projeto. Isso significa que um projeto poderia solicitar milhares de Substance exclusivos para serem gerados se o Traçado dinâmico não fosse configurado corretamente.
* **Consumo de memória** : gerar muitas variações para um gráfico de Substance pode acabar consumindo muita memória (porque essas gerações são voláteis à medida que são feitas dinamicamente).

## Usar configurações de tremulação e espaçamento

Embora seja fácil implementar efeitos impressionantes ou avançados dentro do próprio Substance, às vezes pode ser mais benéfico mantê-lo simples e usar as configurações nativas dos parâmetros de ferramenta do Substance 3D Painter. Essas configurações são muito mais rápidas de calcular para o mecanismo de pintura:

* **Tremulação**: esses parâmetros permitem criar aleatoriedade a um custo muito baixo, alterando alguns atributos sem recalcular o Substance (como ângulo, posição e opacidade).
* **Espaçamento**: quanto menor o espaçamento, mais carimbos são criados ao pintar um traçado. Às vezes, não há necessidade de um traçado contínuo do pincel e o uso de um espaçamento grande também pode ajudar a ver melhor o alfa/material usado.

## Quando e que tipo de Aleatório usar

A Distribuição Aleatória é uma ótima maneira de gerar singularidade. O problema é que a geração pode ser cara e, no caso do recurso Traçado dinâmico, isso pode acontecer com bastante frequência se não for ajustado corretamente. É importante entender quando usar a Distribuição Aleatória e quando evitá-la, e preferir um método alternativo para obter a melhor relação comercial entre recursos visuais e desempenho :

* **Propagação Aleatória por Carimbo** : neste caso, uma nova geração de Substance exclusivo acontecerá para cada Carimbo. Isso é adequado para criar unhas exclusivas em uma prancha de madeira, por exemplo, mas não se você estiver criando trilhos de tinta/pintura.
* **Propagação Aleatória por Traço**: uma Propagação Aleatória exclusiva é criada para o traçado de pincel atual. Isso é útil ao ter poucos carimbos, mas há a necessidade de um novo conjunto de variações com cada traçado (como um efeito de borrifada).
* **Propagação Aleatória Estática**: o Substance é gerado uma vez e nunca será alterado. Ideal para desempenhos, mas talvez muito restritivo, dependendo das suas necessidades.

E quanto a **Hora** ($time) ?\
O tempo pode ser útil para criar algumas aparências muito específicas, mas na verdade é uma das variáveis mais caras para usar em um gráfico de Substance. O motivo é que é muito difícil obter valores semelhantes de um traçado de pincel para outro, portanto, o mecanismo do pincel provavelmente gerará novas variações o tempo todo. Evite isso se puder, use o espaçamento e o índice de carimbo, que combinados podem levar a resultados semelhantes.

## Uso de StampIndex e StampCycleCount

O **StampIndex** é a identificação de um carimbo individual dentro de um traçado de pincel. Por padrão, começa em 0 e aumenta em 1 para cada novo carimbo. O **StampCycleCount** é uma maneira de limitar a quantidade de índices exclusivos e instrui o Substance 3D Painter a reciclar/reutilizar os gráficos de Substance já gerados. Quando a ID atual atingir o limite, o Substance 3D Painter começará novamente de 0, criando um loop.

A melhor solução para ter aleatoriedade, mantendo bons desempenhos, é, portanto, aproveitar a Contagem de Ciclos com o seguinte:

* **StampIndex como RandomSeed** : ao criar um gráfico de Substance, é possível definir a Distribuição Aleatória como Absoluta. Ao fazer isso, você pode alimentá-lo com um valor personalizado, que pode ser o Índice de carimbo. Isso criará uma versão de gráfico de Substance exclusiva para cada carimbo dentro do traçado.
* **Combinado com StampCycleCount**: você pode criar um conjunto limitado de novas variações e reutilizá-las.
* **Início Aleatório** : se a contagem cíclica for definida para iniciar a partir de um valor aleatório em vez de 0, isso significa que ele usará uma versão de Substance diferente no início para cada traço dentro do pool de gráficos já gerados.

## Desabilitando o cálculo com base em valores de parâmetros

O Substance 3D Painter não pode determinar quando ajustar um parâmetro que pode resultar na mesma saída, simplesmente porque a computação está oculta dentro do gráfico de Substance. Isto é basicamente uma caixa preta.

Para ajudar no desempenho ao ajustar parâmetros e pintar com Traçados dinâmicos, é possível especificar quando novas instâncias de gráfico devem ser geradas usando valores condicionais nos campos userdata do gráfico de Substance.

Os valores possíveis são:

| *Variável* | *Uso* |
| --- | --- |
| **IsStampIndexActive** | Usado para determinar se o índice de carimbo deve ser alterado durante a pintura. |
| **IsRandomSeedActive** | Usado para determinar se a Distribuição aleatória deve mudar durante a pintura. |
| **IsTimeActive** | Usado para determinar se o Tempo ($time) deve ser incrementado durante a pintura. |

Por exemplo:

```
IsRandomSeedActive=input.roundness_jitter>0 || input.flip_x_jitter || input.flip_y_jitter
```


Nesse caso, a semente aleatória será alterada somente se o parâmetro de gráfico (identificador) **arredondamento\_tremulação** for maior que 0 ou se o booleano **inverter\_x\_tremulação** ou **inverter\_y\_tremulação** estiver habilitado. Se a condição não for atendida, o gráfico não será regenerado. Os parâmetros de gráfico devem ser prefixados por &quot; **input.**  &quot; para ser reconhecido.
