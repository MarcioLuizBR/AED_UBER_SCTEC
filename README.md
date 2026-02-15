# AED — Uber Ride Analytics (SCTEC)

![Python](https://img.shields.io/badge/Python-Data%20Analytics-blue)
![Data Analysis](https://img.shields.io/badge/Data-Analysis-green)
![Machine Learning](https://img.shields.io/badge/AI-Foundations-purple)
![Azure](https://img.shields.io/badge/Cloud-Azure-informational)
![EDA](https://img.shields.io/badge/EDA-Exploratory%20Analysis-orange)
![AI Ready](https://img.shields.io/badge/AI-Ready-purple)
![Cloud](https://img.shields.io/badge/Cloud-Azure-informational)

Este projeto apresenta uma **Análise Exploratória de Dados (EDA)** desenvolvida em Python para o desafio prático extra do curso **Introdução à Inteligência Artificial (SCTEC / LAB365)**.

O objetivo é compreender padrões de utilização do serviço de transporte por aplicativo, identificar variações temporais e características relevantes das corridas, além de preparar o dataset para possíveis aplicações futuras em Inteligência Artificial.

---

## Dataset

- Fonte: Kaggle — *uber-ride-analytics-dashboard*
- Arquivo utilizado: `ncr_ride_bookings.csv`
- Contém informações como:

  - Data e horário das corridas
  - Tipo de veículo
  - Valor da corrida
  - Distância percorrida
  - Status (completed, cancelled, etc.)
  - Avaliações de motoristas
  - Métodos de pagamento

---

## Estrutura da Análise

O notebook segue um fluxo estruturado de análise de dados:

1. **Carregamento e entendimento inicial**
   - Inspeção de colunas, tipos de dados e valores ausentes.
2. **Engenharia de variáveis temporais**
   - Criação da coluna `datetime`
   - Extração de `hour`, `day_of_week` e `month`
3. **Análise exploratória**
   - Volume de corridas por horário e dia da semana
   - Distribuição por tipo de veículo
   - Análise de status das corridas
   - Distribuição de avaliações
4. **EDA Avançado**
   - Heatmap temporal (Dia x Hora)
   - Cruzamento status x tipo de veículo
   - Relação distância vs valor (scatterplot)
   - Boxplot comparativo por categoria

---

## Principais Insights

- Horário de pico identificado por volta das **18h**, indicando padrão típico de deslocamento urbano.
- Segunda-feira apresentou maior volume relativo de corridas.
- Distribuição geral dos status:

  - Completed ≈ 62%
  - Cancelled by Driver ≈ 18%
  - No Driver Found ≈ 7%
  - Cancelled by Customer ≈ 7%
  - Incomplete ≈ 6%

- Correlação entre distância e valor próxima de zero, sugerindo influência de outros fatores na precificação.

---

## Possíveis Aplicações em Inteligência Artificial

- Previsão de demanda por horário (modelos de regressão).
- Classificação de cancelamentos.
- Modelos de estimativa de preço.
- Análise preditiva de padrões de mobilidade urbana.

---

## Tecnologias Utilizadas

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn

---

## Como executar

1. Coloque o arquivo `ncr_ride_bookings.csv` na mesma pasta do notebook.
2. Abra o arquivo `Aed_Uber.ipynb` no Jupyter Notebook, VS Code ou Google Colab.
3. Execute as células em ordem.

---

## Estrutura sugerida para entrega (.zip/.rar)

- `Aed_Uber.ipynb`
- `ncr_ride_bookings.csv`
- `README.md`

---

## Autor

Márcio Luiz  

🔗 [LinkedIn](https://www.linkedin.com/in/marcioluiz-br/)  
💻 [GitHub](https://github.com/MarcioLuizBR)

