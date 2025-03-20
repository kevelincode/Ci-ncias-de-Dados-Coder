# Ci-ncias-de-Dados-Coder
Projeto final do curso de Data Science

# README - Análise dos Dados do ENEM 2021

## Introdução
Este projeto tem como objetivo analisar os microdados do ENEM 2021, aplicando técnicas de análise exploratória e aprendizado de máquina para identificar padrões nos desempenhos dos candidatos. Além disso, foi realizada uma redução de dimensionalidade com PCA e testes com modelos preditivos.

---

## 1. Carregamento e Limpeza dos Dados
### 1.1 Carregamento dos Dados
Os microdados do ENEM 2021 foram carregados a partir de um arquivo CSV de grande porte. Para otimizar a leitura e processamento, utilizamos a biblioteca Pandas e especificamos as colunas de interesse.

### 1.2 Tratamento de Valores Ausentes
Foram identificados e tratados valores ausentes nas colunas de interesse. Estratégias como preenchimento com valores médios ou remoção de linhas específicas foram adotadas conforme a relevância dos dados.

### 1.3 Codificação de Variáveis Categóricas
Variáveis categóricas foram transformadas em numéricas utilizando técnicas como one-hot encoding e label encoding, possibilitando sua utilização em modelos estatísticos e de machine learning.

---

## 2. Análise Exploratória
A análise exploratória envolveu a geração de diversas estatísticas descritivas e visualizações para melhor compreensão dos dados.

### 2.1 Distribuição das Notas por Matéria
Foram gerados histogramas para visualizar a distribuição das notas em Linguagens, Matemática, Ciências da Natureza e Ciências Humanas. 

- As notas tendem a seguir distribuições assimétricas com concentração na faixa intermediária.
- Matemática apresentou uma distribuição mais dispersa, indicando maior variação no desempenho.
- Linguagens mostrou um leve viés à esquerda, com mais candidatos abaixo da média.

### 2.2 Correlação entre as Notas
A matriz de correlação foi utilizada para identificar relações entre as disciplinas.

- Forte correlação entre Matemática e Ciências da Natureza.
- Correlação moderada entre Linguagens e Ciências Humanas.

### 2.3 Análise por Região e Tipo de Escola
Boxplots foram utilizados para comparar as notas entre diferentes regiões e entre escolas públicas e privadas.

- Candidatos de escolas privadas apresentaram melhor desempenho.
- O Sudeste teve as maiores notas medianas, enquanto Norte e Nordeste apresentaram distribuições mais baixas.

---

## 3. Redução de Dimensionalidade (PCA)
### 3.1 Aplicação do PCA
A técnica de Análise de Componentes Principais (PCA) foi aplicada para reduzir a dimensionalidade dos dados mantendo a maior variabilidade possível.

- As duas primeiras componentes explicam aproximadamente 70% da variabilidade total.
- A distribuição dos candidatos no espaço de PCA indicou que poucos componentes são suficientes para resumir o desempenho geral.

---

## 4. Modelagem Preditiva
### 4.1 Seleção de Modelos
Foram testados diferentes modelos de aprendizado de máquina para prever a nota final dos candidatos com base em variáveis socioeconômicas e desempenho nas provas.

### 4.2 Modelos Avaliados
- **Regressão Linear**: Modelo simples, mas com baixa capacidade de capturar relações complexas.
- **Random Forest**: Melhor desempenho, com menor erro médio absoluto.
- **XGBoost**: Bom desempenho, porém com maior tempo de processamento.

---

## 5. Conclusão
A análise dos microdados do ENEM 2021 permitiu identificar padrões importantes no desempenho dos candidatos, especialmente em relação a fatores socioeconômicos e tipo de escola. Os modelos preditivos testados mostraram que é possível estimar a nota com boa precisão, especialmente ao utilizar modelos de aprendizado de máquina como Random Forest.

### 5.1 Próximos Passos
- Expandir a análise incluindo dados de anos anteriores para identificar tendências.
- Explorar novas técnicas de engenharia de atributos para melhorar a precisão dos modelos.
- Aplicar técnicas mais avançadas de visualização para uma melhor interpretação dos dados.




---
Projeto desenvolvido para fins acadêmicos e exploratórios.

