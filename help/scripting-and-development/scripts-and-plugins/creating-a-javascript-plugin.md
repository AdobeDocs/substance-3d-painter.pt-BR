---
helpx_url: "https://helpx.adobe.com/br/substance-3d-painter/scripting-and-development/scripts-and-plugins/creating-a-javascript-plugin.html"
breadcrumb-title: ''
description: Saiba como criar plug-ins JavaScript para o Substance 3D Painter a fim de ampliar a funcionalidade e automatizar fluxos de trabalho personalizados.
helpx_creative_field: ""
helpx_description: Painter > Scripting and development > Scripts and plugins > Creating a Javascript plugin
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Criação de um plug-in Javascript
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '408'
ht-degree: 1%

---


# Criação de um plug-in Javascript

Este guia passo a passo descreve como criar um plug-in simples que permite exportar a máscara da camada atualmente selecionada em um projeto.

O objetivo do plug-in neste guia é exportar todos os canais do conjunto de texturas atual dentro de um projeto como texturas individuais.

## 1 - Navegar até a pasta de plug-ins

Para adicionar um novo plug-in Javascript, uma pasta deve ser criada na pasta de plug-ins do Substance 3D Painter.

Para acessar a pasta **plug-ins**, navegue até:

<table data-preserve-html="true" style="width: 100.0%;"> <colgroup> <col style="width: 15.0%;"/> <col style="width: 15.0%;"/> <col style="width: 70.0%;"/> </colgroup> <tbody> <tr> <th>Plataforma</th> <th>Versão</th> <th>Caminho</th> </tr> <tr> <td rowspan="2"><strong>Windows</strong></td> <td><strong>7.2</strong> ou mais recente</td> <td colspan="1">C:\Users\username\Documents\Adobe\Adobe Substance 3D Painter</td> </tr> <tr> <td colspan="1">Legado</td> <td colspan="1">C:\Users\username\Documents\Allegorithmic\Substance Painter</td> </tr> <tr> <td rowspan="2"><strong>Mac</strong></td> <td colspan="1"><strong>7.2</strong> ou mais recente</td> <td colspan="1">/Users/username/Documents/Adobe/Adobe Substance 3D Painter</td> </tr> <tr> <td colspan="1">Legado</td> <td colspan="1">/Users/username/Documents/Allegorithmic/Substance Painter</td> </tr> <tr> <td rowspan="2"><strong>Linux</strong></td> <td colspan="1"><strong>7.2</strong> ou mais recente</td> <td colspan="1">/home/username/Documents/Adobe/Adobe Substance 3D Painter</td> </tr> <tr> <td>Legado</td> <td colspan="1">/home/username/Documents/Allegorithmic/Substance Painter</td> </tr> </tbody> </table>

### 2 - Criar a pasta de plug-ins

O nome de um plug-in se baseia no nome da pasta pai.

Para este exemplo, basta criar uma nova pasta chamada **export-texturas** dentro da pasta de plug-ins.

### 3 - Criar os arquivos dos plug-ins

Abra a pasta recém-criada e crie dois arquivos de texto vazios (bloco de notas):

* **main.qml**
* **toolbar.qml**

A extensão de arquivo qml é uma extensão Javascript para scripts criados para a linguagem Qt QML. Ele permite executar código Javascript, mas também criar UIs personalizadas.

O arquivo **main.qml** é obrigatório. É o primeiro arquivo que será procurado pelo aplicativo para carregar o plug-in. Arquivos adicionais podem ser criados com qualquer nome, permitindo dividir um script em partes para facilitar o gerenciamento. Nesse caso, o **toolbar.qml** será usado para descrever a aparência de um botão que será adicionado na interface pelo plug-in.

### 4 - Conteúdo do script

Abra os arquivos de script em um editor de texto como o Notepad++ e cole os seguintes snippets de código. Dê uma olhada nos comentários do código para obter mais detalhes.

**toolbar.qml**

```
import QtQuick 2.7 

import AlgWidgets 2.0 

import AlgWidgets.Style 2.0 

 

AlgButton 

{ 

 tooltip: "" 

 iconName: "" 

 text: "Export Textures" 

}
```


**main.qml**

```
// Default includes, to acces Qt/QML 

// and Substance 3D Painter APIs 

import QtQuick 2.7 

import Painter 1.0 

 

// Root object for the plugin 

PainterPlugin 

{ 

 // Disable update and server settings 

 // since we don't need them 

 tickIntervalMS: -1 // Disabled Tick 

 jsonServerPort: -1 // Disabled JSON server 

 

 // Implement the OnCompleted function 

 // This event is used to build the UI 

 // once the plugin as been loaded by Substance 3D Painter 

 Component.onCompleted: 

 { 

  // Create a toolbar button 

  var InterfaceButton = alg.ui.addToolBarWidget("toolbar.qml"); 

 

  // Connect the function to the button 

  if( InterfaceButton ) 

  { 

   InterfaceButton.clicked.connect( exportTextures ); 

  } 

 } 

 

 // Custom function called by the Button, 

 // this is the core of the plugin 

 function exportTextures() 

 { 

  // Catch errors in the script during execution 

  try 

  { 

   // Verify if a project is open before  

   // trying to export something 

   if( !alg.project.isOpen() ) 

   { 

    return; 

   } 

 

   // Retrieve the currently selected Texture Set (and sub-stack if any) 

   var MaterialPath = alg.texturesets.getActiveTextureSet() 

   var UseMaterialLayering = MaterialPath.length > 1 

   var TextureSetName = MaterialPath[0] 

   var StackName = "" 

 

   if( UseMaterialLayering ) 

   { 

    StackName = MaterialPath[1] 

   } 

 

   // Retrieve the Texture Set information 

   var Documents = alg.mapexport.documentStructure() 

   var Resolution = alg.mapexport.textureSetResolution( TextureSetName ) 

   var Channels = null 

 

   for( var Index in Documents.materials ) 

   { 

    var Material = Documents.materials[Index] 

 

    if( TextureSetName == Material.name ) 

    { 

     for( var SubIndex in Material.stacks ) 

     { 

      if( StackName == Material.stacks[SubIndex].name ) 

      { 

       Channels = Material.stacks[SubIndex].channels 

       break 

      } 

     } 

    } 

   } 

 

   // Create the export settings 

   var Settings = { 

    "padding":"Infinite", 

    "dithering":"disbaled", // Hem, yes... 

    "resolution": Resolution, 

    "bitDepth": 16, 

    "keepAlpha": false 

   } 

 

   // Build the base of the export path 

   // Files will be located next to the project 

   var BasePath = alg.fileIO.urlToLocalFile( alg.project.url() ) 

   BasePath = BasePath.substring( 0, BasePath.lastIndexOf("/") ); 

 

   // Export the each channel 

   for( var Index in Channels ) 

   { 

    // Create the stack path, which defines the channel to export 

    var Path = Array.from( MaterialPath ) 

    Path.push( Channels[Index] ) 

 

    // Build the filename for the texture to export 

    var Filename = BasePath + "/" + TextureSetName 

 

    if( UseMaterialLayering ) 

    { 

     Filename += "_" + StackName 

    } 

 

    Filename += "_" + Channels[Index] + ".png" 

 

    // Perform the export 

    alg.mapexport.save( Path, Filename, Settings ) 

    alg.log.info( "Exported: " + Filename ) 

   } 

  } 

  catch( error ) 

  { 

   // Print errors in the log window 

   alg.log.exception( error ) 

  } 

 } 

} 
```


Depois de concluído, salve e feche o arquivo.

### 5 - Carregar e ativar o plug-in

Inicie o Substance 3D Painter. Por padrão, os novos plug-ins são carregados e ativados automaticamente.

Abra um projeto e clique no botão da interface do usuário criado pelo plug-in para exportar os canais do conjunto de texturas selecionado atualmente:

![](../../assets/button-plugin.png)

Para ativar ou desativar um plug-in, use o menu JavaScript na parte superior da interface:

![](../../assets/disable-plugin.png)
