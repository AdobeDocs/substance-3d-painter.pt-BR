---
breadcrumb-title: ""
description: Saiba como corrigir problemas de viewport corrompidos ou que não respondem no Ubuntu no Substance 3D Painter para uma renderização 3D adequada.
title: O visor parece quebrado ou não responde no Ubuntu
user-guide-description: ""
user-guide-title: ""
source-git-commit: 6b6d52207ca1d043aaa1b2b14145b6b49d4c1942
workflow-type: tm+mt
source-wordcount: '150'
ht-degree: 0%
---

# O visor parece quebrado ou não responde no Ubuntu

Ao executar o Painter no Steam no Ubuntu a partir da versão 11.1, a viewport poderá parecer quebrada ou não responder.

Isso está relacionado ao Painter não começar com a GPU correta atribuída a ele. No Ubuntu, a GPU integrada em vez da discreta pode acabar sendo selecionada. O Painter herda essa configuração por meio do Steam, o que pode criar problemas.

Existem algumas soluções:

1. Execute o Steam a partir de um Terminal. Isso forçará um contexto diferente e deverá fazer com que o Steam e o Painter sejam executados na GPU correta.
1. Edite o atalho Steam para desabilitar a configuração <b>Executar usando placa gráfica dedicada</b>. Depois, faça o Steam funcionar normalmente.

Para obter mais informações, consulte [este problema do github](https://github.com/ValveSoftware/steam-for-linux/issues/9940).
