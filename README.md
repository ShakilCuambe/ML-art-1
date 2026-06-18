# Comparação entre Modelos Lineares e uma Mini Rede Neural em Python

Este projeto demonstra a diferença entre **modelos lineares tradicionais** e uma **rede neural implementada manualmente utilizando apenas NumPy**

O objetivo é mostrar como redes neurais conseguem aprender padrões não lineares que modelos lineares possuem dificuldade em representar.

# Funcionalidades

O projeto possui dois experimentos principais:

- **Regressão**
  - Linear Regression
  - Ridge Regression
  - Mini Rede Neural (implementação própria)

- **Classificação**
  - Logistic Regression
  - Mini Rede Neural

Além disso, o programa gera gráficos para facilitar a comparação entre os modelos.



# Tecnologias Utilizadas

- Python 3
- NumPy
- Matplotlib
- Scikit-Learn




# Estrutura do Projeto

# Geração de Dados

# `gera_dados_regressao()`

Cria um conjunto de dados de regressão contendo:

- componente linear;
- componente não linear (função seno);
- ruído gaussiano.

Essa combinação permitiu visualizar as limitações de modelos lineares.



# `gera_dados_classificacao()`

Gera um conjunto de dados bidimensional para classificação.

Os dados possuem formato circular (anel), tornando o problema **não linear**, ideal para comparar uma Regressão Logística com uma Rede Neural.



## Mini Rede Neural

A classe `MiniNN` implementa uma rede neural simples utilizando apenas **NumPy**, sem frameworks de Deep Learning.


A implementação inclui:

 propagação direta (Forward Pass);
 função de ativação ReLU;
 Backpropagation;
 Gradiente Descendente;
 treinamento para regressão;
 treinamento para classificação.



# Comparação dos Modelos

# Regressão

A função:


realiza:

 divisão entre treino e teste;
 normalização dos dados;
 treinamento dos modelos;
 cálculo do MSE (Mean Squared Error);
 geração de um gráfico comparativo.

Modelos avaliados:

- Linear Regression
- Ridge Regression
- MiniNN



# Classificação

executa:

 divisão treino/teste;
 normalização;
 treinamento da Regressão Logística;
 treinamento da MiniNN;
 cálculo da acurácia;
 geração da fronteira de decisão da rede neural.

Modelos avaliados:

 Logistic Regression
 MiniNN


