---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/technical-support/technical-issues/startup-issues/software-conflicts.html"
breadcrumb-title: ''
description: Saiba como resolver conflitos de software que impedem que o Substance 3D Painter seja iniciado corretamente no sistema.
helpx_creative_field: ""
helpx_description: Painter > Technical support > Technical Issues > Startup Issues > Software conflicts
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Conflitos de software
user-guide-description: ''
user-guide-title: ''
source-git-commit: 22871eab2f25d09bd82f1292d8b3e5f8c4f1c2cf
workflow-type: tm+mt
source-wordcount: '681'
ht-degree: 0%

---


# Conflitos de software

Esta página contém uma lista de problemas conhecidos com outros softwares que podem travar ou impedir a execução correta do Substance 3D Painter.

| *Fonte potencial de conflito* | *Problema* |
| --- | --- |
| **Antivírus/Anti-Spyware** | O software antivírus ou antisspyware pode criar alguns dos seguintes problemas:<ul data-preserve-html="true"> <li data-preserve-html="true"><b> Falso positivo</b>: o Painter está sinalizado incorretamente como um vírus ou malware.</li> <li data-preserve-html="true"><b> Arquivos bloqueados</b>: o Painter não pode ler ou gravar arquivos (exportação, criação de predefinição etc.).</li> <li data-preserve-html="true"><b> Exclusão de arquivo</b>: o Painter não pode iniciar ou funcionar normalmente porque os arquivos necessários foram removidos.</li> </ul>Se uma dessas situações surgir, recomendamos desativar temporariamente o antivírus para ver se ele ajuda ou adicionar exceções manualmente ao Painter. |
| **AMD CrossFire e NVIDIA SLI** | Várias configurações de GPU não são compatíveis com o Painter, levando a falhas. Recomendamos desativar esse recurso. |
| <b> Assistente da Autodesk </b> | O aplicativo do assistente da Autodesk pode criar conflitos e fazer com que o aplicativo trave na inicialização ou ao abrir um arquivo de projeto. Atualize o aplicativo da Autodesk para resolver o problema. |
| <b> Alienware/Computadores Dell</b> | Consulte esta página para obter mais informações: [Falha ao abrir ou salvar um arquivo](../stability-issues/crash-when-opening-or-saving-a-file.md). |
| **APFS pelo Software Paragon** | Este software pode registrar um local na variável de ambiente Caminho do Windows que pode travar o aplicativo na inicialização. A desinstalação do software pode não ser suficiente e a variável de ambiente pode precisar ser removida manualmente. Exemplo de local problemático: `C:Program Files (x86)Paragon SoftwareAPFS for Windowsï–›éŒ à €è¸€ì‡ì‡ç¿¹` |
| **Avecto** | Ter uma versão mais antiga do Avecto em execução pode causar lentidão e falhas. Certifique-se de atualizá-la para a versão mais recente. |
| **Ajuste da GPU Asus** | Esse software pode causar problemas durante a compilação de shaders no Substance 3D Painter ou até mesmo impedir o início da compilação de shader. Se esse problema for encontrado, recomendamos desinstalar o software para ver se ele corrige o problema. |
| **Asus RAMCache** | Esse software pode impedir que o Substance 3D Painter seja iniciado corretamente ou torná-lo instável durante a execução. Recomendamos desativar ou instalar o Asus RAMCache se você estiver com problemas de estabilidade. |
| **Asus Sonic Suite** | Em computadores com uma placa-mãe ASUS, o <b>Asus Sonic Suite</b> pode estar instalado por padrão. A desinstalação deste software pode corrigir alguns problemas de exibição/interface no Substance 3D Painter. |
| **Software de Backup na Nuvem** **(** OneDrive,**GDrive,** **Dropbox,** **Filestream etc.)** | O software de backup em nuvem pode ser a origem de várias falhas ao salvar um projeto. Se isso acontecer, é recomendável trabalhar e salvar o arquivo de projeto em uma pasta não sincronizada e, em vez disso, copiar os arquivos de projeto de volta na unidade na nuvem assim que as alterações não forem mais feitas. |
| **Chitubox** | Este software pode criar um conflito e travar o aplicativo ao abrir uma caixa de diálogo de arquivo (como abrir ou salvar um projeto). Você pode desabilitar a configuração <b>Habilitar visualização em miniatura do modelo de área de trabalho</b> nas preferências da Caixa de Texto para evitar esse problema. |
| **Exibição do Dueto** | O <b>Duet Display</b> é conhecido por criar problemas de drivers de GPU que podem afetar o comportamento do Substance 3D Painter. É recomendável desinstalá-lo. |
| **Google Chrome** | O Google Chrome pode causar algumas falhas ao ser executado com o Substance 3D Painter. Para melhorar a estabilidade do Substance 3D Painter, é recomendável atualizar o Google Chrome e os drivers de GPU. Se ainda ocorrerem falhas, desative a Aceleração de hardware no Google Chrome (que impedirá o Chrome de usar a GPU). |
| **Software de áudio nahimic** | O <b>Nahimic</b> pode congelar ou travar o Painter. Pará-lo pode ajudar, e atualizá-lo também pode evitar problemas. O Nahimic também executa serviços em segundo plano que podem interferir no aplicativo e podem precisar ser interrompidos ou desativados. |
| **Software de Vídeo Openshot** | O <b>Software de Vídeo Openshot</b> pode criar um conflito com o Substance 3D Painter com as visualizações da prateleira. Atualizar o Openshot deve corrigir o problema. |
| **Instalador** | Este aplicativo pode produzir uma configuração de ambiente incorreta, levando a um erro na inicialização. Para obter mais informações, consulte [Falha ao iniciar o aplicativo devido ao Qt](application-failed-to-start-because-of-qt.md). |
| **Rptr/Plays.tv** | O <b>Rptr</b> (ou <b>[Plays.tv](http://plays.tv/) </b>) é instalado por padrão com alguns drivers de GPU. Este software pode criar instabilidades e travar o aplicativo. É recomendável desinstalar o aplicativo. |
| **RGBFusion** | Esse software pode criar conflitos com drivers de tablet gráfico, interromper o processo pode corrigir temporariamente o problema ou desinstalar o RGBFusion para uma correção permanente. |
