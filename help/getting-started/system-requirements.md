---
breadcrumb-title: ""
description: Revise os requisitos de sistema do Substance 3D Painter para garantir que seu computador atenda às especificações de hardware e software.
title: Requisitos do sistema
user-guide-description: ""
user-guide-title: ""
source-git-commit: fbfe7e52b226b5a92f5b46ebbf82728f0ff9e3c5
workflow-type: tm+mt
source-wordcount: '814'
ht-degree: 1%
---

# Sistemas compatíveis

Veja abaixo uma lista de hardware e sistemas suportados pelo aplicativo:

## Windows

|  | Mínimo | Recomendado | Ideal |
| --- | --- | --- | --- |
| **SO** | Windows 11 64 bits versão 23H2 | Windows 11 64 bits versão 24H1 | Windows 11 64 bits versão 24H2 |
| **CPU** | Intel Core i5 AMD Ryzen 5 | Intel Core i7 AMD Ryzen 7 | Intel Core i9 AMD Ryzen 9 |
| **GPU** | NVIDIA GeForce RTX 2060 Super NVIDIA Quadro RTX 4000 AMD Radeon RX 5700 XT AMD Radeon Pro W5700 | NVIDIA GeForce RTX 3080 NVIDIA Quadro RTX A4000 AMD Radeon RX 6800 XT AMD Radeon Pro W7700 | NVIDIA GeForce RTX 4090 NVIDIA Quadro RTX 5000 Ada Generation AMD Radeon RX 7900 XTX AMD Radeon Pro W7800 |
| **VRAM** | 8 GB | 16 GB | 24 GB |
| **RAM** | 16 GB | 32 GB | 64 GB |
| **Armazenamento** | SSD com 30 GB de espaço disponível | SSD com 50 GB de espaço disponível | SSD com 70 GB de espaço disponível |

### macOS

|  | Mínimo | Recomendado | Ideal |
| --- | --- | --- | --- |
| **SO** | macOS 15 Sequoia | Porta dourada do macOS 27 | macOS 27 Golden Gate |
| **CPU** | Apple M1 | Apple M2 Pro | Apple M4 Pro |
| **GPU** | Apple M1 | Apple M2 Pro | Apple M4 Pro |
| **RAM** | 16 GB | 32 GB | 64 GB |
| **Armazenamento** | SSD com 30 GB de espaço disponível | SSD com 50 GB de espaço disponível | SSD com 70 GB de espaço disponível |

>[!WARNING]
>
> Para pipelines criados com a [Plataforma de Referência VFX](https://vfxplatform.com/) em mente, o Substance 3D Painter ainda pode ser instalado no macOS 14 Sonoma. No entanto, o Painter não é mais testado em versões do sistema operacional abaixo dos requisitos mínimos de sistema, portanto, a estabilidade não é garantida.

### Linux

| Corporativo | Vapor |
| --- | --- |
| RHEL 8<br>RHEL 9 | Ubuntu 22.04 |

## Recomendações gerais

Para obter um bom desempenho ao usar o fluxo de trabalho do Bloco UV, recomendamos usar:

* 32 GB de RAM
* GPU com 8 GB de VRAM
* SSD para armazenar o cache do projeto e do aplicativo.

Diversos:

* Muitos aplicativos Substance dependem do OpenSSL 1.1.1 para compatibilidade com RHEL8/9. Para sistemas com versões mais recentes do OpenSSL, o cliente precisará fornecê-lo manualmente
* Para trabalhar em condições confortáveis, recomendamos um monitor com uma resolução vertical superior a 1000 pixels e mais largo do que 1280 pixels.
* Exportar a **8K** (8192\*8192 pixels) requer uma GPU com **mais de** 2 GB de VRam.
* Apenas as versões 2019.x e posteriores foram autenticadas para serem executadas no MacOS 10.15 (Catalina).
* Para usar o software via RDP (Área de Trabalho Remota), consulte a [página de documentação](../pipeline-and-integration/configuration/remote-desktop.md) dedicada.
* A falha na CPU Ryzen ao fazer bake pode ser corrigida com a atualização do BIOS.

## Configurações sem suporte

**Windows**

* Não há suporte para máquinas virtuais.
* Não há suporte para o Windows Server.

**Mac**

* Somente configurações oficiais do Apple são compatíveis.
* Atualmente, não há suporte para eGPUs e elas podem apresentar problemas de estabilidade.

**Linux**

* Drivers Mesa no Linux não são suportados.

**Qualquer plataforma**

* As GPUs integradas não são compatíveis com CPUs x86-64 (Intel, AMD).

## Versões mínimas do driver de GPU

Veja abaixo uma lista das versões mínimas de driver de GPU necessárias para que o aplicativo seja executado sem problemas. Esta lista está sujeita a alterações à medida que novas versões são lançadas.

Para baixar novos drivers, consulte: [A GPU tem drivers desatualizados](../technical-support/technical-issues/gpu-issues/gpu-has-outdated-drivers.md).

| SO | NVIDIA | AMD | Intel |
| --- | --- | --- | --- |
| **Windows** | GeForce 442,50 Quadro 442,50 | Radeon 19.7.1 Radeon Pro/FirePro 18.Q4 | 15.33 |
| **Linux** | 535.171.04 ou posterior | Radeon 22.40.6 | Sem suporte |

>[!NOTE]
>
> No **sistema operacional Mac**, o driver de GPU é fornecido pelo próprio sistema operacional. Atualize para a versão mais recente do seu sistema operacional para acessar o driver mais recente.

### Problemas de compatibilidade de drivers

Para obter uma lista detalhada dos problemas dos drivers de GPU por construtor, consulte a [página de documentação dedicada](../technical-support/technical-issues/gpu-issues/gpu-drivers-compatibility.md).

## Rastreamento de raios do GPU para fazer bake

Para ativar o Rastreamento de raios do GPU via Optix ou DXR, os drivers mínimos recomendados acima devem ser instalados.

**DXR** também requer a seguinte configuração mínima:

* **Windows 10** versão 1809, consulte [esta página](https://experienceleague.adobe.com/en/docs/substance-3d/bakers/features/gpu-raytracing) para obter mais informações
* **GPU com arquitetura Pascal** (Nvidia GeForce 10XX)

>[!TIP]
>
> O Rastreamento de raios do GPU funciona de maneira ideal em hardware de Rastreamento de raios dedicado como GPUs NVIDIA GeForce RTX ou NVIDIA Quadro RTX.

## Tablets gráficos compatíveis

Veja abaixo uma lista de tablets gráficos compatíveis que foram testados com o Substance 3D Painter versão **7.4.2**:

+++Wacom

**Modelos:** Intuos Pro (tamanho M), Intuos (tamanho S)

| SO | Versão do driver |
| --- | --- |
| Windows | 6.3.45-1 |
| macOS | 6.3.45-3 |

+++

+++XPen

**Modelo:** Deco 01

| SO | Versão do driver |
| --- | --- |
| Windows | XP-PENWin_3.2.2.211027 |
| macOS | XP-PENMac_3.2.3_211203 |
| Linux | XP-PEN-pentablet-3.2.1.211019-1 |

+++

+++Huion

**Modelo:** Q11K

| SO | Versão do driver |
| --- | --- |
| Windows | XP-PENWin_3.2.2.211027 |
| macOS | XP-PENMac_3.2.3_211203 |

+++

+++Xencelabs

**Modelo:** Caneta Tablet Média

| SO | Versão do driver |
| --- | --- |
| Windows | XencelabsWin_1.2.1-14 |
| macOS | XencelabsMac_1.2.1-18 |
| Linux | XencelabsLinux_1.1.0-2 |

+++

## Modelos compatíveis do 3Dconnection SpaceMouse

Abaixo há uma lista de versões de driver compatíveis para o [3Dconnection Space Mouse](https://3dconnexion.com/us/spacemouse/) que foram testadas com o Substance 3D Painter versão **8.1.**

As versões de driver aplicam-se aos modelos **Compactos**, **Pro** e **Corporativos**.

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
