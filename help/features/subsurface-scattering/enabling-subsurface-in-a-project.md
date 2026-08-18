---
helpx_url: "https://helpx.adobe.com/br/substance-3d-painter/features/subsurface-scattering/enabling-subsurface-in-a-project.html"
breadcrumb-title: ''
description: Saiba como ativar a dispersão superficial em projetos do Substance 3D Painter para criar efeitos de material translúcido realistas.
helpx_creative_field: ""
helpx_description: Painter > Features > Subsurface Scattering > Enabling Subsurface in a Project
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Ativando o Subsurface em um projeto
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '267'
ht-degree: 0%

---


# Ativando o Subsurface em um projeto

Para ativar corretamente a dispersão da subsuperfície no Substance 3D Painter, alguns parâmetros precisam ser definidos primeiro.\
Esta página fornece um guia sobre os parâmetros a serem ativados.

## 1 - Configurações do conjunto de textura

No [Conjunto de Texturas](../../interface/texture-set/texture-set.md), adicione um canal de **Dispersão** se ainda não estiver presente:

![](../../assets/add-channel.png)

>[!NOTE]
>
> O canal de dispersão funciona como uma **máscara** sobre a **superfície**: se o canal for preto, não haverá subsuperfície nenhuma, enquanto se for branco, a intensidade da subsuperfície será no máximo. Este canal é um valor em tons de cinza que é **preto por padrão**. Adicione uma camada de preenchimento na pilha de camadas para controlar a cor padrão ou use uma camada de pintura para controlar manualmente a intensidade.

## 2 - Configuração de Subsuperfície Global

Habilite a configuração principal de dispersão da subsuperfície nas [Configurações de exibição](../../interface/display-settings/display-settings.md) (abaixo das configurações de Pós-Efeitos):

![](../../assets/enable-subsurface.png)

>[!NOTE]
>
> Ativar/desativar o efeito Subsuperfície afeta o projeto inteiro. Pode ser útil usar esse parâmetro global se ele for muito pesado em termos de desempenho.

## 3 - Configurações do sombreador

![](../../assets/shader-parameters.png)

Na janela [Configurações do sombreador](../../interface/shader-settings/shader-settings.md) com sombreadores padrão, pode ser encontrado um grupo &quot; **Parâmetros SSS**” com duas configurações.\
Altere a escala e a cor para ajustar o material de destino. Para obter mais detalhes sobre essas configurações, consulte: [Parâmetros da Subsuperfície](subsurface-parameters.md)

## Bônus : Ativando sombras

O efeito de dispersão da subsuperfície funciona bem, mas pode parecer estranho, se estiver sozinho.\
Ativar a sombra pode ajudar na aparência final do visor e melhorar o realismo do material final.

Na janela [Configurações do ambiente](../../interface/display-settings/environment-settings.md), habilite a configuração &quot; **Sombras** “:

![](../../assets/shadow-2.png)
