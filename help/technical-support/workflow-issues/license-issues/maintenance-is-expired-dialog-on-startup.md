---
helpx_url: "https://helpx.adobe.com/br/substance-3d-painter/technical-support/workflow-issues/license-issues/maintenance-is-expired-dialog-on-startup.html"
breadcrumb-title: ''
description: Saiba como resolver a caixa de diálogo de manutenção expirada que aparece na inicialização no Substance 3D Painter para gerenciamento de licenças.
helpx_creative_field: ""
helpx_description: Painter > Technical support > Workflow Issues > License Issues > Maintenance is expired dialog on startup
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: A caixa de diálogo Manutenção expirou na inicialização
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '410'
ht-degree: 1%

---


# A caixa de diálogo Manutenção expirou na inicialização

![](../../../assets/expired-mainteance-message.png)

Ao iniciar o aplicativo, uma caixa de diálogo com a mensagem “Sua manutenção atual expirou” pode ser exibida. Esta página lista soluções sobre como evitar esta caixa de diálogo.

## Solução 1: atualize o arquivo de licença

A mensagem de aviso aparece porque o arquivo de licença é muito antigo e precisa ser atualizado. Para fazer isso, basta **reativar o produto** por meio do assistente de aplicativos. O arquivo de licença também pode ser baixado manualmente pelo site da Substance 3D: <https://www.substance3d.com/>.

## Solução 2: edite as configurações de preferência para ocultar a caixa de diálogo

>[!NOTE]
>
> Recomendamos tentar atualizar o arquivo de licença primeiro, antes de usar esta solução alternativa.

Outra solução é ocultar a mensagem de aviso, colocando uma configuração específica.

Navegue até o local de preferência do aplicativo:

<table data-preserve-html="true"><colgroup> <col/> <col/> <col/> </colgroup><tbody><tr><th>Sistema</th><th>Versão</th><th>Caminho</th></tr><tr><td rowspan="2"><p><strong>Windows</strong></p><p>(registro)</p></td><td><strong>7.2</strong> ou mais recente</td><td>HKEY_CURRENT_USER\Software\Adobe\Adobe Substance 3D Painter</td></tr><tr><td>Legado</td><td>HKEY_CURRENT_USER\Software\Allegorithmic\Substance Painter</td></tr><tr><td rowspan="2"><p><strong>Mac</strong></p><p>(biblioteca)</p></td><td><strong>7.2</strong> ou mais recente</td><td>/Users/[nome do usuário]/Library/Preferences/com.adobe.Adobe Substance 3D Painter.plist</td></tr><tr><td>Legado</td><td>/Users/[nome do usuário]/Library/Preferences/com.substance3d.Substance Painter.plist</td></tr><tr><td rowspan="2"><strong>Linux</strong></td><td><strong>7.2</strong> ou mais recente</td><td>/home/[nome do usuário]/.config/Adobe/Adobe Substance 3D Painter.conf</td></tr><tr><td>Legado</td><td>/home/[nome do usuário]/.config/Allegorithmic/Substance Painter.conf</td></tr></tbody></table>

### Windows

Para definir a variável no Windows, siga estas etapas:

1. Abra o menu Iniciar.
1. Procure por **Regedit** para abrir o editor do Registro.
1. Navegue até a chave de registro listada na tabela acima.
1. Clique na chave de registro nomeada como software na exibição de árvore à esquerda.
1. Clique com o botão direito do mouse na área vazia no painel direito e escolha **Novo > Valor da cadeia de caracteres**.
1. Nomeie o novo valor como **DisableLicenseWarningPopup** e pressione enter para validar.
1. Clique duas vezes no valor recém-criado.
1. Definir o campo de dados Valor como: **true**
1. Salve a alteração.
1. Inicie o aplicativo.

### MacOS

1. Abrir uma nova janela do **Finder**
1. Navegue até o caminho listado na tabela acima.
1. Clique com o botão direito no arquivo **plist** e escolha **Abrir com > Xcode**.
1. Na parte superior da lista, adicione uma nova chave denominada **DisableLicenseWarningPopup**
1. Definir o tipo de chave como **cadeia**
1. Definir o valor da chave como **verdadeiro**
1. Salvar e fechar o arquivo.
1. Inicie o aplicativo.

### Linux

Para definir a variável no Linux, siga estas etapas:

1. Navegue até a lista de caminhos na tabela acima.
1. Abra o arquivo **.conf** presente na pasta.
1. Adicione uma nova linha sob a linha **[Geral]**
1. Na nova linha, cole o seguinte texto: **DisableLicenseWarningPopup=true**
1. Salve o arquivo.
1. Inicie o aplicativo.
