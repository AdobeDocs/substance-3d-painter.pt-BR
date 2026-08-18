---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/features/color-management.html"
breadcrumb-title: ''
description: Saiba como configurar o gerenciamento de cores no Substance 3D Painter para garantir uma precisão de cores consistente em todo o fluxo de trabalho.
helpx_creative_field: ""
helpx_description: Painter > Features > Color management
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Gerenciamento de cores
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '732'
ht-degree: 4%

---


# Gerenciamento de cores

![](../../assets/banner-cm-doc.jpg)

O gerenciamento de cores é a manipulação e a conversão de cores. Desde a importação de recursos à exibição de cores na tela até a exportação final de texturas. A calibração de cores é importante para garantir a mesma aparência em todos os aplicativos.

No aplicativo, o gerenciamento de cores é processado por meio da integração do [OpenColorIO](https://opencolorio.org/) (OCIO para short) versão 2. OCIO é o padrão em filme e animação para converter e exibir cores. Para ativar o gerenciamento de cores, basta criar um novo projeto ou abrir um existente e ativar as configurações dedicadas.

>[!NOTE]
>
> O gerenciamento de cores está disponível desde a versão 7.4.0.

## Configurações do projeto

Configurações de gerenciamento de cores:

* [Gerenciamento de cores com Adobe ACE - ICC](color-management-with-adobe-ace-icc.md)
* [Gerenciamento de cores com o OpenColorIO](color-management-with-opencolorio.md)

## Vocabulário

Pode ser útil conhecer alguns termos técnicos relacionados ao gerenciamento de cores para entender melhor o fluxo de trabalho associado:

| Palavra-chave | Descrição |
| --- | --- |
| **Espaço de cores** | Sistema de coordenadas no qual as cores são definidas. |
| **Espaço de trabalho** | O espaço de cores usado dentro do aplicativo para mesclar textura, pintura etc. |
| **Transformação de exibição** | A transformação de exibição converte as cores lineares do espaço de trabalho para o espaço de cores do monitor para exibir cores perceptivamente (para serem vistas pelos olhos humanos). As transformações de exibição geralmente incluem uma passagem de mapeamento de tons para compactar cores a fim de se ajustarem à faixa limitada de valores permitida por uma tela. |
| **Configuração** | Um arquivo de configuração OCIO. Define o que é o espaço de trabalho, uma lista de espaços de cores e uma lista de transformações de vídeo. |
| **ACES** | ACES significa Academy Color Encoding System e é o padrão em muitos aplicativos para troca de arquivos de imagem digital. Duas versões deste padrão estão incluídas dentro do aplicativo por padrão. |
| **Mapeamento de tons** | É o processo de mapeamento de valores de cor de HDR (intervalo dinâmico) para LDR (intervalo dinâmico baixo). Esse processo ajuda a exibir uma exibição aproximada de uma ampla variedade de cores. |

## Lista de canais gerenciados por cores

Dentro do aplicativo, quais canais são gerenciados por cores ou não (dados/passagem) são predefinidos.

| Canal | A cor é gerenciada |
| --- | --- |
| **oclusão de ambiente** | Não |
| **Ângulo de anistotropia** | Não |
| **Nível de Anisotropia** | Não |
| **Cor base** | **Sim** |
| **Máscara de mesclagem** | Não |
| **Cor do revestimento** | **Sim** |
| **Revestimento normal** | Não |
| **Opacidade da camada** | Não |
| **Aspereza do revestimento** | Não |
| **specular level de revestimento** | Não |
| **Difusa** | **Sim** |
| **Deslocamento** | Não |
| **Textura reluzente** | Não |
| **Height** | Não |
| **Ior** | Não |
| **Metálico** | Não |
| **Normal** | Não |
| **Opacidade** | Não |
| **Reflexo** | Não |
| **Aspereza** | Não |
| **Dispersão** | Não |
| **Dispersão de cores** | **Sim** |
| **Cor do brilho** | **Sim** |
| **Opacidade do brilho** | Não |
| **Aspereza de brilho** | Não |
| **Specular** | **Sim** |
| **Specular edge color** | **Sim** |
| **Specular level** | Não |
| **Transparência** | Não |
| **Transmissivo** | **Sim** |
| **UserX (0-15)** | Depende das [configurações do Conjunto de Texturas](../../interface/texture-set/texture-set-settings.md). Por padrão, os canais do usuário não são gerenciados por cores. <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r31-column-c1_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/user-demo.png"/></div> |

## Seletor de cores

Quando o gerenciamento de cores está habilitado, o comportamento do [seletor de cores](../../interface/color-picker.md) muda um pouco:

* As cores são editadas com base na exibição atual selecionada.
* Algumas informações adicionais são adicionadas à interface.

Para obter mais informações, consulte a [página de documentação](../../interface/color-picker.md) do seletor de cores.

## Controles do visor

Ambas as visualizações 2D e 3D têm gerenciamento de cores e uma configuração dedicada disponível na parte superior da janela de visualização para controlar qual transformação de exibição usar:

![](../../assets/viewport-cm.png)

* **Botão esquerdo**: habilitar/desabilitar a transformação de exibição do visor. Se desativada, a viewport exibirá cores como raw/passthrough. Esse botão fica ativado por padrão.
* **Menu suspenso de direita**: especifique qual transformação de exibição usar para converter as cores para exibi-las na tela. O valor padrão é baseado na configuração OCIO. Esta configuração não é salva com o projeto, pois ele pode ser dependente do monitor.

>[!NOTE]
>
> No modo solo (visualizando canais individualmente), o gerenciamento de cores é automaticamente desativado ao visualizar canais de dados (veja a lista acima).

## Exportar configurações

As principais configurações de exportação são orientadas pela configuração do projeto (veja acima).

Dentro da janela [exportar texturas](../../export/export.md), há uma palavra-chave que pode ser usada para acrescentar aos nomes de arquivo o espaço de cores usado por textura: **$colorSpace**.

<table>
<tr style="border: 0;">
<td style="border: 0;" valign="top">

![](../../assets/export-list-1.png){width="320px"}

</td>
<td style="border: 0;" valign="top">

![](../../assets/export-list-2.png){width="500px"}

</td>
</tr>
</table>

## Substituição de espaços de cores

Talvez seja necessário especificar um espaço de cores alternativo para que um recurso seja diferente dos padrões. Isso pode ser feito por meio do menu espaço de cores.

### Alterar o espaço de cores de um recurso

Dentro da [janela de propriedades](../../interface/properties.md) é possível substituir o espaço de cores de um recurso específico (onde ele é usado atualmente).

Para fazer isso, expanda a seção do espaço de cores e use o menu suspenso para especificar o novo espaço de cores:

![](../../assets/color-space-menu.png)

### Alterar o espaço de cores do mapa de ambiente

Dentro das [configurações de exibição](../../interface/display-settings/display-settings.md), habilite o **espaço de cores Substituir mapa de ambiente** e escolha um espaço de cores na lista que corresponda ao seu recurso.

![](../../assets/color-sace-menu-env.png)
