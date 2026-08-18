---
helpx_url: "https://helpx.adobe.com/br/substance-3d-painter/technical-support/technical-issues/stability-issues/crash-when-opening-or-saving-a-file.html"
breadcrumb-title: ''
description: Saiba como corrigir falhas do Substance 3D Painter ao abrir ou salvar arquivos para gerenciamento de projeto confiável.
helpx_creative_field: ""
helpx_description: Painter > Technical support > Technical Issues > Stability Issues > Crash when opening or saving a file
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Falha ao abrir ou salvar um arquivo
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '225'
ht-degree: 0%

---


# Falha ao abrir ou salvar um arquivo

Existem alguns motivos pelos quais o Substance 3D Painter trava no Windows ao abrir uma caixa de diálogo de arquivo. Esta página agrupa motivos e soluções para esse problema.

## Conflitos de software

Alguns programas podem adicionar extensões de shell personalizadas que podem levar a instabilidades ou falhas. Confira a lista de [Conflitos de software](../startup-issues/software-conflicts.md) para obter mais informações.

## Extensões do shell/Temas personalizados

Os temas personalizados não são compatíveis com nossa estrutura de GUI, portanto, é altamente recomendável desinstalar o tema atual antes de usar o Substance 3D Painter.

Os computadores **Alienware** / **Dell** integram por padrão algumas extensões de shell que são conhecidas por serem incompatíveis com o Substance 3D Painter. Recomendamos que você os desinstale. Embora não saibamos exatamente todas as extensões incompatíveis, na maioria das vezes elas correspondem a:

* Classe DBROverlayIconBackup.DBROverlayIconBackuped
* Classe DBROverlayIconNotBackuped.DBROverlayIconNotBackup

É possível ver quais extensões estão instaladas no computador usando a seguinte ferramenta. Veja um procedimento aproximado sobre como proceder:

1. Baixar e instalar ShellExView da NirSoft: <http://www.nirsoft.net/utils/shexview.html>
1. Executar o programa
1. Clique em **Opção** e escolha **Filtrar por tipo de extensão**
1. Selecionar **Manipulador de Sobreposição de Ícone**
1. Você deve ver as duas entradas para **Reprodução de Alienígena**.
1. Selecione **ambos** e clique no botão vermelho para desabilitá-los.
