---
source-git-commit: 6b6d52207ca1d043aaa1b2b14145b6b49d4c1942
workflow-type: tm+mt
source-wordcount: '155'
ht-degree: 0%
---
# Remover metadados HelpX legados

Com o Python 3.10 ou posterior, execute os seguintes comandos na raiz do repositório:

```shell
python remove_helpx_metadta.py 1 <path>
python remove_helpx_metadta.py 2 <path>
```

O modo `1` é uma simulação: lista os arquivos correspondentes e relata o número de arquivos
digitalizados, arquivos com correspondências e campos de metadados correspondentes sem alterar arquivos.
O modo `2` remove esses campos e relata as contagens de remoção. Omitir `<path>` para
examinar a pasta atual. Caminhos de cotação que contêm espaços.

O script verifica recursivamente `.md` arquivos (não diferencia maiúsculas de minúsculas) e remove arquivos de nível superior
Campos de frente YAML cujos nomes começam com `helpx`, incluindo suas várias linhas
valores. Preserva outros metadados, comentários, linhas em branco, conteúdo de Markdown,
e finais de linha. Ele não remove as referências `helpx` no corpo.
Revise a simulação antes de usar o modo `2`; remova os arquivos editados sem
criação de backups. Os erros de arquivo e os assuntos iniciais não fechados são reportados e produzem
um status de saída diferente de zero. Os arquivos com o front matter não fechado são deixados inalterados.