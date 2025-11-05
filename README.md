# 🏡 Previsão de Preços de Imóveis: EDA e Regressão

## Visão Geral do Projeto
Este projeto tem como objetivo principal prever o preço de venda de imóveis usando o dataset House Prices. O processo abrange desde a análise inicial dos dados até a implementação de um modelo preditivo.

## 🛠️ Metodologia e Pipeline de Data Science

1.  **Análise Exploratória de Dados (EDA):**
    * Análise da distribuição da variável alvo (`SalePrice`) e aplicação de **transformação logarítmica** para normalização.
    * Identificação e tratamento de **outliers** (pontos atípicos na relação Preço vs. Área).
    * Cálculo e visualização da **matriz de correlação** para selecionar as *features* mais importantes (`OverallQual`, `GrLivArea`, etc.).

2.  **Pré-processamento e Feature Engineering:**
    * Tratamento exaustivo de **dados ausentes (NaN)**, substituindo por 'None' em variáveis categóricas e por 0 ou mediana em variáveis numéricas.
    * Aplicação de **One-Hot Encoding** (`pd.get_dummies`) para converter variáveis categóricas em formatos numéricos utilizáveis pelo modelo.

3.  **Modelagem Preditiva:**
    * Implementação do modelo **Regressão Ridge** (ou o modelo que você preferir) para lidar com a alta dimensionalidade das *features* (após One-Hot Encoding).
    * Avaliação do desempenho usando a métrica **Root Mean Squared Error (RMSE)** na escala real de preço.

## 💻 Tecnologias e Bibliotecas

| Categoria | Ferramenta/Biblioteca |
| :--- | :--- |
| **Linguagem** | Python |
| **Manipulação** | Pandas, NumPy |
| **Visualização** | Matplotlib, Seaborn |
| **Modelagem** | Scikit-learn (Ridge) |
| **Controle de Versão** | Git & GitHub |

## 🔗 Como Abrir o Notebook

O projeto principal está no arquivo `[NomeDoSeuNotebook.ipynb]`. Você pode visualizá-lo diretamente no GitHub ou baixá-lo e executá-lo no Jupyter Notebook/Lab ou Google Colab.
