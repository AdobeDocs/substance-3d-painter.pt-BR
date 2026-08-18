---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/pipeline-and-integration/configuration/environment-variables.html"
breadcrumb-title: ''
description: Saiba como usar variáveis de ambiente no Substance 3D Painter para configurar o comportamento do aplicativo e a integração de pipeline.
helpx_creative_field: ""
helpx_description: Painter > Pipeline and integration > Configuration > Environment variables
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Variáveis de ambiente
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '513'
ht-degree: 3%

---


# Variáveis de ambiente

Esta página lista variáveis de ambiente que podem ser usadas para substituir o comportamento padrão do aplicativo.

| Variável | Descrição | Versão |
| --- | --- | --- |
| **SUBSTANCE\_PAINTER\_LICENSE** | Valor: caminho direto para o próprio arquivo de licença.Permitir que o substitua o local padrão do arquivo de licença. Exemplo: se o arquivo de licença estiver em **H:/allegorithmic/licenses/substance\_painter.key**, os dados da variável deverão ser **”H:/allegorithmic/licenses/substance\_painter.key”**.  **Observação:** use SUBSTANCE\_PAINTER\_2\_LICENSE para versões anteriores a 3.x (2017.x). | <ol data-preserve-html="true"><li data-preserve-html="true">1</li></ol> |
| **ALLEGO\_LICENSE\_IDLE\_DELAY** | Valor: 7200Especifique quanto tempo em segundos antes de liberar uma licença no caso de uma configuração multiusuário. O padrão é 2 horas (7200s). | <ol data-preserve-html="true"><li data-preserve-html="true">1</li></ol> |
| **ALG\_PAINTER\_SKIP\_CHECK\_FOR\_UPDATES** | Valor : 0 ou 1 (1 = Desabilitar verificação de atualização)Permite ignorar a verificação de atualização quando o aplicativo for iniciado. Desative o painel Novidades. | <ol data-preserve-html="true"><li data-preserve-html="true">2.2</li></ol> |
| **SUBSTANCE\_PAINTER\_SVT\_HARDWARE\_ACCELERATION** | Valor: 0 ou 1 (1 = Ativado)Use o recurso Esparso na GPU. Se não for suportado pela GPU ou pelo sistema operacional, a configuração será ignorada. Para configurações de hardware compatíveis, consulte a documentação: [Texturas virtuais esparsas](../../features/sparse-virtual-textures.md)Esta variável substitui o parâmetro disponível na janela [Configurações](../../interface/settings/settings.md). | <ol data-preserve-html="true"><li data-preserve-html="true">3</li></ol> |
| **SUBSTANCE\_PAINTER\_TEMP\_LOCATION** | Valor: caminho direto para uma pastaDefine onde o Substance Painter deve gravar seus arquivos temporários (incluindo o cache SVT). Essa variável substitui o parâmetro disponível na janela [Configurações](../../interface/settings/settings.md). | <ol data-preserve-html="true"><li data-preserve-html="true">3</li></ol> |
| **SUBSTANCE\_PAINTER\_PREVIEWS\_MEMORY\_BUDGET** | Valor: 500Define a quantidade de memória (Ram) que o aplicativo pode usar para carregar e armazenar visualizações temporárias a partir da janela Ativos. Quando o limite do orçamento é atingido, as visualizações antigas são descarregadas. Esse valor controla somente a exibição de visualizações na janela Ativos.O valor é definido em megabytes. O valor padrão é 500 MB. | <ol data-preserve-html="true"><li data-preserve-html="true">2</li></ol> |
| **SUBSTANCE\_PAINTER\_PLUGINS\_PATH** | Localização dos plug-ins Python adicionais. | 6.1 |
| **PYTHONPATH** | Módulos Python adicionais a serem carregados com a integração Python do aplicativo. Para obter mais informações, consulte [Carregando módulos Python externos](https://helpx.adobe.com/substance-3d/unlisted/documentation/spdoc/loading-external-python-modules-205363420.html). | <ol data-preserve-html="true"><li data-preserve-html="true">1</li></ol> |
| **OCIO** | Caminho para um arquivo **config.ocio** que será usado para orientar as configurações de [Gerenciamento de cores](../../features/color-management/color-management.md) com OpenColorIO.  **Observação:** esta variável de ambiente tem prioridade sobre a variável **PAINTER\_ACE\_CONFIG**. | <ol data-preserve-html="true"><li data-preserve-html="true">4</li></ol> |
| **PAINTER\_ACE\_CONFIG** | Caminho para um arquivo json que será usado para orientar as configurações de [Gerenciamento de cores](../../features/color-management/color-management.md) com o Adobe ACE. | <ol data-preserve-html="true"><li data-preserve-html="true">1</li></ol> |
| **SUBSTANCE\_DISABLE\_SPECIFIC\_FEATURES** | Desative várias funcionalidades dentro dos aplicativos:<ul data-preserve-html="true"><li data-preserve-html="true">Links para recursos externos (ajuda, páginas da Web, exemplos etc.)</li><li data-preserve-html="true">Desabilitar verificações de atualizações</li><li data-preserve-html="true">Desabilitar o envio de estatísticas de uso</li><li data-preserve-html="true">Desativar a exportação para o Substance share</li><li data-preserve-html="true">Desative os painéis Boas-vindas e Novidades</li></ul> | <ol data-preserve-html="true"><li data-preserve-html="true">1</li></ol> |
| **ALG\_PAINTER\_DEBUG\_FPS** | Exibir dentro da viewport um contador do número de quadros por segundo renderizados pela viewport. | <ol data-preserve-html="true"><li data-preserve-html="true">1</li></ol> |
| **SUBSTANCE\_PAINTER\_VRAM\_BUDGET** | Especifique quanta memória de GPU o Painter pode usar. Isso define um orçamento global em MB. Por exemplo, para definir um limite de 4 GB, use o valor 4000. Um argumento de linha de comando também pode ser usado para executar a mesma ação. Consulte [Linhas de comando](command-lines.md). | <ol data-preserve-html="true"><li data-preserve-html="true">2.1</li></ol> |
