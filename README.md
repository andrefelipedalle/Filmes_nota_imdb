# Previsão de Notas do IMDb
O objetivo desse projeto é a análise em cima de um banco de dados cinematográfico para orientar qual tipo de filme deve ser o próximo a ser desenvolvido.
A análise exploratória dos dados foi realizada para identificar padrões e tendências nos dados. Foram utilizados gráficos e estatísticas descritivas para analisar a distribuição das variáveis, a correlação entre elas e a relação entre as variáveis e o sucesso do filme (medido pela nota do IMDB).


## Pré-requisitos
As seguintes bibliotecas Python foram utilizadas (estão listadas as versões no arquivo requirements):
- Pandas
- NumPy
- Seaborn
- Scikit-learn 
- Pickle

Para instalar as bibliotecas, execute os comandos abaixo no git bash

```bash
conda create -n ml python=3.8
conda activate ml
pip install -r requirements.txt
```

## Estrutura do Projeto
- **Notebook/desafio_indicium**: Este diretório contém o Jupyter Notebook principal (`desafio_indicium.ipynb`), onde todo o código de análise e visualização é realizado.
- **Data/**: Pasta que contém os dados de entrada utilizados para análise. Os arquivos CSV estão localizados aqui.
- **Model/**: Contém o modelo salvo em .pkl

## Como Executar
1. Clone este repositório: git clone https://github.com/andrefelipedalle/Filmes_nota_imdb.git
2. Navegue até o diretório `Notebook/`: cd Notebook
3. Inicie o Jupyter Notebook: jupyter notebook
4. Abra o arquivo `desafio_indicium.ipynb` e execute as células conforme necessário.

## Conjunto de Dados
A base de dados de treinamento contém 15 colunas, sendo elas: 

Series_Title – Nome do filme
Released_Year - Ano de lançamento
Certificate - Classificação etária
Runtime – Tempo de duração
Genre - Gênero
IMDB_Rating - Nota do IMDB
Overview - Overview do filme
Meta_score - Média ponderada de todas as críticas 
Director – Diretor
Star1 - Ator/atriz #1
Star2 - Ator/atriz #2
Star3 - Ator/atriz #3
Star4 - Ator/atriz #4
No_of_Votes - Número de votos
Gross - Faturamento

# Modelagem de Machine Learning
Um modelo de machine learning foi treinado para prever o sucesso potencial de diferentes tipos de filmes, através da previsão da nota do imdb. O modelo utiliza algoritmos de machine learning, como regressão linear e random forest para aprender a partir dos dados históricos e fazer previsões para as notas do IMDb de novos filmes.
Os modelos de machine learning foram avaliados utilizando métricas como R2, RMSE e MAE. O modelo com melhor desempenho foi o RandomForestRegressor