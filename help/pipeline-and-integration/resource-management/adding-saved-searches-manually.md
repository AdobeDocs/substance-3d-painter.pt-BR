---
helpx_url: "https://helpx.adobe.com/br/substance-3d-painter/pipeline-and-integration/resource-management/adding-saved-searches-manually.html"
breadcrumb-title: ''
description: Saiba como adicionar pesquisas salvas manualmente no Substance 3D Painter para acessar rapidamente os filtros de recursos usados com frequência.
helpx_creative_field: ""
helpx_description: Painter > Pipeline and integration > Resource management > Adding saved searches manually
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Adicionando pesquisas salvas manualmente
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '240'
ht-degree: 2%

---


# Adicionando pesquisas salvas manualmente

As consultas de pesquisa de ativos (ou pesquisas salvas) podem ser definidas editando um arquivo de configuração. Esta página explica como.

## Local do arquivo de configuração

Para adicionar consultas personalizadas salvas, navegue até a pasta Documentos do usuário e abra o arquivo **Shelf.ini**.

<table data-preserve-html="true" style="width: 100.0%;"> <colgroup> <col style="width: 15.0%;"/> <col style="width: 15.0%;"/> <col style="width: 70.0%;"/> </colgroup> <tbody> <tr> <th>Plataforma</th> <th>Versão</th> <th>Caminho</th> </tr> <tr> <td rowspan="2"><strong>Windows</strong></td> <td><strong>7.2</strong> ou mais recente</td> <td colspan="1">C:\Users\username\Documents\Adobe\Adobe Substance 3D Painter</td> </tr> <tr> <td colspan="1">Legado</td> <td colspan="1">C:\Users\username\Documents\Allegorithmic\Substance Painter</td> </tr> <tr> <td rowspan="2"><strong>Mac</strong></td> <td colspan="1"><strong>7.2</strong> ou mais recente</td> <td colspan="1">/Users/username/Documents/Adobe/Adobe Substance 3D Painter</td> </tr> <tr> <td colspan="1">Legado</td> <td colspan="1">/Users/username/Documents/Allegorithmic/Substance Painter</td> </tr> <tr> <td rowspan="2"><strong>Linux</strong></td> <td colspan="1"><strong>7.2</strong> ou mais recente</td> <td colspan="1">/home/username/Documents/Adobe/Adobe Substance 3D Painter</td> </tr> <tr> <td>Legado</td> <td colspan="1">/home/username/Documents/Allegorithmic/Substance Painter</td> </tr> </tbody> </table>

## Exemplo

Veja a seguir um exemplo de conteúdo que pode ser colocado no arquivo de configuração:

```
[filters] 

size=4 

1name=Grunge 

1query="u:basematerial=,smartmaterial=,smartmask=,texture=,procedural=,brush=,alpha= grunge" 

2name=Procedural 

2query="u:procedural=" 

3name=Environment 

3query="u:environment=" 

4name=Default Filters 

4query="p:/allegorithmic/^ u:filters="
```


Veja como a sintaxe funciona:

* **Tamanho**: determina o número de predefinições personalizadas que precisam ser lidas e carregadas pelo aplicativo.
* **Número**: no início da linha define a predefinição atual que ela destina (por exemplo: **1/**).
* **Consulta**: (após o número) define os termos de pesquisa reais usados. No exemplo, ele usa **u:** para usos, **p:** para caminhos ou uma cadeia de caracteres para um termo de pesquisa. O conteúdo da consulta deve ser delimitado por aspas. Para saber mais sobre os termos que podem ser usados, [veja esta página](../../interface/assets/advanced-search-queries.md).
* **Nome**: o nome da predefinição.
