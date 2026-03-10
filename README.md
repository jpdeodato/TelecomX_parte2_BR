📊 Previsão de Evasão de Clientes em Telecomunicações
📌 Descrição do Projeto

Este projeto tem como objetivo desenvolver modelos de Machine Learning capazes de prever a evasão de clientes (churn) em uma empresa fictícia de telecomunicações.

A evasão de clientes representa um grande desafio para empresas desse setor, pois a perda de clientes impacta diretamente a receita e os custos de aquisição de novos consumidores. Assim, identificar clientes com maior probabilidade de cancelamento permite que a empresa adote estratégias de retenção mais eficientes.

Neste projeto foi desenvolvido um pipeline de análise de dados e modelagem preditiva, incluindo etapas de:

tratamento dos dados

análise exploratória

engenharia de variáveis

treinamento de modelos de Machine Learning

avaliação de desempenho

análise da importância das variáveis


📊 Base de Dados

A base de dados utilizada contém informações fictícias de clientes de uma empresa de telecomunicações, incluindo:

características demográficas

tipo de contrato

serviços contratados

método de pagamento

tempo de relacionamento com a empresa

valor total gasto

A variável alvo do modelo é:

evasao

Onde:

0 → Cliente permaneceu
1 → Cliente cancelou o serviço
🔎 Etapas do Projeto
1️⃣ Análise Exploratória dos Dados

Foram realizadas análises para compreender:

distribuição das variáveis

presença de dados desbalanceados

correlação entre variáveis

possíveis padrões relacionados à evasão

Também foram utilizados gráficos como:

matriz de correlação

boxplots

scatter plots

2️⃣ Pré-processamento dos Dados

As seguintes etapas foram aplicadas:

remoção de variáveis irrelevantes

tratamento de variáveis categóricas com One-Hot Encoding

normalização das variáveis numéricas

divisão do conjunto de dados em treino e teste

Divisão utilizada:

80% treino
20% teste
🤖 Modelos de Machine Learning

Foram testados diferentes modelos para prever a evasão de clientes.

1️⃣ Modelo Baseline

Foi utilizado um DummyClassifier como modelo de referência, que prevê sempre a classe majoritária.

Esse modelo serve como linha de base para comparação com modelos mais sofisticados.

2️⃣ K-Nearest Neighbors (KNN)

O modelo KNN classifica os clientes com base na proximidade entre os dados no espaço das variáveis.

Como esse modelo depende da distância entre os pontos, foi aplicada normalização dos dados.

3️⃣ Árvore de Decisão

A árvore de decisão foi utilizada para capturar relações não lineares entre as variáveis e melhorar a capacidade de identificação da evasão.

📈 Avaliação dos Modelos

Os modelos foram avaliados utilizando as seguintes métricas:

Accuracy

Precision

Recall

F1-score

Essas métricas permitem avaliar não apenas a taxa de acerto do modelo, mas também sua capacidade de identificar corretamente clientes que irão cancelar o serviço.

📊 Comparação dos Modelos
Modelo	Accuracy	Precision	Recall	F1-score
Dummy	0.73	0.00	0.00	0.00
KNN	-	-	-	-
Árvore de Decisão	-	-	-	-

O modelo Dummy apresentou underfitting, pois não foi capaz de identificar clientes que cancelaram o serviço.

Os modelos de Machine Learning apresentaram desempenho superior, sendo capazes de capturar padrões relevantes nos dados.

🔎 Análise das Variáveis Mais Relevantes

Foi realizada uma análise das variáveis mais importantes para a previsão de evasão utilizando diferentes abordagens:

Regressão Logística

Os coeficientes do modelo foram analisados para identificar quais variáveis aumentam ou reduzem a probabilidade de evasão.

KNN

Como o KNN utiliza distância entre observações, as variáveis mais influentes são aquelas que mais contribuem para diferenciar os clientes no espaço de atributos.

Random Forest

A importância das variáveis foi avaliada com base na contribuição de cada atributo para a redução da impureza nas árvores do modelo.

Essa análise permite identificar fatores importantes relacionados ao churn, como:

tipo de contrato

tempo de relacionamento com a empresa

valor total gasto

método de pagamento

🧠 Conclusões

A aplicação de modelos de Machine Learning permitiu identificar padrões relevantes relacionados à evasão de clientes.

Entre os principais insights obtidos:

clientes com contratos de curto prazo tendem a apresentar maior probabilidade de cancelamento

clientes com menor tempo de relacionamento com a empresa possuem maior risco de evasão

o tipo de serviço contratado e o método de pagamento também influenciam o churn

Essas informações podem auxiliar empresas de telecomunicações a desenvolver estratégias de retenção mais eficientes, direcionando ações para clientes com maior risco de cancelamento.

🛠 Tecnologias Utilizadas

Python

Pandas

NumPy

Matplotlib

Seaborn

Scikit-learn
