# PROJETO FINAL DE MACHINE LEARNING II
---
### Integrantes
[José P. Marchezi](https://github.com/zemarchezi)

[Zibia Cunha](https://github.com/zibia-cunha)

[Manuela Sodré](https://github.com/ManuSodre)

[Jaqueline Zanão](https://github.com/Jaquerida)


## Objetivos
O objetivo principal deste projeto é avaliar o conjunto de dados sob três perspectivas, utilizando ferramentas de análise e ciência de dados:

1. **Análise Exploratória de Dados**:
   - Entender as características do dataset.
   - Identificar tendências, correlações e outliers.

2. **Análise de Segmentação**:
   - Identificar grupos ou clusters dentro do dataset.
   - Associar padrões comportamentais a variáveis específicas.

3. **Análise Preditiva**:
   - Construir modelos para prever os casos de dengue.
   - Testar diferentes abordagens de aprendizado de máquina e séries temporais.

## Conjunto de Dados
- **Fonte**: [DengAI Dataset - Kaggle](https://www.kaggle.com/datasets/qianyigang129/dengai-dataset)
- Este dataset contém informações climáticas e epidemiológicas para prever os casos de dengue em duas cidades: **Iquitos** (Peru) e **San Juan** (Porto Rico).

---

## Estrutura do Projeto

### 1. Análise Exploratória de Dados (EDA)
- **Descrição Geral**:
  - Inspeção inicial do dataset: dimensões, colunas e tipos de dados.
  - Tratamento de valores ausentes e análise estatística.
- **Visualizações**:
  - Gráficos de tendências temporais para os casos de dengue.
  - Correlações entre variáveis climáticas e número de casos.

### 2. Análise de Segmentação
- **Métodos Utilizados**:
  - Agrupamento utilizando K-Means.
  - Redução de dimensionalidade com PCA para visualização.
- **Resultados**:
  - Identificação de clusters baseados em padrões climáticos e características específicas de cada cidade.

### 3. Análise Preditiva
- **Modelos Treinados**:
  - Ridge e Lasso Regression.
  - XGBoost para padrões não lineares.
- **Previsão Mensal**:
  - Construção de variáveis de defasagem para prever casos futuros.
  - Comparação das séries reais e previstas.

---

## Resultados

### Modelos e Métricas
- **Ridge Regression**: 
  - RMSE: 51.288261
  - R²: 0.180565
- **Lasso Regression**:
  - RMSE: 51.672851  
  - R²: 0.168230
- **XGBoost**:
  - RMSE: 28.673578  
  - R²: 0.743881

### Observações
1. A análise exploratória revelou que a sazonalidade desempenha um papel importante na variação dos casos de dengue.
2. A análise de segmentação destacou diferenças entre as cidades e permitiu identificar padrões únicos.
3. Os modelos preditivos capturaram bem as tendências gerais, mas tiveram dificuldades nos picos extremos de casos.

---

## Conclusões e Próximos Passos

### Conclusões
- O XGBoost foi o modelo mais eficiente para prever os casos de dengue.
- A previsão mensal mostrou boa aderência geral, mas com desvios nos valores extremos.

### Próximos Passos
1. Explorar técnicas de séries temporais, como ARIMA ou Prophet.
2. Aumentar a complexidade dos modelos preditivos com aprendizado profundo.
3. Adicionar variáveis explicativas adicionais, como índices de vulnerabilidade ou alertas climáticos.
