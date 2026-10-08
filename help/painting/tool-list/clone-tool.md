---
breadcrumb-title: ""
description: Use a ferramenta Clonar no Substance 3D Painter para copiar detalhes da textura de uma área para outra, proporcionando uma pintura de textura perfeita.
title: Ferramenta Clonar
user-guide-description: ""
user-guide-title: ""
source-git-commit: 6b6d52207ca1d043aaa1b2b14145b6b49d4c1942
workflow-type: tm+mt
source-wordcount: '273'
ht-degree: 1%
---

# Ferramenta Clonar

Introduzida no Substance 3D Painter 2, a ferramenta Clonar compartilha o mesmo tipo de parâmetros que a [ferramenta tinta](https://support.allegorithmic.com/documentation/display/SPDOC/Paint+brush). Como seu nome sugere, a ferramenta clone permite duplicar o conteúdo de uma camada específica ou da pilha de camadas completa de um ponto para outro.

![](../../assets/clone-01.gif)

## Uso

A maneira mais simples de usar a ferramenta Clonar é usá-la no conteúdo de uma camada de pintura.

Isso pode ser feito em duas etapas:

* Selecione o local de origem colocando o mouse no modelo e pressionando a tecla &quot; **V** “.
* Em seguida, posicione o mouse onde a área duplicada será exibida e comece a pintar.

É possível atualizar a origem a qualquer momento pressionando &quot; **V** &quot; novamente.

![](../../assets/2018-06-12-18-11-59.png)

Por padrão, ao pintar com a ferramenta clone, o local de origem seguirá e atualizará seu local depois que o pincel for liberado. Ao desabilitar o botão usado para o &quot; **comportamento da origem do Clonar** “, a origem retornará ao local definido ao pressionar &quot; **V** “. Isso pode ser útil ao pintar várias vezes com a mesma área de origem.

Uma maneira mais inteligente de usar a ferramenta Clonar é criar uma camada de pintura e definir o modo de mesclagem de todos os canais como “Passagem”. Isso permitirá duplicar qualquer informação de uma forma não destrutiva de todas as camadas localizadas abaixo da “camada Clonar”. As camadas abaixo permanecem intactas e quaisquer modificações aplicadas posteriormente serão levadas em conta pela camada Clonar:

![](../../assets/clone-02.gif)
