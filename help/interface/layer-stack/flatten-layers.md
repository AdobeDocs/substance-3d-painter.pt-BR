---
title: Achatar camadas
description: ''
helpx_description: "Substance 3D Painter"
helpx_url: "https://helpx.adobe.com/substance-3d-painter/interface/layer-stack/flatten-layers.html"
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '883'
ht-degree: 1%

---


# Achatar camadas

![](../../assets/v12_banner_flatten.jpg)

## Achatar camadas

O nivelamento de camadas permite condensar os dados de textura visíveis de um grupo selecionado em uma única camada. Isso pode ajudar a simplificar a pilha de camadas, melhorando o desempenho e facilitando o gerenciamento de projetos.

>[!NOTE]
>
> Quando você usa a função Nivelar, uma nova camada é criada, mas o grupo original de camadas não é excluído. Em vez disso, o grupo de origem é desativado, deixando a opção de excluí-lo ou salvá-lo como um material inteligente para edição posterior.

## Como nivelar camadas

Para nivelar uma série de camadas:

1. Selecione as camadas desejadas.
1. Use <b>CTRL + G (CMD + G) </b> para agrupar a seleção.
1. Use <b>CTRL + M (CMD + M)</b> para mesclar a seleção.

Também é possível acessar essas opções no menu do botão direito do mouse, em vez de usar atalhos de teclado.

![](../../assets/v12_flatten_menu.jpg)

Quando as camadas são niveladas, uma nova camada de preenchimento é criada com texturas niveladas e o grupo de origem é desativado.

## Achatar canais específicos

* Em uma camada de preenchimento, use o painel Propriedades para desativar os canais que não deseja nivelar. As informações não são perdidas quando os canais são desativados. Depois de nivelar a camada, você pode reativar os canais, e os dados ainda estarão lá
* Para grupos ou camadas de pintura, você pode usar modos de mesclagem para desativar canais:
  * Na parte superior da Pilha de camadas, selecione o canal a ser desativado.
  * Altere o modo de mesclagem da camada desejada para “Desativado”.
  * Você pode aplicar o mesmo modo de mesclagem a todos os canais de uma camada clicando com o botão direito do mouse no modo de mesclagem e selecionando “Aplicar a todos os canais”.

## Exportar mapas achatados da pilha de camadas

Use o <b>Exportar grupo nivelado para arquivos</b> no menu de contexto na pilha de camadas para exportar texturas rapidamente. Essa opção está disponível quando uma camada ou um grupo é selecionado. Quando várias camadas ou grupos são selecionados, eles serão tratados como um lote, como se você exportasse cada um deles um por um.

>[!NOTE]
>
> Assim como na função <b>Achatar grupo </b>, canais e camadas vazios ou desabilitados não serão exportados. Se uma máscara de geometria estiver sendo usada, somente os blocos gráficos UV ativados dentro da máscara de geometria serão exportados.

### Gerenciamento de arquivos

Ao selecionar <b>Exportar grupo nivelado para arquivos</b>, você terá a oportunidade de selecionar um local de pasta para os arquivos exportados.

Os arquivos exportados são nomeados de acordo com o padrão no campo do nome do arquivo. O padrão é:

* <b>$textureSet\_$layerName\_$srcMap(.$udim)</b>

Com esse padrão, os mapas terão o nome do conjunto de texturas, o nome da camada, o nome do canal e, se for um projeto de bloco UV, o número UDIM.

Se você modificar o padrão, ele estará disponível novamente na próxima vez que a janela for aberta.

### Propriedades do arquivo exportado

As propriedades dos arquivos exportados são baseadas nos seguintes valores no momento da exportação:

* A resolução é baseada na resolução do conjunto de Textura.
* A profundidade de bits se baseia na profundidade de bits do canal nas configurações do conjunto de textura.

As seguintes propriedades são codificadas e não podem ser alteradas:

* O preenchimento está bloqueado para 1 px.
* O formato do arquivo depende do canal que está sendo exportado. Mapas como height e normal geralmente precisam de mais profundidade de bits e são exportados como EXR, enquanto outros canais são exportados como PNG.
* Se apenas uma máscara for exportada, você poderá selecionar o formato de exportação.

## Como a camada achatada é gerada?

A função achatar cria um bitmap por canal habilitado dentro de uma nova camada de preenchimento. A resolução é baseada na resolução do conjunto Textura, e a profundidade de bits é determinada pelas configurações do conjunto Textura.

Achatar funciona quando há dados de textura dentro de um canal específico. Nivelar não funcionará em uma camada de pintura vazia e postará uma mensagem de erro no log se não houver dados na seleção.

Somente camadas e efeitos visíveis podem ser nivelados. Se algumas camadas no grupo estiverem desativadas quando o grupo for nivelado, os efeitos dessas camadas não serão incluídos no resultado nivelado.

### Camadas desativadas

Somente camadas e efeitos visíveis podem ser nivelados. Se algumas camadas no grupo estiverem desativadas quando o grupo for nivelado, os efeitos dessas camadas não serão incluídos no resultado nivelado.

### Máscaras de camada e de geometria

As máscaras são niveladas separadamente dos dados de textura. Isso significa que, se você nivelar um grupo com uma máscara, o preenchimento nivelado e a máscara nivelada serão gerados.

Ao usar uma máscara de geometria, se apenas alguns blocos UV forem selecionados dentro da máscara de geometria, a camada achatada manterá essa seleção. Os ladrilhos UV que não foram selecionados na máscara geométrica são considerados vazios e, portanto, sua texturização não é mantida no resultado nivelado.

## Gerenciar conteúdo achatado

>[!NOTE]
>
> Imagens achatadas são armazenadas dentro do arquivo de projeto (.SPP). Isso significa que eles terão um impacto no tamanho do seu arquivo de projeto.

Imagens achatadas são marcadas automaticamente como “achatadas” para que você possa pesquisá-las facilmente no painel Ativos. Eles também são armazenados automaticamente na categoria Pesquisas salvas “Camadas niveladas”.

### Limpar imagens não utilizadas

Remover imagens não usadas do arquivo de projeto pode ajudar a clarear o tamanho do projeto. No painel Ativos, você pode excluir imagens pelo menu do botão direito. Ou, para remover todas as imagens não utilizadas, use <b>Arquivo > Remover recursos não utilizados</b>. Lembre-se de que isso excluirá não apenas imagens niveladas, mas também todos os recursos que não estiverem sendo usados na pilha de camadas, em slots de mapas com suporte ou em outro local na interface.
