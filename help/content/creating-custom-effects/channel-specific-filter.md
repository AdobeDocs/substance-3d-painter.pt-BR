---
helpx_url: "https://helpx.adobe.com/br/substance-3d-painter/content/creating-custom-effects/channel-specific-filter.html"
breadcrumb-title: ''
description: Saiba como criar efeitos de filtro específicos do canal para que o Substance 3D Painter processe canais de textura individuais.
helpx_creative_field: ""
helpx_description: Painter > Content > Creating custom effects > Channel specific filter
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Filtro específico do canal
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '455'
ht-degree: 0%

---


# Filtro específico do canal

Um efeito pode ser específico a um canal específico. Nesse caso, se você quiser afetar um canal específico, será necessário criar uma entrada E uma saída que identifique esse canal. Como regra geral, a estrutura de entrada/saída deve sempre respeitar uma regra de 1:1. Se desejar inserir um canal específico, será necessário gerar a saída do mesmo canal.

Exemplo de um filtro que afeta somente o canal **basecolor**:

![](../../assets/specific-filter-basecolor.png)

>[!NOTE]
>
> Não é possível combinar a configuração genérica (nós de entrada/saída) e canais específicos (basecolor/basecolor).

## gerenciamento de componente de Alpha

Canais armazenados como RGBA suportam alfa (basecolor por exemplo). Para esses canais, a entrada/saída alfa pode ser armazenada diretamente na saída de cores do Substance. No entanto, o mecanismo Substance não suporta Alpha para imagens em tons de cinza: ele tem que ser gerenciado usando um mapa secundário. Para obter o componente alfa de um canal específico em um gráfico do substance, crie uma entrada em tons de cinza denominada &#39;**channelname\_Alpha**&#39;, exemplo: **basecolor\_Alpha**, **rugosidade\_Alpha** e assim por diante.\
Para gerar a saída desse componente alfa, crie um nó de saída com a mesma convenção de nome.

>[!NOTE]
>
> A saída específica “**\_Alpha**” por canal não funciona com **materiais** comuns. Para ocultar um canal com uma máscara, uma saída específica deve ser criada com a seguinte convenção de nomenclatura:
> 
> * Identificador : **channels\_Alpha**
> * Uso: **channels\_Alpha**

## Lista de usos e identificadores de entrada/saída

>[!NOTE]
>
> É possível usar o **uso** ou o **identificador** em um nó de entrada (o uso tem a prioridade).

| Nome do canal | Uso | Identificador / Alpha do identificador |
| --- | --- | --- |
| *Oclusão de ambiente* | **ambientOcclusion** | **ambientOcclusion / ambientOcclusion\_Alpha** |
| *Ângulo de Anisotropia* | **anisotropyangle** | **anisotropyAngle / anisotropyAngle\_Alpha** |
| *Nível de Anisotropia* | **anisotropylevel** | **anisotropyLevel / anisotropyLevel\_Alpha** |
| *Cor base* | **basecolor** | **baseColor / baseColor\_Alpha** |
| *Máscara de Mesclagem* | **máscara de mesclagem** | **blendingmask / blendingmask\_Alpha** |
| *Difusa* | **difuso** | **difusa / difusa\_Alpha** |
| *Deslocamento* | **deslocamento** | **deslocamento / deslocamento\_Alpha** |
| *Emissivo* | **emissivo** | **emissivo/emissivo\_Alpha** |
| *Textura reluzente* | **textura reluzente** | **glossiness / glossiness\_Alpha** |
| *Height* | **height** | **height / height\_Alpha** |
| *IOR* | **i** | **i/i\_Alpha** |
| *Metálico* | **metálico** | **Alpha\_metálico/metálico** |
| *Normal* | **normal** | **normal / normal\_Alpha** |
| *Opacidade* | **opacidade** | **opacidade/\_Alpha** |
| *Reflexo* | **reflexo** | **reflexo/ reflexo\_Alpha** |
| *Aspereza* | **aspereza** | **aspereza / aspereza\_Alpha** |
| *Dispersão* | **dispersão** | **dispersão/dispersão\_Alpha** |
| *Specular* | **specular** | **specular / specular\_Alpha** |
| *Specular level* | **nível especulativo** | **specularLevel / specularLevel\_Alpha** |
| *Transmissivo* | **transmissivo** | **transmissivo/transmissivo\_Alpha** |
| *Usuário 0* | **usuário0** | **user0 / user0\_Alpha** |
| *Usuário 1* | **usuário1** | **user1 / user1\_Alpha** |
| *Usuário 2* | **usuário2** | **usuário2 / usuário2\_Alpha** |
| *Usuário 3* | **usuário3** | **user3 / user3\_Alpha** |
| *Usuário 4* | **usuário4** | **user4 / user4\_Alpha** |
| *Usuário 5* | **usuário5** | **user5 / user5\_Alpha** |
| *Usuário 6* | **usuário6** | **user6 / user6\_Alpha** |
| *Usuário 7* | **usuário7** | **user7 / user7\_Alpha** |

## Exemplos

![](../../assets/single-channel.png){width="650px"}

Neste exemplo, o canal alfa da Cor de Base é extraído por um nó de tons de cinza para substituir o canal **Aspereza**.

![](../../assets/mix-channel.png){width="650px"}

Neste exemplo, o canal **Aspereza** é multiplicado pela **Cor Base**.
