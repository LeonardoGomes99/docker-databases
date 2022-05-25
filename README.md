# Docker Databases

> Esse projeto está sujeito a mudanças de porta entre outras configurações alteradas no docker-compose.yml

## 💻 Pré-requisitos

Antes de começar, verifique se você atendeu aos seguintes requisitos:
<!---Estes são apenas requisitos de exemplo. Adicionar, duplicar ou remover conforme necessário--->
* Você instalou a versão mais recente de `Docker e Docker Compose`

### Credencias (Username e senhas)

O projeto ainda está em desenvolvimento e está sujeito a mudanças

- mysql (porta 5433) :
  user: root , password: *vazio* , database: database

- postgres (porta 5432) :
  user: user , password: password , database: database

- mongoDB : porta (5434)

## 🚀 Usando docker-database

Para usar esse projeto, siga estas etapas:

```
após clonar o repositório entre em qual DB voce deseja usar
```

```
após entrar na pasta do DB que escolheu, irá encontrar o arquivo *docker-compose.yml*
```

```
abra o terminal na pasta e rode o comando * docker-compose up -d * para começar a construir o seu container
```

```
assim que finalizar a construção voce já pode realizar a conexão ao banco e utilizar
```

```
caso queira encerrar a execução do DB, rode o comando * docker-compose up -d * dentro da pasta do próprio
```
