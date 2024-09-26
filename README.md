# MVP Análise de Dados e Boas Práticas

Este projeto realiza uma análise de dados de uma campanha bancária, focada em prever o comportamento dos clientes em relação à assinatura de um produto financeiro, aplicando boas práticas de ciência de dados.

## Acessar o notebook no Google Colab

Clique no link abaixo para abrir o notebook diretamente no Google Colab:

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Danielbalthazar/MVP_AnaliseDeDados_e_BoasPraticas/blob/main/MVP_AnáliseDeDados_e_BoasPráticas.ipynb)

## Estrutura do Projeto

### Definição do Problema
O problema envolve a previsão de assinatura de um depósito a prazo pelos clientes com base em características demográficas, financeiras e histórico de campanhas. É um problema de classificação binária.

### Tipos de Dados
Os atributos do dataset são divididos em dois grupos:
- **Numéricos**: Incluem idade, saldo bancário, duração da chamada, entre outros.
- **Categóricos**: Como ocupação, estado civil, nível de educação, tipo de contato e resposta ao produto bancário.

### Análise de Valores Faltantes
O dataset analisado não contém valores faltantes, o que simplifica a limpeza dos dados.

## Conteúdo do Notebook

### Resumo Estatístico
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



### 2. Análise de Dados

Esta seção contém uma exploração inicial dos dados, utilizando diversas bibliotecas e funções do Python para entender melhor o comportamento dos atributos e a relação entre eles.

#### Bibliotecas Utilizadas

As principais bibliotecas Python utilizadas são:

- `pandas`: Manipulação e análise de dados.
- `numpy`: Operações numéricas e vetorização.
- `matplotlib` e `seaborn`: Criação de visualizações gráficas.
- `scikit-learn`: Modelagem e pré-processamento de dados.

#### Funções Utilizadas

Aqui são descritas as funções específicas utilizadas ao longo da análise, como para carregamento dos dados, geração de gráficos e cálculos estatísticos.

#### Carregando Arquivos do Github

Os dados são carregados diretamente de um repositório no GitHub, usando funções que garantem a leitura adequada e preparação dos dados para análise.

#### Estatísticas Descritivas

Uma análise descritiva é realizada, apresentando as principais estatísticas dos atributos do dataset, como média, mediana, valores máximos e mínimos, além de uma análise de dispersão e distribuição dos dados.

#### Visualizações

A análise visual dos dados inclui gráficos de distribuição e correlação entre os atributos, o que ajuda a entender melhor as relações e possíveis padrões no comportamento dos clientes.

##### Análise sobre a Distribuição dos Atributos

Gráficos de distribuição são criados para os principais atributos do dataset, permitindo visualizar a dispersão e detectar padrões ou possíveis assimetrias.

##### Análise sobre a Correlação dos Atributos

Matrizes de correlação são geradas para verificar as relações entre as variáveis numéricas, ajudando a identificar quais atributos podem ter maior impacto na previsão da variável alvo.

### 3. Pré-processamento de Dados

Após a análise inicial, os dados são preparados para a modelagem, passando por uma série de transformações necessárias para melhorar a performance dos modelos.

#### Tratamento de Outliers

Os outliers são identificados e tratados de maneira apropriada, seja através de sua remoção ou transformação, para evitar que distorçam os resultados do modelo.

#### Criação de Categorias e Flags

Nesta etapa, são criadas novas variáveis categóricas e flags para melhorar a qualidade dos dados e adicionar informações relevantes ao modelo, como agrupamento de idades e saldo bancário.

#### Conversão de Variáveis Categóricas (One-Hot Encoding)

Variáveis categóricas são convertidas em variáveis numéricas utilizando a técnica de one-hot encoding, permitindo que possam ser utilizadas pelos algoritmos de machine learning.

#### Separação dos Dados para Treino e Teste

Os dados são divididos em conjuntos de treino e teste, garantindo uma validação adequada do modelo. A divisão é feita de maneira estratificada para manter a proporção da variável alvo nos dois conjuntos.

#### Normalização

A normalização é aplicada para padronizar os valores numéricos, garantindo que todos os atributos tenham o mesmo peso e importância durante o processo de modelagem.

#### Balanceamento

Técnicas de balanceamento são aplicadas para lidar com a desproporção entre as classes da variável alvo, melhorando a capacidade do modelo de prever corretamente ambas as classes.
