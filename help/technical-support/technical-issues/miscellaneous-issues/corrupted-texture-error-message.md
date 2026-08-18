---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/technical-support/technical-issues/miscellaneous-issues/corrupted-texture-error-message.html"
breadcrumb-title: ''
description: Saiba como corrigir mensagens de erro de textura corrompidas no Substance 3D Painter para restaurar a funcionalidade da textura.
helpx_creative_field: ""
helpx_description: Painter > Technical support > Technical Issues > Miscellaneous Issues > Corrupted texture error message
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Mensagem de erro de textura corrompida
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '385'
ht-degree: 0%

---


# Mensagem de erro de textura corrompida

Texturas corrompidas em um projeto causarão falhas durante o processo de salvamento e podem levar a projetos totalmente corrompidos e não recuperáveis. No entanto, isso pode ser corrigido manualmente.\
Um recurso corrompido se manifesta no log ao abrir um projeto com uma mensagem de erro semelhante a esta na janela de log:

![](../../../assets/corrupt1.png)

## Corrigindo uma referência de recurso corrompida

### 1 - Localizando o recurso

A primeira etapa quando um erro aparece é localizar e identificar o recurso problemático.\
Na maioria dos casos, o culpado é os **mapas de malha** (texturas assadas). Uma maneira rápida de verificar isso é observar os geradores de máscara na pilha de camadas.

Os recursos corrompidos serão semelhantes a estes:

![](../../../assets/corrupt2.png)

>[!NOTE]
>
> Isso também pode significar que o recurso está simplesmente faltando.\
> Para isso, tente limpar o slot e reafetar manualmente a torta. Se a miniatura da cruz vermelha ainda estiver aqui, isso significa que o recurso está corrompido.

### 2 - Substituindo o recurso

Para substituir um recurso corrompido, todas as referências a ele devem ser removidas primeiro. Se a corrente é relativamente pequena, isso pode ser feito manualmente.\
No entanto, se o projeto se estender por vários conjuntos de texturas ou muitas camadas, o [Atualizador de Recursos](../../../features/plugins/resources-updater.md) poderá ser útil para localizar o recurso corrompido e substituí-lo temporariamente por outro.

>[!NOTE]
>
> * No caso das texturas assadas, não se esqueça de limpar também os slots de Mapas de Malha na janela [Configurações do Conjunto de Texturas](../../../interface/texture-set/texture-set-settings.md).
> * As tortas usadas apenas nas Configurações do conjunto de texturas, como o mapa normal, também podem estar corrompidas. Tente removê-los também se os erros persistirem.

### 3 - Limpeza

Quando todas as referências aos recursos corrompidos forem perdidas, execute uma Limpeza do projeto no menu principal (**Arquivo** > **Limpar**).\
Isso deve remover todos os recursos corrompidos não utilizados do projeto. É possível verificar navegando até a guia Projeto na prateleira para certificar-se de que todos os recursos problemáticos foram perdidos.

### 4 - Salvar

Após a limpeza, tente salvar o projeto:

* Se for salvo sem erro, o projeto agora está livre de corrupções (mapas de malha agora podem ser recuperados e os recursos reimportados).
* Se os erros permanecerem, isso significa que ainda há uma referência a um recurso corrompido no projeto.
