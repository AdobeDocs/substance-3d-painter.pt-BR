---
helpx_url: "https://helpx.adobe.com/br/substance-3d-painter/technical-support/technical-issues/gpu-issues/forcing-the-external-gpu-on-mac-os.html"
breadcrumb-title: ''
description: Saiba como forçar o Substance 3D Painter a usar a GPU externa no macOS para melhorar o desempenho de renderização.
helpx_creative_field: ""
helpx_description: Painter > Technical support > Technical Issues > GPU Issues > Forcing the external GPU on Mac OS
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Forçar a GPU externa no sistema operacional Mac
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '149'
ht-degree: 0%

---


# Forçar a GPU externa no sistema operacional Mac

No Mac OS Mojave, é possível especificar por aplicativo para usar a GPU externa. O desempenho e a estabilidade do Substance 3D Painter podem melhorar com essa configuração ativada.

Para obter mais informações, consulte a [documentação da Apple](https://support.apple.com/en-us/HT208544).

Para ativá-lo:

1. Feche o Substance 3D Painter se ele já estiver em execução.
1. Selecione o Substance 3D Painter no Finder. Ele pode ser encontrado na pasta **Aplicativos**&#x200B;**.**
1. Pressione **Command-I** ou clique com o botão direito no aplicativo **Substance 3D Painter** e escolha **Obter informações**.
1. Na nova janela, habilite a configuração **Preferir GPU externa**.
1. Reinicie o Substance 3D Painter.

>[!NOTE]
>
> Essa configuração não ficará visível se uma eGPU não estiver conectada ou se a versão atual do MacOS for muito antiga.
