# AED — Uber Ride Analytics (SCTEC)

![Python](https://img.shields.io/badge/Python-3.x-blue)
![Data Analysis](https://img.shields.io/badge/Data-Analysis-green)
![Machine Learning](https://img.shields.io/badge/AI-Foundations-purple)
![Azure](https://img.shields.io/badge/Cloud-Azure-informational)
![EDA](https://img.shields.io/badge/EDA-Exploratory%20Analysis-orange)
![AI Ready](https://img.shields.io/badge/AI-Ready-purple)


Este projeto contém uma **Análise Exploratória de Dados (AED)** desenvolvida em Python para o desafio prático extra do curso **Introdução à Inteligência Artificial (SCTEC / LAB365)**.  
O objetivo é compreender padrões de utilização do serviço (variações temporais, características das corridas, status e cancelamentos), além de organizar uma base que possa ser utilizada futuramente em tarefas introdutórias de **IA** (classificação/regressão).

## Dataset
- Fonte: Kaggle — **“uber-ride-analytics-dashboard”**  
- Arquivo utilizado localmente: `ncr_ride_bookings.csv`  
- Observação: mantenha o CSV na mesma pasta do notebook (ou ajuste o caminho no `pd.read_csv`).

## O que foi analisado (visão geral)
O notebook percorre um fluxo completo de AED:

1. **Carregamento e entendimento inicial**
   - Dimensões do dataset, colunas, tipos, estatísticas descritivas e valores ausentes.
2. **Engenharia de variáveis temporais**
   - Criação de `datetime` (junção de `Date` + `Time`)
   - Extração de `hour`, `day_of_week` e `month`
3. **Análises e visualizações**
   - Volume de corridas por **hora** e por **dia da semana**
   - Distribuição por **tipo de veículo**
   - **Valor médio** por tipo de veículo
   - Distribuição de **status** (incluindo cancelamentos)
   - Distribuição de **ratings** de motoristas
4. **EDA avançado (cruzamentos)**
   - Heatmap **Dia da Semana x Hora** para identificar picos de demanda
   - Status das corridas por **tipo de veículo** (comparação direta)
   - Relação entre **distância** e **valor** (scatter), útil para pensar em regressão

## Possíveis aplicações futuras em IA
A partir das variáveis existentes (tempo, distância, valor, status, ratings, tipo de veículo), algumas aplicações introdutórias possíveis são:
- **Previsão de demanda** por horário/dia (regressão ou séries temporais simples)
- **Classificação de cancelamento** (prever se uma corrida tende a ser cancelada)
- **Modelos de preço** (estimar `Booking Value` com base em distância, tempo e categoria)

## Requisitos
Bibliotecas utilizadas no notebook:
- `pandas`
- `numpy`
- `matplotlib`
- `seaborn`

Instalação (recomendado em ambiente virtual):
```bash
pip install pandas numpy matplotlib seaborn
```

## Como executar
1. Baixe/coloque o arquivo `ncr_ride_bookings.csv` na mesma pasta do notebook.
2. Abra o notebook `Aed_Uber.ipynb` no Jupyter/VS Code/Colab.
3. Execute as células em ordem (Kernel → Restart & Run All).

## Estrutura sugerida para entrega (.zip/.rar)
Para a submissão no SCTEC, compacte em **um único .zip/.rar** contendo, no mínimo:
- `Aed_Uber.ipynb`
- `ncr_ride_bookings.csv`
- `README.md`

Opcional (mas recomendado):
- pasta `outputs/` com imagens exportadas dos gráficos (caso você salve figuras)

## Autor

**Márcio Luiz**

🔗 [LinkedIn](https://www.linkedin.com/in/marcioluiz-br/)  
💻 [GitHub](https://github.com/MarcioLuizBR)

