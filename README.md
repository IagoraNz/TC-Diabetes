# 🩺 TC-Diabetes

## 📘 Descrição

Este projeto tem como objetivo explorar dados sobre diabetes, treinando modelos de machine learning para prever e classificar diferentes tipos de diabetes ou riscos associados. O repositório contém notebooks, modelos treinados, figuras e resumo dos resultados.

Principais componentes:

- Um **notebook principal** (`main.ipynb`) com o fluxo completo de análise de dados, engenharia de features, treinamento e avaliação de modelos.  
- Pasta `models/` com os modelos treinados salvos.  
- Pasta `figs/` com figuras e gráficos gerados durante a análise.  
- Um arquivo `resumo_resultados.csv`, com as métricas e comparações dos modelos.

## 🚀 Funcionalidades

- 🚧 Pré-processamento de dados (limpeza, tratamento de valores faltantes, normalização, etc.)  
- 📊 Análise exploratória de dados 
- 🤖 Treinamento de modelos de machine learning para classificação  
- 📈 Avaliação de modelos
- 📚 Salvamento de modelos para reuso  

## 🧪 Tecnologias e ferramentas

- **Python** (principal linguagem)  
- **Jupyter Notebook** para experimentação interativa  
- Bibliotecas: `pandas`, `numpy`, `scikit-learn`, `matplotlib` / `seaborn`  e outras

## 📂 Estrutura do repositório

```
TC-Diabetes/
├── figs/                  # Pastas com figuras / gráficos
├── models/                # Modelos treinados
├── main.ipynb             # Notebook principal
└── resumo_resultados.csv  # Sumário de métricas e resultados
```

## 💻 Como executar

1. Clone o repositório:

```bash
git clone https://github.com/IagoraNz/TC-Diabetes
```

2. Crie e ative um ambiente virtual (recomendado):

```bash
python -m venv venv
source venv/bin/activate     # no Linux / macOS
venv\Scripts\activate        # no Windows
```

3. Instale as dependências manualmente
4. Execute o notebook
   
```bash
jupyter notebook main.ipynb
```
