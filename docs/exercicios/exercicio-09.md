# Exercícios: Programação Web com net/http 🌐

!!! info "Instruções"
    Pratique a criação de servidores e manipulação de requisições HTTP.

---

### 🟢 Nível: Básico

1.  **Servidor Simples**: Crie um servidor que responda "Bem-vindo ao Go Web!" na rota `/home`.
2.  **Portas**: Tente rodar dois servidores Go simultâneos em portas diferentes (ex: 8080 e 9090).

---

### 🟡 Nível: Intermediário

3.  **Status Codes**: Crie um handler que verifique se um parâmetro `admin` na URL é igual a `true`. Se for, responda `200 OK`. Se não, responda `403 Forbidden`.
4.  **JSON Response**: Modifique seu handler para que ele retorne um JSON simples: `{"status": "ativo", "mensagem": "API rodando"}`. Lembre-se de definir o `Content-Type` como `application/json`.

---

### 🔴 Nível: Desafio

5.  **Calculadora Web**: Crie um servidor que receba dois números via Query Params (ex: `/?a=10&b=5`) e uma operação (`op=soma`). O servidor deve realizar o cálculo e retornar o resultado em texto puro. Trate o erro caso os valores não sejam números válidos.