# 📊 Previsão de Estoque Inteligente na AWS com [SageMaker Canvas](https://aws.amazon.com/pt/sagemaker/canvas/)

Bem-vindo ao desafio de projeto "Previsão de Estoque Inteligente na AWS com SageMaker Canvas. Neste Lab DIO, você aprenderá a usar o SageMaker Canvas para criar previsões de estoque baseadas em Machine Learning (ML). Siga os passos abaixo para completar o desafio!
Antes de começar, certifique-se de ter uma conta na AWS. Se precisar de ajuda para criar sua conta, confira nosso repositório [AWS Cloud Quickstart](https://github.com/digitalinnovationone/aws-cloud-quickstart).

##  Relatório de Projeto de Machine Learning com AWS SageMaker Canvas

## 🎯 Introdução
Olá! Este é o relatório do meu projeto de Machine Learning utilizando a plataforma AWS SageMaker Canvas, que permite criar modelos de aprendizado de máquina sem a necessidade de codificação. O objetivo deste projeto foi prever a demanda de produtos em estoque com base em um conjunto de dados fornecido.

### 1. Selecionando Dataset

Descrição do Conjunto de Dados
O conjunto de dados utilizado contém 243.000 células (6 x 40.500) com as seguintes colunas:

item_id: Identificação do produto
Location: Localização
time_stamp: Data
demand: Demanda do produto
price: Preço do produto
Product_category: Categoria do produto

### 2. Treinando dataset

Análise das Métricas de Performance
Após o treinamento do modelo, as métricas de performance foram as seguintes:

Métrica de otimização (accuracy): 98.173%
Média do F1 Score: 98.168%
Média de precisão (precision): 98.237%
Média de recall: 98.173%
Perda de validação (validation loss): 0.079
Colunas mais influentes
price: 33.379%
product_category: 32.924%
demand: 22.816%
time_stamp: 10.484%
location: 0.197%
Previsão
Utilizei o modelo treinado para prever a demanda de estoque. Abaixo, seguem as principais observações a partir das previsões geradas.

Impacto do preço na previsão de item_id

### 3. Analisar

-   Após o treinamento, examine as métricas de performance do modelo.
-   Verifique as principais características que influenciam as previsões.
-   Faça ajustes no modelo se necessário e re-treine até obter um desempenho satisfatório.

### 4. Prever

Predições vs. Valores Reais
Conclusões e Insights
Impacto do Preço: Conforme observado, o preço tem uma influência significativa nas previsões, sendo a característica mais importante para o modelo.
Desempenho do Modelo: O modelo mostrou um desempenho excelente com uma precisão média superior a 98%. Isso indica que o modelo é altamente confiável para fazer previsões de demanda de estoque.
Distribuição das Predições: A visualização das predições versus os valores reais mostra que o modelo conseguiu mapear corretamente a maioria das classes de item_id, com poucas discrepâncias.

