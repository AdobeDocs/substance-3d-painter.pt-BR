---
helpx_url: "https://helpx.adobe.com/br/substance-3d-painter/painting/presets/photoshop-brush-presets-abr/photoshop-brush-parameters-compatibility.html"
breadcrumb-title: ''
description: Saiba mais sobre a compatibilidade de parâmetros de pincel do Photoshop no Substance 3D Painter ao importar predefinições de pincel ABR.
helpx_creative_field: ""
helpx_description: Painter > Painting > Presets > Photoshop Brush Presets (ABR) > Photoshop Brush Parameters Compatibility
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Compatibilidade dos parâmetros do pincel Photoshop
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '645'
ht-degree: 1%

---


# Compatibilidade dos parâmetros do pincel Photoshop

Esta página lista todos os parâmetros de pincel do Photoshop e seus compatibilidade com o mecanismo de pincel do Substance 3D Painter.

## Compatibilidade geral

Ao olhar dentro do arquivo ABR, o Substance 3D Painter recuperará apenas predefinições específicas de Pincel/Ferramenta:

| *Tipo de predefinição* | *Suporte* | *Descrição* |
| --- | --- | --- |
| **Pincel (bitmap)** | Importado | Predefinições de pincel baseadas em bitmaps, pois seus alfas serão importados. |
| **Pincel (procedimento)** | Ignorado | As predefinições de pincel baseadas em formas de procedimento (como um círculo) não são importadas. |
| **Pincel (Aerógrafo)** | Ignorado | As predefinições de pincel com configurações de aerógrafo não são importadas. |
| **Pincel (Cerdas)** | Ignorado | As predefinições de pincel com configurações de cerdas não são importadas. |
| **Pincel (Erodível)** | Ignorado | As predefinições de pincel com configurações Erodible não são importadas. |
| **Lápis** | Ignorado | As predefinições de lápis não são importadas. |
| **Pincel de mistura** | Ignorado | As predefinições de pincel de mistura não são importadas. |
| **Carimbo** | Ignorado | As predefinições do Carimbo não são importadas. |
| **Borrar** | Ignorado | As predefinições de borrar não são importadas. |

## Parâmetros

Para saber mais sobre o que esses parâmetros podem fazer, consulte a [documentação oficial da Photoshop](https://helpx.adobe.com/br/photoshop/using/creating-modifying-brushes.html).

Nem todos os parâmetros de pincel Photoshop são compatíveis. Consulte a legenda para saber o status de cada parâmetro descrito abaixo:

* **Quadrado (■)** : indica que há suporte para o parâmetro, consulte a descrição para saber como acessá-lo.
* **Cruz (✖)** : indica que o parâmetro não tem suporte.

>[!NOTE]
>
> Embora os parâmetros de controle nas predefinições de pincel possam ser controlados por vários métodos, como Inclinação da caneta, Atenuação e Pressão da caneta, somente a **Pressão da caneta** é suportada atualmente.

| *Grupo* | *Parâmetro* | *Suporte* | *Descrição* |
| --- | --- | --- | --- |
| Forma da ponta do pincel | **Tamanho** | ■ | Correspondente ao parâmetro Tamanho da ferramenta Pintura.  **Observação:** o Photoshop define o tamanho em pixels, enquanto o tamanho do Substance 3D Painter se baseia na Caixa Delimitadora do projeto. Uma correspondência exata não é, portanto, possível e será apenas relativa. |
| **Inverter X** | ■ | Manuseado pelo arquivo de Substance “Brush Maker Photoshop”. |  |
| **Inverter Y** | ■ | Manuseado pelo arquivo de Substance “Brush Maker Photoshop”. |  |
| **Ângulo** | ■ | Correspondente ao parâmetro Ângulo da ferramenta Pintura. |  |
| **Arredondamento** | ■ | Manuseado pelo arquivo de Substance “Brush Maker Photoshop”. |  |
| **Dureza** | ■ | Manuseado pelo arquivo de Substance “Brush Maker Photoshop”. |  |
| **Espaçamento** | ■ | Correspondente ao parâmetro de espaçamento da ferramenta Pintura. |  |
|  |  |  |  |
| Dinâmica da forma | **Tremulação de tamanho** | ■ | Correspondente ao parâmetro de tremulação de tamanho da ferramenta Pintura. |
| **Controle (para Tamanho)** | ■ | Correspondente à configuração de pressão da ferramenta de pintura do parâmetro Tamanho . |  |
| **Diâmetro Mínimo** | ■ | Correspondente ao parâmetro Tamanho mínimo da ferramenta Pintura. |  |
| **Escala de Inclinação** | ✖ |  |  |
| **Tremulação de ângulo** | ■ | Correspondente ao parâmetro Tremulação de ângulo da ferramenta Pintura. |  |
| **Controle (para Ângulo)** | ✖ |  |  |
| **Tremulação de arredondamento** | ■ | Manuseado pelo arquivo de Substance “Brush Maker Photoshop”. |  |
| **Arredondamento Mínimo** | ■ | Manuseado pelo arquivo de Substance “Brush Maker Photoshop”. |  |
| **Inverter tremulação X** | ■ | Manuseado pelo arquivo de Substance “Brush Maker Photoshop”. |  |
| **Inverter tremulação Y** | ■ | Manuseado pelo arquivo de Substance “Brush Maker Photoshop”. |  |
| **Projeção de pincel** | ✖ |  |  |
|  |  |  |  |
| Dispersão | **Dispersão** | ■ | Correspondente ao parâmetro de tremulação de posição da ferramenta Pintura. |
| **Ambos os Eixos** | ■ | Correspondente ao parâmetro do Eixo de tremulação de posição da ferramenta Pintura. |  |
| **Controle (para Dispersão)** | ✖ |  |  |
| **Contagem** | ■ | Compensado por meio do parâmetro Espaçamento da ferramenta Pintura. |  |
| **Contar tremulação** | ✖ |  |  |
| **Controle (para Tremulação de Contagem)** | ✖ |  |  |
|  |  |  |  |
| Textura | **Padrão de Textura** | ✖ |  |
| **Inverter** | ✖ |  |  |
| **Escala** | ✖ |  |  |
| **Brilho** | ✖ |  |  |
| **Contraste** | ✖ |  |  |
| **Texturizar Cada Ponta** | ✖ |  |  |
| **Modo** | ✖ |  |  |
| **Profundidade** | ✖ |  |  |
| **Profundidade Mínima** | ✖ |  |  |
| **Tremulação de Profundidade** | ✖ |  |  |
| **Controle (para tremulação de Profundidade)** | ✖ |  |  |
|  |  |  |  |
| Pincel duplo | **Modo** | ✖ |  |
| **Tamanho** | ✖ |  |  |
| **Espaçamento** | ✖ |  |  |
| **Dispersão** | ✖ |  |  |
| **Ambos os Eixos** | ✖ |  |  |
| **Contagem** | ✖ |  |  |
|  |  |  |  |
| Dinâmica de cores | **Aplicar por ponta** | ✖ |  |
| **Tremulação de Primeiro Plano/Plano de Fundo** | ✖ |  |  |
| **Controle (para tremulação F/B)** | ✖ |  |  |
| **Tremulação de matiz** | ✖ |  |  |
| **Tremulação de saturação** | ✖ |  |  |
| **Tremulação de brilho** | ✖ |  |  |
| **Pureza** | ✖ |  |  |
|  |  |  |  |
| Transferir | **Tremulação de opacidade** | ■ | Correspondente à ferramenta Pintura Carimba o parâmetro de mesclagem definido como “Clarear”. |
| **Controle (para Opacidade)** | ■ | Correspondente à configuração de pressão da ferramenta Pintura para o parâmetro Fluxo. |  |
| **Mínimo (para controle de opacidade)** | ■ | Correspondente ao parâmetro Fluxo mínimo da ferramenta Pintura. |  |
| **Tremulação de fluxo** | ■ | Correspondente ao parâmetro de tremulação de fluxo da ferramenta Pintura. |  |
| **Controle (para Fluxo)** | ■ | Correspondente à configuração de Pressão da ferramenta Pintura para o parâmetro Fluxo (se for inferior a Opacidade). |  |
| **Mínimo (para Controle de Fluxo)** | ■ | Correspondente ao parâmetro Fluxo mínimo da ferramenta Pintura (se inferior a Opacidade). |  |
| **Tremulação de umidade** | ✖ |  |  |
| **Controle (para tremulação de umidade)** | ✖ |  |  |
| **Mínimo (para o Controle de Umidade)** | ✖ |  |  |
| **Tremulação de mix** | ✖ |  |  |
| **Controle (para Mix)** | ✖ |  |  |
| **Mínimo (para Controle de Combinação)** | ✖ |  |  |
|  |  |  |  |
| Posição do pincel | **Inclinação X** | ✖ |  |
| **Substituir Inclinação X** | ✖ |  |  |
| **Inclinar Y** | ✖ |  |  |
| **Substituir Inclinação Y** | ✖ |  |  |
| **Rotação** | ✖ |  |  |
| **Substituir Rotação** | ✖ |  |  |
| **Pressão** | ✖ |  |  |
| **Substituir Pressão** | ✖ |  |  |
|  |  |  |  |
| Outro | **Ruído** | ✖ |  |
| **Bordas Molhadas** | ✖ |  |  |
| **Compilação** | ✖ |  |  |
| **Suavização** | ■ | Não correspondida diretamente, mas pode ser tratada pela configuração [Mouse Lento](../../lazy-mouse.md). |  |
| **Textura do Protect** | ✖ |  |  |
