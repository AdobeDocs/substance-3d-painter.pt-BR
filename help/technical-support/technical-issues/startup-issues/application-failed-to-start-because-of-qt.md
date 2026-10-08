---
breadcrumb-title: ""
description: Saiba como corrigir as falhas de inicialização do Substance 3D Painter causadas por problemas na estrutura Qt para a inicialização adequada do aplicativo.
title: O aplicativo falhou ao iniciar devido ao Qt
user-guide-description: ""
user-guide-title: ""
source-git-commit: 6b6d52207ca1d043aaa1b2b14145b6b49d4c1942
workflow-type: tm+mt
source-wordcount: '130'
ht-degree: 0%
---

# O aplicativo falhou ao iniciar devido ao Qt

A seguinte mensagem de erro pode aparecer ao iniciar o aplicativo:

&#x200B;>> 

Este aplicativo falhou ao iniciar porque nenhum plug-in de plataforma Qt pôde ser inicializado. A reinstalação do aplicativo pode corrigir esse problema.

Os plug-ins de plataformas disponíveis são: minimum, offscreen, webgl, windows.

Este erro pode ser gerado porque outra variável de ambiente definida por software está em conflito com o aplicativo.

Certifique-se de remover as seguintes variáveis do ambiente atual antes de iniciar o aplicativo:

```
QT_PLUGIN_PATH 

QML2_IMPORT_PATH
```


>[!NOTE]
>
> Essas variáveis também podem ser herdadas de um contexto Python, por exemplo, com o **pyinstaller**. Certifique-se de removê-los do contexto em que o aplicativo é iniciado.
