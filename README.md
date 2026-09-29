# projeto-aplicado-4
Produto Analítico de Séries Temporais para Previsão do Mercado de Trabalho (ODS 8) - Ciência de Dados Mackenzie
# 📈 Produto Analítico de Séries Temporais: Previsão do Mercado de Trabalho (ODS 8)

**Curso:** Ciência de Dados (EaD) - Universidade Presbiteriana Mackenzie  
**Componente Curricular:** PROJETO APLICADO IV (2026/02)  
**Autor:** Rafael Tapigliani Rodrigues  

---

## 🎯 Objetivo e Contexto
Este projeto tem como objetivo desenvolver um produto analítico baseado em modelos estatísticos e de aprendizado de máquina para a previsão e análise de séries temporais do mercado de trabalho brasileiro (taxas de desocupação e informalidade), com foco nas Regiões Metropolitanas.

O projeto vincula-se diretamente ao **ODS 8 (Trabalho Decente e Crescimento Econômico)** da ONU, fornecendo subsídios quantitativos para o acompanhamento de indicadores socioeconômicos.

---

## 📊 Fonte de Dados
Os dados primários são extraídos diretamente das APIs oficiais:
* **IBGE - PNAD Contínua:** Taxas de desocupação e informalidade por trimestre/mês (API SIDRA).
* **Banco Central do Brasil (SGS):** Indicadores macroeconômicos exógenos (IPCA, Taxa Selic).

---

## ⚙️ Arquitetura do Pipeline
1. **Ingestão:** Extração automatizada via scripts em Python.
2. **Pré-processamento:** Decomposição temporal, tratamento de ausentes e testes de estacionariedade (ADF / KPSS).
3. **Engenharia de Features:** Criação de *lags* temporais, médias móveis e variáveis exógenas.
4. **Modelagem:** Comparação entre modelo estatístico *benchmark* (**SARIMAX**) e algoritmos de *Machine Learning* (**XGBoost / LightGBM**).
5. **Avaliação:** Validação cruzada por janela expandida (*Expanding Window Cross-Validation*) e métricas MAE, RMSE e MAPE.

---

## 📅 Cronograma de Entregas
* **Etapa 1 (31/08):** Definição do Projeto e Equipe *(Concluído)*
* **Etapa 2 (28/09):** Referencial Teórico, Pipeline e Cronograma *(Concluído)*
* **Etapa 3 (26/10):** Análise Exploratória, Pré-processamento e Modelo Base *(A realizar)*
* **Etapa 4 (30/11):** Implementação Final, Repositório e Apresentação em Vídeo *(A realizar)*

---

## 🛠️ Tecnologias Utilizadas
* **Linguagem:** Python 3.11+
* **Manipulação e Análise:** Pandas, NumPy
* **Modelagem Temporal:** Statsmodels, Prophet, XGBoost, LightGBM
* **Visualização:** Matplotlib, Seaborn, Plotly
