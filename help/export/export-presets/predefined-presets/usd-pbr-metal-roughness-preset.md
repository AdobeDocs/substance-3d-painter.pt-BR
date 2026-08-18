---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/getting-started/export/export-presets/predefined-presets/usd-pbr-metal-roughness-preset.html"
breadcrumb-title: ''
description: Saiba como usar a predefinição de exportação USDz (Apple AR) no Substance 3D Painter para exportar texturas para fluxos de trabalho do Apple AR.
helpx_creative_field: ""
helpx_description: Painter > Getting Started > Export > Export presets > Predefined Presets > USDz (Apple AR) Preset
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: USDz (Apple AR)
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '220'
ht-degree: 0%

---


# Modelo predefinido de USDz (Apple AR)

>[!NOTE]
>
> Para exportar para USD com um Modelo de saída personalizado, não use o modelo USDz (Apple AR). Em vez disso, use o Modelo de saída escolhido e habilite <b>Exportar ativo do USD</b> na parte inferior da <b>guia Configurações</b>.

O modelo de saída predefinido USDz (Apple AR) exporta seu ativo configurado para uso com aplicativos Apple AR.

Para usar o modelo USDz (Apple AR):

1. Abra a janela de Exportação com <b>Arquivo > Exportar texturas</b> ou com o atalho de teclado <b>Ctrl + Shift + E</b>.
1. Na <b>guia Configurações</b>, abra o <b>menu suspenso Modelo de saída</b> e selecione <b>USDz (Apple AR)</b>.

![Uma imagem da janela de exportação mostrando o menu suspenso modelo de saída aberto e USDz (Apple AR) selecionado.](../../../assets/export-usd.png){zoomable="yes"}

Cinco arquivos de textura são criados e salvos (cor base, metálico, normal, oclusão e aspereza). Todos os arquivos são salvos como JPG, exceto o mapa normal, que é salvo como PNG para evitar artefatos devido à compactação com perdas.

Além disso, dois outros arquivos são criados com a extensão usdc e usdz:

Aqui está um exemplo do JadeToad aberto diretamente no MacOS a partir do Finder:

![](../../../assets/usdz.png){width="400px"}

Aqui está um exemplo do arquivo USDZ enviado para um iPhone, usando o modo AR para colocar o modelo JadeToad em um ambiente real:

![](../../../assets/3d-usdz.jpg){width="500px"}
