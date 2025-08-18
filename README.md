# checkpoint1-iot-consumidores
Repósitorio destinado ao primeiro checkpoint de iot sobre consumidores de energia.

📊 Individual Household Electric Power Consumption

Este projeto utiliza o dataset Individual Household Electric Power Consumption, disponível no UCI Machine Learning Repository, para realizar análises exploratórias, estatísticas e modelagens preditivas relacionadas ao consumo elétrico em uma residência entre 2006 e 2010.

O trabalho foi desenvolvido em Python (Jupyter Notebook) e segue um conjunto de 20 tarefas propostas, abordando desde manipulação e limpeza de dados até visualização, clustering e modelagem de regressão.


📂 Estrutura do Repositório

notebook.ipynb → Arquivo principal contendo a resolução das tarefas.
README.md → Este documento, com as instruções e descrição do projeto.
data/ → Pasta destinada ao dataset (não versionada no GitHub por questões de tamanho).


📑 Informações do Dataset

Nome: Individual Household Electric Power Consumption
Fonte: UCI Machine Learning Repository
Descrição:

Consumo elétrico de uma residência localizado em Sceaux, França, entre dezembro de 2006 e novembro de 2010.
Frequência de amostragem: 1 minuto.
Número de instâncias: ~2.075.259 registros.
Número de variáveis: 9 (8 numéricas e 1 categórica).


🔑 Principais variáveis

Global_active_power: Potência ativa global consumida (em kilowatts).
Global_reactive_power: Potência reativa global (em kilowatts).
Voltage: Tensão média (em volts).
Global_intensity: Corrente elétrica média (em amperes).
Sub_metering_1: Consumo do submedidor 1 (em watt-hora).
Sub_metering_2: Consumo do submedidor 2 (em watt-hora).
Sub_metering_3: Consumo do submedidor 3 (em watt-hora).


✅ Tarefas Realizadas

1) Carregamento e exibição das 10 primeiras linhas do dataset.
2) Explicação da diferença entre Global_active_power e Global_reactive_power.
3) Verificação e quantificação de valores ausentes.
4) Conversão da coluna Date para datetime e criação da coluna de dia da semana.
5) Filtragem dos registros de 2007 e cálculo da média de consumo diário.
6) Gráfico de linha da variação de Global_active_power em um único dia.
7) Histograma da variável Voltage e análise da distribuição.
8) Cálculo do consumo médio por mês em todo o período.
9) Identificação do dia com maior consumo de energia ativa.
10) Comparação do consumo médio em dias de semana vs finais de semana.
11) Cálculo da correlação entre Global_active_power, Global_reactive_power, Voltage e Global_intensity.
12) Criação da variável Total_Sub_metering (soma dos três submedidores).
13) Verificação de meses em que Total_Sub_metering ultrapassa a média de Global_active_power.
14) Série temporal do Voltage para o ano de 2008.
15) Comparação do consumo entre meses de verão e inverno.
16) Amostragem aleatória de 1% dos dados e comparação da distribuição.
17) Normalização das variáveis numéricas principais com Min-Max Scaling.
18) Aplicação do algoritmo K-Means para segmentar dias em 3 grupos distintos de consumo.
19) Decomposição de série temporal de Global_active_power (tendência, sazonalidade e resíduo).
20) Treinamento de um modelo de Regressão Linear Simples para prever Global_active_power a partir de Global_intensity.


🚀 Tecnologias Utilizadas

Linguagem: Python 3.9+
Bibliotecas principais:
pandas
numpy
matplotlib
seaborn
scikit-learn
statsmodels


📌 Como Executar

1) Clone este repositório: git clone https://github.com/carmowa/checkpoint1-iot-consumidores.git
2) Acesse a pasta do projeto: cd checkpoint1-iot-consumidores
3) Crie um ambiente virtual:
python -m venv venv
venv\Scripts\activate   
4) Instale as dependências: pip install -r requirements.txt
5) Execute o notebook: jupyter notebook notebook.ipynb