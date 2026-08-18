---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/technical-support/workflow-issues/export-issues/my-exported-opacity-map-is-totally-black.html"
breadcrumb-title: ''
description: Saiba como corrigir mapas de opacidade exportados que aparecem totalmente pretos no Substance 3D Painter para uma exportação de transparência adequada.
helpx_creative_field: ""
helpx_description: Painter > Technical support > Workflow Issues > Export Issues > My exported opacity map is totally black
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Meu mapa de opacidade exportado está totalmente preto
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '117'
ht-degree: 0%

---


# Meu mapa de opacidade exportado está totalmente preto

Quando você cria um novo projeto, a cor padrão vem do sombreador e não das texturas. Portanto, quando você exportar todas as partes que não foram pintadas, elas serão pretas com um valor alfa definido em 0 (porque não existem dados nessas partes).

A maneira mais fácil de corrigir isso é colocar uma camada de preenchimento na parte inferior da sua pilha de camadas: ela preencherá todos os UVs com uma cor padrão, que é idêntica à cor padrão do sombreador.
