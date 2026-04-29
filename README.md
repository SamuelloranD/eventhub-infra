# EventHub - Infraestrutura

## Sobre o projeto
O EventHub é um sistema de gerenciamento de eventos, permitindo o cadastro, listagem e inscrição de participantes.

Este repositório é responsável pela **infraestrutura do projeto**, utilizando Docker para orquestrar os serviços.

---

## Tecnologias utilizadas
- Docker
- Docker Compose
- PostgreSQL
- Spring Boot
- React

---

## Pré-requisitos
Antes de iniciar, você precisa ter instalado:

- Docker Desktop
- Docker Compose (já incluso no Docker Desktop)

---

## Como executar o projeto

```bash
git clone https://github.com/SamuelloranD/eventhub-backend
git clone https://github.com/SamuelloranD/eventhub-infra
cd eventhub-infra
docker-compose up --build
```
## Acessos
- Backend: http://localhost:8080/test

## Configuração do Banco de Dados
Host: localhost
Porta: 5432
Database: eventhub
Usuário: postgres
Senha: postgres

## Estrutura dos serviços
db → PostgreSQL rodando em container
backend → API Spring Boot rodando em container
## Observações
O banco de dados é criado automaticamente ao subir o container
O backend se conecta ao banco usando o nome do serviço (db)
Não é necessário instalar PostgreSQL localmente
Caso já exista algo rodando na porta 5432, pode ocorrer conflito

## 👨‍💻 Grupo
- Samuel Araujo
- José Pereira Neto
- José Mailson
