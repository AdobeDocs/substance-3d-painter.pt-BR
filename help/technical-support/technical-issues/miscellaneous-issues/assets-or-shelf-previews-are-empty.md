---
breadcrumb-title: ""
description: Saiba como corrigir visualizações vazias de ativos e prateleiras no Substance 3D Painter para restaurar a funcionalidade de exibição em miniaturas.
title: As visualizações de ativos (ou prateleiras) estão vazias
user-guide-description: ""
user-guide-title: ""
source-git-commit: 6b6d52207ca1d043aaa1b2b14145b6b49d4c1942
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
