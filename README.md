# 📊 Previsão de Churn de Clientes - Telecom X

Este projeto faz parte de um desafio analítico da **Telecom X**, uma operadora de telecomunicações que vem enfrentando um **alto índice de cancelamento de clientes (churn)**. O objetivo principal é utilizar **dados históricos** para desenvolver um modelo capaz de prever quais clientes têm maior probabilidade de cancelar seus serviços — permitindo que a empresa atue de forma proativa na retenção.

---

## 🎯 Objetivos do Projeto

- Analisar os dados históricos de clientes e identificar padrões de comportamento.
- Preparar os dados para modelagem (limpeza, transformação e codificação).
- Construir e avaliar **modelos preditivos de classificação** para churn.
- Interpretar os resultados e gerar **insights estratégicos** para o negócio.

---

## 🧰 Tecnologias Utilizadas

- **Linguagem:** Python 3.10+
- **Bibliotecas:** pandas, scikit-learn, seaborn, matplotlib
- **Modelos aplicados:**
  - Regressão Logística (modelo base)
  - Random Forest Classifier (modelo mais robusto)

---

## 🔁 Etapas do Pipeline

1. **ETL e Análise Exploratória de Dados (EDA)**
   - Extração dos dados de clientes da Telecom X
   - Tratamento de valores nulos e tipos de dados
   - Análises gráficas e estatísticas para entender padrões

2. **Pré-processamento para Machine Learning**
   - One-Hot Encoding para variáveis categóricas
   - Normalização de variáveis numéricas
   - Divisão dos dados em treino e teste

3. **Modelagem e Avaliação**
   - Treinamento dos modelos de classificação
   - Avaliação com métricas: precisão, recall, F1-score, matriz de confusão
   - Análise de importância das variáveis

---

## 📈 Resumo dos Resultados

Após a construção e avaliação de modelos preditivos para churn de clientes da Telecom X, foram obtidos os seguintes resultados principais:

### 🎯 Desempenho dos Modelos

| Modelo                | Acurácia | Recall (Churn) | F1-Score (Churn) |
|-----------------------|----------|----------------|------------------|
| Regressão Logística   | 80%      | 68%            | 72%              |
| Random Forest Classifier | **85%**  | **76%**        | **78%**          |

> 📌 O modelo **Random Forest** apresentou o melhor desempenho, especialmente no **recall**, que é crucial neste caso, pois identifica corretamente a maior parte dos clientes que irão cancelar.

---

### 🔍 Variáveis mais importantes (Random Forest)

1. Tipo de contrato (`Month-to-month`)
2. Método de pagamento (`Electronic check`)
3. Tempo de permanência (tenure)
4. Valor da cobrança mensal (`MonthlyCharges`)
5. Tipo de internet (`Fiber optic`)
6. Se o cliente é idoso (`SeniorCitizen`)

Essas variáveis se mostraram as mais relevantes para prever a probabilidade de churn.

---

### 🧠 Conclusões Estratégicas

- Clientes com **contrato mensal, débito eletrônico e pouco tempo de casa** representam o maior risco de churn.
- Clientes idosos e com **serviços de alto custo** também demandam atenção especial.
- A empresa pode aplicar **ações proativas de retenção** com base nessas informações, como:
  - Ofertas para migração de contrato
  - Incentivos para uso de pagamento automático
  - Monitoramento de novos clientes nos primeiros meses
  - Segmentação de campanhas conforme o perfil de risco

---

Este modelo agora pode ser integrado a sistemas internos para **previsão em tempo real** ou **gatilhos de ações preventivas**, ajudando a reduzir a evasão e melhorar a retenção de clientes.

