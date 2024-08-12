# Análise de Churn para Plataforma de Streaming

Este projeto realiza uma análise preditiva para identificar usuários que têm maior probabilidade de cancelar a assinatura (churn) de uma plataforma de streaming. O projeto envolve o pré-processamento de dados, construção e avaliação de modelos de Machine Learning, incluindo Regressão Logística e Random Forest.

## Pré-requisitos

Certifique-se de ter as seguintes bibliotecas instaladas:

```bash
pip install pandas numpy seaborn matplotlib scikit-learn yellowbrick
```

## Descrição do Projeto

### 1. Importação e Carregamento dos Dados

O projeto começa com a importação das bibliotecas necessárias e o carregamento dos dados de um arquivo CSV (`streaming_data.csv`). As bibliotecas utilizadas incluem:

- `pandas` e `numpy` para manipulação de dados.
- `seaborn` e `matplotlib` para visualização.
- `scikit-learn` para construção e avaliação de modelos de Machine Learning.
- `yellowbrick` para visualização dos resultados dos modelos.

### 2. Entendimento dos Dados

Foram realizadas análises iniciais para entender a estrutura dos dados, identificar valores nulos e verificar as distribuições das variáveis. Um `pairplot` foi utilizado para observar a correlação entre as variáveis.

### 3. Preparação dos Dados

Foram realizadas as seguintes etapas de preparação dos dados:

- Imputação de valores nulos com valores padrão.
- Conversão de tipos de dados para garantir consistência.
- Divisão dos dados em variáveis independentes (X) e a variável dependente (y), que representa o churn.

### 4. Modelagem

Foram utilizados dois modelos de Machine Learning:

1. **Regressão Logística**:
    - Uma pipeline foi construída para aplicar o pré-processamento e treinar o modelo de Regressão Logística.
    - A acurácia, precisão, recall, F1 score e AUC-ROC foram utilizados para avaliar o modelo.
    - Um `GridSearchCV` foi usado para otimizar os hiperparâmetros.

2. **Random Forest**:
    - Uma pipeline foi construída para aplicar o pré-processamento e treinar o modelo Random Forest.
    - RMSE e R² foram utilizados para avaliar o desempenho do modelo.
    - Assim como na Regressão Logística, um `GridSearchCV` foi usado para otimizar os hiperparâmetros.

## Resultados

Os resultados dos modelos foram comparados para determinar qual abordagem forneceu as melhores previsões para o churn de usuários na plataforma de streaming.

## Conclusão

Este projeto demonstrou a aplicação de técnicas de Machine Learning para a previsão de churn em uma plataforma de streaming. A análise comparativa dos modelos permite insights valiosos sobre o comportamento dos usuários e as métricas de desempenho do modelo.

## Instruções de Uso

1. Clone o repositório para sua máquina local.
2. Certifique-se de que todas as bibliotecas necessárias estejam instaladas.
3. Execute o Jupyter Notebook `Desafio_06.ipynb` para reproduzir a análise e os resultados.
