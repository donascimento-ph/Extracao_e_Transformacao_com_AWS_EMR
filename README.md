# Processamento de Big Data com Amazon EMR e Dados da Redfin

Este projeto fornece um guia para o processamento de grandes volumes de dados usando Amazon EMR (Elastic MapReduce) em combinação com dados da Redfin, uma fonte de informações imobiliárias. As ferramentas e abordagens utilizadas são explicadas a seguir:

## 1. Introdução ao Amazon EMR

Amazon EMR é um serviço de gerenciamento de clusters que simplifica a implantação e a escalabilidade de estruturas de processamento de dados, como Apache Hadoop, Apache Spark e outros, em uma infraestrutura flexível e altamente escalável na AWS. Ele automatiza tarefas complexas de configuração, gerenciamento e escalabilidade de clusters, permitindo que os profissionais de dados se concentrem no que é realmente importante: a análise de dados e insights.

## 2. Configuração de um Ambiente VPC

Uma Virtual Private Cloud (VPC) é um serviço da Amazon Web Services (AWS) que permite criar uma rede virtual isolada, na qual você tem total controle sobre a configuração da rede, incluindo sub-redes, tabelas de roteamento e gateways. Ela é um componente fundamental para a criação de ambientes seguros e isolados na nuvem AWS. Para garantir um ambiente de processamento seguro e isolado ao trabalhar com dados sensíveis e de grande escala, é essencial criar uma VPC.

## 3. Provisionamento de Clusters EMR

Clusters EMR são provisionados dentro da VPC para fornecer poder de processamento escalável e sob demanda. Isso permite que você execute tarefas de análise de dados em grande escala.

## 4. Criação do Amazon EMR Studio e JupyterLab

O Amazon EMR Studio é um ambiente de desenvolvimento e análise totalmente integrado que simplifica o processo de trabalhar com clusters EMR. Ele oferece uma interface unificada e colaborativa que permite que você execute código, visualize resultados e colabore com colegas.

Por que Usar o JupyterLab?

O JupyterLab é uma aplicação web que fornece uma interface flexível e extensível para a criação de notebooks Jupyter interativos. Ele é amplamente utilizado para escrever código, executar análises de dados, criar visualizações e documentar o trabalho de processamento de dados.

## 5. Conexão de Notebooks Jupyter

A conexão de notebooks Jupyter a um cluster EMR é fundamental para realizar análises de big data de forma interativa e eficaz. Isso permite que você execute consultas, processe dados e visualize resultados diretamente no ambiente EMR, aproveitando a capacidade de processamento do cluster.

## 6. Processamento de Dados com PySpark

O código Python com PySpark é utilizado para extrair dados da fonte Redfin, realizar transformações e salvar os dados em um formato eficiente. Aqui estão as etapas-chave:

- Os dados são extraídos da fonte Redfin e carregados no ambiente PySpark.
- Os dados são limpos e as informações nulas são tratadas.
- Colunas de data são transformadas em ano e mês.
- Colunas irrelevantes são removidas.
- Os meses são mapeados para seus nomes correspondentes.

Os dados transformados são, então, salvos no formato Parquet em um bucket Amazon S3, tornando-os acessíveis e eficientes para futuras análises.

Este projeto serve como um guia para lidar com grandes conjuntos de dados usando Amazon EMR e demonstra como aproveitar essa poderosa ferramenta para extrair e transformar dados da Redfin de forma eficaz.


 
