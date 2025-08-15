# 🤖 Detecção de Patologias Cardíacas com Aprendizado de Máquina

## 🎯Sobre esse repositório

Este repositório foi criado para armazenar a solução do projeto final, escrito em Python, para a disciplinade de **Aprendizado de Máquina**, cursada durante o **Mestrado (Programa de Pós-graduação em Ciência da Computação - PPGCC)** na **Universidade Federal de São Carlos (UFSCar)** em 2024/2.

É um estudo para a detecção de patologias cardíacas em pacientes pediátricos utilizando técnicas de aprendizado de máquina. O principal objetivo é avaliar a eficácia de diferentes algoritmos na classificação de pacientes saudáveis e com doenças cardíacas, a partir de dados reais.

## 🏥 Fonte dos Dados

Os dados utilizados neste projeto foram coletados no Real Hospital Português (RHP), localizado no Brasil, em parceria com a Universidade do Porto. A base de dados principal (`RHP_data.csv`) contém informações clínicas dos pacientes, como peso, altura, IMC, frequência cardíaca, entre outros.

## 🛠️ Metodologia Aplicada

O projeto foi estruturado em etapas de pré-processamento dos dados, aplicação de diversos modelos de classificação e avaliação de performance.

### 🧹 Pré-processamento de Dados

Uma análise exploratória foi realizada para tratar inconsistências nos dados. As principais etapas incluem:

- Tratamento de Valores Nulos: Substituição de valores ausentes pela mediana ou moda da respectiva coluna;

- Tratamento de Valores Negativos e Zerados: Correção de registros inválidos (ex: peso negativo);

- Cálculo de Features: O IMC (Índice de Massa Corporal) foi calculado a partir do peso e altura para preencher valores faltantes;

- Limpezado de Dados Categóricos: Padronização de categorias (ex: "Normal" e "Normais" para a classe alvo) e mapeamento para valores numéricos;

- Remoção de Features: Colunas com grande quantidade de dados faltantes ou sem relevância para o modelo;

- Tratamento de Outliers: Identificação e tratamento de valores atípicos.

### 🤖 Modelos de Aprendizado de Máquina utilizados

Foram implementados e avaliados os seguintes algoritmos de classificação:

- K-Nearest Neighbors (KNN);

- Naive Bayes (NB);

- Regressão Logística (RL);

- Redes Neurais Artificiais (RNA);

- Máquina de Vetores de Suporte (SVM);

- Algoritmos adicionais: Random Forest e Gradient Boosting Classifier.

A implementação foi realizada em Python, utilizando a biblioteca Scikit-learn.

### 📊 Métricas de Avaliação

O desempenho dos modelos foi avaliado utilizando as seguintes métricas:

- AUC (Área Sob a Curva ROC) - Métrica principal da análise;

- Acurácia;

- Precisão;

- Recall;

- F1-Score.