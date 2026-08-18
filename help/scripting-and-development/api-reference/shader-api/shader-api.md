---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/scripting-and-development/api-reference/shader-api.html"
breadcrumb-title: ''
description: Acesse a referência de API de sombreamento do Substance 3D Painter para criar sombreadores personalizados e estender os recursos de renderização.
helpx_creative_field: ""
helpx_description: Painter > Scripting and development > API Reference > Shader API
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: API de sombreamento
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '702'
ht-degree: 0%

---


# API de sombreamento

![](../../../assets/header-shader.jpg)

O Substance Painter usa sombreadores para renderizar materiais em sua viewport em tempo real. É possível gravar sombreadores personalizados para implementar novos comportamentos ou simplesmente fazer com que a viewport corresponda a outros renderizadores.

Sombreadores adicionais para Substance Painter podem ser encontrados no [Substance share](https://share.allegorithmic.com/libraries?by_category_type_id=6).

>[!NOTE]
>
> O API de sombreamento também está disponível diretamente no aplicativo, indo para o menu **Ajuda > Documentação > API de sombreamento**.

## Referência de sombreador

## Changelog

* [Arquivo de registro de alterações completo](changelog-shader-api.md)

## Aquecimento

No Substance Painter, você pode escrever seus próprios shaders no *GLSL*. Permitimos que você grave somente uma *parte* do sombreador de fragmentos, que às vezes é chamado de *sombreador de superfície*. Sem mais delongas, vamos apresentar o sombreador de superfície de Substance Painter “Hello world”:

```
void shade(V2F inputs) { 

  diffuseShadingOutput(vec3(1.0, 0.0, 1.0)); 

}
```


Agora, se você salvar este trecho em um arquivo *.glsl* e carregá-lo no Substance Painter, soltando-o na guia de sombreador da sua prateleira, poderá usá-lo e ver uma bela cor rosa uniforme na malha.

## Sombreador de superfície

* [surface-shader.glsl](shaders-shader-api/surface-shader-shader-api.md)

## Dados fornecidos pelo mecanismo (ou como acessar meus canais?)

No Substance Painter, é possível acessar os parâmetros do mecanismo de renderização (canais do documento, texturas adicionais, dados relacionados à câmera e assim por diante). Aqui está uma lista completa de todos os parâmetros fornecidos pelo mecanismo:

* [all-engine-params.glsl](parameters-shader-api/all-engine-params-shader-api.md)

## Configurações do mecanismo (ou como especificar estados de renderização?)

Em alguns casos, convém usar uma configuração de renderização específica (seleção, mesclagem, localidade de amostra e semelhantes) para um efeito. Alguns estados de renderização são expostos e podem ser definidos no sombreador. Veja uma lista completa de todos os estados de renderização expostos:

* [all-rendering-states-params.glsl](parameters-shader-api/all-rendering-states-params-shader-api.md)

## Ajustes personalizados (ou como ajustar meu sombreador?)

É comum ter ajustes personalizados em um sombreador. Para fazer isso em Substance Painter, introduzimos uma maneira de especificar ajustes personalizados. Veja uma lista completa de todos os tipos de ajustes personalizados de sombreador:

* [all-custom-params.glsl](parameters-shader-api/all-custom-params-shader-api.md)

## Bibliotecas incorporadas

A fim de evitar a escrita de um monte de código boilerplate em todos os seus shaders, nós criamos uma pequena, mas prática biblioteca de funções úteis. **Observe que você não pode editá-lo nem criar seu próprio no momento.**

* [lib-alpha.glsl](libraries-shader-api/lib-alpha-shader-api.md) : contém auxiliares relacionados a opacidade
* [lib-bayer.glsl](libraries-shader-api/lib-bayer-shader-api.md) : contém auxiliares de matriz de baias
* [lib-defined.glsl](libraries-shader-api/lib-defines-shader-api.md) : contém constantes matemáticas úteis
* [lib-emissive.glsl](libraries-shader-api/lib-emissive-shader-api.md) : contém auxiliares de propriedades emissivas
* [lib-env.glsl](libraries-shader-api/lib-env-shader-api.md) : contém auxiliares relacionados ao mapa de ambiente
* [lib-normal.glsl](libraries-shader-api/lib-normal-shader-api.md) : contém auxiliares relacionados ao mapa normal (e mapa de height gerado mapa normal)
* [lib-pbr.glsl](libraries-shader-api/lib-pbr-shader-api.md) : contém auxiliares de renderização baseados fisicamente
* [lib-pbr-aniso.glsl](libraries-shader-api/lib-pbr-aniso-shader-api.md) : contém auxiliares de renderização baseados fisicamente anisotrópicos
* [lib-pom.glsl](libraries-shader-api/lib-pom-shader-api.md) : contém auxiliares de mapeamento de oclusão de paralaxe
* [lib-random.glsl](libraries-shader-api/lib-random-shader-api.md) : contém utilitários aleatórios (sequências de baixa discrepância)
* [lib-sampler.glsl](libraries-shader-api/lib-sampler-shader-api.md) : contém os auxiliares getters do canal
* [lib-sparse.glsl](libraries-shader-api/lib-sparse-shader-api.md) : contém auxiliares de amostragem de textura esparsa segura
* [lib-sss.glsl](libraries-shader-api/lib-sss-shader-api.md) : contém auxiliares de dispersão de subsuperfície
* [lib-utils.glsl](libraries-shader-api/lib-utils-shader-api.md) : contém funções de utilitário de cores (conversões sRGB, mapeamento de tons)
* [lib-vetors.glsl](libraries-shader-api/lib-vectors-shader-api.md) : contém auxiliares de vetores comuns

## Metadados

É possível declarar informações adicionais não necessárias para dar alguma dica ao sistema de renderização. Aqui está a sintaxe:

```
//: metadata { 

//:   "key1":"value1", 

//:   "key2":"value2" 

//: }
```


As chaves compatíveis são:

* **custom-ui**: substitui a interface de usuário de parâmetros de sombreador padrão por uma exibição personalizada escrita como um módulo QML (consulte a documentação de scripts). O caminho pode ser absoluto ou relativo a uma de suas prateleiras *custom-ui* pasta.
* **mdl**: defina o material mdl Iray a ser usado com o sombreador. A sintaxe do caminho é a seguinte: *mdl::folder1::folder2::mdl\_filename::material\_name* onde *folder1::folder2::mdl\_filename* é o caminho dentro de uma das pastas de prateleira *mdl* para um arquivo mdl e *::material\_name* é o nome de um material declarado dentro desse arquivo mdl. (ex: “mdl” : “mdl::alg::materials::physical\_metallic\_roughness::physical\_metallic\_roughness”)

## Exemplos de sombreadores (yeah, finally!)

Para se ter uma ideia do que parece ser um sombreador real, aqui estão algumas amostras de sombreador, ordenadas pelo aumento da complexidade:

* [pixelated.glsl](shaders-shader-api/pixelated-shader-api.md) : um sombreador de pixelização
* [toon.glsl](shaders-shader-api/toon-shader-api.md) : um sombreador toon
* [pbr-metal-rough.glsl](shaders-shader-api/pbr-metal-rough-shader-api.md) : o sombreador PBR padrão incorporado no Substance Painter

## Camadas de material dinâmico

A Camadas de material dinâmico é um fluxo de trabalho específico em que os materiais são misturados dentro de um sombreador e permitem que o usuário edite máscaras de mesclagem dinamicamente no Substance Painter. Para ativar esse fluxo de trabalho, há duas novas funcionalidades:

* declare pilhas editáveis de uma definição de sombreador: [camadas\_declare\_stacks.glsl](parameters-shader-api/layering-declare-stacks-shader-api.md)
* vincular materiais como parâmetros de sombreador: [camadas\_vincular\_materiais.glsl](parameters-shader-api/layering-bind-materials-shader-api.md)
