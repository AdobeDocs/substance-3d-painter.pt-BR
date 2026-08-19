---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/release-notes/old-versions/version-2-3.html"
breadcrumb-title: ''
description: Consulte as notas de versão do Substance 3D Painter versão 2.3 para saber mais sobre novos recursos, aprimoramentos e correções de erros.
helpx_creative_field: ""
helpx_description: Painter > Release notes > Old versions > Version 2.3
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Versão 2.3
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '671'
ht-degree: 0%

---


# Versão 2.3

O **Substance Painter 2.3** aprimora a API de script para liberar seu primeiro plug-in oficial: uma exportação de Photoshop com a pilha de camadas completa disponível.

Data de Lançamento: *15 de setembro de 2016*

## Principais recursos

### Novo plug-in de exportação para Photoshop

![](../../assets/ps-230.jpg)

Com esta versão, nos concentramos em adicionar novas possibilidades na API de script para implementar o **um exportador avançado para o Photoshop**. Para acessar essa nova exportação, basta clicar no ícone do Photoshop disponível na barra de ferramentas principal (se o plug-in estiver ativado, o que garante maiúsculas e minúsculas por padrão). O plug-in permite exportar toda a pilha de camadas disponível em um conjunto de texturas e criar uma estrutura semelhante dentro de um arquivo PSD. Este recurso **requer que o Photoshop esteja instalado** no computador para poder gerar o arquivo de PSD.

Algumas opções estão disponíveis por meio do botão configurar do menu de plug-in:

![](../../assets/configure-ps.png)

## Tutorial

Nosso tutorial mais recente explica o processo de exportação com o novo plug-in:

## Notas de versão

### 2.3.1

(Lançado em 7 de outubro de 2016)

**Adicionado:**

* [Plug-in]&#x200B;[Photoshop] Permite especificar qual material/pilha/canais exportar
* [Scripting] Os nomes de função têm algumas inconsistências

**Corrigido:**

* [Exportar] o Alpha pode ser descartado nas predefinições de exportação personalizadas
* [Exportar] o Alpha obtém conversão gama incorreta em canais sRGB
* [Exportar] Documentos não quadrados são exportados como quadrados
* [Exportar] Não é possível exportar mapas adicionais se algum estiver ausente
* [Iray] Alguns parâmetros (como Intensidade de emissivo) não têm efeito
* [NVIDIA] Falha na inicialização com a NVIDIA Quadro K2200/GTX 750/760
* [AMD] Conjunto incorreto de cores para miniaturas e visualizações
* [AMD] Congela e falha de driver em Novo arquivo e Abrir arquivo
* [Log] “software-version” está ausente no arquivo de log

### 2.3.0

(Lançado em 15 de setembro de 2016)

**Adicionado:**

* [Plug-in] Novo plug-in “Exportar para o Photoshop” (exportar pilha de camadas completa)
* [Exportar] Permite especificar a largura do preenchimento (em pixels ou infinito)
* [Exportar] Permite definir o tipo de fundo fora dos UVs
* [Prateleira] Novo sombreador de camada de material para misturar 10 materiais
* [Prateleira] Novo sombreador de argila para ver detalhes com o canal height/normal
* [Prateleira] Novo filtro de iluminação cozido com entrada de ambiente
* [Prateleira] Alguns geradores de máscara atualizados para adicionar transformações não quadradas
* [Janela de visualização] Adiciona o mapa normal composto (normal+height+bake) ao modo solo
* [Script] Permitir a exportação de mapas adicionais
* [Scripts] Permitir consultar mapas adicionais disponíveis por conjunto de texturas
* [Script] Permitir recuperação de formato de canal
* [Roteiro] Adicione exemplos na documentação de cozimento
* [Script] Permitir consulta da visibilidade de uma camada
* [Script] Permitir consulta do modo de mesclagem e da opacidade da camada
* [Scripting] Permitir exportar mapas convertidos (mapas normais finais, AO misto, etc.)
* [Substance] Ler e conectar usos personalizados
* [Atalhos] Adicionar tecla modificadora (SHIFT) para percorrer o modo solo para trás
* [Exportar] Predefinição de exportação padrão atualizada para desativar alfa
* [IU] Agora, as miniaturas são calculadas somente se o mecanismo estiver disponível
* [IU] Exibir uma menção quando as miniaturas estiverem em processamento

**Corrigido:**

* Falha com alguns projetos antigos ao abri-los
* Falha com cache de canais de textura corrompido
* Falha ao mesclar mais de 4 materiais com o fluxo de trabalho de Camada de material
* [IU] Os atalhos de ferramenta não funcionam se a barra de ferramentas estiver oculta
* [UI] A barra de ferramentas do Iray está marcada como “Sem título” no menu Exibir
* [UI] As barras de ferramentas do plug-in são chamadas de “Não inclinadas” no menu Exibir
* [Baker] Pressionar Enter durante a edição de uma configuração de cozimento inicia o processo de cozimento
* [Baker] Intervalos incorretos para alguns parâmetros
* [Importar] Não é possível importar malhas OBJ devido a números muito grandes
* [Importar] Alguns arquivos OBJ são importados com muitos subobjetos
* [Exportar] o fundo do canal é preenchido com preto em vez da cor padrão na exportação
* [Ferramenta] As partículas não funcionam corretamente se o CDV for muito baixo
* [Ferramenta] A cor de visualização do pincel está incorreta com máscaras em subpilhas
* [Visor] Quando o pincel vai para áreas vazias na exibição 2D, ele se torna gigantesco
* [Visor] Visualização de pincel em branco ao pintar texturas Normais
* [Scripting] Documentação incorreta : “ao” listado em vez de “ambientocclusion”
* [Scripting] O processo iniciado com subprocess() é finalizado ao fechar o Painter
* [Prateleira] Filtro de iluminação assado usa entrada de AO incorreta
* [MacOS] Projeto de hidrante contra incêndio removido (incompatível)
* O projeto padrão é aberto ao carregar um arquivo \*.spt (em vez de \*.spp)
