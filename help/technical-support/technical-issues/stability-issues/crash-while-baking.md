---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/technical-support/technical-issues/stability-issues/crash-while-baking.html"
breadcrumb-title: ''
description: Saiba como corrigir falhas do Substance 3D Painter durante as operações de cozimento para obter fluxos de trabalho de cozimento de textura confiáveis.
helpx_creative_field: ""
helpx_description: Painter > Technical support > Technical Issues > Stability Issues > Crash while baking
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Falha durante a cozedura
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '278'
ht-degree: 0%

---


# Falha durante a cozedura

O Substance 3D Painter pode travar durante o processo de cozimento em algumas configurações. Esta página agrupa uma lista de problemas conhecidos e como mitigá-los.

## Falha com a visualização de preparo

Por padrão, o Substance 3D Painter exibe no visor o estado em andamento da cozimento de uma textura. Em alguns computadores, esse recurso pode causar instabilidades.

Para desativá-la:

1. Use **Editar > Configurações** para abrir as configurações principais
1. Em **Geral**, rola para baixo até a seção denominada **Opções de Preparação**.
1. Desmarque/desabilite a opção **Habilitar processo de preparação de visualização ao vivo** .

## Falha com Rastreamento de raios do GPU

Em algumas GPUs com drivers instáveis, o processo de cozimento pode levar a falhas devido ao recurso de Rastreamento de raios do GPU.

Para desativá-la:

1. Use **Editar > Configurações** para abrir as configurações principais
1. Em **Geral**, rola para baixo até a seção denominada **Opções de Preparação**.
1. Desmarque/Desabilite a opção **Habilitar Rastreamento de raios do GPU**.

## Falha com CPUs Ryzen

O aplicativo pode travar durante o processo de cozimento em alguma configuração de computador em execução com uma CPU Ryzen. Em geral, uma atualização do BIOS corrige o problema.

Isso está relacionado a cálculos multi-threaded. Muitos construtores de motherboard lançaram novas atualizações do BIOS para corrigir esse problema, então recomendamos aplicar a atualização. Consulte o Manual da motherboard e o site do construtor para mais informações.

## Arquivos Assbin incompatíveis

Por padrão, ao assar, as malhas de alto polígono são pré-processadas em arquivos **\*.assbin** para acelerar o retorno mais tarde. Em alguns casos raros, esses arquivos podem travar o aplicativo se tiverem sido gerados com uma versão diferente. Simplesmente excluí-los deve resolver o problema, pois eles serão regenerados.
