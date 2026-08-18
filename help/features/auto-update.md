---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/features/auto-update.html"
breadcrumb-title: ''
description: Saiba como usar a atualização automática de recursos no Substance 3D Painter para manter suas bibliotecas de recursos sincronizadas e atualizadas.
helpx_creative_field: ""
helpx_description: Substance 3D Painter
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Atualização automática de recursos
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '676'
ht-degree: 1%

---


# Atualização automática de recursos

![](../assets/banner_autoupdate.jpg)

A atualização automática de recursos, ou <b>atualização automática</b>, é um recurso da [janela Ativos](../interface/assets/assets.md) que permite recarregar e atualizar recursos quando novas versões estiverem disponíveis. Esse processo pode ser acionado automática ou manualmente na interface ou por meio de scripts Python.

![](../assets/auto_update_menu.png)

## Tutorial

Você pode assistir a um tutorial rápido para obter uma visão geral do recurso:

## Ativar atualização automática

![](../assets/auto_update_red_icon.png)

Para habilitar a <b>atualização automática</b>, basta ir para a parte inferior da janela Ativos e clicar no ícone de setas duplas. Isso abrirá o menu de atualização automática com todas as suas configurações. Em seguida, habilite uma das opções disponíveis na seção <b>atualizações automáticas</b>.

### Atualizações automáticas

![](../assets/auto-update_auto_settings.png)

As configurações de atualização automática controlam a frequência com que o aplicativo deve procurar atualizações e onde.

| Configuração | Descrição |
| --- | --- |
| <b>Painel Ativos</b> | Se ativada, a atualização automática procurará ativos para atualizar em todas as bibliotecas carregadas atualmente. Isso inclui o projeto atual. No entanto, ele não atualizará os recursos usados na pilha de camadas, configurações de exibição, configurações de sombreador etc. |
| <b>Recursos usados no projeto</b> | Se ativado, a atualização automática procurará ativos para atualizar que são atualmente importados e usados pelo projeto atual. Isso se aplica a recursos usados na pilha de camadas, configurações de exibição, configurações de sombreador etc. |
| <b>Atualizar a cada x minutos</b> | Controle a frequência com que o aplicativo procura uma atualização de recursos. Um atraso de 0 minutos acionará uma atualização a cada poucos segundos. Observe que esse atraso baixo pode criar problemas de desempenho. |

>[!NOTE]
>
> Se as atualizações automáticas estiverem ativadas, o aplicativo procurará as alterações automaticamente cada vez que recuperar o foco.

### Atualizações manuais

![](../assets/auto-update_manual.png)

As ações de atualização manual são uma maneira conveniente de acionar o sistema de atualização quando desejado. Eles podem ser usados com ou sem as configurações de atualização automática ativadas.

| Configuração | Descrição |
| --- | --- |
| <b>Atualizar painel de ativos</b> | Inicie o processo de atualização automática. Comporte-se da mesma maneira que a configuração do <b>painel Ativos</b> (veja acima). |
| <b>Atualizar recursos usados no projeto</b> | Inicie o processo de atualização automática. Comporte-se da mesma maneira que os <b>Recursos usados no projeto</b> (veja acima). |

## Configurações avançadas

![](../assets/auto-update_mismatch.png)

As configurações avançadas permitem controlar o comportamento do processo de atualização.

| Configuração | Descrição |
| --- | --- |
| <b>Ignorar ativos quando seus parâmetros não coincidirem</b> | Se ativado, o processo de atualização automática evitará a atualização de recursos se a nova versão não corresponder à versão antiga. Por exemplo, se um material Substance tiver parâmetros que não existem mais na nova versão (porque foram removidos ou renomeados), o processo de atualização ignorará o recurso e manterá a versão antiga. |

>[!NOTE]
>
> Para forçar a atualização de ativos que têm uma incompatibilidade, você pode desabilitar a configuração <b>Ignorar ativos quando seu parâmetro não corresponder</b>.

## Status da atualização e log

![](../assets/auto-update_log.png)

Após a atualização de recursos (automática ou manual), o resultado do processo aparecerá na guia <b>Ativos</b> na janela <b>Log</b>, relatando atualizações e problemas bem-sucedidos. Em caso de incompatibilidade de recursos (veja acima), os detalhes do problema serão fornecidos por recurso.

O registro pode ser aberto rapidamente clicando no ícone dedicado na parte superior direita do menu de atualização automática:

![](../assets/auto_update_log_icon.png)

>[!NOTE]
>
> Quando um ou mais problemas aparecerem após uma atualização, o ícone de registro exibirá um pequeno ícone de aviso.

Dependendo do andamento do processo de atualização, vários tipos de problemas podem aparecer:

| Problema | Descrição |
| --- | --- |
| <b>Não foi possível atualizar no painel Ativos</b> | Esta mensagem significa que um problema impediu que o sistema de atualização prosseguisse. Expanda o nome do recurso para obter mais informações. |
| <b>(nome do arquivo).(formato) não existe. Não é possível recarregar (nome do recurso)</b> | Esta mensagem significa que o arquivo de origem de um recurso não pode mais ser encontrado (porque ele foi movido ou removido). Uma correção simples é reimportar o recurso ou realocá-lo na janela Ativos (por meio do menu do botão direito do mouse). |

## Mensagem antiga do projeto

![](../assets/auto_update_old_project_dialog.png.img.png)

Ao abrir um projeto antigo, uma opção estará disponível no aviso da mensagem pop-up para informar sobre o processo de atualização automática. Essa é uma maneira conveniente de desativar rapidamente o processo de atualização automática, caso ele permaneça ativado antes de abrir o projeto antigo.
