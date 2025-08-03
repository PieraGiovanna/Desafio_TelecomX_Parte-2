# Desafio_TelecomX_Parte-2

## 🤖 Modelos Utilizados e Justificativa

Foram aplicados dois algoritmos de classificação supervisionada para prever o churn de clientes com base em dados históricos:

### 🔹 1. Regressão Logística

A Regressão Logística foi usada como **modelo base** devido à sua simplicidade e interpretabilidade. Ela é adequada para problemas de classificação binária, como prever se um cliente vai ou não cancelar o serviço.

- ✅ Fácil de interpretar os coeficientes
- ✅ Bom desempenho com dados lineares
- ❌ Pode não capturar relações mais complexas entre variáveis

### 🔹 2. Random Forest Classifier

A Random Forest foi escolhida como **modelo principal**, por ser um algoritmo de ensemble baseado em múltiplas árvores de decisão. Ela lida muito bem com dados mistos (categóricos e numéricos), outliers e relações não lineares.

- ✅ Alta precisão e robustez
- ✅ Capaz de capturar interações complexas entre variáveis
- ✅ Fornece estimativa da importância de cada variável
- ❌ Pode ser menos interpretável que modelos lineares

### 📌 Justificativa da Escolha

A combinação dos dois modelos permite:
- Comparar desempenho entre um modelo simples e um mais robusto
- Obter explicações com a Regressão Logística e alta performance com a Random Forest
- Balancear interpretabilidade e precisão, oferecendo uma solução técnica e estrategicamente aplicável

Com base nos testes realizados, a **Random Forest apresentou melhor recall e acurácia**, sendo a mais indicada para auxiliar a Telecom X a identificar clientes com risco de churn.

