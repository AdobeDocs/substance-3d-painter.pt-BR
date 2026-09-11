---
helpx_url: "https://helpx.adobe.com/br/substance-3d-painter/technical-support/technical-issues/miscellaneous-issues/error-with-missing-api-ms-crt-dll.html"
breadcrumb-title: ''
description: Saiba como corrigir erros de DLL de api-ms-crt ausentes no Substance 3D Painter para obter suporte adequado à biblioteca no tempo de execução do Windows.
helpx_creative_field: ""
helpx_description: Painter > Technical support > Technical Issues > Miscellaneous Issues > Error with missing api-ms-crt dll
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Erro com dll api-ms-crt ausente
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '201'
ht-degree: 0%

---


# Erro com dll api-ms-crt ausente

O Substance 3D Painter não pode ser iniciado porque **api-ms-win-crt-runtime-l1-1-0.dll** não está no computador.\
Provavelmente, isso ocorreu porque a atualização KB2999226, que faz parte do **Visual C++ Redistributable** para Visual Studio 2015, falhou ao instalar.

## Como corrigir o problema?

### 1 - Verificar se o Windows está atualizado

1. Abrir o menu Iniciar
1. Selecionar Painel de Controle
1. Clique em **Windows Update**
1. Clique em **Verificar atualizações**
1. **Instalar** todas as atualizações disponíveis.
1. Após a instalação das atualizações, **reinicie** o computador.

Após a reinicialização, repita as etapas acima até que não haja mais atualizações disponíveis.

### 2 - Instalar o Visual C++ Redistribuível

1. Baixe o Visual C++ Redistributable:
   1. Para [Windows 64 bits](http://download.microsoft.com/download/9/3/F/93FCF1E7-E6A4-478B-96E7-D4B285925B00/vc_redist.x64.exe)
   1. Para [Windows 32 bits](http://download.microsoft.com/download/9/3/F/93FCF1E7-E6A4-478B-96E7-D4B285925B00/vc_redist.x86.exe)
1. Execute o **vcredist\_x64.exe** (64 bits) ou o **vcredist\_x86.exe** (32 bits)
1. Selecione Desinstalar e siga o procedimento
1. Executar o executável novamente
1. Selecione Instalar
