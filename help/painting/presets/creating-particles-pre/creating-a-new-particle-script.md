---
helpx_url: "https://helpx.adobe.com/br/substance-3d-painter/painting/presets/creating-particles-presets/creating-a-new-particle-script.html"
breadcrumb-title: ''
description: Saiba como criar um novo script de partícula no Substance 3D Painter para definir o comportamento e os efeitos do pincel de partícula personalizado.
helpx_creative_field: ""
helpx_description: Painter > Painting > Presets > Creating particles presets > Creating A New Particle Script
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Criando Um Novo Script De Partículas
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '728'
ht-degree: 0%

---


# Criando Um Novo Script De Partículas

Baixe o Pacote PopcornFX pré-configurado: [Templates\_EmitterReceiver.pkkg](https://helpx.adobe.com/content/dam/help/en/substance-3d/documentation/spdoc/files/67403778/68419585/1/1411557944000/templates-emitterreceiver.pkkg)

Este pacote é um “kit de inicialização” que contém um emissor e um receptor que editaremos e importaremos no Substance 3D Painter.

## Configuração do Popcorn fx

Inicie o Editor PopcornFX, crie um novo projeto e, em seguida, abra-o.

Em seu projeto, clique com o botão direito do mouse em uma área vazia e selecione “Importar pacote de pipocas”. Em seguida, escolha “Templates\_EmitterReceiver.pkkg”.

Agora, você deve ter:

* Um sistema de partículas “\_Emitter” que é um modelo de base de um Emissor.
* Um sistema de partícula “\_Receiver” que é um modelo base de um Receiver.
* Uma malha de esfera usada como plano de fundo padrão da cena

“\_Emitter” e “\_Receiver” já estão “prontos para Painter”. Eles já foram configurados com os necessários evolvers, campos, cenários etc...

## Importar sua malha

O PopcornFX só oferece suporte a **FBX**. Exporte a malha neste formato. Durante a etapa de exportação, verifique o tamanho da malha para tentar ajustar as unidades corretas no “mundo real”.

Copie e cole na pasta “malhas” do seu projeto (no PopcornFX, você pode clicar com o botão direito do mouse na pasta “malhas” e selecionar “Abrir local do arquivo”).

Volte para o editor, abra sua malha (clique duas vezes nela) e clique em &quot; **Compilação** “. Feche a janela e salve a alteração.

## Edição de emissor/receptor

Vamos duplicar os sistemas de partículas existentes e adaptá-los para levar a nova malha em consideração corretamente.

Clique com o botão direito no sistema de partículas “\_Emitter” (na pasta “Partículas”) e selecione “Clone” (ou “Duplicate”) para criar seu próprio Emissor.

Abra-o e, na janela “Particle Treeview” (parte inferior esquerda), selecione &quot; **Camada\_Modelo** “, que deve estar localizado em : “Propriedades do editor => Tela de fundo => Camadas 3D”.

Depois, na janela “Propriedades do nó”, substitua “dummymesh.fbx” pelo seu modelo. Salve a modificação (Arquivo => Salvar) e feche a janela do emissor.

Agora, **clone “\_Receiver** **”** (na pasta “Partículas”) para criar seu próprio Receiver a partir deste.

Abra-a e, como no emissor, substitua a malha fictícia pelo seu modelo em “Layer\_Model”. Nós **modificamos a malha** **exibida na tela** , mas também precisamos modificar a **malha** **usada pelas partículas** .

Para fazer isso, na janela “Particle Treeview”, clique em &quot; **Shape** “, que deve estar localizado em : “Particle Effect => Spawner => Layer\_1 => Samplers => Mesh”.

Em seguida, substitua “MeshResource” pelo seu modelo.

Depois de feito, há uma última coisa a fazer: precisamos “vincular” o emissor e o receptor ao que acabamos de criar.

Na visualização em árvore do seu receptor, selecione “Propriedades do editor” e, em seguida, selecione seu emissor em “OverSpawnEffect”. Salve o receptor.

Abra seu emissor (aquele que duplicamos anteriormente) e, na janela “Particle Treeview”, clique em “Events”, que deve estar localizado em : “Particle Effect => Spawner”. Em seguida, substitua o receptor pelo seu receptor clicando em “Extern”.\
Está feito! Agora, se você selecionar a visualização 3D (do seu emissor ou receptor), poderá criar partículas pressionando o botão “espaço”.

## Opcional: modifique o comportamento do receptor

Abra seu receptor e, na janela “Particles Treeview”, selecione &quot; CParticleEvolver\_Script &quot; (o mais alto que é dedicado a você :)), que deve estar localizado em : “Particle Effect => Layer\_1 => State\_0”.

Na janela “Specialized Node Editor”, na função, adicione “Life = 0.5;” para alterar o tempo de vida das partículas. Depois, use o atalho “Ctrl+s” para salvar o script. Observe a diferença na visualização 3D.

Para obter mais informações sobre como ele funciona, acesse o link abaixo:

<http://wiki.popcornfx.com/index.php/Main_Page>

## Importar emissor/receptor no Substance 3D Painter

No Substance 3D Painter, escolha “Arquivo” > “Importar partículas” ou Ctrl-Alt-R e, em seguida, selecione o Emissor e o Receptor (ambos no formato .pkfx) no Pacote.

O Substance 3D Painter detectará automaticamente os requisitos (campos de partícula, eventos OnCollide) para decidir se o seu pkfx é um Emissor, Receptor ou nada compatível.

Agora, você deve ver seu Emissor / Receptores na prateleira (nas guias “Emissores” e “Receptores”).

Para usá-los, você primeiro precisa clicar no botão “Alternar partículas”.

Depois, na janela “Ferramenta”, em “Física”, você terá a possibilidade de selecionar seu emissor (para substituir “padrão\_emitter”) e seu receptor (para substituir o padrão\_receptor).

Agora você pode clicar com o botão direito na janela “Ferramenta” e salvar a ferramenta.
