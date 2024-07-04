# 📊 Previsão de Estoque Inteligente na AWS com [SageMaker Canvas](https://aws.amazon.com/pt/sagemaker/canvas/)

Bem-vindo ao desafio de projeto "Previsão de Estoque Inteligente na AWS com SageMaker Canvas. Neste Lab DIO, você aprenderá a usar o SageMaker Canvas para criar previsões de estoque baseadas em Machine Learning (ML). Siga os passos abaixo para completar o desafio!
Antes de começar, certifique-se de ter uma conta na AWS. Se precisar de ajuda para criar sua conta, confira nosso repositório [AWS Cloud Quickstart](https://github.com/digitalinnovationone/aws-cloud-quickstart).

##  Relatório de Projeto de Machine Learning com AWS SageMaker Canvas

### **Introdução**

Olá, este é o relatório do meu projeto de Machine Learning utilizando a plataforma AWS SageMaker Canvas, que permite criar modelos de aprendizado de máquina sem a necessidade de codificação. O objetivo deste projeto foi prever a demanda de produtos em estoque com base em um conjunto de dados fornecido.

## 1. Selecionando Dataset

### **Descrição do Conjunto de Dados**<br>
O conjunto de dados utilizado contém 243.000 células (6 x 40.500) com as seguintes colunas:

**item_id:** Identificação do produto<br>
**Location:** Localização<br>
**time_stamp:** Data<br>
**demand:** Demanda do produto<br>
**price:** Preço do produto<br>
**Product_category:** Categoria do produto<br>

## 2. Treinando dataset

### **Análise das Métricas de Performance**
Após o treinamento do modelo, as métricas de performance foram as seguintes:

**Métrica de otimização (accuracy):** 98.173%.<br>
**Média do F1 Score:** 98.168%.<br>
**Média de precisão (precision):** 98.237%.<br>
**Média de recall:** 98.173%.<br>
**Perda de validação (validation loss):** 0.079.<br>

**Colunas mais influentes:**<br>
**price:** 33.379%.<br>
**product_category:** 32.924%.<br>
**demand:** 22.816%.<br>
**time_stamp:** 10.484%.<br>
**location:** 0.197%.<br>

## 4. Prevendo valores<br><br>

### **Previsão:**<br>
Utilizei o modelo treinado para prever a demanda de estoque. Abaixo, seguem as principais observações a partir das previsões geradas.<br>
Impacto do preço na previsão de item_id
**Predições vs. Valores Reais**

<br><br>FOTO AQUI<br><br>

**Conclusões e Insights:**<br><br>
**Impacto do Preço:** Conforme observado, o preço tem uma influência significativa nas previsões, sendo a característica mais importante para o modelo.<br>
<br>**Desempenho do Modelo:** O modelo mostrou um desempenho excelente com uma precisão média superior a 98%. Isso indica que o modelo é altamente confiável para fazer previsões de demanda de estoque.<br>
<br>**Distribuição das Predições:** A visualização das predições versus os valores reais mostra que o modelo conseguiu mapear corretamente a maioria das classes de item_id, com poucas discrepâncias.<br><br>

O modelo foi treinado com um conjunto de dados com 243,000 mil (6x40,500) celulas, e utilizei as funcionalidades de análise de métricas de performance e predição de estoque para produtos. Este relatório documenta o processo, as previsões realizadas e as análises resultantes.<br><br>

##Análise dos Resultados do Treinamento<br>
Impacto do Preço na Predição do item_id:<br>
A análise visual da imagem mostra o impacto do preço nas previsões do item_id específico sku-001. A variação dos pontos ao longo do eixo horizontal (preço) indica como mudanças no preço afetam a previsão do modelo.<br><br>


## Previsões vs. Valores Reais:
A segunda imagem mostra uma comparação entre os valores previstos pelo modelo e os valores reais. É possível ver a correspondência entre as previsões e os resultados reais para diferentes item_id.<br><br>


## Realizando Previsões
Para demonstrar a capacidade do modelo em fazer previsões úteis, utilizei os seguintes dados de entrada:

Coluna  |  Valor<br>
Location | Seattle<br>
time_stamp | 10/01/17 12:00 am<br>
demand |	235.9<br>
price	| 103<br>
Product_category | Appliances<br>
Inseri esses dados na ferramenta de previsão do AWS SageMaker Canvas, selecionando a opção de previsão única.<br><br>

## Resultados das Previsões<br>
A ferramenta gerou a seguinte previsão para o item_id com base nos dados fornecidos:<br>

item_id	Prediction<br>
sku-090	54.047%<br>
sku-079	3.97%<br>
sku-183	6.137%<br>
sku-146	3.984%<br>
sku-041	2.849%<br>
...	...<br><br>
Com base nos resultados, o sku-090 tem a maior probabilidade de 54.047%. Isso indica que, para os dados de entrada fornecidos, o modelo prevê que sku-090 é o item mais provável a ser demandado.

## Análise dos Resultados<br>
A alta probabilidade associada ao sku-090 demonstra uma forte confiança do modelo de que este é o item que será demandado para as características fornecidas. Este insight pode ser utilizado para ajustar o estoque e estratégias de marketing, garantindo que o item correto esteja disponível para atender à demanda esperada.
