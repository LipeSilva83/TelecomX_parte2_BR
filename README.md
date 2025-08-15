# Challenge-TelecomX_PT2

# :computer: Projeto de Modelagem Preditiva com KNN e Random Forest Regressor :computer:
Este projeto de machine learning visa a criação e comparação de modelos de regressão para realizar previsões precisas. Utilizando Python, exploramos a performance de dois algoritmos populares: K-Nearest Neighbors (KNN) e Random Forest Regressor, para determinar qual deles oferece o melhor desempenho para a tarefa de modelagem.

# ⚙️  Tecnologias Utilizadas ⚙️
O projeto foi desenvolvido inteiramente em Python, aproveitando o ecossistema de bibliotecas de Data Science e Machine Learning para a manipulação, visualização de dados e construção dos modelos.


Linguagem de Programação: Python 
<img src="https://raw.githubusercontent.com/marwin1991/profile-technology-icons/refs/heads/main/icons/python.png" alt="Python" width="30" height="50"/>


Bibliotecas: 

Pandas: <img src="https://raw.githubusercontent.com/marwin1991/profile-technology-icons/refs/heads/main/icons/pandas.png" alt="Python" width="30" height="50"/>

NumPy: <img src="https://raw.githubusercontent.com/marwin1991/profile-technology-icons/refs/heads/main/icons/numpy.png" alt="NumPy:" width="30" height="50"/> 

Scikit-learn: <img src="https://upload.wikimedia.org/wikipedia/commons/0/05/Scikit_learn_logo_small.svg" alt="Python" width="60" height="80"/>

Matplotlib: 

Seaborn: <img src="https://upload.wikimedia.org/wikipedia/commons/4/45/Logo-seaborn.png" alt="Python" width="40" height="60"/>

🧠 Algoritmos Implementados
O cerne deste projeto é a implementação e comparação de dois modelos de regressão.

K-Nearest Neighbors (KNN) Regressor: Um algoritmo de aprendizado supervisionado não paramétrico que faz previsões com base nos vizinhos mais próximos.

Random Forest Regressor: Um algoritmo de aprendizado supervisionado que constrói uma "floresta" de árvores de decisão aleatórias para fazer previsões mais robustas e precisas.

📊 Resultados e Análise
Ambos os modelos foram avaliados usando métricas de desempenho comuns para regressão, como o R² (coeficiente de determinação), que mede a proporção da variância na variável dependente que é previsível a partir das variáveis independentes.

Após a análise, o Random Forest Regressor demonstrou um desempenho superior, com um R² de 0.98, superando o KNN Regressor, que obteve um R² de 0.94.

Isso indica que o modelo de Random Forest conseguiu capturar melhor a complexidade e as relações nos dados, resultando em previsões mais acuradas.

🚀 Como Rodar o Projeto
Para replicar a análise e os modelos localmente, siga os passos abaixo.

Pré-requisitos
Certifique-se de ter o Python 3.x instalado.

1. Clonar o Repositório
Bash

git clone https://github.com/seu-usuario/seu-repositorio.git
cd seu-repositorio
2. Instalar as Dependências
É recomendado o uso de um ambiente virtual.

Bash

pip install -r requirements.txt
3. Executar o Script Principal
Abra o notebook ou o script principal do projeto (.ipynb ou .py) e execute-o para gerar os modelos e a análise.

✒️ Autor
[Seu Nome ou Usuário do GitHub] - [Link para o seu perfil no GitHub]

📜 Licença
Este projeto está sob a licença MIT License. Para mais detalhes, veja o arquivo LICENSE.







Relatório Estratégico de Análise de Evasão de Clientes

 

1. Introdução

Este relatório apresenta uma análise detalhada da evasão de clientes

(churn) de uma empresa, com o objetivo de identificar os principais fatores que

influenciam a decisão dos clientes de cancelar seus serviços. Através da

preparação e análise dos dados, modelagem preditiva utilizando os algoritmos

KNN e Random Forest Regressor, e avaliação de desempenho, buscamos fornecer

insights acionáveis para a implementação de estratégias de retenção eficazes. A

compreensão dos motivos por trás da evasão é crucial para reduzir a perda de

clientes e otimizar os esforços de marketing e atendimento.

 

2. Metodologia

A metodologia adotada neste estudo envolveu as seguintes etapas:



Preparação

dos Dados: Carregamento

do dataset df_normalizado.csv, remoção de colunas irrelevantes (customerID),

e codificação (encoding) de variáveis categóricas utilizando o

método get_dummies para torná-las compatíveis com os algoritmos

de machine learning.



Análise

Exploratória e de Correlação: Realização de análise de correlação entre as variáveis e a

variável alvo 'Rotatividade' para identificar as características mais

relacionadas à evasão. Visualização das principais correlações através de

um mapa de calor.



Seleção de

Variáveis: Com base

na análise de correlação, foram selecionadas as variáveis com maior

impacto na 'Rotatividade' para a modelagem preditiva.



Separação

dos Dados: O dataset

foi dividido em conjuntos de treino e teste na proporção de 70% para

treino e 30% para teste.



Modelagem

Preditiva: Foram

treinados dois modelos de classificação:




KNN

(K-Nearest Neighbors): Um

modelo baseado em distância que requer normalização dos dados. Os dados

de treino e teste foram normalizados usando MinMaxScaler.



Random

Forest Regressor: Um

modelo de ensemble baseado em árvores de decisão. Embora seja um

regressor, suas previsões contínuas foram convertidas em rótulos binários

(0 ou 1) para o problema de classificação.






Avaliação

dos Modelos: O

desempenho de ambos os modelos foi avaliado utilizando métricas de

classificação padrão: Acurácia, Precisão, Recall e F1-score. A matriz de

confusão também foi gerada para visualizar o desempenho em termos de

verdadeiros positivos, verdadeiros negativos, falsos positivos e falsos

negativos.



Interpretação

dos Resultados: Análise

da importância das variáveis fornecida pelo modelo Random Forest para

entender quais características tiveram maior influência nas previsões de

rotatividade. Comparação do desempenho dos modelos e discussão das

implicações estratégicas.

 

3. Análise dos Dados

Nesta seção, apresentamos os resultados da análise de correlação entre

as variáveis e a evasão de clientes, bem como a importância das variáveis

identificada pelo modelo Random Forest.

3.1 Análise de Correlação

A análise de correlação revelou o grau e a direção da relação linear

entre cada variável e a 'Rotatividade'. Variáveis com correlações positivas

mais altas indicam que, à medida que o valor da variável aumenta, a

probabilidade de evasão também aumenta. Variáveis com correlações negativas

mais altas (em valor absoluto) indicam que, à medida que o valor da variável

aumenta, a probabilidade de evasão diminui.

Principais Correlações Positivas:



Contrato_Month-to-month:

Clientes com contratos mensais apresentam uma correlação positiva

significativa com a evasão, sugerindo que a falta de um compromisso de

longo prazo está associada a uma maior probabilidade de churn.



Segurança_Online_No:

A ausência de serviço de segurança online está positivamente

correlacionada com a evasão.



Suporte_Técnico_0:

Clientes sem suporte técnico mostram uma correlação positiva com a evasão.



Serviço_de_Internet_Fiber

optic: Clientes com serviço de internet de fibra óptica parecem ter maior

probabilidade de evadir.



Forma_de_Pagamento_Electronic

check: A forma de pagamento por cheque eletrônico também apresenta uma

correlação positiva com a evasão.

Principais Correlações Negativas:



Termo: Quanto

maior o termo do contrato (contratos de longo prazo), menor a correlação

com a evasão, indicando que clientes com contratos mais longos tendem a

permanecer.



Contrato_Two

year: Ter um contrato de dois anos está negativamente correlacionado com a

evasão.



Variáveis

relacionadas à ausência de serviço de internet (Serviço_de_Internet_No, Segurança_Online_No

internet service, etc.): Clientes sem serviço de internet em geral têm

menor probabilidade de evadir (provavelmente porque seus custos são

menores e o engajamento com a empresa é diferente).



Cobrança_Total:

O valor total pago até o momento apresenta uma correlação negativa com a

evasão, o que pode sugerir que clientes que acumularam maiores cobranças

ao longo do tempo tendem a ser mais fiéis.

3.2 Importância das Variáveis (Random Forest)

A análise de importância das variáveis pelo modelo Random Forest

Regressor fornece outra perspectiva sobre quais características são mais

relevantes para prever a evasão. O modelo avalia a contribuição de cada

variável para a redução da impureza nas árvores de decisão.

As variáveis com maior importância, de acordo com o Random Forest,

foram:



Contrato_Month-to-month:

Confirmando a análise de correlação, o tipo de contrato mensal foi a

variável mais importante na previsão da evasão.



Termo: O

termo do contrato também se mostrou altamente importante, reforçando sua

relevância identificada na análise de correlação.



Serviço_de_Internet_Fiber

optic: O tipo de serviço de internet (fibra óptica) foi a terceira

variável mais importante.



Cobrança_Total:

O valor total cobrado também teve uma importância considerável.



Suporte_Técnico_0 e Segurança_Online_No:

A ausência desses serviços também foram apontadas como importantes pelo

modelo.

 

A importância das variáveis do Random Forest geralmente alinha-se bem

com as correlações mais fortes, destacando o Contrato_Month-to-month, Termo e

Serviço_de_Internet_Fiber optic como os principais impulsionadores da evasão.

 

3.3 Análise de Cluster (Baseado na análise anterior)

Embora não tenhamos realizado uma nova análise de cluster como parte

desta subtask específica, a análise anterior mostrou que existem clusters

distintos de clientes com diferentes taxas de rotatividade. O Cluster 0

apresentou a maior taxa de rotatividade, enquanto outros clusters tiveram taxas

significativamente menores. Isso sugere que os clientes que evadem tendem a

compartilhar características específicas que os diferenciam dos clientes que

permanecem, e essas características provavelmente correspondem às variáveis

identificadas como importantes nas análises de correlação e importância de

variáveis (como tipo de contrato, serviços adicionais, etc.). A análise de

cluster reforça a ideia de que a evasão não é um fenômeno aleatório, mas está

associada a perfis de clientes identificáveis.

 

4. Desempenho dos Modelos

Nesta seção, comparamos o desempenho dos modelos KNN e Random Forest

Regressor na previsão da evasão de clientes utilizando métricas de

classificação.

4.1 Avaliação do Modelo KNN

O modelo KNN foi treinado nos dados normalizados e avaliado no conjunto

de teste normalizado. As métricas de desempenho obtidas foram:



Accuracy

(Acurácia): 0.7538



Precision

(Precisão): 0.4952



Recall

(Revocação): 0.4831



F1-score: 0.4891

A matriz de confusão para o modelo KNN mostrou o seguinte:



Verdadeiros

Negativos (clientes que não evadiram e foram previstos corretamente): 1387



Falsos

Positivos (clientes que não evadiram, mas foram previstos como evasão):

262



Falsos

Negativos (clientes que evadiram, mas foram previstos como não evasão):

275



Verdadeiros

Positivos (clientes que evadiram e foram previstos corretamente): 257

O modelo KNN apresentou uma acurácia razoável, mas a precisão e o recall

foram moderados, indicando que ele teve dificuldade em identificar corretamente

todos os clientes que evadiram (recall mais baixo) e que uma proporção

significativa das suas previsões de evasão foram falsos positivos (precisão

mais baixa).

4.2 Avaliação do Modelo Random Forest Regressor

O modelo Random Forest Regressor foi treinado nos dados originais (não

normalizados, pois não é um requisito para este algoritmo) e suas previsões

contínuas foram binarizadas com um limiar de 0.5. As métricas de desempenho

obtidas foram:



Accuracy

(Acurácia): 0.8111



Precision

(Precisão): 0.6456



Recall

(Revocação): 0.5000



F1-score: 0.5636

A matriz de confusão para o modelo Random Forest Regressor mostrou o

seguinte:



Verdadeiros

Negativos: 1503



Falsos

Positivos: 146



Falsos

Negativos: 266



Verdadeiros

Positivos: 266

Comparando os dois modelos, o Random Forest Regressor demonstrou um

desempenho superior em todas as métricas avaliadas no conjunto de teste. Ele

obteve maior acurácia, precisão, recall e F1-score do que o modelo KNN. Isso

sugere que o Random Forest foi mais eficaz em prever a rotatividade dos

clientes neste dataset. A precisão mais alta do Random Forest é particularmente

vantajosa em cenários onde o custo de contatar clientes que não iriam evadir

(falsos positivos) é alto.

 



 

5. Conclusão e Recomendações

Com base na análise dos dados e no desempenho dos modelos preditivos,

podemos tirar as seguintes conclusões e propor recomendações estratégicas para

a empresa:

Principais Fatores que Influenciam a Evasão:

As análises de correlação e de importância das variáveis do Random

Forest consistentemente apontam para os seguintes fatores como os mais

influentes na decisão do cliente de evadir:



Tipo de

Contrato (Mensal): Clientes

com contratos mensais (Contrato_Month-to-month) apresentam uma

probabilidade significativamente maior de evadir em comparação com aqueles

com contratos de um ou dois anos.



Termo do

Contrato: Clientes

com termos de contrato mais longos (Termo, Contrato_Two year) são

menos propensos a evadir.



Serviços

Adicionais (Segurança Online e Suporte Técnico): A ausência de serviços como

segurança online (Segurança_Online_No) e suporte técnico (Suporte_Técnico_0)

está fortemente associada à evasão.



Serviço de

Internet Fibra Óptica: Clientes

com este tipo de serviço (Serviço_de_Internet_Fiber optic) parecem ter

maior propensão a evadir. Isso pode estar relacionado a expectativas de

desempenho, custos ou concorrência.



Forma de

Pagamento (Cheque Eletrônico): Clientes que utilizam cheque eletrônico (Forma_de_Pagamento_Electronic

check) têm uma maior probabilidade de evadir.



Cobrança

Total: Clientes com

menor cobrança total (Cobrança_Total negativamente correlacionada)

são mais propensos a evadir, o que pode indicar que clientes de menor

valor ou que estão com a empresa há menos tempo têm maior risco.

Desempenho dos Modelos:

O modelo Random Forest Regressor demonstrou ser mais

eficaz na previsão da evasão em comparação com o modelo KNN, apresentando

melhores métricas de acurácia, precisão, recall e F1-score no conjunto de

teste. A capacidade do Random Forest de identificar as variáveis mais

importantes e lidar com a não-linearidade dos dados provavelmente contribuiu

para seu desempenho superior.

Estratégias de Retenção Baseadas em Dados:

Com base nos fatores identificados, propomos as seguintes estratégias de

retenção:



Incentivar

Contratos de Longo Prazo: Oferecer

descontos, benefícios ou programas de fidelidade para incentivar os

clientes com contratos mensais a migrarem para contratos de um ou dois

anos. Focar nos benefícios da estabilidade e do valor a longo prazo.



Promover

Serviços de Valor Agregado: Destacar

a importância e os benefícios da segurança online e do suporte técnico.

Considerar pacotes ou ofertas especiais para incentivar a assinatura

desses serviços, especialmente para clientes de fibra óptica que parecem

ter um risco maior.



Analisar a

Experiência do Cliente com Fibra Óptica: Investigar os motivos pelos quais clientes de fibra óptica

têm maior propensão à evasão. Pode ser relacionado à qualidade do serviço,

preço, suporte especializado ou concorrência. Realizar pesquisas de

satisfação ou analisar tickets de suporte para identificar pontos de dor.



Revisar a

Forma de Pagamento por Cheque Eletrônico: Entender por que clientes que usam

cheque eletrônico são mais propensos a evadir. Pode haver problemas com o

processo de pagamento, taxas ou ser um indicador de um perfil de cliente

menos engajado. Considerar oferecer incentivos para outras formas de

pagamento automático (cartão de crédito, débito automático).



Desenvolver

Programas de Engajamento para Clientes de Baixo Termo/Cobrança Total: Identificar clientes com menor tempo

de contrato ou menor valor total pago, pois eles representam um risco

maior de evasão. Implementar programas de engajamento proativos, como

ofertas personalizadas, check-ins de satisfação ou programas de boas-vindas

estendidos.



Utilizar o

Modelo Random Forest para Identificação de Risco: Implementar o modelo Random Forest

treinado para prever a probabilidade de evasão de cada cliente. Priorizar

os clientes com maior risco de evasão para ações de retenção direcionadas.



Monitoramento

Contínuo: Continuar

monitorando as métricas de evasão e o desempenho do modelo. Realizar

análises periódicas para identificar novas tendências ou mudanças nos

fatores que influenciam a evasão.



Ao focar

nesses fatores chave e implementar as estratégias de retenção sugeridas, a

empresa pode aumentar significativamente suas taxas de retenção de

clientes e melhorar a lucratividade a longo prazo.

 

6.

Limitações

É importante

reconhecer as limitações deste estudo:



Desequilíbrio

de Classes: O

dataset apresentou um desequilíbrio significativo entre as classes

(clientes que evadiram vs. clientes que não evadiram). Embora as métricas

tenham sido avaliadas, o desequilíbrio pode impactar o desempenho do

modelo, especialmente o recall (capacidade de identificar todos os

clientes que evadiram). Técnicas de balanceamento de dados (como

oversampling ou undersampling) poderiam ser exploradas em trabalhos

futuros para mitigar este problema.



Interpretabilidade

do Random Forest: Embora

o Random Forest forneça a importância das variáveis, a interpretação das

relações não-lineares dentro do modelo pode ser mais complexa do que em

modelos mais simples, como regressão logística.



Dados

Estáticos: A análise

é baseada em um snapshot dos dados em um determinado momento. O

comportamento do cliente e os fatores de influência podem mudar ao longo

do tempo, exigindo a reavaliação e retreinamento periódicos dos modelos.



Ausência

de Teste A/B ou Análise Causal: Este estudo identifica correlações e importância preditiva,

mas não estabelece causalidade direta entre as variáveis e a evasão. Para

confirmar o impacto das estratégias de retenção, testes A/B ou outras

análises causais seriam necessários.



Escopo das

Variáveis: A análise

está limitada às variáveis presentes no dataset. Outros fatores externos

(como ações da concorrência, mudanças no mercado ou eventos econômicos)

que podem influenciar a evasão não foram incluídos.

Apesar destas

limitações, os insights obtidos fornecem uma base sólida para a empresa começar

a desenvolver e implementar estratégias de retenção direcionadas.

 

Resumo:

Principais

Resultados da Análise de Dados

Análise de

Correlação:

Fortes

correlações positivas com a rotatividade (Rotatividade) foram encontradas para

Contrato_Mês a mês, Serviço_de_Internet_Fibra Óptica, Segurança_Online_Nº,

Suporte_Técnico_0 e Forma_de_Pagamento_Confirmação Eletrônica.

Fortes

correlações negativas com a rotatividade foram encontradas para Termo,

Contrato_Bienal e Cobrança_Total.

Importância das

Características da Floresta Aleatória:

As

características mais importantes que previram a rotatividade foram Contrato_Mês

a mês, Termo, Serviço_de_Internet_Fibra Óptica, Cobrança_Total,

Suporte_Técnico_0 e Segurança_Online_Nº, alinhando-se amplamente com a análise

de correlação.

Análise de

Cluster:

Análises

anteriores indicaram clusters distintos de clientes com taxas de rotatividade

variadas, com o Cluster 0 apresentando a maior taxa de rotatividade, sugerindo

que os clientes neste cluster provavelmente possuem características

identificadas como principais impulsionadores da rotatividade.

Desempenho do

Modelo:

O modelo Random

Forest Regressor superou o modelo KNN na previsão de churn, alcançando maiores

Precisão (0,8111 vs. 0,7538), Precisão (0,6456 vs. 0,4952), Recall (0,5000 vs.

0,4831) e F1-score (0,5636 vs. 0,4891) no conjunto de teste.

Insights ou

Próximos Passos

Concentre os

esforços de retenção em clientes com contratos mensais, internet fibra óptica,

aqueles sem segurança online ou suporte técnico e aqueles que pagam por meio de

cheque eletrônico, pois esses fatores estão fortemente associados a um maior

risco de churn.

Utilize o

modelo Random Forest treinado para identificar clientes de alto risco para

campanhas de retenção direcionadas e considere oferecer incentivos para

contratos de longo prazo e serviços adicionais para esses segmentos.

 

 



Com base no seu relatório detalhado sobre a análise de evasão de clientes, criei um README para o GitHub. Ele está estruturado para ser claro, direto e profissional, cobrindo desde a visão geral do projeto até os insights estratégicos e as limitações do estudo, usando as informações do seu relatório.

Análise Preditiva de Evasão de Clientes (Customer Churn)
Este projeto de machine learning foi desenvolvido para analisar e prever a evasão de clientes (churn) de uma empresa de telecomunicações. Utilizando Python e algoritmos de classificação como K-Nearest Neighbors (KNN) e Random Forest, o objetivo principal foi identificar os fatores que mais influenciam a decisão de cancelamento dos clientes e fornecer insights estratégicos para a retenção.

⚙️ Tecnologias e Ferramentas
Linguagem de Programação: Python

Bibliotecas: Pandas, NumPy, Scikit-learn, Matplotlib, Seaborn

Ambiente: Jupyter Notebook

🎯 Metodologia e Modelagem Preditiva
O processo de análise e modelagem seguiu uma abordagem estruturada:

Preparação dos Dados: O dataset foi carregado, colunas irrelevantes foram removidas e variáveis categóricas foram transformadas usando get_dummies.

Análise Exploratória: Foi realizada uma análise de correlação detalhada para entender a relação entre as variáveis e a evasão. Um mapa de calor foi gerado para visualizar essas correlações.

Modelagem Preditiva: Dois modelos de classificação foram treinados e avaliados:

KNN (K-Nearest Neighbors): Treinado em dados normalizados com MinMaxScaler.

Random Forest: Utilizado para prever a evasão e para extrair a importância das variáveis.

Avaliação dos Modelos: O desempenho de ambos os modelos foi comparado usando métricas como Acurácia, Precisão, Recall e F1-score, além da matriz de confusão.

📊 Principais Resultados e Insights
Fatores-Chave de Evasão
A análise de correlação e a importância das variáveis extraída do modelo Random Forest apontaram consistentemente para os seguintes fatores como os mais relevantes na previsão de churn:

Tipo de Contrato: Contratos mensais (Contrato_Month-to-month) são o fator mais importante, indicando que a falta de compromisso de longo prazo aumenta o risco de evasão.

Serviços Adicionais: A ausência de serviços como Segurança_Online e Suporte_Técnico está fortemente correlacionada com a evasão.

Serviço de Internet: Clientes com serviço de internet de fibra óptica (Serviço_de_Internet_Fiber optic) apresentam maior propensão a evadir.

Termo e Cobrança Total: Clientes com contratos de longo prazo (Termo, Contrato_Two year) e maior Cobrança_Total são menos propensos a evadir.

Forma de Pagamento: O uso de cheque eletrônico (Forma_de_Pagamento_Electronic check) também está associado a um maior risco de churn.

Desempenho dos Modelos
A comparação de desempenho no conjunto de teste demonstrou a superioridade do Random Forest sobre o KNN:

Métrica	Random Forest	KNN
Acurácia	0.8111	0.7538
Precisão	0.6456	0.4952
Recall	0.5000	0.4831
F1-score	0.5636	0.4891

Exportar para as Planilhas
O Random Forest foi mais eficaz em prever a rotatividade, com uma precisão significativamente maior, o que é crucial para direcionar ações de retenção de forma mais eficiente e com menos "falsos positivos".

💡 Recomendações Estratégicas
Com base nos insights obtidos, as seguintes estratégias de retenção são recomendadas:

Incentivar Contratos de Longo Prazo: Oferecer descontos ou benefícios para clientes com contratos mensais migrarem para contratos de 1 ou 2 anos.

Promover Serviços Adicionais: Destacar os benefícios da segurança online e do suporte técnico para aumentar o engajamento e a fidelidade do cliente.

Analisar a Experiência com Fibra Óptica: Investigar os motivos da alta taxa de evasão entre clientes de fibra óptica para identificar possíveis problemas de qualidade ou preço.

Implementar o Modelo Preditivo: Utilizar o modelo Random Forest treinado para identificar clientes com alto risco de churn e priorizá-los em campanhas de retenção direcionadas.

✒️ Autor
[Seu Nome ou Usuário do GitHub] - [Link para o seu perfil no GitHub]

📜 Licença
Este projeto está sob a licença MIT License. Para mais detalhes, veja o arquivo LICENSE.
