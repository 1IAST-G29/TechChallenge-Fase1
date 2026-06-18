# 🚀 TechChallenge - Fase 1

## 🎯 Objetivo

O objetivo deste projeto é analisar e modelar os dados do desafio NPS (Net Promoter Score) fornecido, explorando a base, pré-processando os dados, treinando modelos de machine learning e reportando resultados reprodutíveis que permitam inferir fatores relacionados ao NPS ou prever a variável-alvo proposta no desafio. 🔍📈

## 🗂️ Descrição da base de dados

- 📁 Arquivo: `data/desafio_nps_fase_1.csv`
- 🧾 Formato: CSV (valores separados por vírgula)
- 📝 Conteúdo: registros relacionados ao desafio NPS — tipicamente contendo informações de clientes, respostas a pesquisas, notas NPS e possíveis variáveis demográficas ou transacionais. Consulte o notebook para inspeção detalhada das colunas e amostras.

> Observação: antes de executar qualquer pipeline, verifique o cabeçalho do CSV (ex.: `head -n 5 data/desafio_nps_fase_1.csv`) para confirmar nomes e tipos de colunas.

## 🛠️ Metodologia utilizada

1. 🔎 Análise exploratória (EDA)
	- Inspeção de valores faltantes, distribuição das variáveis e análises gráficas para entender padrões e outliers.

2. 🧹 Pré-processamento
	- Tratamento de valores faltantes, codificação de variáveis categóricas, normalização/ padronização quando necessário e engenharia de features.

3. ✂️ Seleção de features
	- Avaliação de correlações, importância de variáveis por modelos e técnicas de seleção (ex.: Recursive Feature Elimination).

4. 🤖 Treinamento de modelos
	- Modelos de exemplo: RandomForest, XGBoost, Logistic Regression/Gradient Boosting (dependendo do tipo de problema: regressão ou classificação).
	- Uso de validação cruzada (k-fold) para estimativas robustas de desempenho.

5. 📊 Avaliação
	- Métricas conforme o tipo de tarefa: AUC, Accuracy, F1-score para classificação; RMSE/MAE para regressão.

6. 🧠 Interpretação
	- Análise de importância de variáveis e interpretações qualitativas para suportar conclusões acionáveis.

Observação: a implementação concreta e os hiperparâmetros estão descritos e executáveis no notebook `notebooks/tech-challenge.ipynb`.

## ⚙️ Como reproduzir os resultados

1. Preparar o ambiente (recomendado: Python 3.8+)

```bash

# Criar e ativar ambiente virtual (macOS/Linux)
python3 -m venv .venv
source .venv/bin/activate

# Instalar dependências: use o arquivo requirements.txt (dentro do venv)
pip install -r requirements.txt

# Alternativa: se o projeto usa Poetry
# poetry install
```

2. 🗃️ Estrutura esperada

- `main.py` — script principal (se presente) para rodar pipelines/experimentos.
- `notebooks/tech-challenge.ipynb` — notebook com EDA, pré-processamento, treino e avaliação.
- `data/desafio_nps_fase_1.csv` — base de dados usada pelo notebook e scripts.

3. Executar o notebook (recomendado para reproduzir exatamente os passos)

```bash
# Iniciar JupyterLab/Notebook e abrir o notebook
jupyter lab
# ou
jupyter notebook

# No Jupyter, execute as células do notebook `notebooks/tech-challenge.ipynb` na ordem.
```

4. Executar scripts (se aplicável)

```bash
# Exemplo: rodar pipeline via script (se implementado)
python main.py
```

5. 🧾 Notas sobre reprodutibilidade

- Certifique-se de usar as mesmas versões de pacotes (considere usar um arquivo `requirements.txt` ou `poetry.lock`).
- Defina seeds para geração pseudo-aleatória quando necessário (ex.: `numpy`, `random`, `scikit-learn`).
- Para executar experimentos mais pesados, use o notebook em uma máquina com recursos adequados ou ajuste hiperparâmetros e tamanho de amostra.

## 📁 Estrutura do repositório

- `main.py` — (opcional) runner para pipelines.
- `notebooks/tech-challenge.ipynb` — notebook principal com análise e modelos.
- `data/` — dados brutos (`desafio_nps_fase_1.csv`).
- `models/` — local sugerido para salvar modelos treinados.

## ✉️ Contato

Para dúvidas ou contribuições, abra uma issue neste repositório ou entre em contato com o autor do projeto. 👍

---
Arquivo atualizado automaticamente pelo assistente. Para ajustes, edite este `README.md`.

