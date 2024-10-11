# APS-Otimização-de-Sistemas

Atividade Supervisionada – Otimização de Sistemas
## Informações do Aluno

 -  Disciplina: `Otimização de Sistemas`
 -  Aluno: `Thiago Ribeiro Chaves`
 -  Matricula: `2019200753`
 -  Turma: `962`

## Linguagens e Ferramentas

 - Python
 - Pandas
 - Numpy
 - Scipy.optimize
 - yfinance
 - matplotlib
 - seaborn
 - IDE online: Google Colab


## Escopo do Projeto
- Este projeto tem como foco a construção de um algoritmo de otimização baseado no problema da mochila para montar uma carteira de investimentos. O objetivo é maximizar o retorno esperado de uma carteira de ativos financeiros, considerando um limite de risco aceitável (capacidade da mochila). A implementação segue três etapas: modelagem matemática, implementação em Python, e visualização dos resultados. Toda a resolução do projeto se econtra no arquivo `APS Otimização_de_sistemas.ipynb` encontrada no inicio

Funcionalidades
- Coleta de Dados de Ativos:
 Coleta de dados financeiros usando a API do Yahoo Finanças.

- Calcula os retornos diários dos ativos.

- Otimização da Carteira:
Implementação de uma função objetivo para maximizar o retorno esperado da carteira.

- Utilização do Sharpe Ratio como critério de otimização.

- Restrições que garantem que a soma dos pesos dos ativos na carteira seja igual a 1.

- Visualização dos Resultados:
Gráficos da fronteira eficiente mostrando o equilíbrio entre retorno esperado e risco.

- Cálculo e exibição dos pesos ótimos da carteira.


## Resultados
![download](https://github.com/user-attachments/assets/e7f0b78c-5567-47d8-8b6e-fe263f5c0892)

Resultados:
Pesos Ótimos da Carteira: Os pesos ótimos indicam a porcentagem de cada ativo na carteira otimizada. No seu resultado, temos:

AAPL: 28.96%

MSFT: 0%

GOOGL: 0%

AMZN: 0%

TSLA: 71.04%

Isso significa que a carteira otimizada sugere investir uma grande proporção em TSLA e uma quantidade significativa em AAPL, ignorando os outros ativos para maximizar o retorno esperado com o menor risco possível.

Retorno Esperado:

Retorno Esperado: 0.61 (ou 61% anualizado). Este é o retorno médio que você pode esperar obter anualmente com a carteira otimizada.

Risco:

Risco: 0.58 (ou 58% anualizado). Este é o desvio padrão dos retornos da carteira, representando a volatilidade anualizada.



## Arquitetura do Projeto
A implementação utiliza diversas bibliotecas em Python, como numpy, pandas, scipy.optimize, matplotlib e seaborn. Estas ferramentas são essenciais para a manipulação de dados, otimização e visualização dos resultados.

