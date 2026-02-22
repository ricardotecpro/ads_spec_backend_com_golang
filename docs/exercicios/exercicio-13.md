# Exercícios: Testes em Go ✅

!!! info "Instruções"
    Garanta a qualidade do seu software com testes automatizados.

---

### 🟢 Nível: Básico

1.  **Unitário**: Crie uma função `Multiplicar(a, b int)` e escreva um teste unitário simples em um arquivo separado.
2.  **Execução**: Rode seus testes e gere um relatório de cobertura básico.

---

### 🟡 Nível: Intermediário

3.  **Table-Driven**: Transforme o teste da multiplicação em um teste de tabela com ao menos 5 cenários diferentes (incluindo números negativos e zero).
4.  **Error Testing**: Escreva um teste para uma função que retorna erro (ex: `Dividir`). Verifique se o erro retornado é o esperado quando tentamos dividir por zero.

---

### 🔴 Nível: Desafio

5.  **API Test**: Utilizando o pacote `net/http/httptest`, escreva um teste para um handler que retorna um JSON. O teste deve verificar se o Status Code é `200 OK` e se o corpo da resposta contém um campo específico.