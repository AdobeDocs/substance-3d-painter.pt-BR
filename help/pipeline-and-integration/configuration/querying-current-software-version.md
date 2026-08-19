---
helpx_url: "https://helpx.adobe.com/br/substance-3d-painter/pipeline-and-integration/configuration/querying-current-software-version.html"
breadcrumb-title: ''
description: Saiba como consultar a versão atual do software Substance 3D Painter de forma programática para integração e automação de pipeline.
helpx_creative_field: ""
helpx_description: Painter > Pipeline and integration > Configuration > Querying Current Software Version
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Consultando a Versão Atual do Software
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '160'
ht-degree: 0%

---


# Consultando a Versão Atual do Software

A verificação da versão atual do aplicativo pode ser feita de várias maneiras, dependendo das necessidades (sem ou sem a inicialização do software, por exemplo).

## Verificando a versão por meio do executável

O executável Substance Painter no Windows contém poucas informações que podem ser consultadas por ferramentas externas (como Python).

Exemplo em **Python 3** ([tirado daqui](https://stackoverflow.com/questions/580924/python-windows-file-version-attribute)) :

```
import os 

import imp 

import pip 

import win32api #pypiwin32 

 

 


## Reader


def getFileProperties(fname): 

 """ 

 Read all properties of the given file return them as a dictionary. 

 """ 

 propNames = ('Comments', 'InternalName', 'ProductName', 

  'CompanyName', 'LegalCopyright', 'ProductVersion', 

  'FileDescription', 'LegalTrademarks', 'PrivateBuild', 

  'FileVersion', 'OriginalFilename', 'SpecialBuild') 

 

 props = {'FixedFileInfo': None, 'StringFileInfo': None, 'FileVersion': None} 

 

 try: 

## backslash as parm returns dictionary of numeric info corresponding to VS_FIXEDFILEINFO struc

  fixedInfo = win32api.GetFileVersionInfo(fname, '\') 

  props['FixedFileInfo'] = fixedInfo 

  props['FileVersion'] = "%d.%d.%d.%d" % (fixedInfo['FileVersionMS'] / 65536, 

   fixedInfo['FileVersionMS'] % 65536, fixedInfo['FileVersionLS'] / 65536, 

   fixedInfo['FileVersionLS'] % 65536) 

 

## VarFileInfoTranslation returns list of available (language, codepage)

## pairs that can be used to retreive string info. We are using only the first pair.

  lang, codepage = win32api.GetFileVersionInfo(fname, '\VarFileInfo\Translation')[0] 

 

## any other must be of the form StringfileInfo%04X%04Xparm_name, middle

## two are language/codepage pair returned from above

 

  strInfo = {} 

  for propName in propNames: 

   strInfoPath = u'\StringFileInfo\%04X%04X\%s' % (lang, codepage, propName) 

   ## print str_info 

   strInfo[propName] = win32api.GetFileVersionInfo(fname, strInfoPath) 

    

  props['StringFileInfo'] = strInfo 

 except: 

  pass 

 

 return props 

 

 


## Check exe


Path = "E:/Software/Painter/Substance Painter.exe" 

 

FileInfo = getFileProperties(Path) 

 

print( FileInfo )
```


A saída será:

```
E:SoftwarePainter>query.py 

{'FixedFileInfo': {'Signature': -17890115, 'StrucVersion': 65536, 'FileVersionMS': 132251649, 'FileVersionLS': 65536, 'ProductVersionMS': 132251649, 'ProductVersionLS': 65536, 'FileFlagsMask': 0, 'FileFlags': 0, 'FileOS': 0, 'FileType': 1, 'FileSubtype': 0, 'FileDate': None}, 'StringFileInfo': {'Comments': None, 'InternalName': 'Substance Painter', 'ProductName': 'Substance Painter', 'CompanyName': 'Allegorithmic', 'LegalCopyright': 'Copyright (C) 2017 Allegorithmic', 'ProductVersion': '2018.1.1', 'FileDescription': 'Substance Painter 2018.1.1', 'LegalTrademarks': None, 'PrivateBuild': None, 'FileVersion': '2018.1.1', 'OriginalFilename': 'Substance Painter.exe', 'SpecialBuild': None}, 'FileVersion': '2018.1.1.0'}
```


Verificando a versão por meio da linha de comando

Você pode usar a linha de comando da seguinte maneira: **substance painter.exe** command\_name *[option]*

Para perguntar a versão, use **—versão**, **-v**.

>[!NOTE]
>
> Observe que as ações de linha de comando do Substance Painter gerarão uma janela.

## Verificando a versão por script

A API de script (disponível por meio do menu ajuda) permite consultar a versão atual do aplicativo.

Dê uma olhada no namespace “**alg**” para obter mais detalhes.

Exemplo:

```
//Print current version in the log window (string) 

alg.log.info( alg.version.painter );
```
