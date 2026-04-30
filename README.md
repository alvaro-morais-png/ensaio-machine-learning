# 1.Nome do Projeto
Ensaio de Machine Learning

# 2. Problema de Negócio
## 2.1 Descrição
A empresa Data Money acredita que a expertise no treinamento e ajuste fino dos algoritmos, feito pelos Cientistas de Dados da empresa, é o principal motivo dos ótimos resultados que as consultorias vem entregando aos seus clientes.

## 2.2 Objetivo 
O objetivo desse projeto será realizar ensaios com algoritmos de Classificação, Regressão e Clusterização, para estudar a mudança do comportamento da performance, a medida que os valores dos principais parâmetros de controle de overfitting e underfitting mudam.

# 3. Planejamento da Solução
## 3.1 Produto final
O produto final será 7 tabelas mostrando a performance dos algoritmos, avaliados usando múltiplas métricas, para 3 conjuntos de dados diferentes: Treinamento, validação e teste.

## 3.2 Algoritmos ensaiados

Classificação:

ALgoritmos: KNN, Decision Tree, Random Forest e Logistic Regression

Métricas de performance: Accuracy, Precision Recall e F1-Score

Regressão:
Algoritmos: Linear Regression, Decision Tree Regressor, Random Forest Regressor, Polinomial Regression, Linear Regression Lasso, Linear Regression Ridge, Linear Regression Elastic Net, Polinomial Regression Lasso, Polinomial Regression Ridge e Polinomial Regression Elastic Net

Métricas de performance: R2, MSE, RMSE, MAE e MAPE

Agrupamento:

Algoritmos: K-Means e Affinity Propagation
Métricas de performance: Silhouette Score

## 3.3 Ferramentas utilizadas:
Python 3.8 e Scikit-learn

# 4. Desenvolvimento
## 4.1 Estratégia da solução
Para o objetivo de ensaiar os algoritmos de Machine Learning, eu vou escrever os códigos utilizando a linguagem Python, para treinar cada um dos algoritmos e vou variar seus principais parâmetros de ajuste de overfitting e observar a métrica final.
O conjunto de valores que fizerem os algoritmos alcançarem a melhor performance, serão aqueles escolhidos para o treinamento final do algoritmo.

## 4.2 O passo a passo
Passo 1: Divisão dos dados em treino, teste e validação.
Passo 2: Treinamento dos algoritmos com os dados de treinamento, utilizando os parâmetros “default”.
Passo 3: Medir a performance dos algoritmos treinados com o parâmetro default, utilizando o conjunto de dados de treinamento.
Passo 4: Medir a performance dos algoritmos treinados com o parâmetro “default”, utilizando o conjunto de dados de validação.
Passo 5: Alternar os valores dos principais parâmetros que controlam o overfitting do algoritmo até encontrar o conjunto de parâmetros que apresente a melhor performance dos algoritmos.
Passo 6: Unir os dados de treinamento e validação
Passo 7: Retreinar o algoritmo com a união dos dados de treinamento e validação, utilizando os melhores valores para os parâmetros de controle do algoritmo.
Passo 8: Medir a performance dos algoritmos treinados com os melhores parâmetro, utilizando o conjunto de dados de teste.
Passo 9: Avaliar os ensaios e anotar os 3 principais Insights que se destacaram.

# 5. Os top 3 Insights
## 5.1 Insight Top 1
Os algoritmos baseado em árvores possuem uma performance melhores em todas as métricas, quando aplicados sobre os dados de teste, no ensaio de Classificação.

## 5.2 Insight Top 2
A performance dos algoritmos de classificação sobre os dados de validação ficou bem próxima da performance sobre os dados de teste.

## 5.3 Insight Top 3
Todos os algoritmo de regressão não apresentaram boas métricas de performance, o que mostra uma necessidade de uma seleção de atributos e uma preparação melhor das variáveis independentes do conjunto de dados.

# 6. Resultados


## **Ensaio de Classificação:**
## 6.1 Sobre os dados de treinamento
|Nome_do_algoritmo |Acurácia| Precision| Recall| F1_score|
|:----|:----|:----|:----|:----|
|KNN  |  0.782    | 0.756 | 0.733 |   0.744|
|Decision Tree  |  1.000   |  1.000 | 1.000  |  1.000|
|Random Forest    |1.000    | 1.000|  1.000   | 1.000|
|Logistic Regression   | 0.873    | 0.861|  0.842   | 0.851|

## 6.2 Sobre os dados de validação
|Nome_do_algoritmo |Acurácia |Precision| Recall| F1_score|
|:----|:----|:----|:----|:----|
|                  KNN    |0.676    | 0.632 | 0.603   | 0.617|
|        Decision Tree   | 0.946 |    0.936 | 0.939 |   0.937|
|        Random Forest  |  0.965 |    0.974 | 0.943 |   0.959|
|  Logistic Regression  |  0.870  |   0.860  |0.836 |   0.848|


## 6.3 Sobre os dados de teste
|Nome_do_algoritmo|Acurácia|Precision|Recall|F1_score|
|:----|:----|:----|:----|:----|
|KNN|0.699|0.654|0.666|0.660|
|Decision Tree|0.954|0.954|0.941|0.947|
|Random Forest|0.964|0.973|0.944|0.958|
|Logistic Regression|0.871|0.868|0.831|0.849|



## **Ensaio de Regressão:**
## 6.4 Sobre os dados de treinamento
|Nome_do_algoritmo|R2|MSE|RMSE|MAE|MAPE|
|:----|:----|:----|:----|:----|:----|
|Linear Regression|0.554|0.110|0.331|0.249|0.267|
|Decision Tree Regressor|1.000|0.000|0.000|0.000|0.000|
|Random Forest Regressor|0.984|0.004|0.063|0.022|0.024|
|Polynomial Regression|0.708|0.072|0.268|0.192|0.229|
|Linear Regression Lasso|0.000|0.246|0.331|0.491|0.566|
|Linear Regression Ridge|0.554|0.110|0.331|0.249|0.267|
|Linear Regression Elastic Net|0.000|0.246|0.495|0.491|0.566|
|Polynomial Regression Lasso|0.421|0.142|0.377|0.322|0.357|
|Polynomial Regression Ridge|0.751|0.061|0.247|0.178|0.210|
|Polynomial Regression Elastic Net|0.421|0.142|0.377|0.322|0.357|


## 6.5 Sobre os dados de validação
|Nome_do_algoritmo|R2|MSE|RMSE|MAE|MAPE|
|:----|:----|:----|:----|:----|:----|
|Linear Regression|0.548|0.111|0.333|0.250|0.270|
|Decision Tree Regressor|0.777|0.055|0.234|0.055|0.062|
|Random Forest Regressor|0.886|0.028|0.168|0.059|0.066|
|Polynomial Regression|0.708|0.072|0.268|0.192|0.229|
|Linear Regression Lasso|0.000|0.246|0.495|0.491|0.566|
|Linear Regression Ridge|0.548|0.111|0.333|0.250|0.270|
|Linear Regression Elastic Net|0.000|0.246|0.495|0.491|0.566|
|Polynomial Regression Lasso|0.417|0.143|0.378|0.322|0.358|
|Polynomial Regression Ridge|0.748|0.062|0.249|0.179|0.211|
|Polynomial Regression Elastic Net|0.417|0.143|0.378|0.322|0.358|


## 6.6 Sobre os dados de teste
|Nome_do_algoritmo|R2|MSE|RMSE|MAE|MAPE|
|:----|:----|:----|:----|:----|:----|
|Linear Regression|0.550|0.111|0.333|0.250|0.268|
|Decision Tree Regressor|0.852|0.036|0.191|0.063|0.071|
|Random Forest Regressor|0.889|0.027|0.166|0.056|0.062|
|Polynomial Regression|0.656|0.085|0.291|0.210|0.245|
|Linear Regression Lasso|0.515|0.120|0.346|0.278|0.309|
|Linear Regression Ridge|0.550|0.111|0.333|0.250|0.268|
|Linear Regression Elastic Net|0.549|0.111|0.333|0.251|0.269|
|Polynomial Regression Lasso|0.717|0.070|0.264|0.191|0.233|
|Polynomial Regression Ridge|0.749|0.062|0.249|0.179|0.210|
|Polynomial Regression Elastic Net|0.749|0.062|0.249|0.179|0.210|

## **Ensaio de Clusterização:**
## 6.7 Sobre os dados de treinamento
|Nome_do_algoritmo|Número de clusters|Average Silhouette Score|
|:----|:----|:----|
|K-Means|3|0.560170|
|Affinity Propagation|3|0.551746|


# 7. Conclusões
Nesse ensaio de Machine Learning, consegui adquirir experiência e entender melhor sobre os limites dos algoritmos entre os estados de underffiting e overfitting.
Algoritmos baseados em árvores são sensível quanto a profundidade do crescimento e do número de árvores na floresta, fazendo com que a escolha correta dos valores desses parâmetros impeçam os algoritmos de entrar no estado de overfitting.
Os algoritmos de regressão, por outro lado, são sensíveis ao grau do polinômio. Esse parâmetro controla o limite entre o estado de underfitting e overfitting desses algoritmos.
Esse ensaio de Machine Learning foi muito importante para aprofundar o entendimento sobre o funcionamento de diversos algoritmos de classificação, regressão e clusterização e quais os principais parâmetros de controle entre os estados de underfitting e overfitting.

# 8. Próximos passos
Como próximos passos desse ensaio, pretendo ensaiar novos algoritmos de Machine Learning e usar diferentes conjuntos de dados para aumentar o conhecimento sobre os algoritmos e quais cenários são mais favoráveis para o aumento da performance dos mesmos.

