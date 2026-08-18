---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/interface/color-picker.html"
breadcrumb-title: ''
description: Saiba como usar o seletor de cores no Substance 3D Painter para selecionar cores de texturas e materiais.
helpx_creative_field: ""
helpx_description: Painter > Interface > Color picker
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Seletor de cores
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '1066'
ht-degree: 1%

---


# Seletor de cores

![](../assets/color-picker-12.jpg)

O seletor de cores permite definir uma cor para pintar ou projetar na malha. Ela pode ser usada para selecionar cores de imagens externas ou para ajustar uma existente no aplicativo.

A janela do seletor de cores aparece ao clicar em qualquer campo de cores no Painter, que pode ser encontrado em Propriedades ou em quaisquer configurações ou menus adicionais, como parâmetros de exibição ou de sombreador.

## Visão geral do seletor de cores

Uma vez aberto, o seletor de cores é semipersistente, o que significa que permanecerá aberto até uma alteração de contexto - por exemplo, ao alternar de uma camada de tinta para uma camada de preenchimento. É possível mover a janela e colocá-la em qualquer lugar em qualquer uma das telas disponíveis. No entanto, diferentemente de outras janelas, o seletor de cores não pode ser encaixado.

A janela tem um layout vertical e é composta por três seções:

* Seletor de gradiente (ou espectro)
* Controles deslizantes (RGB/HSV)
* Amostras

![](../assets/colorpicker-7.jpg){width="200px"}

### Seletor de gradiente (espectro)

| Nome e visual | Descrição |
| --- | --- |
| **Seletor de exibição** <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r1-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../assets/display-selector.png" width="250px"/></div> | Permitir a escolha da exibição a ser usada para editar cores (espectro e controles deslizantes). O valor padrão corresponde ao Display usado pelo visor principal.  **Observação:** esta configuração só está disponível quando o [gerenciamento de cores](../features/color-management/color-management.md) está habilitado. |
| **Espectro** <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r2-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../assets/spectrum.png" width="250px"/></div> | O controle deslizante vertical é o matiz geral. Permite selecionar o tom de cor a ser exibido no campo de gradiente.Depois que o tom geral é selecionado, é possível segurar e arrastar o cursor de mira no campo de gradiente para selecionar a cor desejada.  **Observação:** quando o [gerenciamento de cores](../features/color-management/color-management.md) estiver habilitado, as cores HDR da exibição atual serão fixadas (no espaço de cores de trabalho). Isso serve para evitar o valor de saída HDR em canais com gerenciamento de cores. |
| **Cores atual e anterior** <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r3-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../assets/color-preview-current.png"/></div> | O retângulo esquerdo indica a cor final que será saída do seletor de cores.O retângulo à direita mostra a cor anterior (quando o seletor de cores foi aberto). É possível clicar nela para restaurar a cor anterior e torná-la a atual. |
| **Campo hexadecimal** <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r4-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../assets/hexa-field.png"/></div> | Os campos hexadecimais representam a cor atual como valores hexadecimais. Os componentes RGB são representados como um par de letras.Por exemplo, #FF0000 representa a cor vermelha.  **Observação:** quando o [gerenciamento de cores](../features/color-management/color-management.md) está habilitado, o campo hexadecimal sempre funciona no espaço de cores sRGB padrão para facilitar a cópia/colagem de valores entre softwares, independentemente da exibição atual ou do espaço de trabalho usado pelo projeto. |
| **Conta-gotas** <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r5-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../assets/picker.png"/></div> | O conta-gotas pode ser usado para escolher uma cor de uma origem externa. Para usá-lo, **clique** no ícone, mova o mouse e, novamente, para copiar a cor desejada.  **Observação:** ao selecionar uma cor dentro do visor, é possível usar o modificador **Shift** para escolher o canal atual editado diretamente. Isso evita a conversão de cores com perdas entre a textura original e a cor exibida na tela. Isso também é útil para escolher cores sem precisar alternar do modo de exibição **Material**. <div><img data-preserve-html="true" src="../assets/eyedropper-shift.png" width="150"/></div>  **Observação:** os campos de cores também possuem um conta-gotas ao lado deles e podem ser usados para escolher rapidamente as cores sem que seja necessário abrir o seletor de cores. <div><img data-preserve-html="true" height="83" src="../assets/eyedropper.jpg"/></div>  **Observação:** no sistema operacional Mac, o conta-gotas pode não conseguir selecionar cores fora da interface do aplicativo devido às configurações de privacidade. Para corrigir esse problema, atribua os direitos apropriados ao aplicativo em: `System Preferences > Security & Privacy > Privacy > Screen Recording` |

### Configurações de cores

| Configuração | Descrição |
| --- | --- |
| **Espaço de cores do conta-gotas** | Especifique o espaço da cor para a cor selecionada fora da viewport.A configuração **automática** usa o espaço de cores sRGB padrão das configurações do projeto. <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table1_row-r1-column-c1_dynamic_grid_items_grid-cell_position-par_image" src="../assets/eyedropper-color-space-1.png"/></div> **Observação:** esta configuração também se aplica a conta-gotas ao lado de botões de cores.  **Observação:** as cores selecionadas na viewport também usam este perfil quando não usam o modificador Shift. |

### Controles deslizantes

Os controles deslizantes de cores permitem um ajuste manual de valores individuais.

Os controles deslizantes podem ser definidos em dois modos diferentes: **HSV** ou **RGB**. Para alterar o modo, use o menu suspenso dedicado.

![](../assets/slider-mode.png)

#### HSV

**HSV** significa **H** ue, **S** aturation e **V** alue.

O **Matiz** permite percorrer as famílias de cores globais, de forma muito semelhante ao controle deslizante de degradê vertical.

![](../assets/colorpicker-hue.gif)

A **Saturação** controla a intensidade da cor selecionada e vai de tons de cinza a totalmente saturados.

![](../assets/colorpicker-saturation.gif)

O **valor** determina o quão escura ou clara é uma cor, e varia de totalmente preto a totalmente branco.

![](../assets/colorpicker-value.gif)

#### RGB

**RGB** significa **R** ed, **G** reen e **B** lue.

Esses são os principais componentes usados digitalmente para armazenar cores em gráficos de computador. Cada controle deslizante representa quanto do componente está presente na cor final.

Exemplo: a imagem abaixo tem uma cor que contém 100% de vermelho, mas 50% de azul e verde.

![](../assets/rgb-4.jpg)

É mais comum ter os controles deslizantes de RGB medidos por meio de valores de 0 a 255. Isso pode ser feito desabilitando a opção **Valores de ponto flutuante**.

![](../assets/255.jpg)

### Configurações dos controles deslizantes

![](../assets/settings-menu-1.png)

O menu de configurações permite definir alguns comportamentos adicionais:

| Configuração | Descrição |
| --- | --- |
| **Controles deslizantes dinâmicos** | Se ativada, a cor de fundo dos controles deslizantes será ajustada com base na cor atual. |
| **Valores de ponto flutuante** | Se ativado, os valores dos controles deslizantes são representados indo de 0.0 a 1.0. Se desativado:<ul data-preserve-html="true"> <li data-preserve-html="true"><strong>HSV</strong>: o controle deslizante de matiz é medido em graus (como um disco de cores). Porcentagens de uso de Saturação e Valor. </li> <li data-preserve-html="true"><strong>RGB</strong>: componentes são representados como valor indo de 0 a 255.</li> </ul> |

## Espaço de cores de trabalho

![](../assets/working-space-value.png)

Esta seção mostra o valor da cor final de acordo com o espaço da cor de trabalho atual.

Passar o título do **Espaço de cores de trabalho** com o mouse permite exibir o nome do espaço de cores atual.

>[!NOTE]
>
> Esta seção só está disponível quando o [gerenciamento de cores](../features/color-management/color-management.md) está habilitado.

## Amostras

![](../assets/swatches-overview.png)

As amostras de cores oferecem uma maneira de salvar cores para que elas possam ser reutilizadas posteriormente. As amostras estão disponíveis em todas as projeções e sessões.

### Adicionar amostra

![](../assets/add-swatch-4.png)

Clicar neste botão criará uma nova amostra de cor no conjunto atual.

A cor de amostra é criada somente se a última cor (a próxima ao botão) for diferente da cor atualmente editada.

>[!NOTE]
>
> As amostras de cores são gerenciadas e salvas como cores sRGB, independentemente da configuração atual de [gerenciamento de cores](../features/color-management/color-management.md) definida.

### Cor da amostra

![](../assets/swatch-selection.png)

Clique em uma cor de amostra para carregá-la.

Passar o mouse sobre a amostra exibirá seu valor hexadecimal.

>[!NOTE]
>
> Quando o [gerenciamento de cores](../features/color-management/color-management.md) está habilitado, a exibição das cores é ajustada com base na Exibição atualmente selecionada.

### Configurações de amostra

![](../assets/delete-swatch.png)

Clique com o botão direito do mouse em uma cor de amostra para abrir o menu e excluí-lo.

### Menu Configurações

![](../assets/delete-all-swatches.png)

Use o menu de configurações para excluir todas as amostras.

>[!NOTE]
>
> As amostras são salvas em um arquivo de configuração disponível na pasta de documentos do usuário. Para obter mais informações, consulte a página [Local de prateleira e ativos](../pipeline-and-integration/resource-management/shelf-and-assets-location.md).
