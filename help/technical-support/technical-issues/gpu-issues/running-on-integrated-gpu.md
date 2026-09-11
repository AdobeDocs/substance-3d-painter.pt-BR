---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/technical-support/technical-issues/gpu-issues/running-on-integrated-gpu.html"
breadcrumb-title: ''
description: Saiba como configurar o Substance 3D Painter para usar GPU dedicada em vez de gráficos integrados para melhor desempenho.
helpx_creative_field: ""
helpx_description: Painter > Technical support > Technical Issues > GPU Issues > Running on integrated GPU
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Execução em GPU integrada
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '157'
ht-degree: 0%

---


# Execução em GPU integrada

![](../../../assets/integrated-gpu.png){width="500px"}

Pode acontecer de alguns computadores serem configurados por padrão para serem executados em um chipset integrado em vez de em uma GPU dedicada.\
Como o desempenho no chipset integrado é muito baixo, recomendamos usar uma GPU dedicada. Uma janela pop-up pode ser exibida e o avisará sobre isso.

Com uma GPU NVIDIA, a mudança para a GPU NVIDIA depende dos perfis de aplicativos. Se um aplicativo não tiver esse perfil, você poderá atribuir a placa de vídeo manualmente:

1. Clique com o botão direito do mouse na Área de trabalho e selecione Painel de Controle NVIDIA **ou** Navegue até o Painel de Controle e procure por Painel de Controle NVIDIA
1. Em **Configurações 3D**, vá para **Gerenciar configurações 3D**
1. Na guia **Configurações do programa**, adicione um novo perfil para o **Substance 3D Painter**
1. Altere a configuração do processador gráfico preferido para Processador de alto desempenho NVIDIA
