---
helpx_url: "https://helpx.adobe.com/br/substance-3d-painter/getting-started/system-requirements.html"
breadcrumb-title: ''
description: Revise os requisitos de sistema do Substance 3D Painter para garantir que seu computador atenda às especificações de hardware e software.
helpx_creative_field: ""
helpx_description: Painter > Getting Started > System requirements
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Requisitos do sistema
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '779'
ht-degree: 1%

---


# Sistemas compatíveis

Veja abaixo uma lista de hardware e sistemas suportados pelo aplicativo:

## Windows

|  | Mínimo | Recomendado | Ideal |
| --- | --- | --- | --- |
| <b>SO</b> | Windows 11 64 bits versão 23H2 | Windows 11 64 bits versão 24H1 | Windows 11 64 bits versão 24H2 |
| <b>CPU</b> | Intel Core i5 AMD Ryzen 5 | Intel Core i7 AMD Ryzen 7 | Intel Core i9 AMD Ryzen 9 |
| <b>GPU</b> | NVIDIA GeForce RTX 2060 Super NVIDIA Quadro RTX 4000 AMD Radeon RX 5700 XT AMD Radeon Pro W5700 | NVIDIA GeForce RTX 3080 NVIDIA Quadro RTX A4000 AMD Radeon RX 6800 XT AMD Radeon Pro W7700 | NVIDIA GeForce RTX 4090 NVIDIA Quadro RTX 5000 Ada Generation AMD Radeon RX 7900 XTX AMD Radeon Pro W7800 |
| <b>VRAM</b> | 8 GB | 16 GB | 24 GB |
| <b>RAM</b> | 16 GB | 32 GB | 64 GB |
| <b>Armazenamento</b> | SSD com 30 GB de espaço disponível | SSD com 50 GB de espaço disponível | SSD com 70 GB de espaço disponível |

### macos

|  | Mínimo | Recomendado | Ideal |
| --- | --- | --- | --- |
| <b>SO</b> | macOS 12 Monterey | macOS 13 Ventura | macOS 14 Sonoma |
| <b>CPU</b> | Apple M1 | Apple M2 Pro | Apple M4 Pro |
| <b>GPU</b> | Apple M1 | Apple M2 Pro | Apple M4 Pro |
| <b>RAM</b> | 16 GB | 32 GB | 64 GB |
| <b>Armazenamento</b> | SSD com 30 GB de espaço disponível | SSD com 50 GB de espaço disponível | SSD com 70 GB de espaço disponível |

### Linux

| Corporativo | Vapor |
| --- | --- |
| RHEL 8</br>RHEL 9 | Ubuntu 22.04 |

## Recomendações gerais

Para obter um bom desempenho ao usar o fluxo de trabalho de Bloco UV, recomendamos usar:

* 32 GB de RAM
* GPU com 8 GB de VRAM
* SSD para armazenar o cache do projeto e do aplicativo.

Diversos:

* Muitos aplicativos Substance dependem do OpenSSL 1.1.1 para compatibilidade com RHEL8/9. Para sistemas com versões mais recentes do OpenSSL, o cliente precisará fornecê-lo manualmente
* Para trabalhar em condições confortáveis, recomendamos um monitor com uma resolução vertical superior a 1000 pixels e mais largo do que 1280 pixels.
* Exportar a <b>8K</b> (8192\*8192 pixels) requer uma GPU com <b> mais de</b> 2 GB de VRam.
* Apenas as versões 2019.x e posteriores foram autenticadas para serem executadas no MacOS 10.15 (Catalina).
* Para usar o software via RDP (Área de Trabalho Remota), consulte a [página de documentação](../pipeline-and-integration/configuration/remote-desktop.md) dedicada.
* Falha na CPU Ryzen ao assar, pode ser corrigido atualizando o BIOS.

## Configurações sem suporte

<b>Windows</b>

* Não há suporte para máquinas virtuais.
* Não há suporte para o Windows Server.

<b>Mac</b>

* Somente configurações oficiais do Apple são compatíveis.
* Atualmente, não há suporte para eGPUs e elas podem apresentar problemas de estabilidade.

<b>Linux</b>

* Drivers Mesa no Linux não são suportados.

<b>Qualquer plataforma</b>

* As GPUs integradas não são compatíveis com CPUs x86-64 (Intel, AMD).

## Versões mínimas do driver de GPU

Veja abaixo uma lista das versões mínimas de driver de GPU necessárias para que o aplicativo seja executado sem problemas. Esta lista está sujeita a alterações à medida que novas versões são lançadas.

Para baixar novos drivers, consulte: [A GPU tem drivers desatualizados](../technical-support/technical-issues/gpu-issues/gpu-has-outdated-drivers.md).

| SO | NVIDIA | AMD | Intel |
| --- | --- | --- | --- |
| <b>Windows</b> | GeForce 442,50 Quadro 442,50 | Radeon 19.7.1 Radeon Pro/FirePro 18.Q4 | 15.33 |
| <b>Linux</b> | 535.171.04 ou posterior | Radeon 22.40.6 | Sem suporte |

>[!NOTE]
>
> No **sistema operacional Mac**, o driver de GPU é fornecido pelo próprio sistema operacional. Atualize para a versão mais recente do seu sistema operacional para acessar o driver mais recente.

### Problemas de compatibilidade de drivers

Para obter uma lista detalhada dos problemas dos drivers de GPU por construtor, consulte a [página de documentação dedicada](../technical-support/technical-issues/gpu-issues/gpu-drivers-compatibility.md).

## Rastreamento de raios do GPU para panificação

Para habilitar o Rastreamento de raios do GPU via Optix ou DXR, os drivers mínimos recomendados acima devem estar instalados.

O <b>DXR</b> também requer a seguinte configuração mínima:

* <b>Windows 10</b> versão 1809, consulte [esta página](https://experienceleague.adobe.com/pt-br/docs/substance-3d/bakers/features/gpu-raytracing) para obter mais informações
* GPU <b> com arquitetura Pascal</b> (Nvidia GeForce 10XX)

>[!TIP]
>
> O Rastreamento de raios do GPU funciona de maneira ideal em hardware de rastreio de raio dedicado, como GPUs NVIDIA GeForce RTX ou NVIDIA Quadro RTX.

## Tablets gráficos compatíveis

Veja abaixo uma lista de tablets gráficos compatíveis que foram testados com o Substance 3D Painter versão <b>7.4.2</b>:

+++Wacom
<b>Modelos:</b> Intuos Pro (tamanho M), Intuos (tamanho S)


| SO | Versão do driver |
| --- | --- |
| Windows | 6.3.45-1 |
| macOS | 6.3.45-3 |


+++

+++XPen
<b>Modelo:</b> Deco 01


| SO | Versão do driver |
| --- | --- |
| Windows | XP-PENWin\_3.2.2.211027 |
| macOS | XP-PENMac\_3.2.3\_211203 |
| Linux | XP-PEN-pentablet-3.2.1.211019-1 |


+++

+++Huion
<b>Modelo:</b> Q11K


| SO | Versão do driver |
| --- | --- |
| Windows | XP-PENWin\_3.2.2.211027 |
| macOS | XP-PENMac\_3.2.3\_211203 |


+++

+++Xencelabs
<b>Modelo:</b> Caneta Tablet Média


| SO | Versão do driver |
| --- | --- |
| Windows | XencelabsWin\_1.2.1-14 |
| macOS | XencelabsMac\_1.2.1-18 |
| Linux | XencelabsLinux\_1.1.0-2 |


+++

## Modelos compatíveis do 3Dconnection SpaceMouse

Abaixo há uma lista de versões de driver compatíveis para o [3Dconnection Space Mouse](https://3dconnexion.com/us/spacemouse/) que foram testadas com o Substance 3D Painter versão <b>8.1.</b>

As versões de driver aplicam-se aos modelos <b>Compactos</b>, <b>Pro</b> e <b>Corporativos</b>.

| SO | Versão do driver |
| --- | --- |
| Windows | 10.8.6.3431 |
| macOS | 10.7.2.3454 |

## Idiomas

A interface de software está disponível nos seguintes idiomas:

* Inglês (Estados Unidos)
* Alemão
* Espanhol
* Francês
* Italiano
* Japonês
* Coreano
* Português (Brasil)
* Chinês simplificado
