# Exercícios: Arquitetura e Boas Práticas 🏗️

!!! info "Instruções"
    Aplique padrões de design para criar códigos mais limpos e testáveis.

---

### 🟢 Nível: Básico

1.  **Refatoração**: Mova sua struct principal para uma pasta chamada `entities`.
2.  **Interface**: Crie uma interface que defina as operações básicas de persistência de um objeto seu (ex: `Salvar`, `BuscarPorID`).

---

### 🟡 Nível: Intermediário

3.  **Injeção**: Crie uma struct `Gestor` que possua um campo que é a interface do exercício anterior. Crie uma função `NewGestor` para injetar a implementação.
4.  **Internal**: Mova sua lógica de banco de dados para uma pasta `internal/repository` e verifique como as permissões de acesso funcionam entre pacotes.

---

### 🔴 Nível: Desafio

5.  **Mock Manual**: Escreva um teste para o seu `Gestor` (do exercício 3). No teste, crie uma struct "fake" que implementa a interface de repositório (sem usar banco real) e injete-a no gestor. Verifique se o gestor chama os métodos corretamente.