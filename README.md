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

## 3. Criação de um corpus

Esta parte do notebook inicializa uma lista vazia para armazenar cargos e percorre a coluna ‘jobTitle’ dos DataFrames para criar um corpus de cargos.

## 4. Função de remoção de ruído

Aqui, o notebook define uma função para remover ruído dos dados de texto usando a biblioteca NLTK. Ela remove caracteres não alfanuméricos, converte tokens para minúsculas e elimina palavras irrelevantes.

## 5. Criação da matriz tfidf_matrix

Esta seção envolve a criação de uma matriz TF-IDF a partir do corpus de cargos. Ela utiliza o TfidfVectorizer da biblioteca Scikit-Learn para converter os dados de texto em um formato numérico para análise posterior.

## 6. Agrupamento com K-Means

Nesta parte, o notebook aplica o algoritmo de agrupamento K-Means para agrupar cargos com base em suas representações TF-IDF. Ele usa a classe KMeans do Scikit-Learn para criar clusters e atribui rótulos de cluster aos cargos.
