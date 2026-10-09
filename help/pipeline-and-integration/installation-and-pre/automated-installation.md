---
breadcrumb-title: ""
description: Saiba como automatizar a instalação do Substance 3D Painter para fluxos de trabalho de implantação corporativa e integração de pipeline.
title: Instalação automatizada
user-guide-description: ""
user-guide-title: ""
source-git-commit: 6b6d52207ca1d043aaa1b2b14145b6b49d4c1942
workflow-type: tm+mt
source-wordcount: '129'
ht-degree: 0%
---

# Instalação automatizada

Ao usar o instalador autônomo do Substance 3D, é possível instalar o aplicativo no modo silencioso para facilitar a implantação.

Estamos usando o **InnoSetup** para gerar o instalador. O conjunto completo de parâmetros que pode ser usado com o instalador está [disponível aqui](http://www.jrsoftware.org/ishelp/index.php?topic=setupcmdline).

## Instalar no modo silencioso por meio da linha de comando

O sinalizador a ser usado para executar uma instalação silenciosa é **/SILENT**. O sinalizador **/NCRC** também pode ser usado para ignorar o CRC (verificação) do pacote para acelerar o processo.

Exemplo:

```
SubstancePainter_Installer.exe /NCRC /SILENT /DIR="C:InstallationFolder"
```


>[!NOTE]
>
> O caminho de instalação deve estar usando um único caractere de barra invertida para separar as pastas, caso contrário, o instalador não reconhecerá o caminho.
