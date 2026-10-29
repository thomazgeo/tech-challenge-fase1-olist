# Relatório Executivo e Análise de Dados - E-commerce Olist
**Projeto do Tech Challenge - Fase 1 | Pós Tech Data Analytics**

## 1. Contexto do Problema
O objetivo deste projeto é analisar o desempenho comercial e logístico do e-commerce Olist entre 2017 e 2018, identificando gargalos operacionais que impactam a satisfação do cliente para propor recomendações acionáveis a investidores.

## 2. Metodologia Utilizada
O projeto foi estruturado com base no framework **KDD (Knowledge Discovery in Databases)** e **CRISP-DM**, passando pelas etapas de seleção, pré-processamento, transformação, mineração de dados e avaliação de resultados. 

## 3. Modelagem Dimensional e Governança
Os dados transacionais brutos foram organizados seguindo o conceito de **Star Schema**. A tabela de pedidos e itens (`olist_orders` e `olist_order_items`) funcionou como a Tabela Fato central, sendo enriquecida pelas Tabelas Dimensão de contexto, como clientes (`customers`), produtos (`products`) e avaliações (`reviews`). Todo o tratamento de dados ausentes (NaN) e conversão de tipos está documentado no notebook.

## 4. Como reproduzir este código
O notebook foi construído no Google Colab e utiliza a biblioteca `kagglehub` para baixar automaticamente o dataset oficial da Olist direto para o ambiente de execução. Basta abrir o arquivo `.ipynb` no Colab e executar as células sequencialmente. Não é necessário fazer o upload manual de arquivos CSV.
