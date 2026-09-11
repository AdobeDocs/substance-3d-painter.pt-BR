---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/technical-support/workflow-issues/project-issues/preserve-brush-strokes-setting-stays-disabled.html"
breadcrumb-title: ''
description: Saiba como corrigir a configuração preservar traçados de pincel permanecendo desativada no Substance 3D Painter para a preservação adequada do traçado do pincel.
helpx_creative_field: ""
helpx_description: Painter > Technical support > Workflow Issues > Project Issues > Preserve brush strokes setting stays disabled
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: A configuração Preservar traçados de pincel permanece desativada
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '162'
ht-degree: 0%

---


# A configuração Preservar traçados de pincel permanece desativada

Devido a um erro infeliz introduzido no Substance 3D Painter 1.5 (parcialmente corrigido no 1.7), alguns projetos perderam metadados relacionados à malha. Este erro faz com que a configuração “Preservar posições de traços na malha” na janela [Configuração de Projeto](../../../interface/project-configuration.md) permaneça desabilitada.

Para resolver o problema, algumas etapas específicas precisam ser seguidas:

* Abra o projeto com o problema no Substance 3D Painter 1.7 ou superior
* Acesse Editar > Configuração do projeto
* Selecione e importe novamente a malha original usada no projeto atual (não a versão atualizada)
* Valide e deixe o Substance 3D Painter calcular as camadas, nada deve mudar se for a mesma malha
* Vá novamente para Editar > Configuração do projeto
* “Preservar posições de traçados na malha” agora deve ser ativado novamente, permitindo importar a nova malha
