# Projeto ETL 
## Objetivo

O objetivo do projeto é realizar um processo de ETL (Extração, Transformação e Carregamento) que consolide as bases de dados de Comunicação de Acidente de Trabalho (CAT) disponibilizadas em somente uma base consolidada. A base de dados de CAT é proveniente do sistema informatizado de Comunicação de Acidentes do Trabalho do INSS (CATWEB) e também de concessão de benefício por incapacidade acidentário, conforme estabelecido no Decreto nº 8.777/16 e Lei de Acesso à Informação nº 12.527/2011.

A base de dados original pode ser encontrada em dados.gov.br.

## Tecnologias Utilizadas

Para a realização do projeto, foram utilizadas as seguintes tecnologias:

- Python: Linguagem de programação utilizada para desenvolver o código do projeto.
- Pandas: Biblioteca em Python utilizada para a manipulação e análise de dados.
- PySpark: Biblioteca para processamento de big data, permitindo o processamento distribuído de dados em escala.
- MongoDB Atlas: Banco de dados NoSQL em nuvem, utilizado para armazenar os dados tratados.
- Google Cloud Storage (GCS): Serviço de armazenamento em nuvem do Google, utilizado para armazenar as bases de dados em formato raw e tratado.
- MySQL: Banco de dados relacional, utilizado para armazenar dados estruturados do projeto.

## Resumo do Notebook

O projeto foi desenvolvido em um ambiente Colab (Google Colaboratory) e está dividido em diferentes seções:

### 1. Instalações
Nesta seção, foram instaladas as bibliotecas necessárias para o desenvolvimento do projeto, como o PySpark, GCSFS, MySQL Connector, e outras.

### 2. Importações
Nesta seção, foram realizadas as importações das bibliotecas e pacotes que serão utilizados ao longo do notebook.

### 3. Enviar Dados ao MongoDB Atlas
Esta seção trata do envio dos dados tratados para o MongoDB Atlas, permitindo que os dados consolidados sejam armazenados em um banco de dados NoSQL.

### 4. Enviar Dados ao CloudStorage
Nesta seção, são configuradas as credenciais para acessar o Google Cloud Storage (GCS) e os dados tratados são enviados para o GCS em formato parquet.

### 5. Trabalhando com PySpark
Nesta seção, é utilizada a biblioteca PySpark para realizar as etapas de transformação dos dados. São criados DataFrames a partir das bases de dados CSV, realizada a concatenação dos DataFrames, tratamento de dados faltantes, limpeza e organização dos dados.

### 6. Trabalhando com Pandas
Nesta seção, é feita a conversão dos DataFrames do PySpark para Pandas para realizar análises exploratórias e encontrar possíveis inconsistências nos dados.

### 7. Análise com Pandas
São realizadas análises exploratórias utilizando a biblioteca Pandas, incluindo filtragem de dados, agrupamentos e plotagem de gráficos.

### 8. Análise com PySpark
Nesta seção, os DataFrames são transformados novamente para PySpark para realizar análises utilizando SparkSQL e funções de janela.

### 9. Salvando Dados Tratados
Os dados tratados são salvos em diferentes formatos, incluindo MongoDB Atlas, Google Cloud Storage e MySQL.

### 10. DASHBOARD LOOKER
Provavelmente, nesta seção, seria criada uma conexão do Looker (ou outra ferramenta de BI) para visualizar os dados de forma mais interativa e amigável.

## Conclusões das Análises

As conclusões das análises feitas com os dados estão disponíveis nos resultados encontrados nas seções de análise com Pandas e análise com PySpark. Nesses resultados, foram identificadas possíveis inconsistências nos dados, insights sobre os acidentes de trabalho, estatísticas relevantes, entre outras informações úteis para o entendimento e tomada de decisões a partir dos dados tratados.

## Contribuições

Este projeto está aberto para contribuições e melhorias. Caso tenha interesse em contribuir, fique à vontade para criar um fork deste repositório, realizar as melhorias desejadas e criar um pull request. Será um prazer revisar e incorporar suas contribuições ao projeto.

## Autor

Este projeto foi desenvolvido por Giovana de Brito Silva e Wilbert Silva durante o bootcamp de Engenharia de Dados da SoulCode Academy.
