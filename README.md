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

Pesos Ótimos da Carteira
Os pesos ótimos indicam a proporção ideal de investimento em cada ativo da carteira para maximizar o retorno esperado ajustado ao risco (Sharpe Ratio). Esses pesos refletem a alocação mais eficiente dos ativos, com alguns ativos podendo receber 0% de alocação caso não contribuam significativamente para otimizar o desempenho da carteira. Por exemplo:

AAPL: 28.96%
TSLA: 71.04%
MSFT, GOOGL, AMZN: 0%
Essa alocação sugere um investimento concentrado em TSLA e AAPL, com exclusão dos outros ativos para atingir o melhor equilíbrio entre risco e retorno, de acordo com o modelo.

Retorno Esperado
Retorno Anualizado: 0.61 (ou 61%). Esse é o retorno médio anualizado esperado com a carteira otimizada. Esse valor representa o potencial de retorno baseado nos dados históricos, embora resultados reais possam variar devido à volatilidade do mercado e a eventos futuros não previstos.
Risco
Risco Anualizado (Desvio Padrão): 0.58 (ou 58%). Esse valor representa a volatilidade anualizada da carteira otimizada, indicando o grau de variação que os retornos podem apresentar ao longo de um ano. Quanto menor o desvio padrão, mais estável tende a ser o desempenho da carteira.
Arquitetura do Projeto
Este projeto utiliza diversas bibliotecas para manipulação de dados, otimização e visualização:


### Pesos Ótimos da Carteira

A tabela abaixo mostra a alocação ideal de cada ativo na carteira após a otimização. Esses pesos representam a proporção recomendada de investimento em cada ativo para alcançar a melhor relação entre retorno e risco.

| Ticker | Peso (%) |
|--------|----------|
| AAPL   | 28.96    |
| MSFT   | 0        |
| GOOGL  | 0        |
| AMZN   | 0        |
| FB     | 0        |
| TSLA   | 71.04    |
| NVDA   | 0        |
| BRK-B  | 0        |
| JPM    | 0        |
| JNJ    | 0        |
| V      | 0        |
| UNH    | 0        |
| HD     | 0        |
| PG     | 0        |
| MA     | 0        |
| DIS    | 0        |
| VZ     | 0        |
| ADBE   | 0        |
| NFLX   | 0        |
| CRM    | 0        |
| INTC   | 0        |
| KO     | 0        |
| CMCSA  | 0        |
| PEP    | 0        |
| PFE    | 0        |
| CSCO   | 0        |
| XOM    | 0        |
| T      | 0        |
| ABT    | 0        |
| NKE    | 0        |
| MRK    | 0        |
| BA     | 0        |
| WMT    | 0        |
| MCD    | 0        |
| AMD    | 0        |
| MMM    | 0        |
| IBM    | 0        |
| ORCL   | 0        |
| GE     | 0        |
| HON    | 0        |
| TXN    | 0        |
| AMGN   | 0        |
| LOW    | 0        |
| CAT    | 0        |
| SPGI   | 0        |
| MS     | 0        |
| INTU   | 0        |
| LMT    | 0        |
| CVX    | 0        |

### Retorno Esperado

- **Retorno Anualizado**: 0.61 (ou 61%). Esse é o retorno médio anualizado esperado com a carteira otimizada.

### Risco

- **Risco Anualizado (Desvio Padrão)**: 0.58 (ou 58%). Esse valor representa a volatilidade anualizada da carteira.

### Observações

Essa alocação indica um investimento concentrado em **TSLA** e **AAPL**. Com o modelo de otimização, foi determinado que os demais ativos não contribuem significativamente para a maximização do Sharpe Ratio, por isso receberam pesos nulos.


NumPy: para operações numéricas e manipulação de arrays.
Pandas: para coleta, organização e manipulação de dados financeiros.
SciPy (optimize): para resolver o problema de maximização do Sharpe Ratio, central no processo de otimização de portfólio.
Matplotlib: para visualização gráfica da Fronteira Eficiente, facilitando a análise dos trade-offs entre risco e retorno.
Essa combinação de ferramentas permite construir uma carteira bem fundamentada e adaptada ao perfil de risco/retorno desejado, utilizando dados históricos e técnicas de otimização quantitativa.

