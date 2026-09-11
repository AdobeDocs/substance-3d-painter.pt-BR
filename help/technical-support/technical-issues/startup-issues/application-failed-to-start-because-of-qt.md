---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/technical-support/technical-issues/startup-issues/application-failed-to-start-because-of-qt.html"
breadcrumb-title: ''
description: Saiba como corrigir as falhas de inicialização do Substance 3D Painter causadas por problemas na estrutura Qt para a inicialização adequada do aplicativo.
helpx_creative_field: ""
helpx_description: Painter > Technical support > Technical Issues > Startup Issues > Application failed to start because of Qt
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: O aplicativo falhou ao iniciar devido ao Qt
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '130'
ht-degree: 0%

---


# O aplicativo falhou ao iniciar devido ao Qt

A seguinte mensagem de erro pode aparecer ao iniciar o aplicativo:

>> 

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
