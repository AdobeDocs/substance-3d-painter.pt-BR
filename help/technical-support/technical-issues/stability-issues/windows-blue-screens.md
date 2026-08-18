---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/technical-support/technical-issues/stability-issues/windows-blue-screens.html"
breadcrumb-title: ''
description: Saiba como evitar erros de tela azul do Windows ao usar o Substance 3D Painter para uma operação estável do sistema.
helpx_creative_field: ""
helpx_description: Painter > Technical support > Technical Issues > Stability Issues > Windows Blue Screens
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Windows Blue Screens
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '526'
ht-degree: 0%

---


# Windows Blue Screens

No Windows, as [Telas Azuis de Morte (BSOD)](https://en.wikipedia.org/wiki/Blue_screen_of_death) geralmente estão relacionadas a drivers ou mau funcionamento de hardware. A própria Substance 3D Painter não é responsável por esses BSODs, mas pode esclarecer um problema com o próprio computador devido à intensidade do aplicativo. No caso do Substance 3D Painter, um BSOD pode ser causado pelos seguintes problemas.

## Drivers de GPU instáveis

O Substance 3D Painter depende muito da GPU para executar seus vários cálculos. Às vezes, os drivers da GPU podem ser instáveis ou ter regressões. Recomendamos manter a GPU atualizada para obter as correções e melhorias de desempenho mais recentes. Consulte: [A GPU tem drivers desatualizados](../gpu-issues/gpu-has-outdated-drivers.md).

### Instalação instável do Windows

O próprio Windows pode ficar instável após algumas atualizações. Use as ferramentas de diagnóstico fornecidas com o Windows para detectar possíveis erros no sistema.

Recomendamos executar a **Manutenção e Gerenciamento de Imagens de Implantação** (DISM) e a ferramenta **Verificador de Arquivos do Sistema** (SFC). O DISM é útil para recuperar os arquivos de substituição necessários para o SFC corrigir arquivos de sistema corrompidos ou ausentes.

Executando **DISM** :

1. Abrir o **Menu Iniciar**
1. Pesquisar **Prompt de Comando**
1. **Clique com o botão direito do mouse** no resultado e escolha &quot; **Executar como Administrador** &quot;
1. Digite o seguinte comando: **DISM /Online /Cleanup-Image /RestoreHealth**
1. Pressione **Enter**

Executando **SFC** :

1. Abrir o **Menu Iniciar**
1. Pesquisar **Prompt de Comando**
1. **Clique com o botão direito do mouse** no resultado e escolha &quot; **Executar como Administrador** &quot;
1. Digite o seguinte comando: **sfc /scannow**
1. Pressione **Enter**

Reinicie o computador depois dos dois comandos para aplicar as atualizações.

Para obter mais informações sobre esse assunto, consulte: [Usar a ferramenta Verificador de Arquivos do Sistema para reparar arquivos do sistema ausentes ou corrompidos](https://support.microsoft.com/en-us/help/929833/use-the-system-file-checker-tool-to-repair-missing-or-corrupted-system)

### Falta de espaço em disco

Desde a introdução das [Texturas Virtuais Esparsas](../../../features/sparse-virtual-textures.md) no Substance 3D Painter, o aplicativo agora usa o disco para armazenar em cache as texturas enquanto trabalha. Se o sistema ficar sem espaço, isso pode causar instabilidades.

Há duas soluções fáceis para esse problema:

* Libere espaço no disco para liberar mais espaço para o sistema de cache.
* Mova o diretório de cache para outra unidade com mais espaço. Este local pode ser alterado acessando as configurações principais do aplicativo, consulte a configuração [”Arquivos Temporários”](https://docs.substance3d.com/display/SPDOC/General).

### Disco com defeito (HDD ou SSD)

Como mencionado no ponto anterior, o sistema de cache depende muito do disco. Se o drive de disco estiver com defeito, isso pode tornar o sistema instável ao tentar gravar ou ler dados.

Para detectar se um disco está com defeito, você pode executar o CHKDSK no Windows:

1. Abrir o **Menu Estrela**
1. Selecionar **Computador/Este PC**
1. **Clique com o botão direito** no disco rígido e escolha **Propriedades.**
1. Alterne para a guia **Ferramentas**.
1. Clique em **Verificar/Verificar agora** em **Verificação de erros**.

### Memória com falha

A memória com falha (RAM) pode causar instabilidades no sistema se um programa não conseguir ler ou gravar na memória com segurança. Para verificar a integridade da memória, recomendamos executar **MemTest**.

Consulte [este guia](https://www.memtest86.com/technical.htm) sobre como instalar e usar o MemTest.
