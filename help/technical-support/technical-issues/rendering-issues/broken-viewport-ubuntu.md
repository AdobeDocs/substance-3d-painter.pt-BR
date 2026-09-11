---
helpx_url: "https://helpx.adobe.com/br/substance-3d-painter/technical-support/technical-issues/rendering-issues/broken-viewport-ubuntu.html"
breadcrumb-title: ''
description: Saiba como corrigir problemas de viewport corrompidos ou que não respondem no Ubuntu no Substance 3D Painter para uma renderização 3D adequada.
helpx_creative_field: ""
helpx_description: Viewport appears broken or unresponsive on Ubuntu
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: O visor parece quebrado ou não responde no Ubuntu
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
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
