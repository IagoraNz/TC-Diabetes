# 🩺 TC-Diabetes: Predição de Diabetes

![Status do Projeto](https://img.shields.io/badge/Status-Concluído-green)
![Python](https://img.shields.io/badge/Python-3.8%2B-blue)
![License](https://img.shields.io/badge/License-MIT-yellow)

Este repositório contém o projeto de análise e classificação de dados clínicos para predição de diabetes, utilizando técnicas de Machine Learning e otimização de hiperparâmetros.

## 📄 Sobre o projeto

O objetivo deste projeto é desenvolver modelos de aprendizado de máquina capazes de prever se um paciente possui diabetes com base em medidas diagnósticas.

O projeto utiliza o dataset **Pima Indians Diabetes**, originalmente do National Institute of Diabetes and Digestive and Kidney Diseases.

### 🎯 Objetivos específicos
- Realizar análise exploratória dos dados (EDA).
- Pré-processar os dados (tratamento de valores faltantes, normalização).
- Implementar e comparar algoritmos de classificação:
    - **Support Vector Machine (SVM)**
    - **Multi-Layer Perceptron (MLP)**
- Otimizar hiperparâmetros utilizando diferentes estratégias:
    - **Grid Search**
    - **Random Search**
    - **Optuna (TPE)**
    - **TPOT (Genetic Algorithm)**

## 📊 Dataset

O conjunto de dados contém 768 registros e 9 atributos (8 preditores e 1 alvo).

- **Fonte:** [Kaggle - Pima Indians Diabetes Database](https://www.kaggle.com/uciml/pima-indians-diabetes-database)
- **Atributos:** Gravidez, Glicose, Pressão Sanguínea, Espessura da Pele, Insulina, IMC, Função Pedigree Diabetes, Idade, Outcome (0 ou 1).

## 🛠️ Tecnologias utilizadas

O projeto foi desenvolvido em **Python** utilizando Jupyter Notebook. As principais bibliotecas são:

- **Pandas** & **Numpy**: Manipulação e análise de dados.
- **Matplotlib** & **Seaborn**: Visualização de dados.
- **Scikit-Learn**: Construção de modelos de ML e métricas.
- **Optuna** & **TPOT**: Otimização de hiperparâmetros e AutoML.

## 🚀 Como executar

### Pré-requisitos
Certifique-se de ter o Python instalado.

### Instalação

1. Clone o repositório:
   ```bash
   git clone https://github.com/IagoraNz/TC-Diabetes.git
   cd TC-Diabetes
   ```

2. Instale as dependências (exemplo):
   ```bash
   pip install pandas numpy scikit-learn matplotlib seaborn optuna tpot
   ```

3. Execute o Jupyter Notebook:
   ```bash
   jupyter notebook main.ipynb
   ```

## 📈 Resultados

Os modelos foram avaliados utilizando validação cruzada. Abaixo um resumo dos melhores resultados obtidos (baseado na métrica ROC AUC e Acurácia):

| Modelo | Estratégia | Acurácia (Teste) | F1-Score | ROC AUC |
| :--- | :--- | :---: | :---: | :---: |
| **SVM** | GridSearch | 73.59% | 0.5611 | **0.8325** |
| **SVM** | TPOT (Genetic) | **75.32%** | **0.6587** | 0.8347 |
| **MLP** | GridSearch | 74.89% | 0.6375 | **0.8410** |
| **MLP** | Optuna (TPE) | **75.32%** | 0.6275 | 0.8042 |

> **Observação:** Os resultados completos comparando todas as estratégias podem ser encontrados no arquivo `resumo_resultados.csv`. O modelo MLP com GridSearch apresentou um excelente equilíbrio entre as métricas, destacando-se no ROC AUC.

## 📂 Estrutura do repositório

```
📂TC-Diabetes/
├── 📂 figs/               # Figuras e gráficos gerados
├── 📂 models/             # Modelos treinados salvos
├── 🐍 main.ipynb          # Notebook principal com o código
├── 📄 resumo_resultados.csv # Tabela comparativa de resultados
└── � README.md           # Documentação do projeto
```

## 📝 Licença

Este projeto está sob a licença MIT.
