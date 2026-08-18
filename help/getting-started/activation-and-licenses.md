---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/getting-started/activation-and-licenses.html"
breadcrumb-title: ''
description: Saiba como ativar e gerenciar licenças do Substance 3D Painter para começar a usar o aplicativo para pintura de textura.
helpx_creative_field: ""
helpx_description: Painter > Getting Started > Activation and licenses
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Ativação e licenças
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '482'
ht-degree: 1%

---


# Ativação e licenças

Esta página tem informações sobre como ativar e gerenciar suas licenças para que você possa começar a usar o Painter.

## Processo de ativação por tipo de aplicativo

O processo de ativação depende de onde você adquiriu ou tem acesso ao Painter:

| Tipo de Aplicativo | Processo de ativação |
| --- | --- |
| Creative Cloud para desktop | Consulte a página dedicada na [documentação do HelpX](https://helpx.adobe.com/download-install/using/download-creative-cloud-apps.html). Caso haja problemas, a [documentação do Creative Cloud](https://helpx.adobe.com/creative-cloud/user-guide.html) poderá fornecer respostas adicionais. |
| Vapor | Inicie o produto diretamente da biblioteca do Steam. |
| Substance 3D autônomo | Consulte o processo de ativação descrito abaixo. |

## Etapas da Ativação Independente

### O assistente de ativação

O Assistente de ativação aparece em determinadas versões anteriores do Substance 3D Painter.

Se você tiver um arquivo de licença perpétuo baixado do site da Substance 3D antes de 30 de setembro de 2022, ainda poderá usá-lo para ativar as versões qualificadas do Substance 3D Painter por meio do assistente de ativação. [Mais informações sobre licenças e contas de Substance herdadas estão disponíveis aqui.](https://substance3d.adobe.com/faq-end-of-life-accounts/)

![](../assets/activation-wizard.png){width="350px"}

O Assistente de ativação tem 3 opções:

* <b>Avalie este produto</b>: as versões de avaliação herdadas não estão mais disponíveis. Em vez disso, [você pode iniciar uma avaliação de 30 dias para cada aplicativo da Substance 3D aqui](https://www.adobe.com/products/substance3d/free-trial-download.html?msockid=35568f9be2b964ec22d09c04e3eb65af) ou com o Creative Cloud Desktop.
* <b>Ativar usando um arquivo de licença</b>: ative o produto com um arquivo de licença (<b>\*.key</b>) baixado da página da sua conta no site da Substance 3D antes de 30 de setembro de 2022.
* <b>Ative usando sua conta</b>: contas do substance herdadas não podem mais ser usadas para ativação.

>[!WARNING]
>
> Para instalar o arquivo de licença com o Assistente de ativação, execute o Painter como administrador e desative temporariamente o antivírus.

### Ativação manual

Você pode ativar o Substance Painter manualmente colocando o arquivo license.key na seguinte pasta:

>[!NOTE]
>
> Verifique se o arquivo é chamado de **license.key**, caso contrário, o aplicativo não poderá encontrá-lo.

<table data-preserve-html="true"><colgroup> <col/> <col/> <col/> <col/> </colgroup><tbody><tr><th>Plataforma</th><th>Versão</th><th colspan="2">Caminho</th></tr><tr><td rowspan="4"><strong>Windows</strong></td><td rowspan="2"><strong>7.2</strong> ou mais recente</td><td colspan="1">Dados do aplicativo (local)</td><td colspan="1">C:\Users\[nome do usuário]\AppData\Local\Adobe\Adobe Substance 3D Painter</td></tr><tr><td colspan="1">Dados de Aplicativo (roaming)</td><td colspan="1">C:\Users\[nome do usuário]\AppData\Roaming\Adobe\Adobe Substance 3D Painter</td></tr><tr><td rowspan="2">Legado</td><td colspan="1">Dados do aplicativo (local)</td><td colspan="1">C:\Users\[nome do usuário]\AppData\Local\Allegorithmic\Substance Painter</td></tr><tr><td colspan="1">Dados de Aplicativo (roaming)</td><td colspan="1">C:\Users\[nome do usuário]\AppData\Roaming\Allegorithmic\Substance Painter</td></tr><tr><td rowspan="2"><strong>Mac</strong></td><td colspan="1"><strong>7.2</strong> ou mais recente</td><td colspan="2">/Users/[nome do usuário]/Library/Application Support/Adobe/Adobe Substance 3D Painter</td></tr><tr><td colspan="1">Legado</td><td colspan="2">/Users/[nome do usuário]/Library/Application Support/Allegorithmic/Substance Painter</td></tr><tr><td rowspan="2"><strong>Linux</strong></td><td colspan="1"><strong>7.2</strong> ou mais recente</td><td colspan="2">/home/[nome do usuário]/.local/share/Adobe/Adobe Substance 3D Painter</td></tr><tr><td>Legado</td><td colspan="2">/home/[nome do usuário]/.local/share/Allegorithmic/Substance Painter</td></tr></tbody></table>

>[!NOTE]
>
> Alguns dos diretórios nos caminhos mencionados acima podem estar ocultos por padrão. Digite o caminho manualmente no explorador de arquivos ou exiba arquivos ocultos para exibi-los.

### Variável de ambiente

Você pode substituir o local que o Painter verifica para o arquivo **license.key** por uma [Variável de ambiente](../pipeline-and-integration/configuration/environment-variables.md).
