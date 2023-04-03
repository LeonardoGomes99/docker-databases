# Bem Vindo ao Docker-Databases!

O repositório **docker-databases** é um projeto que contém um conjunto de arquivos Docker e Docker Compose para configurar e executar bancos de dados MongoDB, MySQL, PostgreSQL e SQL Server em contêineres separados.


Os arquivos Docker e Docker Compose fornecidos são bem documentados e configuráveis, permitindo que você adapte as configurações para suas necessidades específicas. Com este repositório, é possível simplificar a criação e gerenciamento de ambientes de bancos de dados utilizando o poder do Docker e dos contêineres.

## 💻  Pré-requisitos

* Docker
* Docker Compose

## 🚀  Utilizando docker-database
Assim que você terminar de configurar docker & docker-compose, entra na pasta do projeto e gere o arquivo .env apartir do .env.example que já contém no repositório e assim rode o comando.
>docker-compose up -d nome_do_banco

Atenção!!!
se você rodar apenas o comando
> docker-compose up -d

o docker irá iniciar todos os bancos de dados.

assim que você executar o comando, o sistema iniciará o download das imagens e montara o ambiente para o seu banco de dados! 

caso esteja em dúvida como rodar os bancos que estão presentes no projeto. 
>docker-compose up -d db_postgres
>docker-compose up -d db_mysql
>docker-compose up -d db_mongodb
>docker-compose up -d db_sql-server

caso queira editar as credencias de cada ambiente como [ username | password | database_name | port ] , edite o arquivo .env e coloque as credenciais desejáveis. Depois das alterações rode o comando

caso os containers já estejam rodando no sistema, pare-os e rebuild.
rode os seguintes comandos.
>docker-compose down 

assim que parar os containers utilize o comando.

>docker-compose up --build -d nome_do_banco

assim o containers vão ser reconfigurados.

## 🚀  Credênciais Default
POSTGRES:
* POSTGRES_DB: database_postgres
* POSTGRES_USER: postgres
* POSTGRES_PASSWORD: 123456
* PORT: 5432

MYSQL:
 * MYSQL_DB: database_mysql
 * MYSQL_USER: root
 * MYSQL_PASSWORD: **vazio**
 * PORT: 5433

MONGODB:
* PORT: 5434
* PUID=1000
* PGID=1000

SQL SERVER:
* DATABASE_PID_SQLSERVER=Developer
* DATABASE_PASS=Password123!#
* USERNAME=sa
* PORT: 1433

## ![Document em LG G5](https://em-content.zobj.net/thumbs/120/lg/57/document_1f5ce.png)  Obrigado!
Caso tenha alguma sugestão para melhoria da [ documentação / projeto ] por favor comente!
no caso peço que crie uma issue apontando as melhorias!
