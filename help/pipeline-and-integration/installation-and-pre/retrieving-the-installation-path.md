---
helpx_url: "https://helpx.adobe.com/br/substance-3d-painter/pipeline-and-integration/installation-and-preferences/retrieving-the-installation-path.html"
breadcrumb-title: ''
description: Saiba como recuperar o caminho de instalação do Substance 3D Painter para fins de integração de scripts e pipeline.
helpx_creative_field: ""
helpx_description: Painter > Pipeline and integration > Installation and preferences > Retrieving the installation path
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Recuperação do caminho de instalação
user-guide-description: ''
user-guide-title: ''
source-git-commit: 22871eab2f25d09bd82f1292d8b3e5f8c4f1c2cf
workflow-type: tm+mt
source-wordcount: '259'
ht-degree: 5%

---


# Recuperação do caminho de instalação

Esta página reagrupa informações sobre maneiras de recuperar o caminho de instalação do aplicativo, dependendo da versão e da plataforma.

## Windows

### Creative Cloud para desktop

1. Abra o editor do Registro do Windows (**regedit**).
1. Navegue até a chave de registro: **&#x200B; HKEY\_LOCAL\_MACHINE\Software\Microsoft\Windows\CurrentVersion\App Paths\**
1. Abra a subchave denominada **Adobe Substance 3D Painter.exe**
1. O valor da chave contém o caminho para o executável do aplicativo no qual ela está instalada

>[!NOTE]
>
> Esta chave de registro está disponível somente desde a versão 7.2.\
>  Para versões mais antigas, o caminho de instalação pode ser recuperado das associações de arquivos no **HKEY\_CURRENT\_USER\Software\Microsoft\Windows\CurrentVersion\ Explorer\FileExts**.

### Substance 3D Autônomo

1. Abra o editor do Registro do Windows (**regedit**).
1. Navegue até a chave do Registro: **HKEY\_LOCAL\_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\Uninstall**
1. Localize a subchave correspondente à AppID da versão do seu aplicativo (consulte a tabela abaixo)
1. O valor da chave contém o caminho para o local de instalação do aplicativo

| Versão | AppId |
| --- | --- |
| **Versão 1.x** | `{410F5B6E-A29C-4F43-9DE3-44A1357D6AF5}` |
| **Versão 2.x** | `{f42b7a996fa1d13a1d0a2e33eea2c0800bb5d1b8}` |
| **3.x (2017.x) para 7.1** | `{33C3E9E2-0675-4196-9019-28AB9C5E9BB0}` |
| **7.2 ou mais recente** | `{2a8bbb68-725b-477c-9194-60efc5ece348}` |

### Vapor

O aplicativo está instalado na subpasta **steamapps/common/** da pasta de instalação do Steam.

## Mac

No Mac, o aplicativo é instalado no seguinte:

| Versão | Caminho |
| --- | --- |
| **7.2 ou mais recente** | **/Aplicativos/Adobe Substance 3D Painter.app** |
| **Herdado** | **/Aplicativos/Substance Painter.app** |

## Linux

No Linux, o pacote rpm é instalado no seguinte caminho:

| Versão | Caminho |
| --- | --- |
| **7.2 ou mais recente** | **/opt/Adobe/Adobe\_Substance\_3D\_Painter** |
| **Herdado** | **/opt/Allegorithmic/Substance\_Painter** |
