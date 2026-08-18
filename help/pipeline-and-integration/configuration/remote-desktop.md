---
helpx_url: "https://helpx.adobe.com/br/substance-3d-painter/pipeline-and-integration/configuration/remote-desktop.html"
breadcrumb-title: ''
description: Saiba como configurar o Substance 3D Painter para acesso remoto ao desktop para habilitar fluxos de trabalho e colaboração remotos.
helpx_creative_field: ""
helpx_description: Painter > Pipeline and integration > Configuration > Remote Desktop
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Área de Trabalho Remota
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '395'
ht-degree: 0%

---


# Área de Trabalho Remota

Esta página descreve soluções e alternativas para permitir que o Substance 3D Painter seja executado por meio da Área de trabalho remota (RDP) no Windows.

Por padrão, o RDP no Windows é executado em um contexto OpenGL inexistente ou muito baixo, o que torna o aplicativo incapaz de funcionar corretamente ou falha. O Substance 3D Painter requer um contexto OpenGL 3.3. Veja a seguir as soluções para atenuar o problema, mas não há garantias de que elas funcionarão, pois o problema inicial depende do Windows e de alguns drivers de GPU.

>[!NOTE]
>
> As GPUs Nvidia Quadro podem executar o aplicativo no modo RDP por padrão, enquanto as GPUs Nvidia GeForce fornecem apenas um contexto OpenGL 1.4 (muito baixo para o Substance 3D Painter). É possível instalar um executável para corrigir isso, consulte: <https://developer.nvidia.com/designworks>

## Configuração da Política do Windows

No Windows 10 pode ser necessário alterar a **Política de Grupo** para permitir que a GPU seja executada enquanto estiver no modo RDP.

Para fazer isso:

1. Pressione **Win + R** para abrir a janela de execução
1. Digite &quot; **gpedit.msc** &quot; e digite Enter
1. Navegue até **Política de Computador Local\Configuração do Computador\Modelos Administrativos\Componentes do Windows\Serviços de Área de Trabalho Remota\Host da Sessão da Área de Trabalho Remota\Ambiente de Sessão Remota**
1. Habilite a opção **Usar o adaptador gráfico padrão de hardware para todas as sessões dos Serviços de Área de Trabalho Remota**.

## comando TSCON do Windows

Se a alteração de Política anterior não funcionar, você pode tentar usar a linha de comando **tscon**. Este comando desconecta o computador remoto e conecta um novo ao hardware físico (mouse, teclado, etc.). Em seguida, simplesmente executar o aplicativo e reconectar remotamente deve permitir o trabalho com o aplicativo na GPU.

1. Pressione a tecla **Windows+R** para abrir a janela **executar**.
1. Digite **cmd** e pressione **Enter**.
1. No tipo de linha de comando e no seguinte comando: **tscon 1 /dest:console**
1. Pressione Enter
1. Na linha de comando, digite o próximo comando: **start “Path/To/Substance/Painter/Folder/Substance 3D Painter.exe”** (certifique-se de alterar o caminho para que corresponda ao seu computador)
1. Pressione Enter

Após essas etapas, aguarde alguns segundos para permitir que o aplicativo seja inicializado e, em seguida, reconecte-se à sua sessão.

Talvez seja necessário executar a linha de comando do Windows no modo de administrador caso esse procedimento não funcione.

## Alternativas

Se as sugestões anteriores ainda não funcionarem, recomendamos o uso de soluções alternativas, como VNC ou Teamviewer, que ofereçam suporte à GPU por meio de conexões remotas.
