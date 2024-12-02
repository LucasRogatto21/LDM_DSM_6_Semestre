# LDM_DSM_6_Semestre
Repositório para arquivos referente a atividade final do curso Laboratório de Desenvolvimento Multiplataforma

Integrantes:

Davi Aquila Sirqueira da Silva
João Vitor Moreira Mariano da Silva
Leonardo Rodrigues Dezoti Ferraz
Lucas Augusto Borges Rogatto
Pedro Henrique Pires de Godoy
Vitor Gabriel Montini Melo


Linhas Itapira

Este projeto foi desenvolvido para Web, Desktop e Mobile, com o objetivo de fornecer informações sobre as linhas e horários de ônibus, além da funcionalidade de visualizar a localização em tempo real dos ônibus em um mapa.

A solução foi construída utilizando quatro serviços da AWS para garantir alta performance, escalabilidade e segurança:

-Amazon EC2: Utilizado como servidor para hospedar o projeto e o banco de dados relacional, oferecendo flexibilidade na configuração do ambiente.

-Amazon DynamoDB: Armazena as coordenadas das localizações dos ônibus em um banco de dados NoSQL, garantindo escalabilidade automática e alto desempenho.

-AWS Lambda: Contém a função responsável por consultar a localização dos ônibus e enviar essas informações para a API, de forma rápida e econômica.

-Amazon API Gateway: Gerencia a API que entrega as informações da localização dos ônibus, fornecidas pelo AWS Lambda, até o projeto, com configuração simples e comunicação segura.


Ferramentas Utilizadas:

-Visual Studio Code: Conectado ao Amazon EC2 via SSH para o desenvolvimento e manutenção do código.


Implementações:
O código foi ajustado para, em vez de consultar o MongoDB como no projeto original, se preparar para receber informações da API, tratá-las e utilizá-las.

Desenvolvido em Python:
Função Lambda para consultar e enviar a localização dos ônibus em formato JSON.
Simulação da atualização em tempo real das localizações no DynamoDB.


Funcionalidades:
-Integração em tempo real das localizações no mapa, acessível via Web, Desktop e Mobile.
-Tratamento eficiente dos dados para garantir a entrega correta e rápida das informações.

Segurança e Permissões
IAM (Identity and Access Management):
Utilizado o perfil LabRole para conectar os serviços da AWS entre si, garantindo que cada serviço tenha as permissões necessárias para executar suas funções.

Práticas de Segurança:
Uso de chaves privadas para acessar a instância Amazon EC2 via SSH, garantindo uma conexão segura.
