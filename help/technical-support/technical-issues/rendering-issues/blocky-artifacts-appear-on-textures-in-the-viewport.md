---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/technical-support/technical-issues/rendering-issues/blocky-artifacts-appear-on-textures-in-the-viewport.html"
breadcrumb-title: ''
description: Saiba como corrigir artefatos de blocos que aparecem em texturas no visor do Substance 3D Painter para obter uma qualidade visual limpa.
helpx_creative_field: ""
helpx_description: Painter > Technical support > Technical Issues > Rendering Issues > Blocky artifacts appear on textures in the viewport
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Artefatos de blocos aparecem em texturas na viewport
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '194'
ht-degree: 0%

---


# Artefatos de blocos aparecem em texturas na viewport

A partir da versão 2018.3.0, os seguintes tipos de artefatos podem aparecer no visor:

![](../../../assets/viewport-artifacts.jpg){width="400px"}

Esses artefatos estão relacionados a problemas com drivers de GPU Nvidia.\
Para evitar os artefatos, o suporte de hardware Texturas Virtuais Esparsas precisa ser desativado.

Os **Drivers 440.97** da GeForce agora **corrigiram esse problema**. Recomendamos atualizar para esses drivers e manter a SVT ativada para obter bons desempenhos.

Novos drivers estão disponíveis no site da Nvidia: <https://www.nvidia.com/Download/index.aspx>

## Desativando a aceleração de Hardware de Texturas Virtuais Dispersas

### 1 - Inicie o Substance 3D Painter e abra as Configurações

![](../../../assets/settings-34.png)

Abra as Configurações principais em Editar > Configurações.

### 2 - Localize a seção denominada “Texturas virtuais dispersas”

![](../../../assets/svt-subsection.png)

Dentro da seção “Geral”, role para baixo e encontre a subseção chamada “Texturas virtuais esparsas”

### 3 - Desmarque a configuração

![](../../../assets/uncheck-hardware.png)

Desative a configuração “Aceleração do suporte de hardware” desmarcando-a.

### 4 - Validar e reiniciar o Substance 3D Painter

![](../../../assets/validate-1.png)

Valide a alteração clicando no botão “OK”.

![](../../../assets/restart-3.png)

Reinicie o Substance 3D Painter clicando no botão “Sim” para aplicar a alteração.
