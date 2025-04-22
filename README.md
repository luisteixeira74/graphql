# graphql

lib para criar uma estrutura pronta para GraphQL

https://gqlgen.com/


para baixar uma estrutura

go run github.com/99designs/gqlgen init

Exec "go run ./server.go" to start GraphQL server

Gerar o schema

go run github.com/99designs/gqlgen generate

> Esse projeto usa Query/SQL manual (sem ORM) e necessita criar as tabelas

# Acessar o DB

sqlite3 data.db

# Rodar os scripts

CREATE TABLE categories (id string, name string, description string)
CREATE TABLE courses (id string, name string, description string, category_id string)
