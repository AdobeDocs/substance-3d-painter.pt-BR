---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/features/post-processing/color-profile.html"
breadcrumb-title: ''
description: Saiba como usar o pós-processamento de perfil de cores no Substance 3D Painter para aplicar a correção de cores e as transformações de LUT.
helpx_creative_field: ""
helpx_description: Painter > Features > Post Processing > Color Profile
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Perfil de cor
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '622'
ht-degree: 0%

---


# Perfil de cor

![](../../assets/doc-lut-example.jpg){width="700px"}

O Substance 3D Painter permite atribuir **perfis de cores** às **viewports** carregando texturas **LUT**.\
Um perfil de cores pode ser usado para calibrar a cor final da tela para corresponder a um destino, como uma câmera específica. Geralmente, um perfil manipula cores alterando o brilho, a gama, o contraste ou até mesmo o equilíbrio de cores.

>[!NOTE]
>
> **LUT** significa “**Pesquisar Tabela**”. É uma maneira otimizada de executar a correção de cores como um pós-efeito. Uma LUT é usada para fazer a diferença entre uma origem e um resultado.\
>  O Substance 3D Painter usa **3D** LUTs armazenadas como **textura 2D** (flutuante) de qualquer resolução possível (o padrão é **2048x128 pixels** ). Isso significa que o cubo que armazena as operações de cores é separado em fatias que são exibidas lado a lado. Para obter mais detalhes técnicos, consulte o artigo **GPU Gem**: <http://http.developer.nvidia.com/GPUGems2/gpugems2_chapter24.html>

## Uso de um perfil de cores

Um perfil de cores pode ser carregado pela janela Configurações de exibição.\
Marque a caixa de seleção &quot; **Ativar perfil de cores**” para afetar o visor e habilitar um perfil de cores.

![](../../assets/color-profile-ui.png)

* Quando a opção “Ativar Perfil de Cor” está **desabilitada**, a renderização do visor é feita em **sRGB** para a exibição de Material (e Linear para alguns canais específicos)
* Quando a opção “Ativar Perfil de Cor” está **habilitada**, a renderização do visor é feita em **Linear/Raw** para cada exibição (incluindo canais individuais)

Se uma textura LUT for carregada no slot de recursos, ela será usada para manipular a renderização do visor no **Modo de material**.\
Caso contrário, a renderização será exibida como Linear/Raw (por exemplo, com exibições de canais individuais).

A configuração **ponto branco** pode ser usada para alterar o mapeamento de tom da imagem de entrada (antes que a LUT entre em vigor).\
Se você estiver olhando para o sol, por exemplo, o valor deve ser maior que 1 (padrão). Para uma exposição perfeita, a ponto branco deve ser definida com o valor alto da imagem.

A fórmula do ponto branco é a seguinte:

```
float Value = 1.0f / WhitePoint; // Value from the user interface 

float3 Output = clamp( HDR.rgb * Value, 0.0f, 1.0f );
```


É possível aplicar um mapeamento de tons específico antes de usar um perfil de cores. Veja as funções disponíveis no [Mapeamento de tons](tone-mapping.md).\
O Substance 3D Painter só processa a cor de entrada através da configuração de ponto branco. Não há nenhum Shaper LUT aplicado, por exemplo.

## Criação de perfis de cores

O Substance 3D Painter mudará o visor para a renderização **Linear** quando a opção &quot; **Ativar perfil de cores**” estiver habilitada. Isso significa que, quando uma LUT é aplicada, ela precisa converter a cor de um perfil linear no destino desejado.

### Método 1: Modificando o LUT de Identidade

A edição da identidade LUT pode ser feita em um software com suporte a texturas <b>32 bits flutuantes</b>, como o <b>Substance 3D Designer</b>. Baixe o LUT de identidade como ponto de partida para criar um novo perfil:

[Baixar color\_profile\_linear.exr](https://github.com/AdobeDocs/painter-python-api/raw/refs/heads/main/static/misc/color_profile_linear.exr)

### Método 2: Uso do OpenColor IO para gerar uma Textura LUT

Instale as ferramentas do **OpenColor IO**. Em seguida, baixe o Exemplo de Configuração OCIO, disponível aqui: <http://opencolorio.org/downloads.html>\
A partir daí, execute o programa **ociolutimage** com os seguintes argumentos:

```
ociolutimage --generate --cubesize 64 --config nuke-default/config.ocio --colorconvert linear srgb --output lutLinearToSRGB.exr
```


**Observação**: também é possível modificar o LUT de identidade com a **OpenColor IO** usando o programa **ocioconvert** para aplicar a conversão de cores a este lut.

### Importação de um novo perfil de cor

Basta abrir a janela de importação (ou arrastar e soltar a LUT na prateleira). Ao importar a textura LUT no Substance 3D Painter, atribua o uso de &quot; **colorlut** &quot; **ao novo recurso.** Caso contrário, o recurso não estará visível corretamente na prateleira.

Para obter mais informações, consulte a documentação sobre a importação de novos recursos: [Adicionando recursos por meio da janela de importação](https://helpx.adobe.com/substance-3d/unlisted/documentation/spdoc/adding-content-via-the-import-window-151584824.html)
