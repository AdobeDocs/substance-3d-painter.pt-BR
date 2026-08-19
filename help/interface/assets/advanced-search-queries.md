---
helpx_url: "https://helpx.adobe.com/br/substance-3d-painter/interface/assets/advanced-search-queries.html"
breadcrumb-title: ''
description: Saiba como criar consultas de pesquisa avançada no Substance 3D Painter para encontrar ativos específicos usando critérios de pesquisa complexos.
helpx_creative_field: ""
helpx_description: Painter > Interface > Assets > Advanced search queries
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Consultas de pesquisa avançada
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '458'
ht-degree: 0%

---


# Consultas de pesquisa avançada

Consultas de pesquisa avançadas permitem construir pesquisas complexas e reutilizá-las como [pesquisas salvas](saved-searches.md).

Consultas avançadas podem ser usadas na barra de pesquisa e podem conter -

1. **Caminho** : permite refinar o resultado de uma pesquisa por uma estrutura de pasta/pasta.
1. **Uso** : lista todos os usos possíveis que estão disponíveis no aplicativo
1. **Consulta de texto**: permita adicionar qualquer outro tipo de consulta livremente (como palavras-chave personalizadas)

Seleções múltiplas são permitidas ao definir uma nova consulta de pesquisa.

## Caminho

A consulta de caminho permite refinar uma consulta com base em um caminho. O painel **Filtrar por caminho** lista todas as bibliotecas disponíveis (que você pode adicionar por meio de Editar > Configurações > Bibliotecas).\
É possível usar a definição de caminho para filtrar por caminho de biblioteca personalizado ou por subpastas específicas na hierarquia.

## Uso

Uso defina o que é um recurso e como usá-lo no Substance 3D Painter. Alguns podem ser definidos pelo tipo de arquivo do recurso.\
Por exemplo-

* **pbr.glsl**: um arquivo de sombreador - ele só pode ser usado como um sombreador e nada mais.
* **effect.sbsar**: um arquivo substance - ele pode ser um gerador, um filtro ou até mesmo um material. Portanto, se seu uso não estiver definido no gráfico original (no Designer), ele deverá ser indicado pelo usuário no Painter no momento da importação.

## Texto

A consulta de texto suporta vários tipos de filtragem, alguns mais avançados que a interface normal.\
Eles podem ser ativados digitando as palavras-chave corretas.

* **Tipos de pesquisa disponíveis** :
  * &quot; **n:** &quot; : nome
  * &quot; **s:** &quot; : prateleira/biblioteca (inclui “sessão” e “projeto”)
  * &quot; **p:** &quot; : caminho
  * &quot; **u:** &quot; : uso
* **Escapando** : é possível usar &quot; **\** &quot; antes do caractere que precisa ser escapado ou usar aspas, por exemplo:
  * **um\ nome\ com\ espaços**
  * **”um nome com espaços”**
* **Atributos específicos (ou grupo)**: para pesquisar atributos específicos, coloque um &#39;ou grupo&#39; antes de um especificador de tipo. Exemplo:
  * **n:a,b,c,d** : o nome é a ou b ou c ou d
* **Comportamento da pesquisa** :
  * Para filtrar usos específicos, adicione a **palavra-chave** específica à sua pesquisa, por exemplo: &quot; **imagens** ambiente”
  * Para adicionar várias solicitações, use uma vírgula &quot; **,** “, por exemplo: “cobalt **,** gold” (se uma vírgula for usada, a pesquisa mostrará apenas um recurso que corresponda às duas palavras-chave ao mesmo tempo)
  * Para pesquisar um nome exato, use um ponto de exclamação “!” no final, exemplo : **di!**  (retornará **dirt**, mas não **gotas**, esta palavra-chave desabilitará a correspondência difusa)
  * Para excluir um padrão de uma pesquisa, use um hífen &quot; **-** “, por exemplo: **u:image n:-normal** (retornará imagens que não contenham “normal”)
* **Funções correspondentes (sufixo de padrão) :**
  * **padrão** : correspondência aproximada (difusa)
  * **contém** : !
  * **regex** : #
  * **igual** : =
  * **começa com** : ^
  * **termina com** : &amp;
