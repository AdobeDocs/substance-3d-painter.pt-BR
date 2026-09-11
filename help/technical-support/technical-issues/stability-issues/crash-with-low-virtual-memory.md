---
helpx_url: "https://helpx.adobe.com/br/substance-3d-painter/technical-support/technical-issues/stability-issues/crash-with-low-virtual-memory.html"
breadcrumb-title: ''
description: Saiba como corrigir falhas do Substance 3D Painter causadas por memória virtual insuficiente para garantir um desempenho estável do aplicativo.
helpx_creative_field: ""
helpx_description: Painter > Technical support > Technical Issues > Stability Issues > Crash with low virtual memory
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Falha com pouca memória virtual
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '196'
ht-degree: 0%

---


# Falha com pouca memória virtual

O Substance 3D Painter poderá ficar instável se o arquivo de **paginação** (**troca** de memória/ **virtual** de memória) estiver definido com um valor **muito baixo** .\
É aconselhável deixar o sistema operacional manipular essas configurações (que normalmente é o caso por padrão). O Substance 3D Painter requer um **mínimo** de **16GB** de memória virtual para funcionar corretamente.

## Como alterar o tamanho da memória virtual no Windows?

>[!NOTE]
>
> Alterar o tamanho da memória virtual no Windows exigirá a reinicialização do computador.

Acesse as configurações da memória virtual seguindo estas etapas

1. Clique com o botão direito no ícone **Computador/Este PC** e escolha **Propriedades**
1. Selecione “**Configurações Avançadas do Sistema**
1. Clique no botão **Configurações** da seção **Desempenho**
1. Clique na guia **Avançado**
1. Clique em **Alterar** na seção **Memória Virtual**

Agora é possível:

* Habilitar a caixa de seleção **Gerenciar automaticamente o tamanho do arquivo de paginação de todas as unidades**

**ou**

* Selecione o disco rígido no qual deseja alterar o tamanho da memória virtual, escolha **Tamanho gerenciado pelo sistema** e clique no botão **Definir**.

**Automático:**

![](../../../assets/virtual-memory-default.png)

**Manual:**

![](../../../assets/virtual-memory-settings.png)
