---
helpx_url: "https://helpx.adobe.com/br/substance-3d-painter/features/plugins/autosave.html"
breadcrumb-title: ''
description: Saiba como usar o plug-in de Salvamento automático no Substance 3D Painter para salvar automaticamente seus projetos em intervalos regulares.
helpx_creative_field: ""
helpx_description: Painter > Features > Plugins > Autosave
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Salvamento automático
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '375'
ht-degree: 0%

---


# Salvamento automático

![](../../assets/autosave-details.png){width="500px"}

Os plug-ins de salvamento automático permitem **criar backups** do projeto aberto no momento. Isso cria um arquivo na lateral enquanto mantém o projeto atual intacto.

Os arquivos de backup estarão localizados em três locais possíveis:

* Se o projeto atual tiver sido salvo, os backups estarão ao lado dele.
* Se o projeto nunca tiver sido salvo (sem título), os backups estarão na pasta de salvamento automático na pasta Documentos do usuário. ( **Documentos/Allegorítmico/Substance 3D Painter/salvamento automático** )
* Se a configuração de substituição tiver sido habilitada, os backups serão localizados no caminho fornecido nas configurações.

*Um botão de adiamento está disponível na interface para adiar o salvamento automático.*

## Como o salvamento automático é acionado?

O salvamento automático é baseado em um temporizador interno, uma vez que o temporizador esteja sobre o início do processo de salvamento automático.\
O botão de adiamento será ativado quando estiver próximo do final do temporizador, permitindo atrasar o salvamento automático por um certo tempo.

Todos os valores baseados em tempo podem ser modificados por meio da janela de configurações.

## Como desativar o salvamento automático?

Se, por algum motivo, for necessário desativar o processo de salvamento automático, isso poderá ser feito através do menu de plug-ins. Para fazer isso, clique no menu **Plug-ins** > **Salvamento automático** > **Desabilitar**.

## Configurar o Salvamento automático

Para configurar o comportamento de salvamento automático, clique no menu **Plug-ins** > **Salvamento automático** > **Configurar**.

* **Intervalo de salvamento automático em minutos** : indica o tempo de espera entre cada salvamento automático.
* **Número de arquivos de salvamento automático** : a quantidade máxima de arquivos de backup criados para um determinado projeto.
* **Intervalo de adiamento em minutos**: quanto tempo o salvamento automático será adiado ao clicar no botão de adiamento.
* **Tempo de aviso antes de salvar em segundos**: quanto tempo antes do botão de adiamento estar ativo e a barra de progresso estar visível antes do disparador de salvamento automático.

>[!NOTE]
>
> O timer de salvamento automático será pausado se:
> 
> * O mecanismo está fazendo uma computação
> * Texturas estão sendo exportadas
> * A janela de configuração está aberta
> * O projeto está sendo salvo no momento

Na parte inferior da janela é possível substituir o local padrão dos arquivos de backup.\
Quando a configuração &quot; **Sempre salvar no seguinte diretório** &quot; estiver habilitada, todo o arquivo de backup estará localizado na pasta especificada (o caminho padrão é a pasta Documentos do usuário).
