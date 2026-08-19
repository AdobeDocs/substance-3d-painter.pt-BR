---
helpx_url: "https://helpx.adobe.com/br/substance-3d-painter/features/smart-materials-and-masks.html"
breadcrumb-title: ''
description: Saiba como usar materiais e máscaras inteligentes no Substance 3D Painter para criar texturas de procedimento que se adaptam à geometria.
helpx_creative_field: ""
helpx_description: Painter > Features > Smart Materials and Masks
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Materiais e máscaras inteligentes
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '382'
ht-degree: 0%

---


# Materiais e máscaras inteligentes

O Substance 3D Painter oferece suporte ao uso de **predefinições de camada** avançadas. Essas predefinições podem ser usadas para **compartilhar rapidamente** Conjuntos ou Projetos de Textura um **processo de texturização semelhante**, mantendo os resultados diferentes, **adaptados à topologia de malha** .

>[!NOTE]
>
> Observe que, uma vez adicionado à pilha de camadas, não há como recuperar qual material inteligente foi usado. Caso um material inteligente precise ser atualizado, o processo terá de ser feito manualmente.\
> No entanto, recursos individuais podem ser atualizados com o [Atualizador de Recursos](plugins/resources-updater.md).

## Como usar materiais/máscaras inteligentes?

Materiais inteligentes podem ser usados em qualquer lugar na pilha de camadas, enquanto máscaras inteligentes só podem ser usadas na pilha de efeitos.\
Para saber mais sobre as diferenças, consulte: [Pilha de camadas](../interface/layer-stack/layer-stack.md) e [Efeitos](effects/effects.md)

### Adicionar um material inteligente

Materiais inteligentes podem ser adicionados de duas maneiras diferentes:

* Ao arrastar e soltar materiais inteligentes da prateleira na pilha de camadas:\
  ![](../assets/sm-drop.gif)
* Clicando no botão Material inteligente para abrir uma miniprateleira:\
  ![](../assets/sm-button.gif)

### Adição de uma máscara inteligente

Como as Máscaras inteligentes são predefinições de efeitos, elas só podem ser adicionadas às pilhas de efeitos (especificamente para máscaras).

* Para adicionar uma Máscara Inteligente, basta **arrastar e soltar** uma da Prateleira para a camada **destino**:\
  ![](../assets/smm-drop.gif)
* Arrastar e soltar **várias** máscaras inteligentes as acumularão:\
  ![](../assets/smm-drop-accum.gif)
* No entanto, é possível **substituir** toda a pilha de efeitos pressionando **CTRL** durante a operação de arrastar e soltar:\
  ![](../assets/smm-drop-replace.gif)

### Como criar materiais/máscaras inteligentes?

Para criar materiais inteligentes, é necessário ter uma **pasta**.\
O conteúdo dos materiais inteligentes estará contido na pasta. Em seguida, clique com o botão direito do mouse na pasta e selecione &quot; **Criar material inteligente** “. O material inteligente será adicionado à prateleira atual e será nomeado de acordo com a pasta selecionada.

![](../assets/create-sm.png)

Para criar uma Máscara Inteligente, basta clicar com o botão direito do mouse sobre uma camada e escolher &quot; **Criar máscara inteligente** “.

![](../assets/create-smm.png)

## Como compartilhar/recuperar um material/máscara inteligente?

As predefinições são salvas **no disco** e podem ser recuperadas de sua pasta dedicada.\
Para localizar o **local da prateleira** , consulte: [Adicionando conteúdo ao disco rígido](../content/importing-assets/adding-content-on-the-hard-drive.md) .

Qualquer pessoa pode simplesmente **importar** o arquivo para a prateleira do Substance 3D Painter para usar a predefinição.
