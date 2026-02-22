# Projeto Final: Checklist de Entrega 🏆

!!! info "Instruções"
    Utilize este checklist para garantir que seu projeto final atenda a todos os requisitos de qualidade e funcionalidade.

---

### ✅ Requisitos de Funcionalidade

1.  [ ] A rota `POST /livros` funciona corretamente?
2.  [ ] A rota `POST /emprestimos` valida se o livro está disponível antes de concluir?
3.  [ ] É possível listar todos os empréstimos realizados?

---

### ✅ Requisitos Técnicos

4.  [ ] O código está organizado em pastas seguindo a Clean Architecture?
5.  [ ] O banco de dados PostgreSQL sobe corretamente via `docker-compose up`?
6.  [ ] Existe ao menos um arquivo `_test.go` com testes passando?

---

### 🚀 Desafio Extra (Opcional)

7.  [ ] **Autenticação**: Adicione um middleware de proteção simples (API Key) em rotas de cadastro.
8.  [ ] **Swagger**: Gere a documentação Swagger da sua API final.
9.  [ ] **Deploy**: Realize o deploy da imagem Docker em algum serviço gratuito (como Render ou Fly.io).