---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/getting-started/export/export-window/export-settings.html"
breadcrumb-title: ''
description: Saiba como definir configurações de exportação no Substance 3D Painter para controlar a resolução da textura, o formato e as opções de saída.
helpx_creative_field: ""
helpx_description: Painter > Getting Started > Export > Export window > Export settings
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Exportar configurações
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '958'
ht-degree: 1%

---


# Exportar configurações

![](../../assets/image2023-1-30-13-22-30.png){width="500px"}

A <b>guia Configurações de exportação</b> da <b>janela Exportar texturas</b> permite configurar a composição, o tamanho e o local das texturas exportadas.

## Configuração de Conjuntos Gerais e de Texturas

![](../../assets/texture-set-list-1.png)

O primeiro elemento da janela é a lista de Conjuntos de texturas à esquerda. A seção Configurações globais fornece acesso a parâmetros comuns em todos os Conjuntos de texturas. Isso facilita o ajuste de um único conjunto de configurações para aplicar a todos os conjuntos de texturas do projeto. As alterações feitas nas configurações individuais do conjunto de texturas substituirão as configurações globais desse conjunto de texturas. Por exemplo, definir a resolução como 2048 nas configurações globais e 1024 como uma substituição para um conjunto de texturas específico resultará na exportação de todos os conjuntos de texturas com resolução de 2048, exceto o definido como 1024.

A caixa de seleção ao lado de cada nome de Conjunto de texturas indica se as texturas associadas serão exportadas ou não.

O menu suspenso é útil com projetos que possuem um grande número de conjuntos de texturas, pois permite modificar rapidamente a seleção com <b>Marcar tudo</b>, <b>Desmarcar tudo</b> e <b>Inverter todas as </b>ações.

## Parâmetros gerais de exportação

![](../../assets/image2023-1-30-13-23-7.png)

Esta seção contém as configurações compartilhadas para cada textura que será gerada:

| Configuração | Descrição |
| --- | --- |
| <b>Diretório de saída</b> | Salvar local para texturas exportadas. |
| <b>Modelo de saída</b> | Selecione o modelo de saída usado para nomear e compor os canais em arquivos de textura. Para obter mais informações sobre modelos, consulte a lista de [Modelos de saída](../export-presets/export-presets.md). |
| <b>Tipo de arquivo </b> | O formato do arquivo e sua profundidade de bits. Se a opção <b>Com base no modelo de saída</b> for selecionada, o formato do arquivo será herdado da predefinição de exportação (que permite que o formato e a profundidade de bits sejam determinados por textura em vez de globalmente). A profundidade de bits disponível depende do tipo de arquivo. Consulte a tabela abaixo para obter mais informações. |
| <b>Tamanho </b> | A resolução do arquivo de textura exportado. Valores possíveis:<ul data-preserve-html="true"> <li data-preserve-html="true"><b>Com base no tamanho de cada conjunto de textura</b></li> <li data-preserve-html="true"><b>128</b></li> <li data-preserve-html="true"><b>256</b></li> <li data-preserve-html="true"><b>512</b></li> <li data-preserve-html="true"><b>1024</b></li> <li data-preserve-html="true"><b>2048</b></li> <li data-preserve-html="true"><b>4096</b></li> <li data-preserve-html="true"><b>8192</b> (disponível somente com GPUs que têm mais de 1,5 GB de Vram)</li> </ul> |
| <b>Preenchimento </b> | Como a área fora das Ilhas UV é preenchida dentro da textura. Os valores possíveis são:<ul data-preserve-html="true"> <li data-preserve-html="true"><b>Sem preenchimento (passagem)</b>: use o estado atual da textura como ela está.</li> <li data-preserve-html="true"><b>Dilatação infinita</b>: estique as bordas da Ilha UV até que elas atinjam as bordas vizinhas ou o final da textura.</li> <li data-preserve-html="true"><b>Dilatação + transparente</b>: estica as bordas de Ilha UV até a distância especificada em pixels. O restante é transparente.</li> <li data-preserve-html="true"><b>Dilatação + cor de fundo padrão</b>: esticar as bordas de Ilha UV até a distância especificada em pixels, o restante é preenchido com a cor padrão do canal do Conjunto de Texturas.</li> <li data-preserve-html="true"><b>Dilatação + cor de fundo padrão</b>: esticar as bordas de Ilha UV até a distância especificada em pixels, o restante é preenchido com a cor padrão do canal do Conjunto de Texturas.</li> <li data-preserve-html="true"><b>Dilatação + difusão</b>: alongar as bordas da Ilha UV até a distância especificada em pixels, o restante é preenchido com uma versão desfocada da Ilha UV (com base em mapas mip).</li> </ul> |

>[!NOTE]
>
> O formato de arquivo **psd** é um contêiner; isso significa que os mapas de saída serão reunidos dentro de um único arquivo no disco.

### Pontilhamento

A exportação de texturas de 8 bits pode levar a bandas em gradientes. Isso é especialmente perceptível com os mapas Normal e Height. Há duas maneiras de resolver esse problema: usando maior precisão ou compensando com pontilhamento.

Uma precisão mais alta (16 ou 32 bits) é ideal, mas pode não ser compatível com todos os aplicativos. Mais notavelmente, os mecanismos de jogos geralmente compactam para 8 bits. O pontilhamento introduz ruído que ajuda a mitigar problemas de faixas enquanto ainda usa 8 bits de informação.

![](../../assets/dither-1.jpg)

### Formatos de arquivo de textura

Veja abaixo uma lista de todos os formatos de arquivo de exportação compatíveis com o Painter:

| Nome do formato | Formatar extensão | Profundidade de bits suportada |
| --- | --- | --- |
| **Bitmap** | bmp | 8, 8 + pontilhamento |
| **OpenEXR** | exr | 16 (flutuante), 32 (flutuante) |
| **Formato de intercâmbio de gráficos** | gif | 8, 8 + pontilhamento |
| **HDR do Radiance** | hdr | 32 (flutuante) |
| **Ícone** | ico | 8, 8 + pontilhamento |
| **Jpeg 2000** | j2k | 8, 8 + pontilhamento, 16 |
| **Gráficos De Rede Jpeg** | jng | 8, 8 + pontilhamento, 16 |
| **Jpeg 2000** | jp2 | 8, 8 + pontilhamento, 16 |
| **Jpeg** | jpeg | 8, 8 + pontilhamento |
| **intervalo estendido do JPEG** | jpeg-xr | 8, 8 + pontilhamento, 16, 32 (flutuante) |
| **Mapa de bits portátil** | pbm | 8, 8 + pontilhamento, 16 |
| **Mapa flutuante portátil** | pfm | 32 (flutuante) |
| **Mapa de Cinza Portátil** | pgm | 8, 8 + pontilhamento, 16 |
| **Gráficos de Rede Portáteis** | png | 8, 8 + pontilhamento, 16 |
| **Mapa de pixels portáteis** | ppm | 8, 8 + pontilhamento, 16 |
| **Documento do Photoshop** | psd | 8, 8 + pontilhamento, 16 |
| **TGA da Truevision** | targa | 8, 8 + pontilhamento |
| **Formato de Arquivo de Imagem de Marca** | tiff | 8, 8 + pontilhamento, 16, 32 (flutuante) |
| **Formato de Bitmap do Protocolo de Aplicativo sem Fio** | wbmp | 8, 8 + pontilhamento |
| **WebP** | webp | 8, 8 + pontilhamento |
| **X PixMap** | xpm | 8, 8 + pontilhamento |

## Mapas de saída

Quando um conjunto de texturas específico é selecionado, a seção Mapas de saída fica visível para esse conjunto de texturas.

![](../../assets/export-output-maps.png)

Esta seção lista todas as texturas que serão geradas com base na predefinição de exportação atual. Indica o modelo de nome de textura, o formato de arquivo e a profundidade de bits, além do espaço de cores, se o [Gerenciamento de cores](../../features/color-management/color-management.md) estiver habilitado.

Esta seção permite desabilitar a exportação de arquivos específicos ou substituir o <b>formato de arquivo</b> e a <b>profundidade de bits</b>.

![](../../assets/export-override.gif)

## Exportar ativo em USD

Marcar esta caixa permitirá que você exporte no formato USD. Diferentemente da predefinição USDz (Apple AR) disponível em <b>Modelos de saída</b>, esta exportação levará em consideração qualquer modelo ou parâmetro que você configurou para sua exportação. Os arquivos a seguir são exportados quando você marca a caixa Ativos em USD -

* Uma pasta com mapas de textura
* Um *.usda* que aponta para a pasta de mapas de textura.
* Um .usd opcional que monta materiais com o arquivo de malha original. Ele pode ser usado diretamente no Omniverse para mostrar sua malha com materiais aplicados automaticamente.
* Um arquivo .usd opcional, que inclui a malha usada no projeto. Ele é exportado apenas se o arquivo de malha original não for um USD ou se o desajuste automático do Painter tiver sido usado para gerar UVs.
