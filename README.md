# 📊 Telecom X - Challenge 2

## 📌 Sobre o Projeto

Este projeto tem como objetivo desenvolver modelos preditivos capazes de identificar clientes com maior probabilidade de cancelar seus serviços (churn).

A análise foi realizada utilizando técnicas de **Machine Learning**, passando por etapas de **pré-processamento de dados, análise exploratória, balanceamento de classes, treinamento de modelos e avaliação de desempenho**.

O objetivo é permitir que a empresa **antecipe possíveis cancelamentos e implemente estratégias de retenção de clientes**.

---

# 🧠 Objetivo do Projeto

Construir um pipeline de Machine Learning para:

* Preparar e tratar os dados
* Realizar análise exploratória
* Transformar variáveis categóricas
* Treinar modelos de classificação
* Avaliar desempenho dos modelos
* Identificar os fatores que mais influenciam o churn

---

# 🧰 Tecnologias Utilizadas

* Python
* Pandas
* NumPy
* Scikit-Learn
* Matplotlib
* Seaborn
* Imbalanced-learn (SMOTE)
* Jupyter Notebook / Google Colab

---

# 📂 Estrutura do Projeto

```
telecomx-churn-analysis/
│
├── data/
│   └── TelecomX_Data.json
│
├── notebooks/
│   └── telecomx_churn_pipeline.ipynb
│
├── README.md
│
└── requirements.txt
```

---

# 📊 Etapas do Projeto

## 1️⃣ Carregamento e Normalização dos Dados

O dataset está em formato **JSON aninhado**, sendo necessário utilizar a função `json_normalize` do Pandas para transformar os dados em formato tabular.

---

## 2️⃣ Limpeza e Preparação dos Dados

Nesta etapa foram realizadas as seguintes ações:

* Remoção de colunas irrelevantes (ex: ID do cliente)
* Conversão de colunas numéricas
* Tratamento de valores ausentes
* Conversão da variável alvo (`Churn`) para formato numérico

---

## 3️⃣ Transformação de Variáveis Categóricas

As variáveis categóricas foram convertidas utilizando:

**One-Hot Encoding**

Isso permite que algoritmos de Machine Learning consigam interpretar os dados.

---

## 4️⃣ Análise de Balanceamento de Classes

Foi identificada uma **distribuição desbalanceada** entre clientes que cancelaram e clientes ativos.

Para corrigir esse problema foi utilizada a técnica:

**SMOTE (Synthetic Minority Over-sampling Technique)**

---

## 5️⃣ Treinamento dos Modelos

Foram treinados dois modelos de classificação:

### 🔹 Regressão Logística

Modelo estatístico amplamente utilizado para classificação binária.

### 🔹 Random Forest

Modelo baseado em árvores de decisão que combina múltiplas árvores para melhorar a performance.

---

# 📈 Avaliação dos Modelos

Os modelos foram avaliados utilizando as seguintes métricas:

* Accuracy
* Precision
* Recall
* F1-Score
* Matriz de confusão

O modelo **Random Forest apresentou melhor desempenho geral** para o problema de churn.

---

# 🔎 Variáveis Mais Importantes

A análise de importância das variáveis indicou que os principais fatores associados ao churn são:

* Tipo de contrato
* Tempo de permanência do cliente
* Valor mensal do plano
* Tipo de serviço de internet
* Serviços adicionais como suporte técnico

---

# 💡 Insights Estratégicos

A análise sugere que clientes com as seguintes características apresentam maior risco de cancelamento:

* Contratos mensais
* Baixo tempo de permanência
* Planos com valores elevados
* Falta de serviços adicionais de suporte

Com base nesses insights, a empresa pode:

* Criar incentivos para contratos de longo prazo
* Desenvolver programas de retenção para novos clientes
* Melhorar serviços de suporte e experiência do usuário

---

# 🚀 Possíveis Melhorias

Para evoluir o projeto futuramente, podem ser implementadas melhorias como:

* Testar modelos mais avançados (XGBoost, LightGBM)
* Aplicar técnicas de Feature Engineering
* Realizar validação cruzada
* Criar um dashboard interativo para monitoramento de churn

---

# 👨‍💻 Autor

Bruno Cruz
Estudante de tecnologia e desenvolvimento de software.
