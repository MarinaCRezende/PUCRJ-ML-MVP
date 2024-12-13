# PUCRJ-ML-MVP
Projeto MVP para compor nota da Pós Graduação de Ciência de Dados e Analytics, Sprint de Machine Learning, na PUC-RJ

link para acesso ao Google Colab: https://colab.research.google.com/drive/1w6ICtPpgTYhZpmjbrKcBMJn6UeE4jnyl?usp=sharing


# **Previsão de Eficiência de Combustível em Sistemas de Propulsão Naval**

Este projeto utiliza algoritmos de aprendizado de máquina baseados em árvores (Random Forest e Extra Trees) para prever valores contínuos a partir de um conjunto de dados. O objetivo é avaliar a eficácia desses modelos e identificar os fatores mais relevantes que impactam as previsões.

---

## 📋 **Sumário**
- [Contexto](#📖-contexto)
- [Objetivos](#🎯-objetivos)
- [Modelos e Técnicas](#📊-modelos-e-técnicas)
- [Pré-requisitos](#🛠️-pré-requisitos)
- [Resultados](#📈-resultados)
- [Melhorias Futuras](#📌-melhorias-futuras)
- [Contribuições](#🤝-contribuições)

---

## 📖 **Contexto**
A análise foi desenvolvida para resolver um problema de regressão, onde o objetivo principal é prever valores contínuos com base em variáveis explicativas. Modelos baseados em árvores foram escolhidos devido à sua robustez e capacidade de capturar relações não lineares nos dados.

Os dados fornecidos contêm informações do sistema de propulsão de uma embarcação e foram retiradas de um simulador numérico de um navio de guerra (Fragata) caracterizado por uma planta de propulsão de Turbina a Gás (GT). 

---

## 🎯 **Objetivos**
1. **Prever valores contínuos** com alta precisão utilizando Random Forest e Extra Trees.
2. Identificar os **fatores mais relevantes** que influenciam as previsões.
3. Comparar o desempenho dos modelos e validar sua generalização.

---

## 📊 **Modelos e Técnicas**
- **Modelos Utilizados:**
  - Random Forest Regressor
  - Extra Trees Regressor
  - Lasso
  - Ridge

- **Técnicas Aplicadas:**
  - Ajuste de hiperparâmetros com **GridSearchCV**
  - Validação cruzada para avaliação de generalização

- **Métricas de Avaliação:**
  - \(R^2\) (Coeficiente de Determinação)
  - RMSE (Root Mean Squared Error)
  - MAE (Mean Absolute Error)

---

## 🛠️ **Pré-requisitos**
Para executar este projeto, você precisará de:
- Python 3.8 ou superior
- Bibliotecas:
  - `numpy`
  - `pandas`
  - `scikit-learn`
  - `matplotlib`
  - `seaborn`

## 📈 **Resultados**
### Desempenho dos Modelos

#### **Modelos Lineares**
| Modelo       | MSE    | RMSE   | MAE    | \(R^2\) |
|--------------|--------|--------|--------|--------|
| **Ridge**    | 11.928 | 3.454  | 2.694  | 0.821  |
| **Lasso**    | 11.928 | 3.454  | 2.694  | 0.821  |

#### **Modelos Baseados em Árvores**
##### Random Forest (Otimizado)
- **Conjunto de Treinamento:**
  - MSE: 0.044, RMSE: 0.210, MAE: 0.125, \(R^2\): 0.999
- **Conjunto de Teste:**
  - MSE: 0.236, RMSE: 0.486, MAE: 0.299, \(R^2\): 0.996

##### Extra Trees (Otimizado)
- **Conjunto de Treinamento:**
  - MSE: 0.109, RMSE: 0.330, MAE: 0.195, \(R^2\): 0.998
- **Conjunto de Teste:**
  - MSE: 0.240, RMSE: 0.490, MAE: 0.309, \(R^2\): 0.996

---

## 📌 **Melhorias Futuras**
1. **Exploração de outros modelos:** Testar outras combinações de modelos para testar o desempenho.

---

## 🤝 **Contribuições**
Contribuições são bem-vindas!

