---
helpx_url: "https://helpx.adobe.com/br/substance-3d-painter/technical-support/workflow-issues/shelf-issues/font-import.html"
breadcrumb-title: ''
description: Saiba como corrigir problemas de importação de arquivos de fonte no Substance 3D Painter para importar e usar recursos de fonte com êxito.
helpx_creative_field: ""
helpx_description: Substance 3D Painter
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: O arquivo de fonte não pode ser importado
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '276'
ht-degree: 0%

---


# O arquivo de fonte não pode ser importado

Com a introdução do [Recurso de texto](../../../painting/text-resource.md), o arquivo de fontes é automaticamente reunido na inicialização. Os arquivos de fonte também podem ser importados manualmente.

Nesses casos, algumas mensagens de erro podem ser exibidas:

* Ao arrastar e soltar um arquivo na interface do Painter.
* Quando o Painter está descobrindo fontes no disco (rastreamento de bibliotecas).

## Como corrigir o problema

Se for exibida uma mensagem de erro sobre um <b>arquivo corrompido</b>, tente encontrar uma versão alternativa dele e o Painter poderá carregá-lo. Observe que há suporte apenas para os formatos <b>.ttf</b> e <b>.otf</b>.

Se uma mensagem de erro for gerada sobre um <b>problema de licenciamento</b>, a fonte simplesmente não é compatível com o Painter e não pode ser importada.

### Visão geral das mensagens

|  |  |
| --- | --- |
| <b>Mensagem de erro</b> | <b>Explicação</b> |
| Existem problemas na biblioteca “LIBRARYNAME” afetando 4 arquivo(s) de fonte: FONTNAME, FONTNAME, FONTNAME,... | Esta mensagem reúne uma pequena lista de nomes de arquivos de fontes que foram identificados como não sendo importáveis no Painter. Esses arquivos serão ignorados e não aparecerão na janela Ativos. |
| Problemas de fonte encontrados. Para obter detalhes, acesse https://... | Mensagem genérica para indicar que foi encontrado um problema com as fontes. |
| Não é possível importar FONTNAME devido a suas restrições de licenciamento. Para obter detalhes, acesse https://... | O Painter precisa ser capaz de incorporar fontes em seu arquivo de projeto para usá-las. Portanto, fontes que não permitem isso (especificadas em seus metadados) não podem ser importadas. |
| Não é possível importar FONTNAME porque o arquivo está corrompido ou é de um tipo não suportado. Para obter detalhes, acesse https://... | O Painter não pode ler o arquivo de fonte fornecido. |
