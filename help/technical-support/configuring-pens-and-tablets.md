---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/technical-support/configuring-pens-and-tablets.html"
breadcrumb-title: ''
description: Saiba como configurar canetas e tablets no Substance 3D Painter para obter a sensibilidade à pressão e a experiência de desenho ideais.
helpx_creative_field: ""
helpx_description: Painter > Technical support > Configuring Pens and Tablets
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Configuração de Canetas e Tablets
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '877'
ht-degree: 0%

---


# Configuração de Canetas e Tablets

Esta página lista várias recomendações para configurar uma caneta gráfica tablet no Windows, a fim de melhorar a sua compatibilidade com o aplicativo.

## O que é o Windows Ink?

O Windows Ink é um software/serviço que lida com canetas, como canetas digitalizadoras ou canetas de tablets gráficos. Ele oferece vários aplicativos, como Notas Autoadesivas e Sketchpad, para interagir com uma caneta no computador.

Desde a versão 2019.3, o aplicativo se baseia nele para lidar com tablets gráficos. Antes desta versão, Wintab foi usado (serviço mais antigo que não é suportado por todos os modelos de tablets gráficos).

## Ativação do Windows Ink nas configurações do driver do Tablet

Para garantir que a pressão da caneta seja reconhecida corretamente, a Tinta do Windows deve ser ativada nas configurações do driver do Tablet gráfico.

>[!NOTE]
>
> Não há suporte para o Windows Ink em máquinas virtuais, portanto, os eventos de tablet gráfico não serão encaminhados para o aplicativo. Portanto, a pressão da caneta não é suportada nessa configuração.

### Ativação do Windows Ink para tablets Wacom

1. Abra o menu **Iniciar**.
1. Digite **Propriedades do tablet Wacom** e clique no primeiro resultado da pesquisa.
1. Na janela **Propriedades do tablet Wacom**, clique na **Caneta** da lista de ferramentas.\
   ![](../assets/wacom-tool-pen.png)
1. Clique no botão de adição **”+”** para adicionar um perfil de aplicativo.\
   ![](../assets/wacom-profile-plus.png)
1. Clique no botão **Procurar** na nova janela para localizar o executável do Substance 3D Painter.\
   ![](../assets/wacom-profile-browse.png)
1. Clique em **OK** para validar e criar o perfil.\
   ![](../assets/wacom-profile-sp.png)
1. Clique na guia **Mapeamento**.\
   ![](../assets/wacom-tab-mapping.png)
1. Na parte inferior esquerda da janela, verifique se a opção **Usar Windows Ink** está habilitada.\
   ![](../assets/wacom-use-windows-ink.png)

>[!NOTE]
>
> Depois de ativar o Windows Ink, reinicie o aplicativo para garantir que as alterações sejam levadas em consideração corretamente.

### Ativação do Windows Ink para tablets Huion

1. Abra o menu **Iniciar**.
1. Digite **Huion Tablet** e clique no primeiro resultado da pesquisa
1. Na janela **Huion Tablet**, clique em **Caneta Digital**.\
   ![](../assets/huion-pen-settings.png)
1. Na parte inferior esquerda da janela, verifique se a opção **Habilitar Windows Ink** está habilitada.\
   ![](../assets/huion-pen-winink.png)

## Como acessar as configurações do Windows Ink

As configurações do Windows Ink podem ser acessadas nas configurações gerais do Windows:

1. Abra o menu **Iniciar**.
1. Clique no ícone **Configurações**.\
   ![](../assets/setting-menu-start.png)
1. Na janela Configurações, clique em **Dispositivos**.\
   ![](../assets/settings-device.png)
1. Na janela **Dispositivos**, clique em **Caneta e Tinta do Windows** (disponível somente se um tablet gráfico estiver conectado).\
   ![](../assets/setting-pen-windows-ink.png)

## Configurações recomendadas do Windows Ink

Abaixo estão as configurações do Windows Ink e as configurações recomendadas para cada uma delas.

>[!NOTE]
>
> Mesmo depois de seguir este guia, alguns elementos visuais relacionados ao Windows Ink ainda ficarão visíveis. Infelizmente, o Microsoft não oferece configurações no Windows para desativá-las.
> 
> Os visuais restantes são:
> 
> * **Círculo** ao clicar com o botão direito.
> * **Dica de ferramenta** abaixo do mouse ao pressionar um modificador de tecla (Ctrl, Alt ou Shift).

### Configurações da Caneta

![](../assets/ink-settings-main.png)

| ***Configuração*** | ***Descrição*** |
| --- | --- |
| **Escolha com qual mão escrever** | Recomendado: **Mão direita** Estas configurações controlam como a orientação da caneta é reconhecida. Definir essa configuração como Mão esquerda pode fazer com que a interface do usuário congele ao ajustar os parâmetros. |
| **Mostrar efeitos visuais** | Recomendado: **Desabilitado** essas configurações controlam os efeitos visuais que são exibidos durante várias interações da Caneta. Desativá-la permite ocultar o efeito de círculo de ondulação ao clicar em: <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r2-column-c1_dynamic_grid_items_grid-cell_position-par_image" src="../assets/windows-pen-ripple-circle.jpg"/></div> |
| **Mostrar cursores** | Recomendado: **Desabilitado** |
| **Deixe-me usar minha caneta como mouse em alguns aplicativos de desktop** | Recomendado: **Habilitado** Essa configuração permite que a caneta eletrônica gráfica envie entradas regulares do mouse. Se desativada, essa configuração pode levar a alguns problemas de interação com parâmetros de interface. |

### Configurações de Manuscrito

![](../assets/ink-settings-handwriting.png)

| ***Configuração*** | ***Descrição*** |
| --- | --- |
| **Tamanho da fonte ao gravar diretamente no campo de texto** | Recomendado: **Médio (padrão)** |
| **Fonte ao usar manuscrito** | Recomendado: **Segoe UI (padrão)** |
| **Ao tocar em um campo de texto com a caneta, use a escrita manual para inserir o texto** | Recomendado: **Somente no modo tablet** Esta configuração controla como e quando a janela de entrada de texto manuscrito é exibida. Se não estiver definido como “somente no modo tablet”, a janela aparecerá sempre que um campo de texto for selecionado na interface do usuário. Por exemplo, ao digitar um valor específico em um controle deslizante. |
| **Deixe-me usar minha caneta como mouse em alguns aplicativos de desktop** | Recomendado: **Habilitado** Essa configuração permite que a caneta eletrônica gráfica envie entradas regulares do mouse. Se desativada, essa configuração pode levar a alguns problemas de interação com parâmetros de interface. |
| **Escreva com a ponta dos dedos no painel de manuscrito** | Recomendado: **Desabilitado** |

### Configurações de atalhos de caneta

![](../assets/ink-settings-pen.png)

| ***Configuração*** | ***Descrição*** |
| --- | --- |
| **Clique uma vez** | Recomendado: **Nada** |
| **Clique duas vezes** | Recomendado: **Nada** |
| **Mantenha pressionado (apenas algumas canetas são compatíveis)** | Recomendado: **Nada** |
| **Permitir que os aplicativos substituam o comportamento do botão de atalho** | Recomendado: **Habilitado** |
| **Quando disponível, mostrar Espaço de Trabalho de Tinta após eu remover minha caneta do armazenamento** | Recomendado: **Desabilitado** |

## Como acessar as configurações de Caneta e Toque

As configurações de Caneta e Toque podem ser acessadas no Painel de controle:

1. Abra o menu **Iniciar**.
1. Digite **Painel de Controle** e clique no primeiro resultado da pesquisa.
1. Alterne o **modo de exibição** do Painel de Controle para **ícone pequeno**.\
   ![](../assets/control-panel-display-mode.png)
1. Clique nas configurações de **Caneta e Toque**.\
   ![](../assets/control-panel-pen-touch-settings.png)

## Configurações recomendadas de Caneta e Toque

As configurações a seguir são recomendadas para melhorar o comportamento de pintura e a manipulação da câmera.

Para acessar as configurações, clique em uma das **ações de caneta** da janela e clique no botão **configurações**.

![](../assets/control-panel-settings.png)

| ***Configuração*** | ***Descrição*** |
| --- | --- |
| **Toque único** | Nenhum parâmetro. |
| **Toque duas vezes** | Recomendado: **Valores padrão.** |
| **Mantenha pressionado** | Recomendado: **Desabilitar a configuração”Habilitar pressionar e manter pressionado para clicar com o botão direito do mouse”** A desabilitação dessa configuração permitirá arrastar qualquer elemento normalmente sem ativar o círculo de arrastar do Windows: <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table1_row-r3-column-c1_dynamic_grid_items_grid-cell_position-par_image" src="../assets/windows-pen-drag-circle.jpg"/></div> |
| **Usar o botão da caneta como um equivalente do clique com o botão direito** | Recomendado: **Habilitado** |
| **Use a parte superior da caneta para apagar tinta (quando disponível)** | Recomendado: **Habilitado** |
