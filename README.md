## 📦 GraphQL com Go usando gqlgen

**Pronúncia:** *Graph-Queue-Well*

### 🎤 Como se pronuncia "GraphQL"

**GraphQL**  
/\u02c8\u0261r\u00e6f.kju\u02d0.\u02c8w\u025bl/  
**[Graph-Queue-Well]**  
🔴 *Como se pronuncia:* **Graph** (como em "gráfico") + **Queue** (como "fila" em inglês) + **Well** (como "bem")  

🗣️ Exemplo de uso:  
> "Estamos desenvolvendo uma API usando **Graph-Queue-Well** para consultas flexíveis de dados."

---

### 🔗 Biblioteca utilizada
- [gqlgen](https://gqlgen.com/) — Biblioteca para criação de APIs GraphQL em Go.

---

### 🚀 Instruções para iniciar o servidor GraphQL

**1. Inicializar o projeto com gqlgen:**
```bash
go run github.com/99designs/gqlgen init
go mod tidy
```

**2. Gerar o schema (quando alterar os arquivos `.graphql`):**
```bash
go run github.com/99designs/gqlgen generate
```

**3. Iniciar o servidor:**
```bash
go run server.go
```
ou
```bash
go run ./server.go
```

---

### 💃 Banco de Dados

Este projeto **não utiliza ORM**. As queries SQL são feitas manualmente. É necessário criar as tabelas antes da execução.

**Acessar o banco SQLite:**
```bash
sqlite3 data.db
```

**Criar as tabelas:**
```sql
CREATE TABLE categories (
  id TEXT,
  name TEXT,
  description TEXT
);

CREATE TABLE courses (
  id TEXT,
  name TEXT,
  description TEXT,
  category_id TEXT
);
```

---

