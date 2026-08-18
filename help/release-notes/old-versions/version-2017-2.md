---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/release-notes/old-versions/version-2017-2.html"
breadcrumb-title: ''
description: Revise as notas de versão do Substance 3D Painter versão 2017.2 para saber mais sobre novos recursos, aprimoramentos e correções de erros.
helpx_creative_field: ""
helpx_description: Painter > Release notes > Old versions > Version 2017.2
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Versão 2017.2
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '426'
ht-degree: 0%

---


# Versão 2017.2

O **Substance Painter 2017.2** introduz um novo recurso poderoso por meio do sistema de pontos de ancoragem. Ele permite criar configurações mais avançadas na pilha de camadas, o que abre muitas novas possibilidades.

Data de lançamento: *27 de julho de 2017*

## Principais recursos

### Novo efeito de ponto de ancoragem

![](../../assets/anchor-height-blend-optim.gif)

**Um novo tipo de efeito** foi adicionado ao Substance Painter, próximo ao já existente, como **Filtro** e **Nível**. Agora você pode encontrar o novo **Ponto de ancoragem**. Este novo efeito permite definir um **local** na **pilha de camadas** que pode ser **referenciado** no restante do projeto em qualquer outra camada. Isso permite, por exemplo, usar as informações de height de uma camada na máscara de uma camada logo acima dessa, permitindo uma mesclagem mais natural (conforme ilustrado pelo gif acima).

Como a Âncora funciona como efeito, ela pode ser criada em **muitas situações**: o **conteúdo** de uma camada, a **máscara** e até mesmo como um filtro de **passagem**. O efeito também funciona mesmo que a camada onde está localizada esteja desativada. Observe que a Âncora define apenas um local, não o que você pode recuperar dele. Essas informações são definidas no local em que a referência à âncora é criada.

Para obter mais detalhes técnicos e exemplos, consulte a página dedicada: [Ponto de ancoragem](../../features/effects/anchor-point.md)

### Novas várias melhorias

Juntamente com o novo efeito de ponto de ancoragem, também trabalhamos em:

* A capacidade de renomear alguns efeitos, como Preenchimento e Pintura
* Novas funções de script, permitindo criar um link em tempo real com outros aplicativos, como o Unity

## Tutorial

Os novos recursos são abordados em detalhes nos nossos vídeos mais recentes:

## Notas de versão

### 2017.2

(Lançado em 27 de julho de 2017)

**Adicionado:**

* [Efeito] Novo ponto de ancoragem que permite a referência de camada e máscara
* [Camadas] Capacidade de renomear efeitos de preenchimento e pintura
* [Plugin] Plug-in Substance Source atualizado
* [Scripting] Permitir consultar Resolução de Conjunto de Textura
* [Script] Permite obter o status do mecanismo de pintura
* [Desempenho] Otimizações aprimoradas de carregamento e carimbo de pincel no projeto

**Corrigido:**

* [Ferramenta] Problemas de desempenho ao ajustar parâmetros de material
* [Engine] Desaparecimento de pinceladas ao alterar a resolução (4K>2K)
* [Exibição 3D] O espaço tangente não é sincronizado com padeiros
* [Prateleira] O caminho de prateleira nos documentos do usuário não é criado automaticamente
* [Prateleira] Fazer predefinições compatíveis com versões anteriores após uma atualização
* [Shader] O sombreador não PBR não funciona mais
* [Padeiros] Falha no cozimento do mapa de ID com a opção Corresponder pelo nome ativada
* [Amostra] Os nomes dos conjuntos de texturas do projeto de amostra do Mat da reunião estão incorretos
* Salvar um projeto antes de criar um modelo retorna erros de permissão de gravação
