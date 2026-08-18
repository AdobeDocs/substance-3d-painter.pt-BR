---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/technical-support/performances-guidelines/gpu-drivers.html"
breadcrumb-title: ''
description: Saiba mais sobre os requisitos de GPU, VRAM e driver para o Substance 3D Painter otimizar o desempenho e a estabilidade da renderização.
helpx_creative_field: ""
helpx_description: Painter > Technical support > Performances guidelines > GPU Drivers
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Drivers e VRAM de GPU
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '436'
ht-degree: 0%

---


# Drivers de GPU

Não podemos garantir o desempenho sem o uso de drivers recomendados. Os drivers não-WHQL devem ser evitados.\
Os drivers de GPU são como qualquer software, cada nova versão pode apresentar problemas de desempenho. Se ocorrerem problemas após atualizar para uma versão mais recente do driver, recomendamos rebaixar os drivers para uma versão anterior.

## Configurações de drivers NVIDIA

Algumas configurações padrão de NVIDIA podem ter um impacto no desempenho. Recomendamos criar um perfil e desativar os seguintes parâmetros (defina-os como desativados):

* Otimização por Threads
* Sincronização vertical

## Como outros aplicativos podem utilizar a GPU

O Substance 3D Painter não está sozinho trabalhando com a GPU, outros aplicativos fazem o mesmo. Praticamente qualquer aplicativo 3D usará a GPU e a VRAM para execução, incluindo aqueles comumente usados junto com o Painter, como o Blender, o Maya, o Unreal Engine, o Unity, o C4D e outros. Uma solução para garantir um bom desempenho enquanto mantém esses aplicativos abertos é garantir que o Substance 3D Painter seja iniciado primeiro para solicitar sua própria alocação de VRAM. Ainda assim, alguns softwares podem adquirir algumas partes da VRAM dinamicamente e ainda podem estar em conflito com a Substance 3D Painter, mesmo se forem iniciados após a Painter.

Em geral, quanto mais VRAM o Painter tiver acesso, mais rápido ele será executado. Portanto, tente minimizar a quantidade de VRAM usada por outros aplicativos executados simultaneamente com o Painter.

## Quantidade e largura de banda de VRAM da GPU

O Substance 3D Painter depende muito da GPU para realizar a maioria de seus cálculos. É por isso que é importante ter uma GPU que siga os [Requisitos de sistema](../../getting-started/system-requirements.md).

O Painter funciona transferindo texturas para a memória de GPU (VRAM) a fim de realizar os cálculos (como operações de mesclagem para criar as texturas finais). No entanto, se o VRAM estiver começando a ficar cheio, as texturas não utilizadas serão transferidas de volta para a RAM do computador para liberar espaço de VRAM. O Substance 3D Painter grava e lê GBs de dados durante o trabalho. Isso significa que a capacidade do VRAM (quantidade) e a velocidade da largura de banda ao fazer transferências são importantes. Você pode usar ferramentas como o [MSI AfterBurner](https://www.msi.com/page/afterburner) para monitorar esse comportamento.

>[!NOTE]
>
> Sabe-se que a <b>Nvidia GTX 970</b> tem um design problemático com relação à sua memória de GPU que afeta o Substance 3D Painter. Os últimos 500 MB de todos os 4 GB funcionam em um ritmo mais lento do que os 3,5 GB restantes. Se o Substance 3D Painter funcionar nesses últimos 500 MB, o desempenho poderá ser reduzido em até 10 vezes (em relação ao que medimos). Para obter mais detalhes técnicos, consulte: <https://www.pcper.com/news/Graphics-Cards/NVIDIA-Responds-GTX-970-35GB-Memory-Issue>
