---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/technical-support/technical-issues/miscellaneous-issues/impossible-to-use-the-alt-keyboard-shortcut-on-linux.html"
breadcrumb-title: ''
description: Saiba como corrigir problemas de atalho de teclado ALT no Linux no Substance 3D Painter para uma navegação adequada no teclado.
helpx_creative_field: ""
helpx_description: Painter > Technical support > Technical Issues > Miscellaneous Issues > Impossible to use the ALT keyboard shortcut on Linux
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Impossível usar o atalho de teclado ALT no Linux
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '192'
ht-degree: 0%

---


# Impossível usar o atalho de teclado ALT no Linux

Se você estiver executando uma distribuição Linux (**Ubuntu** ou **CentOS**) que usa o **Gnome** como interface do usuário, convém desabilitar o comportamento padrão da chave **ALT** para poder navegar no visor.

## CentOS

1 - Vá para **Sistema > Windows**

![](../../../assets/centos-window.png){width="250px"}

2 - Altere a configuração da “tecla de movimento” para algo diferente de &quot; **Alt** “. Por exemplo, use &quot; **Super** &quot; (para escolher a tecla “Windows” do teclado).

![](../../../assets/centos-setting.png){width="350px"}

## Ubuntu

1 - Abra um terminal e execute o seguinte comando:

```
sudo apt-get install dconf-tools
```


Isso instalará uma ferramenta de configuração avançada; talvez seja necessário permitir a instalação de dependências adicionais para poder executá-la.

2 - Abra o menu Iniciar e procure &quot; **Dconf-tools** “. Abra-o.

3 - Expanda o menu de árvore à esquerda, indo para a seguinte rota: **org > gnome > desktop > wm > preferências**

4 - Edite o “modificador do botão do mouse” e altere seu valor. Defina-o ou, em vez disso, *não deixe-o vazio*. Super é um equivalente à tecla “Windows”.

![](../../../assets/ubuntu-setting.png){width="500px"}
