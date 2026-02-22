# Exercícios: Banco de Dados (GORM) 💾

!!! info "Instruções"
    Pratique a integração de banco de dados em aplicações Go.

---

### 🟢 Nível: Básico

1.  **Conexão**: Crie um programa que conecte a um banco SQLite local chamado `estudos.db`.
2.  **Model**: Crie uma struct `Livro` e use o `AutoMigrate` para criar essa tabela no banco.

---

### 🟡 Nível: Intermediário

3.  **Seed**: Crie uma função que insira 5 livros iniciais no banco caso a tabela esteja vazia.
4.  **Busca**: Escreva uma consulta GORM que retorne todos os livros com preço maior que 50 reais.

---

### 🔴 Nível: Desafio

5.  **API Persistente**: Crie duas rotas no Gin: `GET /livros` (lista todos do banco) e `POST /livros` (salva um novo no banco). Verifique se os dados permanecem salvos mesmo após reiniciar o servidor.