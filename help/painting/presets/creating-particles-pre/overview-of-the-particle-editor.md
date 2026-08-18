---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/painting/presets/creating-particles-presets/overview-of-the-particle-editor.html"
breadcrumb-title: ''
description: Saiba mais sobre o editor de partículas no Substance 3D Painter para criar predefinições de pincel de partícula personalizadas para pintura de textura.
helpx_creative_field: ""
helpx_description: Painter > Painting > Presets > Creating particles presets > Overview of the particle editor
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Visão geral do editor de partículas
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '1677'
ht-degree: 0%

---


# Visão geral do editor de partículas

Esta página aborda vários aspectos do editor de partículas PopcornFX. Alguns títulos e parâmetros de janelas podem estar sujeitos a alterações, dependendo da versão do editor usada.

## Configuração do visor

### Como importar sua própria malha

Copie e cole sua malha na pasta “Malhas” de seu pacote. Depois, no Editor, abra sua malha e clique em “Construir”.

Agora, em seu sistema de partícula, vá para “Backdrop” na visualização de árvore, clique com o botão direito do mouse em “Camadas 3D”, “Novo Backdrop”, “CNEdEditorBackdrop\_Model3D”, e selecione sua malha em “modelo de recurso”.

No Substance 3D Painter, a Malha é dimensionada para ficar dentro de uma caixa de tamanho [-1;1] em cada Eixo. Para obter a escala correta com o Substance 3D Painter no Editor, você deve importar uma malha que já esteja dimensionada para ajustar-se a essa caixa (de maneira fácil) ou brincar com as escalas no Editor.

Observação: somente o formato de malha FBX é suportado.

#### Como exibir a grade

Ctrl-G. Você pode personalizar a cor da grade em “Propriedades do editor” “GridColor”.

## Emissor

### Como criar eventos “OnCollide”

O Physics Evolver lida com a colisão com malhas de fundo na cena. No Substance 3D Painter a cena será sua malha.

Primeiro no Physics Evolver, defina “WorldInteractionMode” como “OneWay” para permitir a colisão de partículas. Em seguida, crie um evento chamado “OnCollide”, o Physics Evolver o acionará na colisão com a cena.

No Substance 3D Painter, a cena é o modelo em que você está trabalhando e todos os eventos chamados “OnCollide” serão substituídos pelo sistema de partículas Emissor do pincel atual.

#### Como disparar partículas da câmera

Na parte superior da viewport, ative o quarto botão “Restringir spawns no plano da câmera”.

O Substance 3D Painter acionará por padrão os emissores da câmera.

#### Como emitir partículas no topo como a chuva

Desative a opção “Restringir spawns no plano da câmera” se estiver ativada.

Crie um atributo de partícula chamado “Global”, agora o Substance 3D Painter gerará suas partículas na origem.

Para criar na parte superior da malha, adicione uma caixa de Sampler de forma ou CILINDRO, coloque-a na parte superior e obtenha uma amostra dela no Spawner Script.

Por exemplo, com uma Shape Sampler BOX chamada “Spawn”, adicione-a ao seu Spawner Script:

*Posição = Spawn.samplePosition();*

## Receptor

### Como gerar o emissor ao criar/editar um receptor

Para ficar ainda mais perto do fluxo de trabalho do Substance 3D Painter ao editar seu Receptor, você pode configurar o Editor para substituir o sistema de partícula gerado.

Na visualização em árvore do seu receptor, selecione “Propriedades do editor”, em seguida, ative “UserOverSpawn” e selecione seu emissor em “OverSpawnEffect”.

Você ainda deve abrir o emissor para definir os eventos “OnCollide” para gerar o receptor que você está editando atualmente.

#### Como configurar campos de partícula

Aqui está a descrição do campo de partículas que você deve ter em seu Receptor:

*”Tamanho” flutuante*

O multiplicador do tamanho do pincel no Substance 3D Painter.

*”Opacidade” flutuante*

O multiplicador da opacidade do pincel no Substance 3D Painter.

*”UV” flutuante3*

A coordenada de textura na malha de partículas.

Em um Script Evolver, obtenha uma amostra da Forma Sampler “Mesh” com a coordenada paramétrica fornecida pelo Evoluidor da Projeção:

UV = Mesh.sampleTexcoord(pCoords);

*”Normal” flutuante3*

O normal da superfície da malha abaixo das partículas.

Em um script Evolver, obtenha uma amostra da Forma Sampler “Mesh” com a coordenada paramétrica fornecida pelo Evoluidor da Projeção:

Normal = normalize(Mesh.sampleNormal(Coords));

*”Semente” int*

Apenas um valor gerado aleatoriamente para o Substance 3D Painter:

Em um Script Evolver, adicione:

Sementes = int(rand(0,20000000));

*”pCoords” int3*

Não usado pelo Substance 3D Painter, mas indispensável para fazer a projeção de partículas na malha e amostrar outros campos.

#### Como projetar a partícula na malha

Adicione um Evoluidor de projeção no “Estado\_0” do seu Receptor.

Cada quadro, o Evolutor de projeção projetará partículas na superfície mais próxima de um Sampler de forma.

O Evoluidor de Projeção pode preencher a coordenada paramétrica da projeção no campo de partículas especificado por “OutputParametricCoordsField” (consulte campo de partículas “Coords”).

E pode reprojetar um vetor na superfície da malha com “ReprojectedField”.

Aqui, queremos projetar partículas na forma de Sampler “Mesh”, preencher coordenadas paramétricas no campo de partículas int3 “Coords” e projetar a “Velocidade” na superfície também:

#### Como obter amostras da malha

No Substance 3D Painter, todos os Shape Samplers chamados “Mesh” e de “ShapeType” “MESH” serão substituídos pela malha usada no Substance 3D Painter.<b>\
</b>

No Editor, defina-o com a mesma malha do plano de fundo.

Para obter amostras de itens em um Script, basta escrever “Mesh.sample~Something~(Coords)” em um Script. Esta é a documentação:

<https://wiki.popcornfx.com/index.php/CParticleSamplerShape#Script_bindings>

Alguns snippets de código úteis que você precisará:

```
// UV is the texture coordinate of the particle on the mesh

// Must be after CParticleEvolver_Projection

UV = Mesh.sampleTexcoord(pCoords);

// Normal is the Normal of the surface on the mesh just below the particle

// Must be after CParticleEvolver_Projection

Normal = normalize(Mesh.sampleNormal(pCoords));
```


## Dicas gerais

### Como importar emissor/receptor no Substance 3D Painter

No Substance 3D Painter, escolha “Arquivo” > “Importar partículas” ou Ctrl-Alt-R e depois escolha o seu Emitter.pkfx ou Receiver.pkfx no seu pacote.

O Substance 3D Painter detectará automaticamente os requisitos (campos de partícula, eventos OnCollide) para decidir se o seu pkfx é um Emissor, Receptor ou nada compatível.

Agora, você deve ver seu Emissor / Receptores na prateleira.

#### Como depurar a partícula com um tamanho de partícula viável

Como o campo de partícula “Tamanho” deve estar entre 0 e 1 para ser um multiplicador do tamanho do pincel no Substance 3D Painter, as partículas serão muito grandes no Editor. Portanto, adicione um float de campo personalizado “BBSize” definido como 0.01 no script Spawner, para ser usado no renderizador de partículas Billboard como o “SizeField” para ver melhor a partícula.

#### Como não bagunçar com a ordem do evolucionador

A ordem do evolver pode ser muito importante.

Por exemplo, você pode querer sempre que seus 2 últimos evolvers sejam o Evoluidor de projeção e, em seguida, o Evoluidor de script que faz a amostragem do UV e do normal com os pCoords gerados pelo Evoluidor de projeção.

Lembre-se de que a ordem dos evolucionadores é literalmente a ordem de execução dentro de um quadro, e que o Substance 3D Painter reunirá os valores do campo de partículas e o final de cada quadro.

#### Como obter uma amostra do mapa normal da malha

O Substance 3D Painter substituirá todos os classificadores de textura chamados “NormalMap” pelo mapa normal da malha (se importado).

Essa é a única textura que você pode ter por enquanto, todas as outras texturas não serão acessíveis pelo Substance 3D Painter.

Depois de adicionar o Texture Sampler chamado “NormalMap”, você pode obter uma amostra em um script:

<http://www.popcornfx.com/wiki/index.php/CParticleSamplerTexture>

Alguns snippets de código úteis:

```
// In Evolver Script convert the NormalMap texture in tangent space to world space normal

// /!\ the "Normal" particle field must always be the normal of the mesh not influenced by the normal map

// /!\ dont forget to initialize your particle fields in your Spawn Script

// otherwise pCoords and Normal will be invalid at the first update

float normalFactor = 1.0; // change the intensity of the normal map

float3 meshnormal = Normal;

float4 rawtangent = Mesh.sampleTangent(pCoords);

float3 binormal = normalize(cross(meshnormal, rawtangent.xyz) * rawtangent.w);

float3 tangent = normalize(cross(meshnormal, binormal));

float3 tsNormal = normalize(((NormalMap.sample(UV).xyz * 2.0 - 1.0).xyz) * float3(-normalFactor, normalFactor, 1));

float3 normal = normalize(tsNormal.x * tangent + tsNormal.y * binormal + tsNormal.z * meshnormal);
```


#### Como criar turbulência

No Editor, crie um Sampler Turbulence.

<http://www.popcornfx.com/wiki/index.php/CParticleSamplerProceduralTurbulence>

Em seguida, você tem 2 maneira de amostrar a turbulência e afetar as partículas:

##### A maneira fácil

No painel Evolução física da camada, defina “VelocityFieldSampler” como o nome do Sampler Turbulence e defina “Arrastar” como um valor > 0.

##### A maneira parametrizada

Você ajusta a turbulência com atributos, obtendo amostras do campo de velocidade gerado pelo Sampler de turbulência em um Script Evolver:

Crie 2 atributos de partícula:

* flutuação “TurbulencePower” minmax: [0;5]
* float “TurbulenceScale” minmax: [0. 001; 5] (precisa ser > 0)

Depois, crie 3 campos de partículas:

float “TurbPower” e float “TurbScale”

Para armazenar atributos neles no Script Spawner:

* TurbScale = 1.0 / TurbulenceScale;
* TurbPower = TurbulencePower;

float3 “VelocityField” no modo de rotação.

Ele será usado como o “VelocityField” no Physics Evolver (já definido por padrão para o campo “VelocityField”).

Então, antes de seu Physics Evolver, em um Script Evolver, dê uma amostra do seu Sampler Turbulence chamado “Turb”:

VelocityField = Turb.sample(Position \* TurbScale) \* TurbPower;

#### Como usar corretamente dt, o tempo delta

O tempo delta é o tempo de simulação em segundos entre cada atualização de quadro. No Editor, o tempo delta é atualizado com o tempo real decorrido. No Substance 3D Painter, o tempo delta é corrigido e cada atualização é iniciada assim que a última é concluída.

Um jogo rodando a 60 FPS terá um tempo delta de 1/60= 0,016 segundos, então tente fazer seus pincéis rodarem em torno de 0,016s do tempo delta.

* Tempo de deltas grandes > 0,016 s
* Atualização rápida PRO

Como o tempo entre as atualizações é grande, o movimento das partículas será maior, portanto, o Pincel será executado mais rapidamente no Substance 3D Painter.

* aproximação CON

PopcornFX é um tipo de grande sistema de discretização, então maior é o dt, maior serão as imprecisões. Ver grande implicação do tempo delta em turbulências: <http://www.popcornfx.com/wiki/index.php/CParticleEvolver_Physics#Dealing_with_turbulences_at_low_framerates>

* Divisões CON

Se o tempo delta for grande, o movimento de partículas entre quadros também será grande. No Substance 3D Painter, pequenas manchas podem aparecer em vez de linhas retas.

Isso acontece porque o Substance 3D Painter desenhará um ponto de traçado para cada partícula no final de cada quadro e não desenhará linhas para cada partícula entre o último quadro e o quadro atual.

* Tempo delta pequeno &lt; 0,016 s
* PRO precision

Quanto menor o tempo delta, menor a distância entre os traçados do pincel, mais nítido será o desenho. E a discretização da simulação também será melhor.

* CON lento

Quanto menor o tempo delta, maior o número de atualizações necessárias para desenhar a mesma distância.

Dicas finais sobre tempos delta : uma boa maneira de obter o dt à direita pode ser começar com um grande (0.1s) e depois diminuir passo a passo para obter o resultado desejado.

#### Como expor parâmetros do seu sistema de partículas

O Substance 3D Painter reunirá os atributos de partículas dos sistemas de partículas e os exibirá nos parâmetros do Pincel físico:

<http://www.popcornfx.com/wiki/index.php/Particle_effect_attributes>

No PopcornFX você tem o recurso chamado “Atributos em Evolução”, que permite que você acesse Atributo em scripts de Evolução: não faça isso . Em vez disso, crie um campo de partícula e armazene o atributo neles no Script Spawner e, em seguida, use esses campos de partícula em Scripts de Revelação. (isso pode ser corrigido no futuro)

#### Como detectar partículas problemáticas

Você nunca deve ter partículas com valores de campo de partícula estranhos, então certifique-se de quebrar em problemático de vez em quando:

<http://www.popcornfx.com/wiki/index.php/Particle_tips_BreakOnProblematicParticle>

#### Como resolver problemas de sistemas de partículas no Substance 3D Painter

No diretório de instalação do Substance 3D Painter, você deve encontrar um arquivo chamado “popcorn.htm”. Este arquivo contém todos os logs do PopcornFX, dê uma olhada dentro para ver o que poderia acontecer de errado.

#### Como inicializar corretamente campos de partícula

Para obter Coords UV e Normal válidos a partir do primeiro quadro, adicione-os ao seu Spawner Script:

<b>  
</b>

```
// PostEval() will be called after particles have been translated to their respective spawn locations

// so, PostEval() is executed in world space

function void PostEval()

{

// we need to initialize correctly the values needed by Substance 3D Painter:

pCoords = Mesh.projectParametricCoords(Position);

UV = Mesh.sampleTexcoord(pCoords);

Normal = normalize(Mesh.sampleNormal(pCoords));

}
```
