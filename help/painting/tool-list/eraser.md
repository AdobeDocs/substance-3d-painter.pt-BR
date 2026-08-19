---
helpx_url: "https://helpx.adobe.com/br/substance-3d-painter/painting/tool-list/eraser.html"
breadcrumb-title: ''
description: Use a ferramenta Borracha no Substance 3D Painter para remover pintura e texturas de seus modelos 3D com controle de precisão.
helpx_creative_field: ""
helpx_description: Painter > Painting > Tool list > Eraser
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Borracha
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '235'
ht-degree: 1%

---


# Borracha

A Borracha é uma ferramenta de pintura que apaga/oculta o que foi pintado anteriormente por outras ferramentas. Essa ferramenta afeta apenas uma camada por vez.

A Borracha compartilha parâmetros e comportamentos comuns com a ferramenta Pintura. Para saber mais sobre os controles pincel, alfa e estêncil, confira a [página da ferramenta de pintura](paint-brush.md).

>[!NOTE]
>
> Tecnicamente, **a borracha não remove realmente as informações**. Isso simplesmente define a camada alfa de volta a zero, o que apaga/oculta as informações da pintura anterior. Isto significa:
> 
> * Todos os traçados de pincel anteriores que foram pintados ainda são calculados quando um projeto é reaberto antes que os traçados com a borracha sejam aplicados.
> * Um filtro Substance pode recuperar as informações de pintura se ignorar as informações alfa
> 
> É por isso que, às vezes, é mais aconselhável **excluir uma camada e recriá-la** do que usar a borracha, pois ela pode melhorar o desempenho.

## Material

Ao apagar informações, é possível afetar apenas canais específicos.

>[!NOTE]
>
> Ao contrário da ferramenta Pintura, a Borracha só permite definir quais canais serão afetados. Não é possível carregar um recurso da Prateleira para afetar cada canal.

* Se todos os canais estiverem ativados, a borracha removerá as informações dentro de todos os canais:

  ![](../../assets/eraser-all-channels-selection.png)

  ![](../../assets/erase-all-channel-optim.gif){width="325px"}
* Se canais específicos forem selecionados, a borracha removerá informações apenas desses canais:

  ![](../../assets/eraser-one-channel-selection.png)

  ![](../../assets/erase-one-channel-optim.gif){width="325px"}
