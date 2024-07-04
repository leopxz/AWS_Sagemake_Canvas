# 📊 Previsão de Estoque Inteligente na AWS com [SageMaker Canvas](https://aws.amazon.com/pt/sagemaker/canvas/)

Bem-vindo ao desafio de projeto "Previsão de Estoque Inteligente na AWS com SageMaker Canvas. Neste Lab DIO, você aprenderá a usar o SageMaker Canvas para criar previsões de estoque baseadas em Machine Learning (ML). Siga os passos abaixo para completar o desafio!
Antes de começar, certifique-se de ter uma conta na AWS. Se precisar de ajuda para criar sua conta, confira nosso repositório [AWS Cloud Quickstart](https://github.com/digitalinnovationone/aws-cloud-quickstart).

##  Relatório de Projeto de Machine Learning com AWS SageMaker Canvas

**Introdução**

Olá, este é o relatório do meu projeto de Machine Learning utilizando a plataforma AWS SageMaker Canvas, que permite criar modelos de aprendizado de máquina sem a necessidade de codificação. O objetivo deste projeto foi prever a demanda de produtos em estoque com base em um conjunto de dados fornecido.

### 1. Selecionando Dataset

**Descrição do Conjunto de Dados**
O conjunto de dados utilizado contém 243.000 células (6 x 40.500) com as seguintes colunas:

**item_id:** Identificação do produto<br>
**Location:** Localização<br>
**time_stamp:** Data<br>
**demand:** Demanda do produto<br>
**price:** Preço do produto<br>
**Product_category:** Categoria do produto<br>

### 2. Treinando dataset

**Análise das Métricas de Performance**
Após o treinamento do modelo, as métricas de performance foram as seguintes:

**Métrica de otimização (accuracy):** 98.173%.<br>
**Média do F1 Score:** 98.168%.<br>
**Média de precisão (precision):** 98.237%.<br>
**Média de recall:** 98.173%.<br>
**Perda de validação (validation loss):** 0.079.<br>

**Colunas mais influentes:**
**price:** 33.379%.<br>
**product_category:** 32.924%.<br>
**demand:** 22.816%.<br>
**time_stamp:** 10.484%.<br>
**location:** 0.197%.<br>

### 4. Prevendo valores

**Previsão:**
Utilizei o modelo treinado para prever a demanda de estoque. Abaixo, seguem as principais observações a partir das previsões geradas.<br>
Impacto do preço na previsão de item_id
**Predições vs. Valores Reais**
FOTO AQUI
**Conclusões e Insights:**
**Impacto do Preço:** Conforme observado, o preço tem uma influência significativa nas previsões, sendo a característica mais importante para o modelo.<br>
<br>**Desempenho do Modelo:** O modelo mostrou um desempenho excelente com uma precisão média superior a 98%. Isso indica que o modelo é altamente confiável para fazer previsões de demanda de estoque.<br>
<br>**Distribuição das Predições:** A visualização das predições versus os valores reais mostra que o modelo conseguiu mapear corretamente a maioria das classes de item_id, com poucas discrepâncias.<br>

