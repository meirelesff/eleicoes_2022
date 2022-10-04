# eleicoes_2022

Este repositório contém dados de votos válidos de todas as candidaturas que disputaram as eleições presidenciais de 2020, 1º turno. Na falta de um fonte mais bem documentada e acessível do que a [página oficial de divulgação do TSE](https://www.tse.jus.br/eleicoes/eleicoes-2022/interessados-na-divulgacao-de-resultados-2022), os dados aqui foram raspados do [website do G1 ](https://especiaisg1.globo/politica/eleicoes/2022/mapas/mapa-da-apuracao-no-brasil-presidente/1-turno/).

## Leitura

Para carregar os dados usando `R` ou `Python`, não é necessário baixar o arquivo no repositório, basta rodar:

```R
link <- "https://github.com/meirelesff/eleicoes_2022/blob/main/votos_presidente_1t_2022.csv?raw=true"
dados <- readr::read_csv(link)
```

Ou:

```Python
import pandas as pd

link = 'https://github.com/meirelesff/eleicoes_2022/blob/main/votos_presidente_1t_2022.csv?raw=true'
dados = pd.read_csv(link, delim=';')
```