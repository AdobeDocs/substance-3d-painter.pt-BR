---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/content/importing-assets/adding-content-on-the-hard-drive.html"
breadcrumb-title: ''
description: Saiba como adicionar conteúdo do disco rígido ao Substance 3D Painter para expandir sua biblioteca de recursos com arquivos locais.
helpx_creative_field: ""
helpx_description: Painter > Content > Importing assets > Adding content on the hard drive
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Adicionar conteúdo no disco rígido
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '488'
ht-degree: 2%

---


# Adicionar conteúdo no disco rígido

É possível adicionar recursos às suas bibliotecas colocando o novo conteúdo diretamente no disco rígido, no local certo.

Uma pasta padrão para ativos do usuário é fornecida por padrão, onde você pode adicionar seu novo conteúdo, por meio da interface do aplicativo ou soltando-o manualmente no seguinte local. Essa biblioteca padrão também é usada ao criar novas predefinições, como pincéis, ferramentas, materiais inteligentes etc. Para obter mais informações, consulte a documentação de [Predefinições](../../painting/presets/presets.md).

## Onde colocar ativos?

Abaixo estão os locais da biblioteca padrão **Seus ativos** em que seu próprio conteúdo personalizado é criado por padrão:

<table data-preserve-html="true" style="width: 100.0%;"><colgroup> <col style="width: 15.0%;"/> <col style="width: 15.0%;"/> <col style="width: 70.0%;"/> </colgroup><tbody><tr><th>Plataforma</th><th>Versão</th><th>Caminho</th></tr><tr><td rowspan="2"><strong>Windows</strong></td><td><strong>7.2</strong> ou mais recente</td><td colspan="1">C:\Users\username\Documents\Adobe\Adobe Substance 3D Painter</td></tr><tr><td colspan="1">Legado</td><td colspan="1">C:\Users\username\Documents\Allegorithmic\Substance Painter</td></tr><tr><td rowspan="2"><strong>Mac</strong></td><td colspan="1"><strong>7.2</strong> ou mais recente</td><td colspan="1">/Users/username/Documents/Adobe/Adobe Substance 3D Painter</td></tr><tr><td colspan="1">Legado</td><td colspan="1">/Users/username/Documents/Allegorithmic/Substance Painter</td></tr><tr><td rowspan="2"><strong>Linux</strong></td><td colspan="1"><strong>7.2</strong> ou mais recente</td><td colspan="1">/home/username/Documents/Adobe/Adobe Substance 3D Painter</td></tr><tr><td>Legado</td><td colspan="1">/home/username/Documents/Allegorithmic/Substance Painter</td></tr></tbody></table>

>[!WARNING]
>
> Os **ativos iniciais** que acompanham o aplicativo estão localizados na pasta de instalação e são substituídos em cada nova versão. Não recomendamos colocar conteúdo pessoal neste local, pois ele será **apagado com cada atualização** e pode até causar problemas de permissão de leitura/gravação.\
> É melhor usar o local **Seus ativos** ou outro local personalizado. Para obter mais informações sobre como adicionar um local de biblioteca personalizado, consulte [Adicionando uma nova biblioteca](../../interface/assets/adding-a-new-library.md).

## Formatos e usos de arquivos

É possível importar diferentes tipos de arquivos para a biblioteca do Substance 3D Painter. Colocá-los nas pastas designadas (como *alfas*, *colorluts*, *efeitos*...) atribuirá um tipo de uso ao ativo, por isso é importante escolher a pasta certa ao adicionar novo conteúdo. Observe que, se você adicionar um local de biblioteca personalizado, ele criará automaticamente as pastas apropriadas nesse local.

| *Formato de arquivo* | *Uso* | *Pasta* |
| --- | --- | --- |
| **SBSAR** | Material do Substance | ativos/materiais |
| **SBSAR** | Filtros | ativos/efeitos |
| **SBSAR** | Geradores | ativos/geradores |
| **PNG, TGA, JPEG etc.** | Textura ou Alpha | ativos / texturas **ou** prateleira / Alpha |
| **HDR, EXR** | Ambiente ou Cor LUT | ativos/ambientes **ou** prateleira/colorida |
| **GLSL** | Sombreamento | ativos/sombreadores |
| **SPPR** | Predefinição de pincel | ativos/predefinições/pincel |
| **SPPR** | Predefinição de partícula | ativos / predefinição / partículas |
| **SPPR** | Predefinição de material | ativos / Predefinições / Materiais **ou** ativos / Materiais |
| **SPPR** | Predefinição de ferramenta | ativos / Predefinição / Ferramentas |
| **SPSM** | Material inteligente | ativos/materiais inteligentes |
| **SPMSK** | Máscara inteligente | ativos/máscaras inteligentes |
| **SPEXP** | Exportar predefinição | Prateleira / Exportar-predefinições |

>[!NOTE]
>
> A partir da versão 7.2.0, pastas e categorias personalizadas podem ser usadas em uma biblioteca. Eles estarão acessíveis na janela Ativos por meio de [Filtrar por caminho](../../interface/assets/filter-by-path.md) ou [Trilhas de navegação](https://helpx.adobe.com/substance-3d/unlisted/documentation/spdoc/navigating-in-the-shelf-147095659.html).

>[!WARNING]
>
> Arquivos **SBS** (não SBSAR) não podem ser usados diretamente; eles precisam ser exportados como SBSAR do Substance 3D Designer.
