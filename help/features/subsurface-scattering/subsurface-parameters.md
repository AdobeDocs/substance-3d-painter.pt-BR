---
helpx_url: "https://helpx.adobe.com/br/substance-3d-painter/features/subsurface-scattering/subsurface-parameters.html"
breadcrumb-title: ''
description: Saiba como configurar os parâmetros de dispersão da subsuperfície no Substance 3D Painter para criar materiais translúcidos realistas.
helpx_creative_field: ""
helpx_description: Painter > Features > Subsurface Scattering > Subsurface Parameters
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Parâmetros da Subsuperfície
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '315'
ht-degree: 0%

---


# Parâmetros da Subsuperfície

A implementação de subsuperfície em tempo real do Substance 3D Painter é um efeito de dispersão de subsuperfície do espaço da tela. Os parâmetros para controlá-la são explicados nesta página.\
A implementação atual é baseada no método “Perfis de Reflexão Aproximados para Dispersão Eficiente de Subsuperfícies” [publicado pela PIXAR](http://graphics.pixar.com/library/ApproxBSSRDF/).

Para exemplos de materiais baseados nesses parâmetros, consulte: [Tipo de Material de Subsuperfície](subsurface-material-type.md).

## Parâmetros de Sombreador/MDL

![](../../assets/shader-parameters.png)

Disponível na janela [Configurações do sombreador](../../interface/shader-settings/shader-settings.md).

| *Configuração* | *Descrição* |
| --- | --- |
| **Habilitar** | Ative ou desative o efeito Dispersão de subsuperfície nesta ocorrência de shader/mdl.  Pode ser usado para desativar o efeito do SSS em materiais que não precisam dele. |
| **Tipo de dispersão** | Define o comportamento da absorção de luz no material:<ul data-preserve-html="true"><li data-preserve-html="true"><strong> Transparente</strong>: adequado para materiais genéricos, como Jade ou Mármore, onde a luz possa penetrar profundamente em um objeto.</li><li data-preserve-html="true"><strong> Pele</strong>: adequada para pele orgânica, onde a luz é absorvida rapidamente e somente dispersão perto da superfície.</li><li data-preserve-html="true"><strong>Red Shift/Rayleigh</strong>: mais preciso do que a configuração da pele para simular a pele humana ou da superfície da criatura.</li></ul> |
| **Escala** | Controla o raio/profundidade da absorção de luz no material. Esse comportamento do parâmetro muda dependendo do tamanho da malha na cena.Comparação entre uma escala de 0,0, 0,2 e 1,0 em uma cabeça do tamanho humano:   <div><img data-preserve-html="true" src="../../assets/scale-sss.jpg" width="650"/></div> |
| **Cor** | A cor da luz quando absorvida pelo material.Comparação entre três cores :   <div><img data-preserve-html="true" src="../../assets/color-sss.jpg" width="650"/></div> |

### Parâmetros de configurações de exibição

![](../../assets/display-settings-1.png)

Disponível na janela [Configurações de exibição](../../interface/display-settings/display-settings.md).

>[!NOTE]
>
> Este parâmetro **afeta** somente a versão **em tempo real** do efeito de dispersão da subsuperfície.

| *Configuração* | *Descrição* |
| --- | --- |
| **Contagem de Amostras** | Controla a quantidade de amostras que serão executadas para gerar o desfoque de Subsuperfície no espaço da tela. Mais amostras significa menos ruído, mas afetará o desempenho.Comparação entre 8, 32 e 64 amostras quando se olha perto de uma superfície:   <div><img data-preserve-html="true" src="../../assets/samples-sss-v2.jpg" width="650"/></div>  **Observação:** a quantidade de ruído também pode ser reduzida habilitando-se as [configurações da câmera](../../interface/display-settings/camera-settings.md) sem aumentar a quantidade de amostras. |
