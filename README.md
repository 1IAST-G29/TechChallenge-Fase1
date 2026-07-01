# 🚀 TechChallenge - Fase 1

## 🎯 Objetivo do projeto

Este projeto tem como objetivo analisar e modelar a base de dados do desafio NPS, entendendo os principais padrões e gerando um modelo preditivo capaz de suportar decisões com base nos dados disponíveis.

## 📊 Descrição da base de dados

- Arquivo: `data/desafio_nps_fase_1.csv`
- Formato: CSV
- Conteúdo: registros relacionados ao desafio NPS, com informações de clientes, atributos de comportamento e variáveis que permitem investigar a nota NPS e possíveis drivers do resultado.

## 🧪 Metodologia utilizada

- 🔎 Análise exploratória de dados (EDA) para identificar distribuição, outliers e dados faltantes.
- 🧹 Pré-processamento com tratamento de valores ausentes, codificação de variáveis categóricas e preparação de features.
- 🤖 Construção e validação de modelos de machine learning usando técnicas como validação cruzada para garantir resultados robustos.
- 📈 Avaliação do desempenho com métricas adequadas ao problema e análise da importância das features.

## ▶️ Como reproduzir os resultados

1. Crie e ative um ambiente virtual:

```bash
python3 -m venv .venv
source .venv/bin/activate
```

2. Instale as dependências:

```bash
pip install -r requirements.txt
```

3. Abra e execute o notebook principal:

```bash
jupyter lab
# ou
jupyter notebook
```

4. No notebook `notebooks/tech-challenge.ipynb`, execute as células na ordem para reproduzir a análise, o pré-processamento e o treinamento dos modelos.

> Caso exista um script adicional como `main.py`, ele também pode ser usado para rodar o pipeline automaticamente.

## 📁 Estrutura do repositório

- `data/` — dados de entrada (`desafio_nps_fase_1.csv`)
- `notebooks/tech-challenge.ipynb` — notebook principal com a análise e os modelos
- `models/` — pasta para modelos treinados
- `requirements.txt` — dependências do projeto

