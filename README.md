# MVP_Machine_Learning_Maykon_Rodrigues_4025025000400
Entrega do MVP - Finalizando a sprint de 'Machine Leaning e Analytics'
# 🧠 MVP — Machine Learning & Analytics

Este repositório contém o desenvolvimento do **MVP da disciplina de Machine Learning & Analytics**, realizado como parte do curso de [coloque aqui o nome do curso/faculdade].

## 📌 Contexto do Projeto
O objetivo do trabalho é aplicar conceitos de **aprendizado de máquina supervisionado** para prever falhas em um processo industrial, utilizando dados do dataset **AI4I 2020 Predictive Maintenance** (UCI Repository).

A proposta é construir um pipeline completo de **ciência de dados**, passando por:
- Definição do problema
- Preparação e limpeza dos dados
- Detecção e remoção de vazamento de variáveis (*leakage*)
- Construção de baselines e modelos candidatos
- Avaliação de desempenho com métricas adequadas

## 🗂️ Estrutura do Repositório
- `MVP_ML_&_Analytics_Maykon_Rodrigues.ipynb` → Notebook principal do projeto  
- `README.md` → Este arquivo

## ⚙️ Tecnologias Utilizadas
- Python 3.12+
- [scikit-learn](https://scikit-learn.org/stable/)
- Pandas / NumPy
- Matplotlib / Seaborn

## 🔎 Definição do Problema
- **Tarefa**: Classificação binária  
- **Alvo**: `Falha Geral` (0 = normal, 1 = falha)  
- **Desafio principal**: Classe **desbalanceada** (baixa ocorrência de falhas reais)

## 🧹 Preparação dos Dados
- Remoção de IDs e colunas que representam falhas específicas (potencial vazamento).
- Separação de treino/teste com `train_test_split` (estratificado).
- Construção de `preprocess_custom` com:
  - Padronização para variáveis numéricas
  - MinMaxScaler específico para `Torque [Nm]`
  - OneHotEncoder para variáveis categóricas (`Tipo`)

## 📊 Modelos Avaliados
- **Baseline**: DummyClassifier (most_frequent)  
- **Random Forest cru** (num-only, sem pré-processamento)  
- **Random Forest** (com pipeline completo)  
- **Logistic Regression** (com pipeline completo)


## 👤 Autor
Projeto desenvolvido por **Maykon Rodrigues**  
📅 2025 — Trabalho acadêmico
