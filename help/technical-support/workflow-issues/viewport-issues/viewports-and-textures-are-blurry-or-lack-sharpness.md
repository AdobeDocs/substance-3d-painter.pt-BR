---
breadcrumb-title: ""
description: Saiba como corrigir viewports e texturas desfocadas no Substance 3D Painter para garantir uma qualidade visual nítida e clara.
title: Os viewports e as texturas estão desfocados ou não possuem nitidez
user-guide-description: ""
user-guide-title: ""
source-git-commit: 6b6d52207ca1d043aaa1b2b14145b6b49d4c1942
workflow-type: tm+mt
source-wordcount: '137'
ht-degree: 1%
---

# Os viewports e as texturas estão desfocados ou não possuem nitidez

As viewports podem parecer desfocadas por diferentes motivos.

## Configurações de telas de alto DPI (retina)

Por padrão, o Substance 3D Painter reduz a resolução da viewport na tela High-DPI/Retina para melhorar o desempenho.

Este comportamento pode ser alterado nas [configurações principais](https://helpx.adobe.com/br/substance-3d/unlisted/documentation/spdoc/general-71008262.html) alterando o parâmetro **Escala de Visor**.

## Filtragem de textura

As viewports usam mipmaps e filtragem de textura para serem capazes de fazer stream de e para [Texturas Virtuais Esparsas](../../../features/sparse-virtual-textures.md) para melhorar o desempenho. Isso pode levar a texturas desfocadas em alguns casos.

A filtragem de textura pode ser ajustada pela janela Configurações de Exibição nos parâmetros [Configurações de Visor](../../../interface/display-settings/viewport-settings.md).
