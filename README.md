# 🌾 Projeto de Classificação de Grãos de Trigo com Machine Learning
Este projeto tem como objetivo automatizar o processo de classificação de três variedades de grãos de trigo: Kama, Rosa e Canadian, utilizando técnicas de Machine Learning aplicadas ao Seeds Dataset do UCI Machine Learning Repository.

### 👨‍🎓 Integrantes:

Lais Kurahashi

Davi Ferreira

Lucas Martinelli

### 👩‍🏫 Professores:
**Tutor(a)**
Lucas Gomes Moreira

**Coordenador(a)**
André Godoi Chiovato

## 📌 Objetivos
- Aplicar a metodologia CRISP-DM para desenvolver um modelo preditivo.

- Comparar o desempenho de diferentes algoritmos de classificação.

- Automatizar a classificação que, tradicionalmente, é feita manualmente.

- Otimizar o processo de análise com base em características físicas dos grãos.

## 📁 Dataset
**Fonte:** UCI Machine Learning Repository – Seeds Dataset

- **Classes:** 3 variedades de trigo

- **Atributos:**

    - Área

    - Perímetro

    - Compacidade

    - Comprimento do Núcleo

    - Largura do Núcleo

    - Coeficiente de Assimetria

    - Comprimento do Sulco do Núcleo

    - Amostra (rótulo)

### Assets
A pasta assets contem imagens dos graficos gerados durante os testes dos modelos.

## 🧪 Etapas Realizadas
### 1. Análise Exploratória
- Visualização com histogramas, boxplots e gráficos de dispersão.

- Estatísticas descritivas para entender a distribuição dos atributos.

### 2. Pré-processamento
- Verificação o tratamento de valores ausentes (não havia).

- Aplicação de StandardScaler para normalização dos dados.

### 3. Treinamento de Modelos
Utilizamos três modelos para fins de comparação:

- Naive Bayes

- SVC (Support Vector Machine)

- RandomForestClassifier

- Dividimos os dados em treino (70%) e teste (30%) usando train_test_split.

### 4. Avaliação dos Modelos
- Avaliação por métricas: Acurácia, Precisão, Recall, F1-Score.

- Geração de relatório de classificação (classification_report).

- Visualização dos resultados em gráficos.

## 📊 Resultados Obtidos
|Modelo	       |Acurácia |Precisão |Recall |F1-Score|
|:-------------|:--------|:--------|:------|:-------|
|Naive Bayes   |88.71%   |89.29%   |87.95% |88.46%  |
|SVM	         |88.71%   |89.23%   |87.95% |88.33%  |
|Random Forest |90.32%   |90.74%   |90.67% |90.56%  |

O modelo Random Forest apresentou melhor desempenho geral e foi considerado o mais apropriado para a classificação automatizada dos grãos.

## 📈 Visualizações
- Histogramas e boxplots para visualização da distribuição dos atributos.

- Gráficos de dispersão para identificar correlações entre características.

- Heatmap da matriz de confusão.

- Gráfico de barras agrupado com as métricas de cada modelo.

## 🛠️ Tecnologias Utilizadas
Python 3.10+

- pandas

- matplotlib

- seaborn

- scikit-learn

- numpy

- Jupyter Notebook

## 💡 Insights Relevantes

**Importância de atributos físicos bem definidos:** A análise exploratória inicial mostrou que características como comprimento do sulco do núcleo e compacidade foram fundamentais para separar bem as variedades — especialmente visíveis nos gráficos de dispersão.

**Aplicabilidade real:** Com base nesses resultados, é possível implementar um modelo automatizado para cooperativas agrícolas que realize a classificação dos grãos com alta precisão, reduzindo erros humanos e tempo de análise.
