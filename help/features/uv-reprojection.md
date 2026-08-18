---
helpx_url: "https://helpx.adobe.com/br/substance-3d-painter/features/uv-reprojection.html"
breadcrumb-title: ''
description: Saiba como usar a reprojeção de UV no Substance 3D Painter para transferir texturas entre diferentes layouts UV.
helpx_creative_field: ""
helpx_description: Painter > Features > UV Reprojection
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Reprojeção UV
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '378'
ht-degree: 0%

---


# Reprojeção UV

A Reprojeção de UV é um processo automático que ocorre quando você altera a resolução da textura ou importa uma nova malha.\
Se você carregar uma nova malha em seu documento (por meio da janela [Configuração de Projeto](https://substance3d.adobe.com/display/draftpainter/project%20configuration) ), todas as suas ações serão reprojetadas nessa nova malha. Não importa se a topologia mudou (desde que seja semelhante) ou se os UVs mudaram. Como a reprojeção funciona recalculando todas as camadas e traçados de pincel, pode levar um pouco de tempo (especialmente em resoluções de textura altas).

Pintura em exibição 2D

Como cada traçado feito na visualização 2D é executado no espaço UV, não há como reprojetá-lo corretamente caso o UV da malha se altere drasticamente após uma reimportação. A melhor maneira de fazer a prova de reprojeção do projeto é usar o mascaramento por um mapa de ID e outro tipo de seleção e pintura em vez da Exibição 3D.

## Como funciona a reprojeção?

O Substance 3D Painter salva seus dados em 3D no espaço global para manter tudo não destrutivo. Isso significa que, ao reimportar uma malha, o Substance 3D Painter tenta pintar onde a malha estava antes da reimportação, ele não tem como saber para onde algumas peças poderiam ter se movido.

Além disso, quando o Substance 3D Painter importa uma malha, ele calcula sua caixa delimitadora para registrar o espaço e definir uma escala relativa para as ferramentas (pincel de pintura, partículas etc.). Essa Caixa delimitadora tem 1 unidade de largura em cada eixo. Ao importar uma nova malha, se desmarcar a opção “preservar traçado”, normalizaremos a caixa delimitadora para a nova malha. Portanto, se a malha for alterada drasticamente em tamanho, os traçados poderão se mover. No entanto, se você marcar a opção “preservar traçados”, redimensionamos a caixa delimitadora original para a nova para reprojetar corretamente os traçados do pincel.

>[!WARNING]
>
> Alterar as unidades da malha 3D pode fazer com que a reprojeção de UV não funcione; a malha antiga e a nova, mesmo que a topologia não tenha sido alterada, podem ser interpretadas como escalas muito diferentes. De preferência, evite alterar a configuração da unidade, pois isso pode ser difícil de corrigir.
