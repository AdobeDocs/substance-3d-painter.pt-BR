---
breadcrumb-title: ""
description: Saiba como corrigir mapas de opacidade exportados que aparecem totalmente pretos no Substance 3D Painter para uma exportação de transparência adequada.
title: Meu mapa de opacidade exportado está totalmente preto
user-guide-description: ""
user-guide-title: ""
source-git-commit: 6b6d52207ca1d043aaa1b2b14145b6b49d4c1942
workflow-type: tm+mt
source-wordcount: '117'
ht-degree: 0%
---

# Meu mapa de opacidade exportado está totalmente preto

Quando você cria um novo projeto, a cor padrão vem do sombreador e não das texturas. Portanto, ao exportar todas as partes que não foram tintas, elas serão pretas com um valor alfa definido em 0 (porque não existem dados nessas partes).

A maneira mais fácil de corrigir isso é colocar uma camada de preenchimento na parte inferior da pilha de camadas : ela preencherá todos os UVs com uma cor padrão, que é idêntica à cor padrão do sombreador.
