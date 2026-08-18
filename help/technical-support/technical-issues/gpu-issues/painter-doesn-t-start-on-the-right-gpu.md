---
helpx_url: "https://helpx.adobe.com/br/substance-3d-painter/technical-support/technical-issues/gpu-issues/painter-doesn-t-start-on-the-right-gpu.html"
breadcrumb-title: ''
description: Saiba como configurar o Substance 3D Painter para iniciar na GPU correta para desempenho e compatibilidade ideais.
helpx_creative_field: ""
helpx_description: Painter > Technical support > Technical Issues > GPU Issues > Painter doesnt start on the right GPU
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: O Painter não é iniciado na GPU certa
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '624'
ht-degree: 0%

---


# O Painter não inicia na GPU correta

No Windows, o aplicativo pode não usar a GPU correta ao ser inicializado, o que pode levar a problemas de desempenho e estabilidade. Veja abaixo uma lista de problemas comuns e suas soluções para garantir que o software funcione com a GPU correta.

Para saber qual GPU é usada, você pode verificar o [arquivo de log](../../exporting-the-log-file.md).

## Windows

### Configuração dos cabos do monitor

No Windows, a GPU atribuída a um aplicativo depende do monitor no qual o aplicativo está sendo executado. Isso ocorre porque os cabos do monitor são vinculados diretamente à saída da própria GPU. O aplicativo pode iniciar na GPU errada, portanto, se o monitor no qual ele é iniciado estiver vinculado à saída gráfica da placa-mãe em vez de à saída da própria placa gráfica. Nesse caso, é provável que o Windows use a GPU integrada em vez da GPU dedicada.

<b>Para resolver esse problema</b>: basta corrigir a configuração do cabo desplugando o monitor vinculado à placa-mãe e, em vez disso, vinculando-o às saídas de GPU.

### Instalação incorreta do driver de GPU

Se os drivers da GPU não estiverem instalados corretamente, o aplicativo não conseguirá acessar a GPU dedicada e terá que fazer fallback na GPU integrada.

<b>Para resolver esse problema</b>: desinstale os drivers de GPU atuais, execute uma limpeza e reinstale os drivers de GPU após uma reinicialização do computador.

### Configuração de perfil do driver de GPU Nvidia

Em alguns computadores, como laptops, o aplicativo pode ser executado na GPU integrada em vez da GPU Nvidia dedicada por padrão. Com uma GPU NVIDIA, a alternância para a GPU direita depende dos perfis de aplicativos. Se um aplicativo não tiver esse perfil, você poderá atribuir um manualmente.

<b>Para resolver este problema</b>:

1. Clique com o botão direito do mouse na Área de trabalho e selecione Painel de Controle NVIDIA <b>ou</b> Navegue até o Painel de Controle e procure por Painel de Controle NVIDIA
1. Em <b>Configurações 3D</b>, vá para <b>Gerenciar Configurações 3D</b>
1. Na guia <b>Configurações do programa</b>, adicione um novo perfil para o <b>Substance 3D Painter</b>
1. Altere a configuração do processador gráfico preferido para Processador de alto desempenho NVIDIA

### Configuração de Desempenho do Windows

O Windows pode ter definido a configuração incorreta de GPU para o aplicativo devido às configurações padrão de desempenho e consumo de energia.

<b>Para resolver esse problema: </b>siga o passo a passo abaixo para substituir a configuração de GPU padrão.

1. Abra as configurações de vídeo clicando com o botão direito do mouse na área de trabalho:

   ![](../../../assets/settings-33.png)
1. Navegue até a parte inferior da janela na página inicial e clique em “Configurações de gráficos”:

   ![](../../../assets/graphics-settings.png)
1. Clique no botão “Procurar” e localize o executável do Substance 3D Painter:

   ![](../../../assets/browse-16.png)
1. Depois de adicionar o aplicativo, clique no botão “Opções”:

   ![](../../../assets/options-19.png)
1. Escolha a configuração “Alto desempenho” e clique no botão “Salvar”

   ![](../../../assets/specs.png)

## Linux

### Desativar “Prefere GPU não padrão”

Ao executar o Painter a partir de um atalho da área de trabalho ou ao executá-lo via Steam, verifique se a configuração <b>PreferencesNonDefaultGPU</b> no arquivo <b>\*.desktop</b> está definida como <b>false</b>.

Essa configuração pode ser enganosa e fazer com que a GPU integrada seja usada/forçada em vez da discreta e mais poderosa. Para obter mais informações, [veja esta discussão](https://github.com/ValveSoftware/steam-for-linux/issues/9940).

### Forçar GPU específica usando a variável de ambiente DRI\_PRIME

Por padrão, o Painter usará a primeira GPU listada pela API de gráficos Vulkan, mas essa GPU pode ser errada (pode ser a GPU integrada listada primeiro), levando a um desempenho ruim. A variável de ambiente DRI\_PRIME pode ser usada para forçar a GPU de sua escolha. Para obter mais informações, [consulte a documentação da wiki do Arch](https://wiki.archlinux.org/title/PRIME#For_open_source_drivers%E2%80%94PRIME). Você também pode consultar a [documentação do Mesa](https://docs.mesa3d.org/envvars.html#envvar-DRI_PRIME).
