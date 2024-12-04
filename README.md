# NLP_DSM_6_Semestre
Repositório para arquivos referente a atividade final do Curso de Desenvolvimento de Software Multiplataforma da disciplina Processamento de Linguagem Natural

Integrantes:

Leonardo Rodrigues Dezoti Ferraz

Lucas Augusto Borges Rogatto

Vitor Gabriel Montini Melo



Análise de Emoções em Textos

Descrição e Motivação do Problema:
O objetivo deste projeto é desenvolver um modelo de aprendizado de máquina para identificar emoções em textos, utilizando postagens de redes sociais. 
A classificação de emoções é uma ferramenta poderosa em áreas como análise de sentimentos, marketing e saúde mental.



Descrição da Base de Dados:

Fonte: Dataset adiquirido no site da Kaggle contendo 5.250 postagens em redes sociais, cada uma classificada em diferentes categorias emocionais, como alegria, raiva, tristeza, e surpresa.

Distribuição: Classes bem distribuídas para evitar viés no treinamento.

Processo de Obtenção: Dataset foi obtido em formato público e preprocessado para adequação ao modelo.



Objetivo de Negócio ou Científico

Criar um modelo que possa ser utilizado para:

-Compreender a percepção do público em campanhas publicitárias.

-Monitorar emoções relacionadas a saúde mental em grandes populações.

-Estudar padrões emocionais em textos para fins científicos.



Etapa de Limpeza e Pré-Processamento:

-Remoção de URLs, menções e caracteres especiais.

-Conversão de textos para letras minúsculas.

-Remoção de palavras irrelevantes (stopwords) e aplicação de stemming para reduzir palavras às suas raízes.


Extração de Características:

-Utilizamos o TfidfVectorizer para transformar os textos em representações numéricas, considerando unigramas e bigramas.

-Configuramos o vetorizador para capturar os padrões mais relevantes nos dados.



Modelos de Machine Learning:

-Inicialmente, foi testado o modelo Naive Bayes.

-Após melhorias, utilizamos a Regressão Logística, que apresentou resultados superiores.



Protocolo de Experimentos e Validação:

O dataset foi dividido em:

70% para treinamento.

15% para validação.

15% para teste.

-Avaliação do modelo foi feita com métricas como precisão, recall e F1-score.



Discussão dos Resultados e Trabalhos Futuros:

Resultados: O modelo final apresentou um F1-score médio de 0.85 no conjunto de validação.

Trabalhos Futuros:

-Experimentar modelos mais avançados, como BERT.

-Ampliar o dataset para melhorar a generalização.

-Implementar uma interface para uso em tempo real.



Arquivos no Repositório

emotions.ipynb: Notebook principal com o pipeline do projeto.

tweet_emotions.csv: Dataset utilizado.

README.md: Este arquivo
