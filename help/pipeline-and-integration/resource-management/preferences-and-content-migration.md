---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/pipeline-and-integration/resource-management/preferences-and-content-migration.html"
breadcrumb-title: ''
description: Saiba como migrar preferências e conteúdo no Substance 3D Painter ao atualizar ou mudar para um novo sistema.
helpx_creative_field: ""
helpx_description: Painter > Pipeline and integration > Resource management > Preferences and content migration
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Preferências e migração de conteúdo
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '484'
ht-degree: 1%

---


# Preferências e migração de conteúdo

Esta página descreve como migrar dados de preferências e Prateleira/Ativos para usá-los nas novas versões.

Após o lançamento da versão 7.2, as preferências e o local da prateleira foram alterados para torná-los comuns em todas as versões do aplicativo (Substance 3D standalone, Steam e Creative Cloud Desktop). Esta alteração significa que as preferências anteriores e os recursos personalizados **foram ignorados** por padrão (**mas não foram perdidos**). Como a **Prateleira** foi renomeada para **Ativos**, a migração envolve algumas etapas detalhadas abaixo.

## Migração de recursos de prateleira e ativo

O local de recurso do usuário padrão foi alterado, o que significa que qualquer conteúdo colocado na pasta Documentos foi ignorado pelas novas versões do aplicativo. Para restaurar esse conteúdo, basta mover os arquivos de um local para outro.

### Onde encontrar o conteúdo

O caminho Prateleira ou Ativos pode ser encontrado nos seguintes locais:

<table data-preserve-html="true" style="width: 100.0%;"><colgroup> <col style="width: 15.0%;"/> <col style="width: 15.0%;"/> <col style="width: 70.0%;"/> </colgroup><tbody><tr><th>Plataforma</th><th>Versão</th><th>Caminho</th></tr><tr><td rowspan="2"><strong>Windows</strong></td><td><strong>7.2</strong> ou mais recente</td><td colspan="1">C:\Users\username\Documents\Adobe\Adobe Substance 3D Painter</td></tr><tr><td colspan="1">Legado</td><td colspan="1">C:\Users\username\Documents\Allegorithmic\Substance Painter</td></tr><tr><td rowspan="2"><strong>Mac</strong></td><td colspan="1"><strong>7.2</strong> ou mais recente</td><td colspan="1">/Users/username/Documents/Adobe/Adobe Substance 3D Painter</td></tr><tr><td colspan="1">Legado</td><td colspan="1">/Users/username/Documents/Allegorithmic/Substance Painter</td></tr><tr><td rowspan="2"><strong>Linux</strong></td><td colspan="1"><strong>7.2</strong> ou mais recente</td><td colspan="1">/home/username/Documents/Adobe/Adobe Substance 3D Painter</td></tr><tr><td>Legado</td><td colspan="1">/home/username/Documents/Allegorithmic/Substance Painter</td></tr></tbody></table>

### Como migrar o conteúdo para prateleira

O antigo conteúdo do Shelf é apenas arquivos no disco, então migrá-los é apenas colocar esses arquivos no lugar certo.

1. Fechar o aplicativo
1. Navegue até a antiga pasta Prateleira
1. Copiar ou cortar as subpastas (alfa, procedimentos, materiais etc.)
1. Navegue até a nova pasta Ativos
1. Cole as subpastas que você copiou anteriormente na pasta Ativos e substitua-as, se solicitado.

Agora reinicie o aplicativo. O conteúdo deve aparecer na janela Ativos.

>[!NOTE]
>
> Certifique-se de copiar as subpastas e não apenas a pasta pai dos recursos. A pasta pai foi renomeada de **prateleira** para **ativos**. Portanto, copiar apenas a pasta pai não tornará os recursos visíveis para o aplicativo.

### Como migrar as predefinições para prateleira

As predefinições de prateleira são salvas em um arquivo de configuração. Para migrar essas predefinições:

1. Fechar o aplicativo
1. Navegue até a antiga pasta Prateleira
1. Copie ou recorte o arquivo Shelf.ini
1. Navegue até a nova pasta Ativos
1. Colar o arquivo e substituir o arquivo existente

Agora reinicie o aplicativo. As pesquisas salvas serão exibidas na seção dedicada ou na janela Ativos.

## Migração de preferências

Recomendamos reajustar manualmente as configurações do aplicativo a partir da interface. Essa é a maneira mais segura de migrar informações sem apresentar problemas de compatibilidade.

Caso contrário, confira a seguinte página para saber onde as preferências estão agora localizadas: [Preferências e local dos dados de aplicativo](https://helpx.adobe.com/substance-3d/unlisted/documentation/spdoc/application-preferences-location-147095594.html).
