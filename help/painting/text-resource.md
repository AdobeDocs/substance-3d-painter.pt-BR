---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/painting/text-resource.html"
breadcrumb-title: ''
description: Saiba como usar recursos de texto no Substance 3D Painter para adicionar texto e tipografia aos seus fluxos de trabalho de pintura de textura.
helpx_creative_field: ""
helpx_description: Substance 3D Painter
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Recurso de texto
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '521'
ht-degree: 0%

---


# Recurso de texto

![](../assets/v10_text_resource_banner-1.jpg)

O <b>recurso de texto</b> do pode ser usado para gravar texto em texturas com o uso de <b>arquivos de fonte</b> específicos. Vários parâmetros estão disponíveis para ajustar a aparência do texto final desenhado.

## Procurar fontes

Para procurar os arquivos de fonte disponíveis, basta clicar no filtro de fonte (o botão <b>T</b>) na [janela Ativos](../interface/assets/assets.md):

![](../assets/v10_text_assets.png)

A fonte também pode ser filtrada por caminhos, dependendo de onde esteja localizada no sistema:

![](../assets/v10_font_path.png)

Os locais de fonte disponíveis dependem do sistema operacional atual:

|  |  |
| --- | --- |
| Windows | <ul data-preserve-html="true"> <li data-preserve-html="true"><b>Sistema</b>: C:/Windows/Fonts</li> <li data-preserve-html="true"><b>Usuário</b>: C:/Users/username/Appdata/Local/Microsoft/Windows/Fonts</li> </ul> |
| MacOS | <ul data-preserve-html="true"> <li data-preserve-html="true"><b>Sistema</b>: /Sistema/Biblioteca/Fontes</li> <li data-preserve-html="true"><b>Local</b>: /Biblioteca/Fontes</li> <li data-preserve-html="true"><b>Usuário</b>: /Usuários/nome do usuário/Biblioteca/Fontes</li> </ul> |
| Linux | <ul data-preserve-html="true"> <li data-preserve-html="true"><b>Sistema</b>: /usr/share/fonts/</li> <li data-preserve-html="true"><b>Local</b>: /usr/local/share/fonts/</li> <li data-preserve-html="true"><b>Usuário</b>: /home/username/.local/share/fonts/</li> </ul> |

### Importação de fontes

As fontes podem ser importadas manualmente ou colocadas em uma biblioteca existente do Painter como qualquer recurso normal. Para fazer isso, consulte a [documentação de importação](../content/importing-assets/import-drag-and-drop.md).

O Painter oferece suporte aos formatos de fonte <b>.ttf</b> e <b>.otf</b>.

>[!NOTE]
>
> Se um recurso falhar ao carregar/importar com a mensagem de erro “não pode ser importado devido à restrição de licenciamento da fonte”, isso significa que não pode ser usado pelo Painter. Somente fontes marcadas como <b>incorporáveis</b> em seus metadados podem ser usadas.

### Usar uma fonte como um recurso de texto

Um recurso de textura funciona como outros recursos (imagens ou materiais de Substance, por exemplo) e pode ser usado em parâmetros de pincel, projeções de preenchimento ou entradas de imagem de Substance.

Para criar um recurso de texto, basta adicionar uma fonte a um slot de recurso. Também é possível arrastar e soltar uma fonte no visor.

![](../assets/v10_text_drag_drop.gif)

### Parâmetros de recurso de texto

Um recurso de texto tem os seguintes parâmetros básicos:

![](../assets/v10_text_params_base.png)

| <b>Parâmetro</b> | <b>Descrição</b> |
| --- | --- |
| <b>Texto</b> | Texto a ser renderizado.  **Observação:** o campo de texto na interface usa uma fonte genérica com uma ampla gama de caracteres, o que pode criar discrepâncias entre o que foi digitado no campo e a fonte selecionada que pode ser renderizada na textura. |
| <b>Tamanho da fonte</b> | Especifique o modo usado para calcular o tamanho da fonte. Os modos disponíveis são:<ul data-preserve-html="true"> <li data-preserve-html="true"><b>Automático</b>: o tamanho é calculado automaticamente a partir do conteúdo do texto e se ajusta à textura.</li> <li data-preserve-html="true"><b>Personalizado</b>: o tamanho pode ser controlado manualmente por meio da configuração dedicada.</li> </ul> |
| <b>Alinhamento</b> | Controla o alinhamento vertical e horizontal. Use os botões para escolher o modo a ser usado. |
| <b>Cor</b> | A cor do texto renderizado. Essa configuração pode ser em escala de cinza se o recurso de texto for usado em uma máscara ou em um canal de escala de cinza. |

Parâmetros mais avançados também estão disponíveis:

![](../assets/v10_text_params_advanced.png)

| <b>Parâmetro</b> | <b>Descrição</b> |
| --- | --- |
| <b>Espaçamento entre linhas</b> | Distância entre as linhas de texto (”entrelinhas”) em relação ao tamanho da fonte. |
| <b>Espaçamento entre caracteres</b> | A quantidade de espaço entre caracteres adjacentes em relação ao tamanho da fonte. Pode ser negativo para subtrair o espaçamento. |
| <b>Deslocamento</b> | Deslocamento horizontal e vertical do texto. Normalizado para o tamanho da fonte. |
| <b>Preenchimento do plano de fundo</b> | Cor do plano de fundo atrás do texto. |
| <b>Opacidade do plano de fundo</b> | A quantidade da cor de fundo que é visível. |
| <b>Resolução</b> | Especifique o modo usado para calcular o tamanho da textura usada para renderizar o texto. Os modos disponíveis são:<ul data-preserve-html="true"> <li data-preserve-html="true"><b>Automático</b>: a resolução é calculada automaticamente.</li> <li data-preserve-html="true"><b>Personalizado</b>: a resolução pode ser definida manualmente por meio da configuração dedicada.</li> </ul> |
