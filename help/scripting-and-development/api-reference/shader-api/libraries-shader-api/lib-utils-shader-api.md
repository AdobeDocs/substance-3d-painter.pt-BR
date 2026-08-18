---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/scripting-and-development/api-reference/shader-api/libraries-shader-api/lib-utils-shader-api.html"
breadcrumb-title: ''
description: Acesse a referência de API de sombreamento de Utilitários de Lib para o Substance 3D Painter usar funções utilitárias no desenvolvimento de sombreador personalizado.
helpx_creative_field: ""
helpx_description: Painter > Scripting and development > API Reference > Shader API > Libraries - Shader API > Lib Utils - Shader API
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Utilitários da biblioteca - API de sombreamento
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '238'
ht-degree: 0%

---


# Utilitários da biblioteca - API de sombreamento

## Funções utilitárias alegorítmicas

## Mapeamento de tons

Estes são exemplos de mapeamento de tom que você pode usar no sombreador. O Painter não aplica nenhum mapeamento de tom, exceto o opcional aplicado pelo Yebis. Se você decidir fazer um mapeamento de tom no sombreador, ele será aplicado antes do mapeamento de tom Yebis.

Execute o mapeamento de tom da curva em S com base nos parâmetros sigma e n.

```
vec3 tonemapSCurve(vec3 value, float sigma, float n) 

{ 

  vec3 pow_value = pow(value, vec3(n)); 

  return pow_value / (pow_value + pow(sigma, n)); 

}
```


## Conversões sRGB

Estas são as conversões usadas no Painter. Você pode anular a conversão linear automática -> sRGB na janela de visualização, colocando esta linha no seu sombreador personalizado:

*#define DISABLE\_FRAMEBUFFER\_SRGB\_CONVERSION*

e fazer sua própria conversão personalizada.

sRGB para conversão de cores linear. Versão escalar.

```
float sRGB2linear(float x) 

{ 

  return x <= 0.04045 ? 

    x * 0.0773993808 : // 1.0/12.92 

    pow((x + 0.055) / 1.055, 2.4); 

}
```


sRGB para conversão de cores linear. versão do RGB.

```
vec3 sRGB2linear(vec3 rgb) 

{ 

  return vec3( 

    sRGB2linear(rgb.r), 

    sRGB2linear(rgb.g), 

    sRGB2linear(rgb.b)); 

}
```


sRGB para conversão de cores linear. RGB + versão de Alpha.

```
vec4 sRGB2linear(vec4 rgba) 

{ 

  return vec4(sRGB2linear(rgba.rgb), rgba.a); 

}
```


Conversão de cores linear para sRGB. Versão escalar.

```
float linear2sRGB(float x) 

{ 

  return x <= 0.0031308 ? 

      12.92 * x : 

      1.055 * pow(x, 0.41666) - 0.055; 

}
```


Conversão de cores linear para sRGB. versão do RGB.

```
vec3 linear2sRGB(vec3 rgb) 

{ 

  return vec3( 

      linear2sRGB(rgb.r), 

      linear2sRGB(rgb.g), 

      linear2sRGB(rgb.b)); 

}
```


Conversão de cores linear para sRGB. RGB + versão de Alpha.

```
vec4 linear2sRGB(vec4 rgba) 

{ 

  return vec4(linear2sRGB(rgba.rgb), rgba.a); 

}
```


A conversão de cores linear para sRGB é opcional. Versão escalar.

```
//: param auto conversion_linear_to_srgb 

uniform bool convert_to_srgb_opt; 

float linear2sRGBOpt(float x) 

{ 

  return convert_to_srgb_opt ? linear2sRGB(x) : x; 

}
```


A conversão de cores linear para sRGB é opcional. versão do RGB.

```
vec3 linear2sRGBOpt(vec3 rgb) 

{ 

  return convert_to_srgb_opt ? linear2sRGB(rgb) : rgb; 

}
```


A conversão de cores linear para sRGB é opcional. RGB + versão de Alpha.

```
vec4 linear2sRGBOpt(vec4 rgba) 

{ 

  return convert_to_srgb_opt ? linear2sRGB(rgba) : rgba; 

}
```


Conversão de cores. Versão escalar.

```
uniform int output_conversion_method; 

float convertOutput(float x) 

{ 

 if (output_conversion_method == 0) return x; 

 else if (output_conversion_method == 1) return linear2sRGB(x); 

 else return sRGB2linear(x); 

}
```


Conversão de cores. versão do RGB.

```
vec3 convertOutput(vec3 rgb) 

{ 

 if (output_conversion_method == 0) return rgb; 

 else if (output_conversion_method == 1) return linear2sRGB(rgb); 

 else return sRGB2linear(rgb); 

}
```


Conversão de cores. RGB + versão de Alpha.

```
vec4 convertOutput(vec4 rgba) 

{ 

 if (output_conversion_method == 0) return rgba; 

 else if (output_conversion_method == 1) return linear2sRGB(rgba); 

 else return sRGB2linear(rgba); 

}
```


## Pontilhamento

Estes são alguns auxiliares para adicionar pontilhamento aos sombreadores.

Usar matriz 8x8 Bayer para o modo de pontilhamento

```
import lib-bayer.glsl 

 

float getDitherThreshold(uvec2 coords) 

{ 

  return bayerMatrix8(coords); 

} 

 

 

vec4 RGB2Gray(vec4 rgba) 

{ 

  float gray = 0.299 * rgba.r + 0.587 * rgba.g + 0.114 * rgba.b; 

  return vec4(vec3(gray), rgba.a); 

}
```


Remoção de AO e sombras em superfícies metálicas brilhantes (próximas a espelhos)

```
float specularOcclusionCorrection(float diffuseOcclusion, float metallic, float roughness) 

{ 

  return mix(diffuseOcclusion, 1.0, metallic * (1.0 - roughness) * (1.0 - roughness)); 

} 

 
```
