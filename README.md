# Detecção de fraude em cartões de crédito.

## Definição do problema.

A detecção de fraudes de cartão de crédito é extremamente importante, pois tem como objetivo identificar e prevenir transações fraudulentas, proporcionando proteção tanto para as instituições financeiras quanto para os titulares dos cartões.

As fraudes de cartão de crédito representam um impacto financeiro significativo para os bancos e podem causar sérios prejuízos aos clientes, além de afetar a confiança no sistema financeiro como um todo. De acordo com um relatório recente da [IBM](https://www.ibm.com/blogs/ibm-comunica/estudo-de-fraude/)(agosto de 2022), diferentes regiões do mundo e gerações têm diferentes frequências e impactos de fraudes financeiras, bem como atitudes das vítimas em relação à detecção dessas fraudes e às instituições responsáveis por protegê-las de indivíduos mal-intencionados.

O Relatório Global de Impacto de Fraude Financeira da IBM em 2022 também revelou que, à medida que os consumidores globais migraram quase que exclusivamente para cartões de crédito e pagamentos digitais, os cidadãos dos EUA foram vítimas com maior frequência do que todos os outros países pesquisados no relatório. Isso resultou em um custo médio de US$ 265 por ano para os consumidores americanos em cobranças financeiras fraudulentas feitas por terceiros não autorizados.

A detecção eficiente de fraudes permite a identificação precoce de atividades suspeitas, evitando perdas financeiras e protegendo os dados sensíveis dos clientes. Além disso, a detecção de fraudes contribui para manter a integridade e a segurança do mercado de cartões de crédito, promovendo a sustentabilidade e a confiança nas transações eletrônicas.

## Sobre os dados.

O conjunto de dados escolhido para este estudo contém transações realizadas por cartões de crédito em setembro de 2013 por portadores de cartões europeus e apresenta transações que ocorreram em dois dias, onde temos 492 fraudes em um total de 284.807 transações. O conjunto de dados é altamente desbalanceado, a classe positiva (fraudes) representa 0,172% de todas as transações.

Ele contém apenas variáveis de entrada numéricas que são o resultado de uma transformação PCA. Infelizmente, devido a questões de confidencialidade LGPD, as características originais e mais informações de fundo sobre os dados não foram fornecidas. As características V1, V2, ... V28 são os componentes principais obtidos com o PCA, as únicas características que não foram transformadas com o PCA são 'Time' (Tempo) e 'Amount' (Valor). A característica 'Time' contém os segundos decorridos entre cada transação e a primeira transação no conjunto de dados. A característica 'Amount' é o valor da transação. A característica 'Class' é a variável de resposta e assume o valor 1 em caso de fraude e 0 caso contrário.

Os dados estão disponiveis no [kaggle](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud)

