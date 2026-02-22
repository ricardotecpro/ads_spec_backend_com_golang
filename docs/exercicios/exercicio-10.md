# Exercícios: Construindo APIs REST 🏗️

!!! info "Instruções"
    Organize seu código e implemente padrões RESTful.

---

### 🟢 Nível: Básico

1.  **Camadas**: Crie uma pasta `models` e mova uma struct de sua escolha para lá. Importe-a no seu `main.go`.
2.  **Verbo POST**: Crie um handler que receba um JSON e apenas o imprima no console do servidor.

---

### 🟡 Nível: Intermediário

3.  **Busca por ID**: Implemente uma lógica que, dada uma lista de produtos, retorne apenas o produto que tenha o ID passado na URL (Dica: use `strings.Split` no Path para pegar o ID).
4.  **Status Codes**: Garanta que sua API retorne `201 Created` ao criar um recurso e `404 Not Found` se um recurso solicitado não existir na lista.

---

### 🔴 Nível: Desafio

5.  **CRUD In-Memory**: Crie um CRUD completo (Create, Read, Update, Delete) para uma struct `Cliente` usando apenas o pacote `net/http` e um slice global para armazenar os dados. Teste cada rota usando o Postman ou Insomnia.