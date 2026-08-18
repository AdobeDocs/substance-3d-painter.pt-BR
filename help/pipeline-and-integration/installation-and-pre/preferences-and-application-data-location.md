---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/pipeline-and-integration/installation-and-preferences/preferences-and-application-data-location.html"
breadcrumb-title: ''
description: Saiba mais sobre preferências e locais de dados de aplicativos para que o Substance 3D Painter gerencie as configurações e os dados do usuário.
helpx_creative_field: ""
helpx_description: Painter > Pipeline and integration > Installation and preferences > Preferences and application data location
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Localização de preferências e dados de aplicativos
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '299'
ht-degree: 4%

---


# Localização de preferências e dados de aplicativos

Esta página agrupa informações sobre onde as preferências do aplicativo são armazenadas por versão e plataforma.\
Pode ser útil saber onde as preferências estão armazenadas caso você queira adicionar **prateleiras personalizadas** (para instalações de estúdios) ou remover essas preferências para executar uma **instalação limpa** do aplicativo.

## Preferências

Esse caminho é o local das preferências do aplicativo (atalhos salvos, caminhos de prateleira/ativo, layout de interface etc.).

<table data-preserve-html="true"><colgroup> <col/> <col/> <col/> </colgroup><tbody><tr><th>Sistema</th><th>Versão</th><th>Caminho</th></tr><tr><td rowspan="2"><p><strong>Windows</strong></p><p>(registro)</p></td><td><strong>7.2</strong> ou mais recente</td><td>HKEY_CURRENT_USER\Software\Adobe\Adobe Substance 3D Painter</td></tr><tr><td>Legado</td><td>HKEY_CURRENT_USER\Software\Allegorithmic\Substance Painter</td></tr><tr><td rowspan="2"><p><strong>Mac</strong></p><p>(biblioteca)</p></td><td><strong>7.2</strong> ou mais recente</td><td>/Users/[nome do usuário]/Library/Preferences/com.adobe.Adobe Substance 3D Painter.plist</td></tr><tr><td>Legado</td><td>/Users/[nome do usuário]/Library/Preferences/com.substance3d.Substance Painter.plist</td></tr><tr><td rowspan="2"><strong>Linux</strong></td><td><strong>7.2</strong> ou mais recente</td><td>/home/[nome do usuário]/.config/Adobe/Adobe Substance 3D Painter.conf</td></tr><tr><td>Legado</td><td>/home/[nome do usuário]/.config/Allegorithmic/Substance Painter.conf</td></tr></tbody></table>

## Dados do aplicativo

Esse caminho é o local dos dados adicionais do aplicativo (miniaturas de ativos, arquivo de registro etc.).

<table data-preserve-html="true"><colgroup> <col/> <col/> <col/> <col/> </colgroup><tbody><tr><th>Plataforma</th><th>Versão</th><th colspan="2">Caminho</th></tr><tr><td rowspan="4"><strong>Windows</strong></td><td rowspan="2"><strong>7.2</strong> ou mais recente</td><td colspan="1">Dados do aplicativo (local)</td><td colspan="1">C:\Users\[nome do usuário]\AppData\Local\Adobe\Adobe Substance 3D Painter</td></tr><tr><td colspan="1">Dados de Aplicativo (roaming)</td><td colspan="1">C:\Users\[nome do usuário]\AppData\Roaming\Adobe\Adobe Substance 3D Painter</td></tr><tr><td rowspan="2">Legado</td><td colspan="1">Dados do aplicativo (local)</td><td colspan="1">C:\Users\[nome do usuário]\AppData\Local\Allegorithmic\Substance Painter</td></tr><tr><td colspan="1">Dados de Aplicativo (roaming)</td><td colspan="1">C:\Users\[nome do usuário]\AppData\Roaming\Allegorithmic\Substance Painter</td></tr><tr><td rowspan="2"><strong>Mac</strong></td><td colspan="1"><strong>7.2</strong> ou mais recente</td><td colspan="2">/Users/[nome do usuário]/Library/Application Support/Adobe/Adobe Substance 3D Painter</td></tr><tr><td colspan="1">Legado</td><td colspan="2">/Users/[nome do usuário]/Library/Application Support/Allegorithmic/Substance Painter</td></tr><tr><td rowspan="2"><strong>Linux</strong></td><td colspan="1"><strong>7.2</strong> ou mais recente</td><td colspan="2">/home/[nome do usuário]/.local/share/Adobe/Adobe Substance 3D Painter</td></tr><tr><td>Legado</td><td colspan="2">/home/[nome do usuário]/.local/share/Allegorithmic/Substance Painter</td></tr></tbody></table>

>[!NOTE]
>
> Alguns dos diretórios nos caminhos mencionados acima podem estar ocultos por padrão. Digite o caminho manualmente no explorador de arquivos ou exiba arquivos ocultos para exibi-los.
