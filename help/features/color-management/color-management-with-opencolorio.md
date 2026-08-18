---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/features/color-management/color-management-with-opencolorio.html"
breadcrumb-title: ''
description: Saiba como usar o gerenciamento de cores do OpenColorIO no Substance 3D Painter para obter fluxos de trabalho de cores consistentes entre pipelines.
helpx_creative_field: ""
helpx_description: Painter > Features > Color management > Color management with OpenColorIO
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Gerenciamento de cores com o OpenColorIO
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '675'
ht-degree: 8%

---


# Gerenciamento de cores com o OpenColorIO

Esta página lista as configurações de gerenciamento de cores relacionadas ao OpenColorIO (OCIO).

## Configurações do projeto

![](../../assets/project-settings-3.png)

As configurações de projeto podem ser definidas ao criar um novo projeto por meio da janela [novo projeto](../../getting-started/project-creation.md) ou usando a janela [configuração de projeto](../../interface/project-configuration.md).

>[!NOTE]
>
> Se a variável de ambiente **OCIO** estiver presente e especificar um arquivo de configuração válido, ela substituirá e desabilitará as configurações na interface do usuário.

As configurações disponíveis são:

<table data-preserve-html="true" style="width: 99.9039%;"><colgroup><col style="width: 12.512%;"/><col style="width: 21.1742%;"/><col style="width: 66.3122%;"/></colgroup><tbody><tr><th style="width: 12.5%;">Seção</th><th style="width: 21.1538%;">Configuração</th><th style="width: 66.25%;">Descrição</th></tr><tr><td rowspan="3" style="width: 12.5%;"><strong>Configuração</strong></td><td style="width: 21.1538%;"><strong>Gerenciamento de cores</strong></td><td style="width: 66.25%;"><p>Defina qual mecanismo usar para gerenciar cores.</p><p>Valores possíveis:</p><ul><li><strong>Legado</strong> (padrão): use a correção de cores gama sRGB/sRGB linear predefinida.</li><li><strong>OpenColorIO</strong>: use a integração OCIO.</li><li><strong>Adobe ACE</strong>: Adobe Color Engine, para suportar perfis ICC.</li></ul></td></tr><tr><td style="width: 21.1538%;"><strong>Configuração do OpenColorIO</strong></td><td style="width: 66.25%;"><p>Qual arquivo de configuração usar para orientar as configurações de gerenciamento de cores.</p><p>Valores possíveis:</p><ul><li><strong>Substance</strong> (padrão): use gama linear como espaço de trabalho.</li><li><strong>ACES 1.0.3</strong>: use ACEScg como espaço de trabalho.</li><li><strong>ACES 1.2</strong>: use ACEScg como espaço de trabalho.</li><li><strong>Personalizado</strong>: use um arquivo de configuração personalizado.</li></ul></td></tr><tr><td style="width: 21.1538%;"><strong>Arquivos de configuração</strong></td><td style="width: 66.25%;">Caminho do arquivo de configuração OCIO. Desabilitado se o modo de configuração não estiver definido como <strong>Personalizado</strong>.</td></tr><tr><th style="width: 12.5%;"><br/></th><th style="width: 21.1538%;"><br/></th><th style="width: 66.25%;"><br/></th></tr><tr><td rowspan="2" style="width: 12.5%;"><strong>Configurações de cores</strong></td><td style="width: 21.1538%;"><strong>Espaço de cores de trabalho</strong></td><td style="width: 66.25%;">O espaço de cores usado pelo mecanismo para trabalhar dentro do aplicativo. Esse é o espaço de cores do qual as texturas podem ser convertidas em (importação) ou de (exportação).</td></tr><tr><td colspan="1"><strong>Espaço de cores sRGB padrão</strong></td><td colspan="1"><p>O espaço da cor que corresponde ao espaço da cor [standard sRGB](https://en.wikipedia.org/wiki/SRGB) (IEC 61966-2-1:1999).</p><p>Esse espaço de cores é usado em vários locais dentro do aplicativo:</p><ul><li>Para converter a cor definida no campo hexadecimal do seletor de cores.</li><li>Para salvar e carregar amostras de cores no seletor de cores.</li><li>A ser listado como uma Exibição na lista de seletores de cores.</li></ul></td></tr><tr><th style="width: 12.5%;"><br/></th><th style="width: 21.1538%;"><br/></th><th style="width: 66.25%;"><br/></th></tr><tr><td rowspan="4" style="width: 12.5%;"><strong>Padrões de espaço de cores de importação de bitmap</strong></td><td style="width: 21.1538%;"><strong>Imagens de 8 bits</strong></td><td style="width: 66.25%;">Espaço de cores a ser usado por padrão ao importar arquivos de imagem de 8 bits.</td></tr><tr><td style="width: 21.1538%;"><strong>Imagens de 16 bits</strong></td><td style="width: 66.25%;">Espaço de cores a ser usado por padrão ao importar arquivos de imagem de 16 bits.</td></tr><tr><td style="width: 21.1538%;"><strong>Imagens de ponto flutuante</strong></td><td style="width: 66.25%;">Espaço de cores a ser usado por padrão ao importar arquivos de imagem HDR/EXR.</td></tr><tr><td style="width: 21.1538%;"><strong>Detecção auto. de espaços de cores</strong></td><td style="width: 66.25%;"><p>Permite definir o espaço de cores de recursos com base em configurações específicas.</p><p>Valores possíveis:</p><ul><li><strong>Desabilitado</strong>: use a configuração de cores padrão, ignore a configuração do recurso.</li><li><strong>Analisar o nome do arquivo</strong> (padrão): use OCIO [convenção de nomenclatura](https://opencolorio.readthedocs.io/en/latest/guides/authoring/rules.html?highlight=filename#strictparsing) para extrair o nome do espaço de cores usado pelo recurso.</li><li><strong>Usar regras de arquivos de configuração</strong>: use a configuração OCIO para determinar como atribuir espaços de cores. Este parâmetro tem prioridade sobre as configurações anteriores do espaço de cores do arquivo de imagem.</li></ul></td></tr><tr><th style="width: 12.5%;"><br/></th><th style="width: 21.1538%;"><br/></th><th style="width: 66.25%;"><br/></th></tr><tr><td style="width: 12.5%;"><strong>material de Substance</strong></td><td style="width: 21.1538%;"><strong>Padrão do espaço de cores do material</strong></td><td style="width: 66.25%;"><p>Defina qual espaço de cor usar para entrada/saída gerenciada por cores de materiais de Substance (veja abaixo a lista de canais).</p></td></tr><tr><th style="width: 12.5%;"><br/></th><th style="width: 21.1538%;"><br/></th><th style="width: 66.25%;"><br/></th></tr><tr><td rowspan="3" style="width: 12.5%;"><strong>Exportar espaços de cor</strong><br/><br/><br/></td><td style="width: 21.1538%;"><strong>Imagens de 8 bits</strong></td><td style="width: 66.25%;">Espaço de cores a ser usado por padrão ao exportar arquivos de imagem de 8 bits.</td></tr><tr><td style="width: 21.1538%;"><strong>Imagens de 16 bits</strong></td><td style="width: 66.25%;">Espaço de cores a ser usado por padrão ao exportar arquivos de imagem de 16 bits.</td></tr><tr><td style="width: 21.1538%;"><strong>Imagens de ponto flutuante</strong></td><td style="width: 66.25%;">Espaço de cores a ser usado por padrão ao exportar arquivos de imagem HDR/EXR.</td></tr></tbody></table>

### Funções do OpenColorIO

As funções a seguir são compatíveis e permitem alterar a seleção padrão de espaços de cores:

| Nome da função | Descrição |
| --- | --- |
| **substance\_3d\_painter\_standard\_srgb** | Função para especificar o espaço de cores correspondente ao [sRGB](https://en.wikipedia.org/wiki/SRGB) padrão (IEC 61966-2-1:1999). |
| **substance\_3d\_painter\_bitmap\_import\_8bit** | Função para especificar o espaço de cores usado para importar imagens de 8 bits. |
| **substance\_3d\_painter\_bitmap\_import\_16bit** | Função para especificar o espaço de cores usado para importar imagens de 16 bits. |
| **substance\_3d\_painter\_bitmap\_import\_floating** | Função para especificar o espaço de cores usado para importar imagens HDR. |
| **substance\_3d\_painter\_substance\_material** | Função para especificar o espaço de cores usado para canais gerenciados por cores em materiais de Substance. |
| **substance\_3d\_painter\_bitmap\_export\_8bit** | Função para especificar o espaço de cores usado ao exportar texturas de 8 bits. |
| **substance\_3d\_painter\_bitmap\_export\_16bit** | Função para especificar o espaço de cores usado ao exportar texturas de 16 bits. |
| **substance\_3d\_painter\_bitmap\_export\_floating** | Função para especificar o espaço de cores usado ao exportar texturas HDR. |

>[!NOTE]
>
> As configurações do OCIO fornecidas com o aplicativo podem ser usadas como exemplos sobre como usar essas funções específicas.
