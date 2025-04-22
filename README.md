# graphQL (pronuncia graphQueueWell)

lib usada para criar uma estrutura GraphQL

https://gqlgen.com/

---

## Instrução do próprio gqlgen para iniciar o server

- Initialise gqlgen config and generate models
> go run github.com/99designs/gqlgen init
> go mod tidy

- Start the graphql server
> go run server.go

Exec "go run ./server.go" to start GraphQL server
Gerar o schema
go run github.com/99designs/gqlgen generate

---

> Esse projeto usa Query/SQL manual (sem ORM) e necessita criar as tabelas

# Acessar o DB

sqlite3 data.db

## Rodar os scripts

CREATE TABLE categories (id string, name string, description string)
CREATE TABLE courses (id string, name string, description string, category_id string)

---