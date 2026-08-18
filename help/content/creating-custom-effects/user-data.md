---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/content/creating-custom-effects/user-data.html"
breadcrumb-title: ''
description: Saiba como usar dados do usuário em efeitos personalizados para que o Substance 3D Painter passe informações personalizadas para efeitos de sombreador.
helpx_creative_field: ""
helpx_description: Painter > Content > Creating custom effects > User data
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Dados do usuário
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '1175'
ht-degree: 1%

---


# Dados do usuário

Esta página descreve propriedades personalizadas (dados do usuário) que podem ser adicionadas ao gráfico de Substance para executar comportamentos específicos.\
As configurações de dados do usuário são normalmente aplicadas a nós de entrada ou saída de um gráfico para indicar como o aplicativo deve interpretá-las. Isso permite que solicitar a entrada de um gráfico para ser, de certa forma, aplicar efeitos é um contexto conhecido (por exemplo, solicitar um espaço de cores específico) ou para indicar como uma saída foi feita caso o aplicativo precise aplicar conversões extras posteriormente.

* As configurações de dados de uso estão definidas como **chave = valor**
* Várias configurações são separadas por ponto e vírgula ( **;** )

## Espaço da cor

A configuração **espaço de cores** pode ser usada para solicitar entradas de gráfico de Substance com um espaço de cores específico ou para definir uma saída configurada de determinada maneira. Por exemplo, especificar o formato da saída normal do mapa.

Exemplo de sintaxe: **colorspace=$working**

Visão geral dos contextos:

* **Botão de cores**: um widget de botão de cores nas propriedades de um gráfico de Substance.
* **Entrada/saída de gráfico**: nó de entrada ou saída de um gráfico conectado a um canal (por exemplo: BaseColor).
* **Entrada de imagem**: entrada genérica de um gráfico, não relacionada a canais específicos.

>[!NOTE]
>
> Com a introdução do gerenciamento de cores, vários comportamentos relacionados à configuração de espaços de cores foram alterados:
> 
> * A tabela abaixo lista primeiro as configurações de espaço de cor compatíveis antes da versão 8.1. A segunda seção é exclusiva da versão 8.1 e mais recentes.
> * Em relação aos contextos nos quais a configuração do espaço de cores pode ser usada, somente a partir da versão 8.1 o botão de cores pode definir um espaço de cores. Em versões anteriores, eles eram considerados como estando em espaço de exibição (sRGB).
> 
> O espaço de cores/transformações **snorm** e **unorm** não devem ser misturados com formatos de textura de GPU; seus objetivos são diferentes.

| ColorSpace | Disponibilidade de contexto | Descrição |
| --- | --- | --- |
| **automático** | Botão Cor Entrada/saída de gráfico Entrada/saída de imagem | Padrão. O aplicativo decide a conversão do espaço de cores a ser executada dependendo das propriedades do nó de entrada e da imagem conectada à entrada. |
| **linear** | Botão Cor Entrada/saída de gráfico Entrada/saída de imagem | Espaço de cores padrão sRGB IEC 61966-2-1:1999 com gama linear/curva de tons. Disponível apenas com o modo de gerenciamento de cores **herdado**. |
| **srgb** | Botão Cor Entrada/saída de gráfico Entrada/saída de imagem | Espaço de cores padrão sRGB IEC 61966-2-1:1999. Disponível apenas com o modo de gerenciamento de cores **herdado**. |
| **passagem** | Botão Cor Entrada/saída de gráfico Entrada/saída de imagem | Descontinuado. Interpretado como **linear** no modo de gerenciamento de cores herdado e **bruto** com OCIO/ACE. Deve ser substituído por **raw**. |
| **normalizar** | Entrada/saída de gráfico Entrada de imagem | Assinado normalizado. Solicite que a imagem de entrada esteja no intervalo [0, 1]. Para imagens de entrada de 8 bits, isso significa que o valor médio é 127. Para entradas de imagem flutuante, o meio é 0,5 e não executa nenhum aperto. |
| **normalxyzright** | Entrada/saída de gráfico Entrada de imagem | Formato de mapa normal OpenGL. |
| **normalxyzleft** | Entrada/saída de gráfico Entrada de imagem | formato de mapa normal de DirectX. |
|  |  |  |
| **unorm** | Entrada/saída de gráfico Entrada de imagem | Entrada flutuante, sem alcance/fixação. |
| **dados** | Botão Cor Entrada/saída de gráfico Entrada/saída de imagem | Sem sinal normalizado ou flutuante. Informação não colorida. |
| **raw** | Botão Cor Entrada/saída de gráfico Entrada/saída de imagem | Nenhuma transformação de cor é aplicada quando essa configuração é usada. |
| **$standardsrgb** | Botão Cor Entrada/saída de gráfico Entrada/saída de imagem | Espaço de cores padrão sRGB IEC 61966-2-1:1999. |
| **$trabalhando** | Botão Cor Entrada/saída de gráfico Entrada/saída de imagem | O espaço de cores de trabalho depende das configurações de gerenciamento de cores. Serão idênticos aos dados dos canais sem gerenciamento de cores e monocanal (estêncil, alfa, máscara) |
| **$raw** | Botão Cor Entrada/saída de gráfico Entrada/saída de imagem | Alias para **raw**. |
| **$auto** | Botão Cor Entrada/saída de gráfico Entrada/saída de imagem | Alias para **automático**. |

## modo Alpha

A configuração **alfa** pode ser usada para especificar como o alfa de uma entrada ou saída de cor (RGBA) é combinado.

Exemplo de sintaxe: **alpha=pré-multiplicado**

| Configuração | Descrição |
| --- | --- |
| reto | Solicite ou defina a alfa como reta. |
| pré-multiplicado | Solicite ou defina o alfa como pré-multiplicado. |
| nenhum | Passagem, use a alfa como está fornecida. |

>[!NOTE]
>
> A **Opacidade** do canal é considerada **reta** por padrão.

## Cor padrão de entrada de imagem

A cor padrão de uma entrada de imagem do gráfico de Substance é preto com seu alfa definido como 0. A configuração **defaultcolor** permite definir um valor diferente quando a entrada da imagem de um gráfico estiver vazia

É possível usar valores flutuantes (intervalo [0, 1]) ou inteiros (intervalo [0, 255]) para especificar a cor. Cada valor de componente é separado por uma vírgula, enquanto o valor de ponto flutuante usa um ponto como separador decimal. Se um ponto flutuante não tem ponto, ele será considerado como um inteiro.

Exemplo de sintaxe:

* **defaultcolor=(1.0,0.5,0.0)**
* **defaultcolor=(0,128,255)**

## Preenchimento de entrada de imagem

Por padrão, as entradas de imagem de um gráfico de Substance não têm nenhum preenchimento, a área fora da Ilha UV é geralmente preenchida com uma cor uniforme por motivos de desempenho. Em vez disso, a configuração de preenchimento pode ser usada para solicitar dilatação infinita, que pode ser usada para filtros a fim de evitar a criação de emendas, por exemplo.

Exemplo de sintaxe: **p**&#x200B;**adding=extension**

## Desativar uma saída por padrão

Ao adicionar uma substância a um slot (como o slot de material da ferramenta de uma camada de preenchimento), é possível especificar por meio do campo de texto de metadados para não ativar um canal específico:

* Em um nó de saída específico (como um material) : **disable=(true)**
* Em um nó de saída genérico (como um filtro) : **disable=(height,diffuse,specular)**

Ao carregar o substance, este canal não será habilitado na interface do usuário e, portanto, não terá efeito na pilha de camadas. O usuário ainda pode ativar o canal de volta.

## Designar uma saída como uma máscara/alfa comum

A saída de um gráfico de Substance pode ser usada como um canal alfa/máscara compartilhados nas outras saídas.

Há duas maneiras de fazer isso:

* Criar um nó de saída com o identificador **channels\_Alpha**
* Ou adicione os seguintes dados de usuário em um nó de saída específico: **IsChannelsAlpha=true**

Algumas condições podem se aplicar:

* Se um nó de saída com o identificador **channels\_Alpha** existir e outras saídas não tiverem os dados do usuário, esse nó será usado como a máscara de canais.
* Se uma saída tiver os dados do usuário, ela será usada como máscara de canais desde que não exista um nó **channels\_Alpha**.
* Se existir um nó **channels\_Alpha** e um nó com userdata, o nó de saída **channels\_Alpha** será usado primeiro.
* Se vários nós tiverem os dados do usuário, o primeiro nó encontrado pelo aplicativo será usado como a máscara de canais. A ordem em que as saídas são encontradas não é garantida para a mesma como definido pelo gráfico de Substance.

>[!NOTE]
>
> Esta configuração se aplica somente ao gráfico de Substance usado no **modo de material**. Ele não se aplica a filtros, geradores, etc.

## Definir modo de mesclagem padrão para saídas de material

É possível definir qual deve ser o modo de mesclagem de uma saída específica em um gráfico de Substance ao arrastar e soltar materiais da prateleira no visor ou na pilha de camadas.

* Em um nó de saída específico: **blendingmode=normal**

Lista de modos de mesclagem compatíveis:

* normal
* passagem
* desativar
* substituir
* multiplicar
* dividir
* inversedivide
* escurecer
* clarear
* lineardodge
* subtrair
* inversesubtract
* diferença
* exclusão
* signedadding
* sobrepor
* tela
* linearburn
* colorburn
* colordodge
* softlight
* luz rígida
* vividlight
* pinlight
* tom
* saturação
* cores
* valor
* normal combinar
* detalhe normal
* normalinversedetail
