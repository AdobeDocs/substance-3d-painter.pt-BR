---
breadcrumb-title: ""
description: Saiba como corrigir faces de malha que desaparecem quando vistas de trás na viewport do Substance 3D Painter para uma visibilidade de malha adequada.
title: Os rostos de malha desaparecem ao olhar para eles por trás
user-guide-description: ""
user-guide-title: ""
source-git-commit: 6b6d52207ca1d043aaa1b2b14145b6b49d4c1942
workflow-type: tm+mt
source-wordcount: '86'
ht-degree: 0%
---

# Os rostos de malha desaparecem ao olhar para eles por trás

Por padrão, as malhas no visor podem não exibir a parte de trás dos polígonos de malha (face de fundo). Isso ocorre porque eles são eliminados pelo sombreador atual.

Para exibir a parte de trás dos rostos, basta alterar o sombreador atual para **pbr-metal-rough-alpha-test** nas [configurações de Sombreador](../../../interface/shader-settings/shader-settings.md).
