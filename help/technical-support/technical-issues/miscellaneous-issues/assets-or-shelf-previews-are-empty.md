---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/technical-support/technical-issues/miscellaneous-issues/assets-or-shelf-previews-are-empty.html"
breadcrumb-title: ''
description: Saiba como corrigir visualizações vazias de ativos e prateleiras no Substance 3D Painter para restaurar a funcionalidade de exibição em miniaturas.
helpx_creative_field: ""
helpx_description: Painter > Technical support > Technical Issues > Miscellaneous Issues > Assets (or shelf) previews are empty
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: As visualizações de ativos (ou prateleiras) estão vazias
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '90'
ht-degree: 0%

---


# As visualizações de ativos (ou prateleiras) estão vazias

Esse problema pode ser causado por outro software, consulte: [Conflitos de software](../startup-issues/software-conflicts.md).

Se for impossível determinar qual atualização/desinstalação de software, procure por uma variável de ambiente chamada “QT\_PLUGIN\_PATH” e remova-a.

**No Windows:**

1. Abra o **Sistema** no Painel de Controle.
1. Na guia Avançado, clique em **Variáveis de Ambiente**
1. Procure a variável chamada **”QT\_PLUGIN\_PATH”**
1. **Remover**
1. **Reiniciar** o computador
