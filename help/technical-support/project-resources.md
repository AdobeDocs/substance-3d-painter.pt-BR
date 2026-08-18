---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/technical-support/project-resources.html"
breadcrumb-title: ''
description: Acesse os recursos do projeto e a documentação técnica do Substance 3D Painter para aprimorar seu fluxo de trabalho e solução de problemas.
helpx_creative_field: ""
helpx_description: Substance 3D Painter
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Recursos do projeto
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '263'
ht-degree: 0%

---


# Recursos e configurações do projeto

O gerenciamento de recursos do projeto pode ajudar a estabelecer uma boa base para o desempenho do seu projeto no Painter.

+++Reduzir mapas baked
Às vezes, nem todos os mapas baked precisam ter resoluções de 2k ou 4k. Não hesite em assar um lote em 2k, em seguida, recarregue em uma resolução mais baixa para ver se há uma diferença visual.

+++

+++Gerenciar bitmaps importados
As imagens importadas podem afetar drasticamente o desempenho, por isso é importante ter cuidado com o que é importado. Se os seus Conjuntos de texturas estiverem definidos como 2k e não forem exportados com uma resolução mais alta, o uso de uma imagem de 8k não terá nenhum impacto positivo, sua qualidade será limitada em 2k, pois é a resolução do Conjunto de texturas.

O formato também é importante - EXR, HDR e até mesmo PNG são muito mais pesados que um JPG, e nem todas as imagens podem precisar do nível de qualidade de um EXR (como cor base vs. detalhes do Height, por exemplo).

+++

+++Ajustar configurações do sombreador
a qualidade do specular na Ultra dará um resultado mais preciso, mas a configuração é cara. Quanto mais efeitos forem ativados de uma só vez no sombreador, maior será o cálculo. Sempre que possível, divida materiais complexos em outro conjunto de texturas com um sombreador separado. Se o deslocamento estiver ativado, tome cuidado com o parâmetro do mosaico.

+++

+++Ajustar opções de arquivo
Usar <b>Arquivo > Salvar > Salvar e reduzir arquivo</b> <b>dimensione </b>para liberar dados desnecessários e use <b>Remover recursos não utilizados</b> para se livrar de arquivos importados para o projeto que não estão sendo usados em nenhum lugar dentro do projeto.

+++
