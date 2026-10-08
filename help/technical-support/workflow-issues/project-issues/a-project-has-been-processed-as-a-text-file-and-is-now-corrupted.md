---
breadcrumb-title: ""
description: Saiba como recuperar arquivos de projeto corrompidos do Substance 3D Painter que foram processados como arquivos de texto.
title: Arquivo de projeto corrompido
user-guide-description: ""
user-guide-title: ""
source-git-commit: 6b6d52207ca1d043aaa1b2b14145b6b49d4c1942
workflow-type: tm+mt
source-wordcount: '119'
ht-degree: 0%
---

# Um projeto foi processado como um arquivo de texto e agora está corrompido

Às vezes, o seguinte erro pode aparecer ao carregar um projeto:

```
[Hdf5Archive] Archive 'project.spp' appears to have been processed as a text file and is irremediably corrupted. 

[Project management] The selected project 'project.spp' isn't valid!
```


Este erro significa que o projeto foi modificado fora do Substance 3D Painter e **não pode ser lido corretamente**.\
Isso geralmente acontece quando um software de controle de versão (como **Perforce** ) processou o projeto do Substance 3D Painter **como um arquivo de texto em vez de um arquivo binário**. A única solução é adicionar uma nova regra/exceção ao software de controle de versão para forçar o processamento de arquivos **spp como binários**. Para obter mais informações com **Perforce**, consulte a documentação dedicada: <https://www.perforce.com/perforce/r16.1/manuals/cmdref/p4_typemap.html>
