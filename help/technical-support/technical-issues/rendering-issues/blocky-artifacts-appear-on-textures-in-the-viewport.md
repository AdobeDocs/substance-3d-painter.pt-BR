---
breadcrumb-title: ""
description: Saiba como corrigir artefatos de blocos que aparecem no textura no visor do Substance 3D Painter para uma qualidade visual limpa.
title: Artefatos de blocos aparecem nas texturas da viewport
user-guide-description: ""
user-guide-title: ""
source-git-commit: 6b6d52207ca1d043aaa1b2b14145b6b49d4c1942
workflow-type: tm+mt
source-wordcount: '194'
ht-degree: 0%
---

# Artefatos de blocos aparecem nas texturas da viewport

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
