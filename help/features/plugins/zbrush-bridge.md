---
breadcrumb-title: ''
description: Revise todas as alterações e atualizações nas versões do Substance 3D Painter para acompanhar a evolução e as melhorias de recursos ao longo do tempo.
title: ZBrush para Painter Bridge
user-guide-description: ''
user-guide-title: ''
source-git-commit: c50b48e520277293b9ddef466baf8e27db4891ab
workflow-type: tm+mt
source-wordcount: '609'
ht-degree: 0%

---


# ZBrush para Painter Bridge

A partir do ZBrush 2026.2.0 (a atualização do Maxon One de abril de 2026) e do Substance 3D Painter 12.0.2 (versão Steam e CC), é possível enviar modelos diretamente do ZBrush para o Painter por meio de um plug-in instalado automaticamente com a versão mais recente do ZBrush.

![Uma imagem promocional que mostra um ativo renderizado enquanto é sobreposto pelo mesmo ativo no Zbrush e no Painter.](../../assets/zbrush_promotional.png)

Com o plug-in Substance Bridge, não há necessidade de passar pelo longo processo de exportação de arquivos separados de polígonos baixos e altos, sua importação para o Painter e sua configuração e execução.

Para começar a usar a ponte Zbrush para Painter:

1. Certifique-se de que você tenha pelo menos a versão 2026.2.0 do ZBrush instalada.
1. Habilite o plug-in no Painter verificando se **Python > zbrush_painter_plugin** está marcado.
1. Do ZBrush, o **Enviar para o Painter** está disponível em **Textura > Ponte de Substance**

![Uma imagem do plug-in Substance Bridge no ZBrush](../../assets/zbrush_painterSendTo.png)

## Configuração

Você pode definir as seguintes configurações para a criação automática de projetos no Painter:

| Configuração | Descrição |
| --- | --- |
| Enviar para o Painter | Envia o modelo para o Substance 3D Painter com as configurações atuais aplicadas. Cada clique cria um novo projeto de Substance a partir do zero. |
| **Subferramentas** | |
| Tudo | Envia todas as Subferramentas independentemente da visibilidade. Se o globo ocular estiver ligado ou desligado, tudo é enviado. |
| Visível | Envia somente Subferramentas com o ícone de olho ativado na lista Subferramentas. |
| Ativo | Envia somente a SubFerramenta atualmente selecionada |
| Enviar PolyPaint | Converte PolyPaint em um mapa de textura e o aplica como uma camada de preenchimento em Substance, onde você pode pintar sobre ele e misturar com ele. |
| Normais suaves | Suaviza os normais tangentes na exportação para que as malhas facetadas pareçam suaves em Substance, combinando com a forma como os mecanismos de jogo as renderizam. Desative para ver a faceta real da geometria. |
| Mapas de Cozimento Automático | Executa os algoritmos de Substance automaticamente após a chegada do modelo, gerando mapas normais, oclusão ambiente, curvatura e outros mapas de detalhes da comparação de malha alta/baixa. |
| Forçar o Desajuste Automático do UV | Aciona o algoritmo de desencapsulamento Substance em cada SubTool que chega. Saia se o seu modelo já tem bons UVs porque isso os sobregrava. |
| Nível de subdivisão | Controla quais níveis de subdivisão são enviados. Atual envia somente o nível exibido. Baixo e alto envia os níveis mais baixo e mais alto para panificação e é a opção recomendada para a maioria dos fluxos de trabalho. |
| Conjuntos de textura | Controla como o espaço UV é dividido em Substance: Por Subferramenta (um conjunto de textura por Subferramenta) ou Por PolyGroup (um conjunto de textura por PolyGroup em cada SubTool). |

Quando o Painter receber o modelo, se o cozimento automático estiver ativado, o cozimento será iniciado. A subdivisão mais baixa do modelo é a malha importada como a malha de baixo-poli, e a subdivisão mais alta é usada como a de alto-poli para assar os detalhes. O ZBrush pode manipular um número muito maior de polígonos do que o Painter, portanto, certifique-se de que a malha poli baixa tenha um tamanho de trabalho ideal (isso dependerá da máquina, mas menos de 1 milhão é o melhor).

Os Conjuntos de texturas no Painter representam atribuições de material. Um conjunto de texturas é igual a um espaço UV.

* Por subferramenta cria um conjunto de textura para cada subferramenta (todas as partes da subferramenta compartilhariam o mesmo espaço UV), que é a opção mais simples.
* Per PolyGroup cria um conjunto de texturas por PolyGroup dentro de cada SubTool, oferecendo um controle mais preciso sobre as atribuições de materiais.

>[!NOTE]
>
>Com a versão Steam do Painter, o Painter precisa estar aberto para receber o modelo ZBrush.


## Recursos adicionais

[Assista a este vídeo](https://www.youtube.com/watch?v=fLkkwV4BzrU) para ver o Bridge em ação ou acesse a [documentação do ZBrush](https://help.maxon.net/zbr/en-us/Default.htm#html/reference-guide/texture/substance-bridge/substance-bridge.html?Highlight=painter) para obter mais informações.
