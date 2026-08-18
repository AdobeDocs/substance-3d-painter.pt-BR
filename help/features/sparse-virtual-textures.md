---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/features/sparse-virtual-textures.html"
breadcrumb-title: ''
description: Saiba como usar texturas virtuais esparsas no Substance 3D Painter para trabalhar com texturas de resolução ultra-alta de maneira eficiente.
helpx_creative_field: ""
helpx_description: Painter > Features > Sparse Virtual Textures
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Texturas Virtuais Dispersas
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '748'
ht-degree: 0%

---


# Texturas Virtuais Dispersas

![](../assets/svt-header.jpg)

A partir da versão **2018.3**, o Substance 3D Painter usa **Texturas virtuais esparsas** ( **SVT** ) em seu visor em tempo real para gerenciar uma grande quantidade de texturas. Essa tecnologia permite fazer a transmissão contínua de texturas de entrada e saída que são necessárias apenas de um determinado ponto de vista para manter um espaço específico na memória da GPU. Isso melhora o desempenho em projetos com uma grande quantidade de conjuntos de texturas (ou UDIMs).

## Plataformas compatíveis

![](../assets/sparse-settings.png)

Texturas esparsas dependem de uma configuração de hardware específica para serem totalmente executadas. Se a configuração atual não oferecer suporte adequado, o Substance 3D Painter **reverterá** para uma implementação de software (que será menos precisa e de menor desempenho).

É possível forçar o Substance 3D Painter a usar o fallback de software em vez da aceleração de Hardware acessando as [Configurações](../interface/settings/settings.md) .

Estas são as configurações que oferecem suporte às Texturas Virtuais Dispersas aceleradas por hardware:

| Plataforma | Compatível (acelerado por hardware) | Sem suporte (fallback de software) |
| --- | --- | --- |
| **Windows** | <ul data-preserve-html="true"><li data-preserve-html="true">Nvidia GeForce (drivers 411.63 ou superior)</li><li data-preserve-html="true">Nvidia Quadro (Drivers 411.63 ou superior)</li><li data-preserve-html="true">AMD FirePro e Radeon Pro (drivers 18.9.3 ou posteriores) <strong> &#42; </strong></li><li data-preserve-html="true">AMD Radeon (Drivers 18.9.3 ou superior)&#42;</li></ul> | <ul data-preserve-html="true"><li data-preserve-html="true"> Nvidia Quadro M2000 </li><li data-preserve-html="true">  Nvidia Geforce GTX 970 </li><li data-preserve-html="true"> GPUs Intel </li></ul> |
| **SO Mac** | <ul data-preserve-html="true"><li data-preserve-html="true"> Recurso de hardware não suportado pelo sistema operacional </li></ul> | <ul data-preserve-html="true"><li data-preserve-html="true">Qualquer modelo de GPU</li></ul> |
| **Linux** | <ul data-preserve-html="true"><li data-preserve-html="true">Nvidia GeForce (drivers 410.73 ou superior)</li><li data-preserve-html="true">Nvidia Quadro (Drivers 410.73 ou superior)</li><li data-preserve-html="true">AMD FirePro e Radeon Pro (drivers 18.9.3 ou posteriores) <strong> &#42; </strong></li><li data-preserve-html="true">AMD Radeon (Drivers 18.9.3 ou superior)&#42;</li></ul> | <ul data-preserve-html="true"><li data-preserve-html="true">GPU Intel</li></ul> |


* **\***: A aceleração por hardware está desabilitada por padrão e pode ser habilitada manualmente nas [Configurações](../interface/settings/settings.md).

## Por que o Substance 3D Painter está usando texturas virtuais dispersas?

O Substance 3D Painter usa seu mecanismo principal para calcular texturas que são exibidas nas viewports. Isso significa que o mecanismo e o visor precisam compartilhar a memória da GPU (VRam) para computação e exibição dessas texturas. Quanto mais **Conjuntos de Textura** (ou Blocos UV) um projeto contiver, mais memória será necessária para o visor. Se a viewport ocupar muita memória na GPU, o mecanismo principal não terá espaço suficiente para computar texturas e terá que remover texturas na memória do sistema (Ram). Isso resultará em desempenhos ruins e cálculos lentos.

O objetivo do SVT é fazer um orçamento de quanto o visor pode usar na memória da GPU, deixando o máximo de espaço possível para o mecanismo principal realizar cálculos. A vantagem do sistema é que ele também desbloqueia a capacidade de carregar projetos muito maiores no Substance 3D Painter enquanto ainda pode funcionar normalmente.

## Como funcionam as Texturas esparsas?

Texturas virtuais esparsas são um tipo de texturas que não estão completas. Isso significa que o aplicativo carrega apenas partes de texturas na memória. Somente o que é necessário é carregado e o restante é colocado na memória do sistema ou no disco (cache). Quando necessário novamente, as texturas são recuperadas do cache e colocadas de volta na viewport. Para fazer transferências rápidas o sistema conta com **mipmaps** e alterna rapidamente entre diferentes resoluções de textura. É por isso que mover-se rapidamente para a viewport pode exibir inicialmente texturas desfocadas que, em seguida, aumentam na qualidade após alguns segundos.

Para obter mais conhecimento técnico, consulte: [Texturas Virtuais Esparsas](https://silverspaceship.com/src/svt/).

## Local do cache

![](../assets/settings-temp.png)

Quando não houver memória do sistema (Ram) suficiente disponível para armazenar o cache SVT, o Substance 3D Painter mudará para o disco rígido do computador em vez de armazenar o cache.\
O local desse cache é, por padrão, a pasta Operating System Temporary Files (Arquivos temporários do sistema operacional). Este local pode ser alterado acessando as configurações principais do aplicativo, consulte as [Preferências gerais](https://helpx.adobe.com/substance-3d/unlisted/documentation/spdoc/general-71008262.html).

## Compatibilidade com shader

Para tirar o máximo proveito do SVT, os Sombreadores têm que solicitar e ler texturas do sistema Esparso. Portanto, as funções anteriores baseadas em **coordenadas de textura vec2** e **amostradores** foram descontinuadas. As funções auxiliares agora são fornecidas em vez de usar as texturas Esparsas.

Para atualizar os Sombreadores:

* Para **sombreador Substance 3D Painter padrão**: siga o procedimento passo a passo a partir da página [Atualizando um sombreador](../interface/shader-settings/updating-a-shader.md).
* Para **Sombreador personalizado** : dê uma olhada na(s) mensagem(ns) de erro no log, bem como na página [API de sombreamento](https://helpx.adobe.com/substance-3d/unlisted/documentation/spdoc/custom-shader-api-89686018.html).

>[!WARNING]
>
> Projetos mais antigos podem exibir flashes brancos se seus sombreadores não estiverem atualizados. Consulte esta página para obter mais informações: [Mesh flash to white ao mover a câmera](../technical-support/technical-issues/rendering-issues/mesh-flash-to-white-when-moving-camera.md).
