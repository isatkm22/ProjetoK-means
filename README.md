# **Implementação e Análise do Algoritmo de K-means com o Dataset Human Activity Recognition**

# Análise de Atividades Humanas com K-means

## Descrição do Projeto
Este projeto aplica o algoritmo de agrupamento **K-means** para analisar o conjunto de dados de *Human Activity Recognition* (HAR). A análise explora padrões em dados de sensores para identificar diferentes tipos de atividades humanas, como caminhada, corrida e repouso.

O objetivo principal é agrupar as atividades de forma não supervisionada, avaliando a eficácia do K-means na descoberta de padrões naturais no dataset.

---

## Estrutura do Projeto

### 1. Análise Exploratória
Realizamos uma análise inicial dos dados, utilizando:
- Visualizações das distribuições das variáveis.
- Análise de correlação para identificar variáveis relevantes.
- Redução de dimensionalidade com PCA para facilitar a interpretação visual dos agrupamentos.

### 2. Implementação do Algoritmo de K-means
O algoritmo de K-means foi configurado para:
- Selecionar os centróides iniciais utilizando o método **K-means++**.
- Determinar o número ideal de clusters (\( k \)) utilizando técnicas como o **método do cotovelo** e **pontuação de Silhouette**.

### 3. Otimização e Ajustes
-  As variáveis foram padronizadas para garantir escalas equilibradas.
-  O K-means foi executado múltiplas vezes para verificar a consistência dos clusters formados.
-  Métricas como Silhouette Score foram analisadas para avaliar a estabilidade dos agrupamentos.


---

## Estrutura dos Dados
O conjunto de dados inclui 561 variáveis derivadas de sensores de aceleração e giroscópio. Entre as variáveis principais:

- `tBodyAcc-mean()-X`: Média da aceleração do corpo no eixo X.
- `tBodyAcc-std()-Y`: Desvio padrão da aceleração do corpo no eixo Y.
- `tBodyGyro-mean()-Z`: Média da velocidade angular no eixo Z.
- `tGravityAccMag-mean()`: Aceleração média devido à gravidade.

Os dados foram normalizados e reduzidos dimensionalmente com PCA para facilitar o agrupamento.

---

## Instalação e Requisitos

### Bibliotecas Necessárias
Certifique-se de ter as seguintes bibliotecas instaladas:
```bash
pip install pandas numpy matplotlib seaborn scikit-learn

git clone https://github.com/https://github.com/isatkm22/ProjetoK-means/projeto_human_activity_kmeans.git
cd ProjetoK-means
python main.py
```



