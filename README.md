# Credit Card Fraud Detection

Projeto desenvolvido para o desafio da DIO, com o objetivo de identificar transações fraudulentas de cartão de crédito utilizando Machine Learning.

## Dataset

Foi utilizado o dataset [Credit Card Fraud Detection](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud), disponível no Kaggle.

O conjunto possui 284.807 transações, sendo 492 fraudulentas (0,17%), apresentando forte desbalanceamento entre as classes.

Para executar o notebook, baixe o arquivo `creditcard.csv` no Kaggle e coloque-o na pasta do projeto.

## Tecnologias

- Python
- Pandas, NumPy, Matplotlib e Seaborn
- Scikit-learn
- XGBoost
- SHAP
- Jupyter Notebook

## Etapas do projeto

1. Análise exploratória e identificação do desbalanceamento.
2. Criação da variável `Log_Amount` e preparação dos dados.
3. Treinamento de Regressão Logística, Random Forest e XGBoost.
4. Avaliação com precisão, recall, F1-score, curvas ROC e Precision-Recall.
5. Comparação de thresholds.
6. Explicabilidade do Random Forest com SHAP.

## Resultados

| Modelo | Precisão (fraude) | Recall (fraude) | F1-score |
|---|---:|---:|---:|
| Regressão Logística | 6,12% | 91,84% | 11,47% |
| Random Forest | 91,86% | 80,61% | 85,87% |
| XGBoost | 33,46% | 86,73% | 48,30% |

O Random Forest apresentou o melhor equilíbrio entre precisão e recall, considerando o F1-score.

## Como executar

1. Baixe o dataset no Kaggle.
2. Coloque `creditcard.csv` na pasta do projeto.
3. Instale as bibliotecas utilizadas.
4. Abra o notebook no Jupyter ou VS Code e execute as células na ordem.

## Conclusão

O projeto demonstrou uma aplicação de modelos de classificação em dados desbalanceados. A comparação pode mostrar a importância de avaliar precisão, recall e F1-score, especialmente em problemas de detecção de fraudes.