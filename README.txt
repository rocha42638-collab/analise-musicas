README – Projeto Análise de Músicas (Discoteca Pandas)
1. Objetivo do Projeto

O objetivo deste projeto é identificar quais características musicais influenciam a popularidade das músicas, utilizando análise de dados com Python e a biblioteca Pandas.

A análise busca encontrar padrões e relações entre variáveis musicais e a variável Popularity.

2. Problemas encontrados no Dataset

Durante a análise, foram encontrados diversos problemas no dataset original:

O arquivo CSV estava desorganizado (dados em uma única coluna)
Existência de vírgulas dentro de strings, atrapalhando a separação
Colunas desalinhadas
Tipos de dados incorretos (números como texto)
Valores ausentes (NaN)
Valores inválidos
Linhas corrompidas

Esses problemas impediram a análise direta dos dados, sendo necessário realizar tratamento e limpeza.

3. Tratamento de Dados

Foram realizadas as seguintes etapas de limpeza e tratamento:

Separação das colunas utilizando split
Remoção de espaços extras com strip
Renomeação das colunas para português
Conversão de colunas numéricas
Tratamento de valores ausentes (NaN)
Remoção de valores inválidos
Remoção de outliers (valores de Popularidade acima de 100)
Uso do comando describe() para análise estatística

Após o tratamento, os dados ficaram prontos para análise.

4. Análise Exploratória de Dados

Foram utilizados os seguintes recursos:

Gráficos de dispersão (scatter plot)
Histogramas
Boxplot
Correlação entre variáveis
Estatísticas descritivas (média, mediana, desvio padrão, quartis)

As variáveis analisadas em relação à Popularidade foram:

Danceability
Energy
Valence
Tempo (BPM)
Duration
Instrumentalness
5. Resultados da Análise
Correlação com Popularidade
Nenhuma variável apresentou correlação forte com a Popularidade.
As variáveis com maior relação (mesmo que fraca) com a popularidade foram:
Danceability
Energy
Instrumentalness apresentou relação negativa com a popularidade (músicas instrumentais tendem a ser menos populares).
Duration e Tempo apresentaram correlação negativa moderada (músicas mais longas e com BPM mais alto tendem a ter menor popularidade).
Histograma da Popularidade

O histograma mostrou que:

A maioria das músicas possui popularidade baixa ou média.
Poucas músicas possuem popularidade muito alta.
A distribuição é assimétrica à direita (cauda longa para músicas muito populares).
Boxplot da Popularidade

O boxplot mostrou que:

50% das músicas possuem popularidade entre 17 e 51.
A mediana da popularidade é 32.
Existem outliers (músicas com popularidade muito alta).
A popularidade está concentrada em poucas músicas.
6. Conclusão

Com base na análise dos dados, foi possível concluir que:

A popularidade não depende de apenas uma variável, mas de um conjunto de características musicais.
Danceability e Energy possuem alguma relação com a popularidade, mas não são determinantes sozinhas.
Músicas instrumentais tendem a ser menos populares.
Músicas mais longas e com BPM muito alto tendem a ter menor popularidade.
A maioria das músicas possui baixa popularidade, e poucas músicas concentram a maior parte da popularidade.

Este projeto demonstrou a importância do tratamento de dados antes da análise e como a análise exploratória pode gerar insights importantes.