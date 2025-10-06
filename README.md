# Previsão de Séries Temporais: Prophet vs LSTM

Comparação de modelos de previsão aplicados a dados de vendas da Superstore.

## Acesso Rápido

**Abrir no Google Colab:** [Clique aqui](https://colab.research.google.com/drive/1YgnZbjE6TiHyIiJsTlcr3CygqGBqhsmc?usp=sharing)

## Sobre o Projeto

Este notebook implementa e compara dois modelos de previsão de séries temporais:

- **Prophet:** Modelo do Facebook para forecasting com sazonalidade
- **LSTM:** Rede neural recorrente para capturar dependências temporais

## Dataset

**Fonte:** [Superstore Sales - Kaggle](https://www.kaggle.com/datasets/vivek468/superstore-dataset-final)

Dados de vendas entre 2015-2018 agregados diariamente.

## Resultados

| Modelo | RMSE | MAE |
|--------|------|-----|
| Prophet | 2453.47 | 1759.82 |
| LSTM | 2436.56 | 1717.77 |

O LSTM apresentou desempenho ligeiramente superior (0.7% de diferença).

## Métricas Utilizadas

- **RMSE:** Penaliza erros grandes, importante para evitar subestimação de demanda
- **MAE:** Interpretável em dólares, representa erro médio absoluto

**Referência:** Hyndman & Athanasopoulos (2021) - Forecasting: Principles and Practice

## Estrutura do Repositório

```cmd
├── ponderada_predicao_serie_temporal_mauro_das_chagas_junior.ipynb    # Notebook principal
├── train.csv                     # Dataset (baixar do Kaggle)
└── README.md                     # Este arquivo
```

## Como Executar

### Opção 1: Google Colab (Recomendado)

1. Acesse o [notebook no Colab](https://colab.research.google.com/drive/1YgnZbjE6TiHyIiJsTlcr3CygqGBqhsmc?usp=sharing)
2. Faça upload do arquivo `train.csv` no ambiente Colab
3. Execute todas as células

### Opção 2: Local

```bash
# Clone o repositório
git clone https://github.com/seu-usuario/seu-repo.git
cd seu-repo

# Instale as dependências
pip install prophet numpy pandas matplotlib scikit-learn tensorflow

# Baixe o dataset do Kaggle e coloque na pasta raiz
# Execute o notebook
jupyter notebook ponderada_predicao_serie_temporal_mauro_das_chagas_junior.ipynb
```

## Dependências

- Python 3.8+
- prophet
- numpy
- pandas
- matplotlib
- scikit-learn
- tensorflow
