# MVP Análise de Dados e Boas Práticas

Este projeto realiza uma análise de dados de uma campanha bancária, focada em prever o comportamento dos clientes em relação à assinatura de um produto financeiro, aplicando boas práticas de ciência de dados.

## Acessar o notebook no Google Colab

Clique no link abaixo para abrir o notebook diretamente no Google Colab:

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Danielbalthazar/MVP_AnaliseDeDados_e_BoasPraticas/blob/main/MVP_AnáliseDeDados_e_BoasPráticas.ipynb)

## Estrutura do Projeto

### 1. Definição do Problema
O problema envolve a previsão de assinatura de um depósito a prazo pelos clientes com base em características demográficas, financeiras e histórico de campanhas. É um problema de classificação binária.

### 2. Tipos de Dados
Os atributos do dataset são divididos em dois grupos:
- **Numéricos**: Incluem idade, saldo bancário, duração da chamada, entre outros.
- **Categóricos**: Como ocupação, estado civil, nível de educação, tipo de contato e resposta ao produto bancário.

### 3. Análise de Valores Faltantes
O dataset analisado não contém valores faltantes, o que simplifica a limpeza dos dados.

### 4. Resumo Estatístico
Foi gerado um resumo estatístico para os atributos numéricos para entender suas distribuições, médias e variações.

### 5. Visualização de Correlações
Foi construída uma matriz de correlação para identificar relações entre as variáveis numéricas e a variável-alvo `y`.

### 6. Tratamento de Outliers
Outliers foram identificados em variáveis como `balance` e `duration`, sendo tratados por meio de transformações logarítmicas para melhorar a distribuição dos dados.

### 7. Engenharia de Features
Novas features foram criadas, como a categorização da duração das chamadas em intervalos (curta, média, longa). Além disso, as variáveis categóricas foram convertidas em variáveis binárias utilizando One-Hot Encoding.

### 8. Preparação dos Dados para Modelagem
Os dados foram finalizados com as devidas transformações e normalizações, garantindo que todas as variáveis estivessem prontas para alimentar modelos de machine learning.

## Conclusão

A análise forneceu insights importantes sobre o comportamento dos clientes em campanhas anteriores e identificou variáveis críticas como saldo bancário e duração da chamada. O tratamento de outliers e a normalização melhoraram a qualidade do dataset, preparando-o para a etapa seguinte de modelagem preditiva.

**Observação**: Todas as análises e comentários detalhados podem ser encontrados no notebook, fornecendo explicações aprofundadas sobre cada etapa do processo.
