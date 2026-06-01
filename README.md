# Análise de Dados e Visualização do Catálogo da Netflix

Este projeto realiza uma análise exploratória de dados (EDA) sobre o catálogo de filmes e séries da Netflix. O foco principal é entender os padrões de lançamento da plataforma e mapear visualmente a distribuição global das suas produções.

---

## Objetivo do Projeto

O objetivo deste projeto é analisar o catálogo da Netflix para entender como a plataforma evoluiu ao longo dos anos e como os seus filmes e séries estão distribuídos pelo mundo.

### O que foi feito:
* **Limpeza dos Dados:** Organização de colunas complexas (como listas de atores e países misturados na mesma célula).
* **Análise de Tendências:** Descoberta de quail o tipo de produção é mais frequente na plataforma.
* **Mapeamento Global:** Criação de um mapa-múndi interativo para mostrar visualmente quais países produzem mais conteúdo.


---

## Tecnologias Utilizadas

O projeto foi desenvolvido em ambiente Jupyter Notebook utilizando a linguagem **Python** e as seguintes bibliotecas:

* **Pandas:** Para a manipulação, limpeza e tratamento de dados multivalorados.
* **Plotly Express:** Para a criação de gráficos interativos e do mapa coroplético global.
* **Matplotlib e Seaborn:** Para suporte na montagem de gráficos

---

## O Desafio do Mapa (Engenharia de Visualização)

Um dos pontos centrais deste projeto foi a correção do mapa-múndi de títulos. Por conta de um *outlier* massivo (os Estados Unidos possuem mais de 3.600 títulos, enquanto o segundo lugar possui cerca de 1.000), as escalas lineares tradicionais deixavam o mapa monocromático.

Para resolver isso, o projeto implementou uma **escala discreta por faixas personalizadas (`pd.cut`)**, abrindo o "zoom" visual para os países que possuem entre 0 e 500 títulos. Isso trouxe contraste e permitiu enxergar a relevância de mercados menores na Europa, Ásia e América Latina.

---
## Fonte

Dataset utilizado: https://www.kaggle.com/datasets/shivamb/netflix-shows
