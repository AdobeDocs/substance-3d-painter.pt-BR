---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/getting-started/project-creation.html"
breadcrumb-title: ''
description: Saiba como criar um novo projeto no Substance 3D Painter para começar a pintar texturas em seus modelos 3D.
helpx_creative_field: ""
helpx_description: Painter > Getting Started > Project Creation
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Criação de projeto
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '1157'
ht-degree: 1%

---


# Criação de projeto

![](../assets/v12_banner_project_window.jpg)

A <b>janela Novo projeto </b>permite criar um arquivo de projeto para armazenar seu modelo 3D e suas informações de texturização.

Um novo [Conjunto de Texturas](../interface/texture-set/texture-set.md) é criado por definição de material encontrada no modelo 3D importado. Isso significa que vários objetos podem ser importados por meio de um único arquivo (mesmo com UVs sobrepostos) se tiverem materiais diferentes.

## Criando um novo projeto

Para criar um novo projeto, clique em <b>Arquivo > Novo</b> ou use o atalho de teclado <b>Ctrl + N</b>.

Veja abaixo uma explicação de todos os parâmetros disponíveis na janela Novo projeto.

### Configurações básicas

| *Parâmetro* | *Descrição* |
| --- | --- |
| **Arquivo** | Clique no botão “Selecionar” para especificar um arquivo de modelo 3D a ser carregado. [Uma lista de formatos de arquivo com suporte está disponível aqui.](https://experienceleague.adobe.com/en/docs/substance-3d/general-knowledge/ecosystem/import-and-export-formats) |
| **Modelo** | Especifique um modelo que definirá as configurações padrão do projeto. Um modelo contém os seguintes parâmetros:<ul data-preserve-html="true"> <li data-preserve-html="true">Configurações do conjunto de texturas.</li> <li data-preserve-html="true">Configurações de exibição.</li> <li data-preserve-html="true">Configurações de cozimento.</li> <li data-preserve-html="true">Recursos de sombreador (incluindo texturas anexadas).</li> <li data-preserve-html="true">Arquivo de Mapa de Ambiente.</li> </ul>  **Observação:** os modelos são arquivos <b>\*.spt</b> criados a partir de um projeto existente por meio do [menu Arquivo](../interface/main-menu/file-menu.md) e salvos na pasta Ativos para serem facilmente compartilhados com os membros da equipe. |
| <b>Resolução</b> | Defina a resolução de textura padrão do projeto para cada Conjunto de texturas. A resolução pode ir até 4K (4096x4096 pixels) ao trabalhar dentro do aplicativo e 8K (8192x8192 pixels) ao exportar. A resolução pode ser alterada posteriormente por meio das [configurações do Conjunto de Texturas](../interface/texture-set/texture-set-settings.md).  **Observação:** a exportação de 8K requer que pelo menos 2,5 GB de VRam na GPU estejam disponíveis. |

### Configurações específicas do tipo de arquivo

Quando um USD é selecionado, outras configurações específicas do tipo de arquivo ficam disponíveis.

| *Parâmetro* | *Descrição* |
| --- | --- |
| <b>Escopo e variantes</b> | Selecione uma parte específica de um arquivo do USD. Por padrão, é definido como “Raiz”, o que significa que o arquivo do USD inteiro será usado para criar o projeto do Painter.  <b>Alterar...</b> abre uma nova janela que exibe o conteúdo do USD. Se forem detectadas variantes, é possível selecionar uma variante específica para a criação do projeto. O escopo e as variantes podem ser alterados após a criação do projeto nas configurações do [Projeto](../interface/project-configuration.md). Observe que:<ul data-preserve-html="true"> <li data-preserve-html="true">Somente a seleção da variante de modelagem terá qualquer impacto no projeto.</li> <li data-preserve-html="true">Variantes aninhadas dentro de variantes não são detectadas no momento.</li> </ul> |
| <b>Nível de subdivisão</b> | Para a geometria que deve ser subdividida, essa configuração permite especificar o quanto você deseja subdividir a malha para texturização no Painter. Se a subdivisão for explicitamente definida como &#39;none&#39; no arquivo USD, essa configuração ficará acinzentada.  A subdivisão é aplicada após o desencapsulamento UV, portanto isso não altera a forma dos UVs da malha. Os níveis de subdivisão podem ser alterados após a criação do projeto nas configurações do [Projeto](../interface/project-configuration.md). |
| <b>Quadro</b> | Para arquivos do USD onde animações são detectadas, essa configuração permite selecionar o quadro que será usado para criar seu projeto do Painter. Se não houver animação no arquivo USD selecionado, essa configuração ficará acinzentada. O quadro pode ser alterado após a criação do projeto nas configurações do [Projeto](../interface/project-configuration.md). |

### Configurações avançadas

| *Parâmetro* | *Descrição* |
| --- | --- |
| **Formato de mapa normal** | Define o Formato de mapa normal do projeto, pode ser<ul data-preserve-html="true"><li data-preserve-html="true"><strong>DirectX</strong> (X+, Y-, Z+)</li><li data-preserve-html="true"><strong>OpenGL</strong> (X+, Y+, Z+)</li></ul>  **Observação:** como lembrete:<ul data-preserve-html="true"> <li data-preserve-html="true">O <b>Unreal Engine</b> usa DirectX por padrão.</li> <li data-preserve-html="true">O <b>Unity</b> usa o OpenGL por padrão.</li> </ul> |
| **Calcular Espaço Tangente por Fragmento** | Se ativado, as Bitangents são computadas no sombreador de fragmentos (pixels) em vez do sombreador de vértices. Esse parâmetro afeta a maneira como o mapa de Normal é decodificado pelo Sombreador no visor. Será necessário alterar essas configurações para refazer o mapa Normal.  **Observação:** como lembrete:<ul data-preserve-html="true"> <li data-preserve-html="true">O <b>Unreal Engine</b> precisa que esta configuração seja Habilitada.</li> <li data-preserve-html="true">A <b>Unidade</b> precisa que esta configuração seja Desabilitada (ou habilitada se você estiver usando o fluxo de trabalho HDRP)</li> </ul> |

### Configurações de bloco UV (UDIMs)

>[!NOTE]
>
> Essas configurações não podem ser modificadas depois que o projeto é criado.

| *Parâmetro* | *Descrição* |
| --- | --- |
| **Usar fluxo de trabalho de Bloco UV** | Se marcada, a malha importada será processada de forma diferente para permitir a pintura fora do intervalo UV normal (0-1). Projetos que usam UDIM devem ativar essa configuração. O processamento da malha pode diferir dependendo da configuração.   Para obter mais informações, consulte a [documentação do UV Tile](../features/uv-tiles/uv-tiles.md). |
| <b>Preservar o layout do Bloco UV por materiais e habilitar a pintura entre blocos</b> | Os blocos UV (UDIMs) são importados e agrupados por atribuição de material na malha. Isso significa que um único Conjunto de Texturas pode conter vários Blocos UV visíveis lado a lado na Visualização 2D. Os blocos UV que estão dentro do mesmo conjunto de textura podem ser pintados perfeitamente.  <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table2_row-r2-column-c1_image_copy" src="../assets/uvtiles-paintacross.jpg" width="500px"/></div> |
| <b>Converter Blocos UV em Conjuntos de Texturas individuais (herdados)</b> | Os Blocos UV (UDIMs) são separados em Conjuntos de texturas individuais e renomeados, ignorando quaisquer atribuições de material. Cada Bloco UV é movido para o intervalo UV [0-1] para ser pintável.  <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table2_row-r3-column-c1_image" src="../assets/uvtiles-legacy.jpg" width="500px"/></div> |

### Configurações de Importação

| ***Parâmetro*** | ***Descrição*** |
| --- | --- |
| **Importar câmeras** | Se câmeras estiverem presentes no arquivo de malha, elas serão importadas para o projeto e acessíveis como predefinições para visualização.  **Observação:** o Substance 3D Painter não oferece suporte a algumas câmeras em determinadas condições:<ul data-preserve-html="true"><li data-preserve-html="true">Câmeras físicas do 3DS Max.</li><li data-preserve-html="true">Câmeras ortográficas armazenadas em arquivos Alembic (&#42;.abc).</li></ul> |
| **Desempacotamento automático** | Se ativado, serão gerados UVs ausentes na malha importada. O processamento pode ser alterado dependendo das configurações selecionadas por meio do botão **Opções**.Para obter mais informações, consulte a [Documentação de desencapsulamento automático de UV](../features/automatic-uv-unwrapping.md). |

### Importar mapas prontos

Use o botão <b>Adicionar</b> para carregar arquivos de textura como mapas de malha e atribuí-los automaticamente nas [configurações do Conjunto de texturas](../interface/texture-set/texture-set-settings.md). Uma convenção de nomenclatura específica deve ser seguida para que os mapas de malha sejam atribuídos automaticamente aos seus conjuntos de texturas. Os mapas de malha também podem ser cozidos diretamente dentro da aplicação; consulte a documentação de cozimento.

Convenção de nomenclatura:<b> TextureSetName\_MeshMapName</b>

Exemplo:<b> DefaultMaterial\_ambiente\_oclusão.png </b>

Lista de mapas de malha compatíveis e seus nomes:

| *Mapa de malha* | *Convenção de nome de arquivo* |
| --- | --- |
| **oclusão de ambiente** | ambiente\_oclusão |
| **Curvatura** | curvatura |
| **Normal** | normal\_base |
| **Espaço Mundial Normal** | world\_space\_normals |
| **ID** | id |
| **Posição** | posição |
| **Thickness** | espessura |

### Tamanho físico

As configurações de tamanho físico permitem ajustar como o Painter determina o tamanho físico da malha em unidades do mundo real. Isso é útil para garantir que os materiais sejam aplicados em uma escala realista.

* Usar escala de unidade interna do arquivo de malha: A maioria dos tipos de arquivo inclui informações sobre o tamanho físico do objeto conforme ele foi exportado do aplicativo de modelagem 3D. Com essa opção selecionada, o Painter usará essas informações do arquivo importado.
* Escala de unidade personalizada: substitua a escala de unidade do arquivo importado ou, se nenhuma escala de unidade estiver incluída, use a caixa de entrada personalizada para ajustar o tamanho de uma única “unidade”.
* Alternar o dimensionamento da camada de preenchimento para o Tamanho físico ao atribuir materiais: se isso estiver ativado, os materiais que têm informações do tamanho físico podem ajustar o dimensionamento para corresponder ao tamanho físico da superfície à qual estão sendo aplicados.

### Gerenciamento de cores

![](../assets/newproj-cm.png)

Esta seção controla as configurações de gerenciamento de cores do projeto. Por padrão, é definido como Legado (sRGB / fluxo de trabalho linear).

Confira a documentação do [gerenciamento de cores](../features/color-management/color-management.md) para saber mais sobre como usar este fluxo de trabalho e o que as configurações estão fazendo.
