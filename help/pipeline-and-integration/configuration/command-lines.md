---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/pipeline-and-integration/configuration/command-lines.html"
breadcrumb-title: ''
description: Saiba como usar argumentos de linha de comando com o Substance 3D Painter para automação, script e integração de pipeline.
helpx_creative_field: ""
helpx_description: Painter > Pipeline and integration > Configuration > Command lines
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Linhas de comando
user-guide-description: ''
user-guide-title: ''
source-git-commit: 22871eab2f25d09bd82f1292d8b3e5f8c4f1c2cf
workflow-type: tm+mt
source-wordcount: '204'
ht-degree: 0%

---


# Linhas de comando

Essa página lista várias linhas de comando que podem ser usadas ao iniciar o aplicativo para criar ou abrir projetos, por exemplo.\
Estas linhas de comando podem ser usadas da seguinte maneira:

```
"Adobe Substance 3D Painter.exe" --command [option] 
```


## Lista de comandos

| Comando | Descrição |
| --- | --- |
| **—ajuda** **-?** **-h** | Exibe informações sobre quais linhas de comando estão disponíveis e como usá-las. |
| **—versão** **-v** | Exibir a versão atual do Substance 3D Painter. |
| **—mesh** | Malha para carregar em um projeto.Exemplo: `// Create a new project with a specific mesh   "Adobe Substance 3D Painter.exe" --mesh "E:/MymeshFolder/MyMesh.obj"       // Update a mesh inside an existing project   "Adobe Substance 3D Painter.exe" --mesh "E:/MymeshFolder/MyMesh.obj" "E:/MyMeshFolder/Project.spp"` |
| **—mesh-map** | Mapas baked associados à malha (AO, Normal, Curvatura). Pode ser especificado várias vezes. Nomenclatura : TextureSetName\_AdditionalMapSlot<ul data-preserve-html="true"> <li data-preserve-html="true">Oclusão de ambiente = <strong> <em> oclusão_ambiente </em> </strong></li> <li data-preserve-html="true">Curvatura = <strong> <em> curvatura </em> </strong></li> <li data-preserve-html="true">Normal = <strong> <em> base_normal </em> </strong></li> <li data-preserve-html="true">Espaço Mundial Normal = <strong> <em> world_space_normals </em> </strong></li> <li data-preserve-html="true">Posição = <strong> <em> posição </em> </strong></li> <li data-preserve-html="true">Thickness = <strong> <em> thickness </em> </strong></li> <li data-preserve-html="true">ID = <em> <strong> id </strong> </em></li> </ul>Exemplo: `"Adobe Substance 3D Painter.exe" --mesh "E:/MyMeshFolder/MyMesh.obj" --mesh-map " E:/MyMeshFolder/DefaultMaterial_ambient_occlusion.png"` |
| **—split-by-udim** | Crie um conjunto de texturas por bloco UDIM. |
| **—export-path** | Caminho de exportação padrão em que as saídas do projeto serão exportadas. |
| **—vram-budget** | Substituir o orçamento de memória de vídeo (VRAM) definido pelo mecanismo do Substance 3D Painter. “Quantidade” é em megabytes.    Exemplo: `// Set the VRam budget to 2GB   "Adobe Substance 3D Painter.exe" --vram-budget 2048` |
| **—disable-version-checking** | Não verificar se uma nova versão do aplicativo está disponível ao iniciar |
| **—enable-remote-scripting** | Permite executar comandos de script de fora do aplicativo. Consulte [Controle remoto com scripts](../../scripting-and-development/scripts-and-plugins/remote-control-with-scripting.md) para obter mais informações. |
