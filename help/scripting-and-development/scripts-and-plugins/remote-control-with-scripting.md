---
helpx_url: "https://helpx.adobe.com/br/substance-3d-painter/scripting-and-development/scripts-and-plugins/remote-control-with-scripting.html"
breadcrumb-title: ''
description: Saiba como usar scripts de controle remoto no Substance 3D Painter para automatizar fluxos de trabalho e controlar o aplicativo programaticamente.
helpx_creative_field: ""
helpx_description: Painter > Scripting and development > Scripts and plugins > Remote control with scripting
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Controle remoto com script
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '346'
ht-degree: 0%

---


# Controle remoto com script

Esta página descreve como controlar remotamente o aplicativo para executar comandos Javascript ou Python.\
Isso requer um argumento de linha de comando específico, então um script Python simples pode executar qualquer comando disponível a partir das APIs Javascript e Python existentes.

## Iniciando o aplicativo

Para controlar remotamente o aplicativo, o Substance 3D Painter precisa ser iniciado com a seguinte linha de comando:

```
"Adobe Substance 3D painter.exe" --enable-remote-scripting
```


>[!NOTE]
>
> Certifique-se de que o aplicativo esteja ativo e em execução com este comando antes de executar qualquer script. Os scripts podem falhar se o aplicativo ainda estiver sendo inicializado ou não estiver pronto ainda.

## Script de controle remoto

O seguinte script Python pode servir como uma biblioteca para se comunicar com o aplicativo.

Salve o script a seguir em um arquivo chamado **lib\_remote.py** para que os exemplos abaixo funcionem corretamente.

```
import sys 

import json 

import base64 

import subprocess 

 

if sys.version_info >= (3, 0): 

 import http.client as http 

else: 

 import httplib as http 

 

class RemotePainter() : 

 def __init__(self, port=60041, host='localhost'): 

  self._host = host 

  self._port = port 

 

## Json server connection

  self._PAINTER_ROUTE = '/run.json' 

  self._HEADERS = {'Content-type': 'application/json', 'Accept': 'application/json'} 

 

## Execute a HTTP POST request to the Substance Painter server and send/receive JSON data

 def _jsonPostRequest( self, route, body, type ) : 

  connection = http.HTTPConnection(self._host, self._port, timeout=3600) 

  connection.request('POST', route, body, self._HEADERS) 

  response = connection.getresponse() 

 

  data = response.read() 

  connection.close() 

 

  if type == "js" : 

   data = json.loads( data.decode('utf-8') ) 

 

   if 'error' in data: 

    OutJson = json.loads( body.decode() ) 

    print( base64.b64decode( OutJson["js"] ) ) 

    raise ExecuteScriptError(data['error']) 

  else : 

## Python can return nothing, so decoding can fail

   try: 

    data = data.decode('utf-8').rstrip() 

   except: 

    pass 

 

  return data 

 

 def checkConnection(self): 

  connection = http.HTTPConnection(self._host, self._port) 

  connection.connect() 

 

## Execute a command

 def execScript( self, script, type ) : 

  Command = base64.b64encode( script.encode('utf-8') ) 

 

  if type == "js" : 

   Command = '{{"js":"{0}"}}'.format( Command.decode('utf-8') ) 

  else : 

   Command = '{{"python":"{0}"}}'.format( Command.decode('utf-8') ) 

 

  Command = Command.encode( "utf-8" ) 

 

  return self._jsonPostRequest( self._PAINTER_ROUTE, Command, type ) 

 

class PainterError(Exception): 

 def __init__(self, message): 

  super(PainterError, self).__init__(message) 

 

class ExecuteScriptError(PainterError): 

 def __init__(self, data): 

  super(PainterError, self).__init__('An error occured when executing script: {0}'.format(data)) 

 
```


## Exemplos

Veja a seguir dois exemplos simples que mostram como executar comandos em ambas as APIs compatíveis com o aplicativo:

### Execução de comandos Javascript

A maioria das funções Javascript na API retorna dados String ou Json que facilitam sua manipulação no script Python. Não deve haver nenhum problema grave ao enviar e receber dados.

Crie um arquivo de script Python chamado **example\_js.py** e adicione o seguinte código:

```
import lib_remote 

 

Remote = lib_remote.RemotePainter() 

Remote.checkConnection() 

 

## Print the API version

Version = Remote.execScript( "alg.version.painter", "js" ) 

print( Version ) 

 

## Get a list of all the files in the default shelf/library:

Files = Remote.execScript( 'alg.resources.findResources("starter_assets", "*")', "js" ) 

 

for File in Files : 

 print( File )
```


Se o aplicativo estiver em execução com a linha de comando, a execução desse script fará com que ele execute comandos e recupere seus resultados.

### Execução de comandos do Python

A maioria das funções Python podem retornar objetos que não podem ser passados para o script remoto, isso significa que, para receber dados, eles precisam ser explicitamente convertidos para strings ou dicionários Json.

Para facilitar as coisas, é possível criar um script Python personalizado que é carregado durante a inicialização do aplicativo e funções de chamada que manipulam esse tipo de conversão sem ter que depender de conversões embutidas.

Crie um arquivo de script Python chamado **example\_py.py** e adicione o seguinte código:

```
import lib_remote 

 

Remote = lib_remote.RemotePainter() 

Remote.checkConnection() 

 

## import the substance_painter module to make

## its API available to us

Remote.execScript( "import substance_painter", "python" ) 

 

## Print the API version

Version = Remote.execScript( "substance_painter.__version__", "python" ) 

print( Version ) 

 

## Get a list of all the files in the default shelf/library

## Because the search function return objects, we have to convert

## the information into a string within the same command (inline)

Command = 'substance_painter.resource.search( "p:starter_assets/" )' 

Command = '"|||".join( [ x.identifier().url() for x in {0}] )'.format( Command ) 

 

Files = Remote.execScript( Command, "python" ) 

Files = Files.split( "|||" ) 

 

for File in Files : 

 print( File )
```


Se o aplicativo estiver em execução com a linha de comando, a execução desse script fará com que ele execute comandos e recupere seus resultados.
