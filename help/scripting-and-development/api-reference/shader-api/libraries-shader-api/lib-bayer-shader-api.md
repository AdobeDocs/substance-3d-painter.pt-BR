---
breadcrumb-title: ""
description: Acesse a referência da API de sombreamento Lib Bayer para o Substance 3D Painter para criar padrões de pontilhamento Bayer em sombreadores personalizados.
title: Lib Bayer - API de sombreamento
user-guide-description: ""
user-guide-title: ""
source-git-commit: 6b6d52207ca1d043aaa1b2b14145b6b49d4c1942
workflow-type: tm+mt
source-wordcount: '32'
ht-degree: 0%
---

# Lib Bayer - API de sombreamento

## lib-bayer.glsl

**Funções Públicas:** *bayerMatrix8*

```
float bayerMatrix8(uvec2 coords) { 

  return (float(bayer(coords.x, coords.y)) + 0.5) / 64.0; 

} 

 
```
