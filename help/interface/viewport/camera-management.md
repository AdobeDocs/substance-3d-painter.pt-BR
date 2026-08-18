---
helpx_url: 'https://helpx.adobe.com/br/substance-3d-painter/interface/viewport/camera-management.html'
breadcrumb-title: ''
description: Saiba como gerenciar as exibições de câmera no visor do Substance 3D Painter para navegar e enquadrar seus modelos 3D de forma eficaz.
helpx_creative_field: ''
helpx_description: Painter > Interface > Viewport > Camera management
helpx_experience_level: ''
helpx_learn_topic: ''
helpx_tags: ''
title: Gerenciamento de câmera
user-guide-description: ''
user-guide-title: ''
source-git-commit: e370ba212d3e90f71e09b75ff41be6123d37c5eb
workflow-type: tm+mt
source-wordcount: '469'
ht-degree: 0%

---


# Gerenciamento de câmera

Câmeras criadas no Maya, Max, Blender, Modo e DAE podem ser importadas para o Substance 3D Painter.

>[!NOTE]
>
> Câmeras ortográficas e proporções de exibição não são corretamente suportadas no formato ABC (Alembic).

## Importar câmeras no Substance 3D Painter

As câmeras devem ser incluídas no arquivo de malha, no formato FBX ou ABC (Alembic).

O nome, os parâmetros de transformação, o CDV e a proporção (se existir) são importados.

Na janela Novo projeto, selecione o arquivo de malha que inclui as câmeras e verifique se a caixa de seleção **Importar câmeras** está marcada. Se você ativar **Reimportar malha** na **janela Editar > Configuração do projeto**, também poderá ativar **Importar câmeras** se as tiver perdido na criação inicial do projeto.

Em seguida, clique em **OK**:

<table>
  <tr style="border: 0;">
    <td style="border: 0;" valign="top"><img src="../../assets/New-project-window-full.png" alt=""/></td>
    <td style="border: 0;" valign="top"><img src="../../assets/project-configuration-full.png" alt=""/></td>
  </tr>
</table>

## Selecionar câmeras

Quando as câmeras forem importadas para o seu projeto atual, você poderá selecionar qual câmera estará ativa no **menu suspenso** no **Visor 3D**.

Por padrão, a câmera do Painter chamada “Câmera padrão” está selecionada e no modo de perspectiva.

![](../../assets/camera-select.png)

No exemplo fornecido acima, 3 câmeras são importadas, totalizando 4 câmeras no menu suspenso quando a câmera padrão é incluída.

## Controle as câmeras

Quando uma câmera importada é selecionada, mover a câmera panoramicamente, aplicando zoom ou girando no Visor muda para a Câmera padrão. Isso evita que as câmeras importadas sejam movidas na cena.

>[!NOTE]
>
> Se precisar alterar a posição da câmera importada, você pode atualizá-la no aplicativo de edição de cena escolhido e reimportar a cena com **Editar > Configuração do projeto**.

Você pode controlar os parâmetros das câmeras importadas na **janela Configurações de exibição**.

![](../../assets/display-settings-cameras.png)

Use o menu suspenso **Predefinição** para selecionar a câmera a ser modificada.

Se qualquer um dos atributos for modificado, é possível reverter para seus valores originais com o **botão Restaurar**.

![](../../assets/camera-restore.png)

Se um parâmetro tiver sido modificado para uma câmera importada, o nome da câmera ficará em itálico e um “\*” será adicionado ao nome da câmera.

### Atributos da câmera

O campo de visão ou CDV é expresso em graus.

A Distância focal é expressa em mm.

No modo de visualização (OpenGL), a distância de foco e a abertura são desativadas. Para ativá-los, é necessário ativar o Post Effects e o DOF.

### Exibir proporção

Se a taxa de exibição estiver presente no arquivo de malha, ela será exibida na seção Câmera. Se uma câmera não tiver uma taxa de exibição definida, ela será listada como **Não Especificada** (como a câmera padrão).

### Bloquear

Para bloquear uma câmera, clique no ícone de cadeado. Bloquear uma câmera evita alterações nos parâmetros da câmera.

![](../../assets/image2018-7-26-15-47-6.png)

## Moldura da câmera

O quadro da câmera pode ser alternado em **Configurações de exibição > Configurações do visor**:

![](../../assets/image2018-7-26-15-54-58.png)

Você também pode ajustar a opacidade da área fora do quadro com a **Opacidade da máscara de porta**.

<table>
  <tr style="border: 0;">
    <td style="border: 0;" valign="top"><img src="../../assets/image2018-7-26-15-58-45.png" alt=""/></td>
    <td style="border: 0;" valign="top"><img src="../../assets/image2018-7-26-15-58-53.png" alt=""/></td>
  </tr>
</table>
