---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/technical-support/technical-issues/startup-issues/crash-or-freeze-during-startup.html"
breadcrumb-title: ''
description: Saiba como corrigir falhas e congelamentos durante a inicialização do Substance 3D Painter para uma inicialização estável do aplicativo.
helpx_creative_field: ""
helpx_description: Painter > Technical support > Technical Issues > Startup Issues > Crash or freeze during startup
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Falha ou congelamento durante a inicialização
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '618'
ht-degree: 0%

---


# Falha ou congelamento durante a inicialização

Esta página lista os problemas conhecidos e suas soluções relacionadas ao aplicativo que não inicializa corretamente.

## Conflitos de software

Confira a seguinte página para obter uma lista de todos os softwares conhecidos que podem criar conflitos: [Conflitos de software](software-conflicts.md).

## Execução na GPU errada

Se o aplicativo não for iniciado na GPU correta, ele pode levar a problemas de estabilidade. Consulte esta página para obter mais informações: [O Painter não inicia na GPU correta](../gpu-issues/painter-doesn-t-start-on-the-right-gpu.md).

## Drivers de GPU desatualizados

O uso de drivers de GPU antigos pode levar a congelamentos e/ou falhas. Recomendamos usar os drivers de GPU mais recentes quando disponíveis. Consulte: [A GPU tem drivers desatualizados](../gpu-issues/gpu-has-outdated-drivers.md).

## Tela branca e sem resposta

Se o aplicativo congelar logo ao ser inicializado no Windows (levando a uma tela branca), pode ser por alguns motivos:

* Um aplicativo externo está criando um conflito. Consulte [Conflitos de software](software-conflicts.md) para saber quais conflitos estão ocorrendo.
* Algumas janelas do aplicativo foram abertas em outro monitor. Restaurar a interface para o layout padrão permite iniciar o aplicativo normalmente:
  1. Abra o editor do Registro (**regedit** do menu Iniciar)
  1. Navegue até as preferências do aplicativo (consulte: [Preferências e local dos dados do aplicativo](https://helpx.adobe.com/substance-3d/unlisted/documentation/spdoc/application-preferences-location-147095594.html))
  1. Expandir a chave do **Adobe Substance 3D Painter**
  1. Selecione a chave da **janela principal 2018** e exclua-a
  1. Reiniciar o aplicativo

## Falha devido a Caminho do sistema/Caminho Python incorreto

O aplicativo verifica o caminho do sistema para carregar módulos Python e configurações de ambiente. Se o sistema tiver uma configuração incorreta, ele pode levar a um travamento durante a inicialização.

No Windows:

1. Abrir o menu **Iniciar**
1. Procure e selecione o **Sistema (Painel de Controle)**
1. Clique em **Configurações avançadas do sistema**
1. Clique em **Variáveis de Ambiente**
1. Em **Variáveis do Sistema**, localize a variável **PATH**

Em seguida, você pode editar a variável para verificar seu conteúdo. Por exemplo, se a variável contiver este tipo de caracteres, ela levará a uma falha

```
ï–›éŒ à €è¸€ì‡ì‡ç¿¹
```


## Atualizações do Windows 10

Algumas atualizações do Windows 10 podem, às vezes, criar instabilidades. Use as ferramentas de diagnóstico fornecidas com o Windows para detectar possíveis erros no sistema.

Recomendamos executar a **Manutenção e Gerenciamento de Imagens de Implantação** (DISM) e a ferramenta **Verificador de Arquivos do Sistema** (SFC). O DISM é útil para recuperar os arquivos de substituição necessários para o SFC corrigir arquivos de sistema corrompidos ou ausentes.

Executando **DISM** :

1. Abrir o menu Iniciar
1. Procurar Prompt de Comando
1. Clique com o botão direito no resultado e escolha “Executar como administrador”
1. Digite o seguinte comando: **DISM /Online /Cleanup-Image /RestoreHealth**
1. Pressione Enter

Executando **SFC** :

1. Abrir o menu Iniciar
1. Procurar Prompt de Comando
1. Clique com o botão direito no resultado e escolha “Executar como administrador”
1. Digite o seguinte comando: **sfc /scannow**
1. Pressione Enter

Reinicie o computador depois dos dois comandos para aplicar as atualizações.

Para obter mais informações sobre este assunto, consulte: [Use a ferramenta Verificador de Arquivos do Sistema para reparar arquivos do sistema ausentes ou corrompidos](https://support.microsoft.com/en-us/help/929833/use-the-system-file-checker-tool-to-repair-missing-or-corrupted-system).

## Falha ao iniciar em versões mais antigas

No Windows, a versão 2018 (4.x) ou anterior pode não ser iniciada porque um dos arquivos dll fornecidos com a pasta de instalação é muito antigo para o sistema operacional. Essa falha pode ser corrigida substituindo manualmente o arquivo por uma versão mais recente.

Para fazer isso:

1. Acesse a pasta de instalação do Substance Painter.
1. Renomeie o arquivo <b>libeay32.dll</b> em <b>backup\_libeay32.dll</b>.
1. Baixe o seguinte arquivo: [updated\_libeay32.zip](https://helpx.adobe.com/content/dam/help/en/substance-3d/documentation/spdoc/files/182266673/225968681/1/1644000679697/updated-libeay32.zip).
1. Extraia o arquivo dll do arquivo zip para a pasta de instalação (ao lado do arquivo Substance Painter.exe).
1. Inicie o aplicativo.
