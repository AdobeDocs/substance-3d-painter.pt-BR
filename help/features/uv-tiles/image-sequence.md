---
breadcrumb-title: ""
description: Saiba como usar sequências de imagem com blocos UV no Substance 3D Painter para fluxos de trabalho de textura animados.
title: Sequência de imagens
user-guide-description: ""
user-guide-title: ""
source-git-commit: 6b6d52207ca1d043aaa1b2b14145b6b49d4c1942
workflow-type: tm+mt
source-wordcount: '279'
ht-degree: 0%
---

# Sequência de imagens

As sequências de imagem são uma coleção de imagens agrupadas como um único recurso na Prateleira. As imagens são agrupadas com base em um padrão específico nos nomes de arquivo.

## Como importar imagens como uma sequência

Ao importar um arquivo de imagem, se o nome do arquivo corresponder a um padrão específico, ele será importado automaticamente como uma sequência. Se houver imagens adicionais ao lado do arquivo importado, elas também serão levadas em consideração. Portanto, não é necessário importar todos os arquivos de uma sequência manualmente. Escolher o primeiro arquivo é suficiente.

Exemplos de correspondência de nome de arquivo:

Os nomes de arquivo a seguir importarão com êxito uma sequência de imagens porque podem reconhecer que a última parte do nome de arquivo se refere a um número UDIM 1032:

* arquivo\_22.1032.jpg
* arquivo\_22-223.1032.jpg
* file\_22-223-1032.jpg
* file\_22-223\_1032.jpg

Os seguintes nomes de arquivo não serão importados como uma sequência de imagens porque não estão estruturados corretamente:

* arquivo\_22-2232032.jpg
* arquivo\_22-223PM2032.jpg
* file\_22-223-0032.jpg
* arquivo\_22-223\_Rec2020.jpg

A correspondência do nome de arquivo é baseada na seguinte expressão regular:

```
 ^(.+?)[\.\-\_](?
```


## Como usar sequências de imagem

As sequências de imagem podem ser carregadas em qualquer slot de recurso na interface como qualquer outro recurso. No entanto, em alguns casos, pode ser necessário que configurações adicionais sejam usadas adequadamente.

Em [Camadas de preenchimento](../../painting/fill-projections/fill-projections.md) (e efeitos de preenchimento), verifique se o modo de projeção está definido como **Preenchimento (Correspondência por Bloco UV)** para garantir que cada imagem da sequência seja atribuída ao [Bloco UV](uv-tiles.md) correto no Conjunto de Textura.
