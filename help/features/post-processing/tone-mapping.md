---
helpx_url: "https://helpx.adobe.com/br/substance-3d-painter/features/post-processing/tone-mapping.html"
breadcrumb-title: ''
description: Saiba como usar o pós-processamento do mapeamento de tom no Substance 3D Painter para ajustar a exposição e a correção de cores no visor.
helpx_creative_field: ""
helpx_description: Painter > Features > Post Processing > Tone Mapping
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Mapeamento de tons
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '690'
ht-degree: 0%

---


# Mapeamento de tons

![](../../assets/tone-mapping.png)

Os parâmetros de mapeamento de tom permitem controlar como as cores serão dimensionadas para serem exibidas na tela. Essas configurações podem ser úteis para redistribuir cores por causa da ampla gama de valores (que pode exceder o que a tela atual é capaz de exibir).

>[!NOTE]
>
> O Substance 3D Painter gera cores **HDR** (Intervalo dinâmico) (no espaço de Gama linear), mas a maioria das telas permite apenas a visualização de cores **LDR** (Intervalo dinâmico baixo). Para mapear o intervalo HDR para o intervalo de LDR, uma conversão deve ser feita. Esse é o princípio do mapeamento de tons.

| *Configuração* | *Descrição* |
| --- | --- |
| **Exposição** | Dimensiona os resultados da renderização de espaço HDR antes da aplicação de qualquer efeito de brilho ou da realização do mapeamento de tons. |
| **Gama** | Este é o valor de gama para a correção de gama. |
| **Função** | Função a ser usada para mapear o intervalo HDR para o intervalo de LDR.  As funções disponíveis são:<ul data-preserve-html="true"><li data-preserve-html="true"><strong> Automático </strong>: A função de mapa de tons é selecionada automaticamente. O padrão é <strong> Sensitometric </strong>. </li><li data-preserve-html="true"><strong> Linear </strong>: A cor de saída não está fixada em 0 a 1 somente para este tipo. Isso é ideal para ao implementar algum efeito no espaço HDR no lado do aplicativo após a aplicação dos efeitos. <br/>Não recomendamos isso, a menos que você tenha algum motivo específico para usá-lo, pois os componentes de alta luminância serão completamente perdidos e realces estourados ocorrerão se o mapeamento linear for usado como a saída de tela final como está.</li><li data-preserve-html="true"><strong> LinearSat </strong> : É quase igual a <strong> Linear </strong> , exceto que a cor de saída está fixada. Além disso, a síntese de brilho é um pouco mais suave do que o <strong> Linear </strong>.</li><li data-preserve-html="true"><strong> Sensitométrico </strong>: função padrão quando a renderização da cena é executada no espaço HDR.</li><li data-preserve-html="true"><strong> Reinhard </strong> : Isso resulta em um mapeamento mais gradual do que <strong> Sensitometric </strong> , e um contraste ligeiramente baixo. Dessa forma, ela faz com que a resolução dos componentes de alta luminância se torne alta e a reprodução mais forte das variações de luminância nas partes brilhantes.</li><li data-preserve-html="true"><strong> ReinhardLum </strong> : Tipo para implementar o mapa de tons <strong> Reinhard </strong> com a luminância como referência e mantendo a saturação original (vivacidade: proporção RGB). Mapeia apenas as informações de luminância para o espaço LDR e, em seguida, reproduz a saturação original. A saturação no espaço HDR também é mantida após o mapeamento de tons.</li><li data-preserve-html="true"><strong> Log </strong> : Isso resulta em um mapeamento ainda mais gradual que <strong> Reinhard </strong> , e um contraste baixo. Isso faz com que a resolução dos componentes de alta luminância se torne alta e a reprodução mais forte das variações de luminância nas partes brilhantes.</li><li data-preserve-html="true"><strong> LogLum </strong> : Tipo para implementação do mapa de tons do espaço logarítmico com a luminância como referência e mantendo a saturação original (vivacidade: proporção de RGB). Isso mapeia apenas as informações de luminância para o espaço logarítmico e, em seguida, reproduz a saturação original. A saturação no espaço HDR também é mantida após o mapeamento de tons.</li></ul> |
| **Fator de Mapeamento** | Isso controla o nível máximo da luminância (brilho) no espaço HDR mapeado para o espaço LDR final no processo de mapeamento de tom. As cores mais brilhantes do que a luminância do espaço HDR especificado não podem ser representadas no espaço LDR, resultando em realces estourados. Em termos concretos, esse valor é a luminância (após a escala de exposição) no espaço HDR que é mapeada para o valor máximo de luminância (1,0) no espaço LDR. No modo de renderização HDR, quanto menor for esse valor, maior será o contraste e maior a probabilidade de realces estourados. Por outro lado, especificar valores mais altos resulta em menor contraste e diminui a probabilidade de realces estourados. No modo de renderização LDR, quando ocorre um remapeamento para um espaço HDR para aplicar um efeito, a faixa de luminância é expandida até o valor especificado em **Fator de mapeamento**. Por outro lado, a luminância do **Fator de Mapeamento** é mapeada para a luminância máxima de LDR durante o mapeamento de tons.Em outras palavras, isso especifica o fator de dimensionamento do intervalo dinâmico aplicado aos resultados da renderização de LDR para a aplicação de efeitos. Defini-lo como um valor alto enfatiza as regiões brilhantes nos efeitos.  **Observação:** essa configuração não terá efeito (será ignorada) se a **função** estiver definida como qualquer uma das seguintes opções no modo de renderização HDR: **Linear**, **LinearSat** ou **Sensitométrica**. |
