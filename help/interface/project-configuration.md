---
helpx_url: 'https://helpx.adobe.com/br/substance-3d-painter/interface/project-configuration.html'
breadcrumb-title: ''
description: Saiba como definir as configurações do projeto no Substance 3D Painter para definir a resolução da textura, os canais e as propriedades do projeto.
helpx_creative_field: ''
helpx_description: Painter > Interface > Project configuration
helpx_experience_level: ''
helpx_learn_topic: ''
helpx_tags: ''
title: Configuração do projeto
user-guide-description: ''
user-guide-title: ''
source-git-commit: 3e4ef9bd5897f042b01d6c0819ec06cc21ba208a
workflow-type: tm+mt
source-wordcount: '839'
ht-degree: 3%

---


# Configuração do projeto

![](../assets/project-configuration-full.png)

A janela de configuração Projeto possui controles para modificar as configurações do projeto. As configurações do projeto geralmente são definidas ao criar um novo projeto, mas às vezes pode ser necessário fazer alterações nessas configurações posteriormente no projeto.

## Malha 3D

Se tiverem sido feitas alterações na malha 3D ou no arquivo de malha, você poderá reimportar a malha enquanto ainda mantém os outros dados do projeto. Verifique **Reimportar malha** e certifique-se de que o arquivo correto está sendo importado.

A reimportação da malha é geralmente útil quando você precisa:

* Atualizar a topologia do modelo 3D
* Atualizar os UVs
* Adicionar ou Remover [Conjuntos de Texturas](texture-set/texture-set.md)

| **Parâmetro** | **Descrição** |
| --- | --- |
| **Malha 3D** | Indica o caminho para o arquivo de modelo 3D. Use o **botão Selecionar** para alterar o arquivo de origem do projeto. |
| **Reimportar malha** | Se habilitado, o arquivo de malha será importado novamente ao clicar em OK na parte inferior da interface. Esse parâmetro é automaticamente marcado se o botão Selecionar for usado para especificar um arquivo de malha diferente do arquivo de malha original. |

>[!NOTE]
>
> Se as IDs de material forem alteradas ou renomeadas ao reimportar a malha do projeto, os Conjuntos de Textura anteriores no projeto podem ser desativados, dando a aparência de texturas ausentes. Isso pode ser corrigido com a [Janela de Reatribuição](texture-set/texture-set-reassignment.md) da **Lista de Conjuntos de Texturas**.

## Configurações do projeto

Esta seção controla várias configurações relacionadas ao projeto:

<table>
  <tr>
    <th><em>Configuração</em></th>
    <th><em>Descrição</em></th>
  </tr>
  <tr>
    <td><strong>Formato de mapa normal</strong></td>
    <td>Define o formato do mapa normal usado para a malha no visor. Este parâmetro afeta somente os <a href="shader-settings/shader-settings.md">sombreadores</a> do visor e dos mapas de malha dos <a href="../baking/baking.md">padeiros</a>. A pilha de camadas é independente. Valor recomendado para aplicativos comuns:<br><br><ul><li><strong>Unidade</strong>: OpenGL</li><li><strong>Mecanismo Irreal</strong>: DirectX</li><li><strong>Maya</strong>: OpenGL</li><li><strong>3DS Máx</strong>: DirectX</li><li><strong>Mesclador</strong>: OpenGL</li></ul></td>
  </tr>
  <tr>
    <td><strong>Calcular espaço tangente por fragmento</strong></td>
    <td>Determina como calcular e exibir mapas normais na viewport para sombreamento e iluminação. Se habilitada, a tangente e os binormais da malha serão computados por pixel em vez de por vértice.<br>Valor recomendado para aplicativos comuns:<br><br><ul><li><strong>Unidade</strong>: desabilitada (habilitada se estiver usando HDRP)</li><li><strong>Mecanismo Irreal</strong>: habilitado</li></ul></td>
  </tr>
</table>

>[!NOTE]
>
> Alterar o formato normal ou o cálculo da tangente requer voltar a preparar os mapas de malha para garantir que a aparência nas viewports esteja correta.

### Configurações específicas do tipo de arquivo

Quando um formato de malha USD é selecionado, outras configurações específicas do tipo de arquivo ficam disponíveis.

![](../assets/image2023-1-30-11-16-6.png){width="473px"}

<table>
  <tr>
    <th><em>Parâmetro</em></th>
    <th><em>Descrição</em></th>
  </tr>
  <tr>
    <td><strong>Escopo e variantes</strong></td>
    <td>Selecione uma parte específica de um arquivo do USD. Por padrão, é definido como “Raiz”, o que significa que o arquivo USD inteiro será usado no projeto do Painter. <strong>Alterar...</strong> abre uma nova janela que exibe o conteúdo do USD. Se forem detectadas variantes, você poderá selecionar uma variante específica para carregar no projeto.<br><br>Observação:<br><ul><li>Somente a seleção da variante de modelagem terá qualquer impacto.</li><li>Variantes aninhadas dentro de variantes não são detectadas no momento.</li></ul></td>
  </tr>
  <tr>
    <td><strong>Nível de subdivisão</strong></td>
    <td>Aplica-se à geometria com subdivisão. Especifique o quanto subdividir a malha para texturização no Painter. Se a subdivisão for explicitamente definida como 'none' no arquivo USD, essa configuração ficará acinzentada. A subdivisão é aplicada após o desencapsulamento UV, de modo que não alteraria a forma dos UVs da malha.</td>
  </tr>
  <tr>
    <td><strong>Quadro</strong></td>
    <td>Aplica-se a USDs nos quais a animação é detectada. Selecione o quadro que será carregado no projeto do Painter. Se não houver animação no arquivo USD selecionado, essa configuração ficará acinzentada.</td>
  </tr>
</table>

## Configurações de Blocos UV

Esta seção tem controles para alternar o uso de UDIMs no projeto. Não é possível alterar essas configurações após a criação do projeto, mas você pode visualizar as configurações do projeto aqui. Para obter mais informações, consulte a [documentação de Blocos UV](../features/uv-tiles/uv-tiles.md).

## Configurações de importação

Estas configurações controlam como a malha selecionada será importada:

| *Configuração* | *Descrição* |
| --- | --- |
| **Importar câmeras** | Se ativadas, as câmeras presentes no arquivo de malha também serão importadas e estarão disponíveis na viewport 3D. |
| **Preservar posições de traçados na malha** | Essa configuração controla como os traçados de pincel serão recalculados após a importação de uma nova malha 3D. É recomendável manter essa configuração ativada na maioria dos casos. Para obter mais detalhes, consulte a documentação da [Reprojeção UV](../features/uv-reprojection.md). |
| **Desempacotamento Automático** | Desempacotamento automático de UV. Clique no botão Opção para configurar o processo. Para obter mais informações, consulte a [Documentação de desencapsulamento automático de UV](../features/automatic-uv-unwrapping.md). |

### Configurações do tamanho físico

Ajuste o [Tamanho físico](../features/physical-size.md) da malha importada.

| *Configuração* | *Descrição* |
| --- | --- |
| **Usar a escala da unidade interna do arquivo de malha** | Se a malha tiver sido criada com medidas fisicamente precisas, deixe essa opção selecionada para manter a mesma tamanho físico no Painter. |
| **Escala de unidade personalizada** | Se a malha não foi criada com o tamanho físico em mente, use essa opção para personalizar o tamanho da malha. Você precisará saber o tamanho físico desejado e o tamanho em unidades da malha importada para determinar esse valor. |
| **Alternar o dimensionamento da camada de preenchimento para o Tamanho físico ao atribuir materiais** | Quando ativadas, as camadas e efeitos de preenchimento alternarão automaticamente o método de dimensionamento para Tamanho físico ao atribuir um material que tenha propriedades de Tamanho físico. |

### Configurações de gerenciamento de cores

Esta seção controla as configurações relacionadas à conversão de cores. Para obter mais informações, consulte a documentação do [Gerenciamento de cores](../features/color-management/color-management.md).
