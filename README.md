# Análise de dados de empregos

Este repositório contém um Jupyter Notebook para a análise de dados de empregos usando Python e várias bibliotecas. O notebook aborda várias etapas fundamentais do processo de análise de dados, incluindo extração, limpeza, transformação e agrupamento de dados. Abaixo, você encontrará uma visão geral de cada seção do notebook.

## Índice

1. [Preparar arquivos JSON](#prepare-json-files)
2. [Preparar DataFrames](#prepare-dataframes)
3. [Criação de um corpus](#creating-a-corpus)
4. [Função de remoção de ruído](#remove-noise-function)
5. [Criação da matriz tfidf](#creating-tfidf_matrix)
6. [Agrupamento com K-Means](#agrupamento-com-k-means)
7. [Visualização de dados](#visualização-de-dados)
8. [Criação de um contexto Spark e leitura dos dados](#criação-de-um-contexto-spark-e-leitura-dos-dados)
9. [Criação de um pipeline e agrupamento usando o algoritmo K-Means](#creating-a-pipeline-and-clustering-using-k-means-algorithm)

## 1. Preparar arquivos JSON

Esta seção demonstra como extrair dados de vagas de sites usando o Scrapy. Ela fornece código Python para definir spiders do Scrapy, executá-los e salvar os dados extraídos no formato JSON.

## 2. Preparar DataFrames

Nesta seção, o notebook lê os arquivos JSON criados anteriormente e tenta criar dois DataFrames do Pandas, ‘df1’ e ‘df2’. Ele também inclui uma função de limpeza de dados para limpar os dados. Se os arquivos JSON não puderem ser carregados, ele exibe uma mensagem de erro.

