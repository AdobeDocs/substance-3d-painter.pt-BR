---
breadcrumb-title: ""
description: Saiba como corrigir problemas de reconhecimento de GPU que aparecem como genérico GDI no Substance 3D Painter para a aceleração adequada da GPU.
title: A GPU não é reconhecida e é mencionada como GDI genérica
user-guide-description: ""
user-guide-title: ""
source-git-commit: 6b6d52207ca1d043aaa1b2b14145b6b49d4c1942
workflow-type: tm+mt
source-wordcount: '134'
ht-degree: 0%
---

# A GPU não é reconhecida e é mencionada como GDI genérica

Esse problema é um pouco complicado de controlar e pode ser causado por várias fontes:

* Se você estiver em um computador com Nvidia Optimus, consulte o seguinte link: [GPU não reconhecida](gpu-is-not-recognized.md)
* Verifique se o monitor está conectado à GPU principal (e se no Windows esse monitor está definido como a tela principal)
* Verifique se a profundidade de bits de cores do vídeo principal está definida como 32 bits no Windows
* Se você ainda tiver problemas, tente uma reinstalação limpa dos drivers da GPU (desinstalação completa com a limpeza dos itens restantes no registro do Windows).
