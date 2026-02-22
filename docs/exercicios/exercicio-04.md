# Exercícios: Estruturas de Dados Avançadas 🗄️

!!! info "Instruções"
    Exercite o uso de Slices, Maps e Structs em Go.

---

### 🟢 Nível: Básico

1.  **Slices**: Crie um slice de strings com 3 nomes de cidades. Use `append` para adicionar uma quarta cidade.
2.  **Maps**: Crie um mapa que armazena nomes de países (chave) e suas capitais (valor). Imprima a capital do Brasil.

---

### 🟡 Nível: Intermediário

3.  **Structs**: Defina uma struct `Produto` com `Nome`, `Preco` e `Quantidade`. Crie uma instância e imprima o valor total em estoque (`Preco * Quantidade`).
4.  **Slicing**: Dado o slice `numeros := []int{10, 20, 30, 40, 50}`, extraia um novo slice que contenha apenas os valores `20, 30, 40`.

---

### 🔴 Nível: Desafio

5.  **Sistema de Estoque**: Crie um programa que use um `map[string]Produto`. O usuário deve poder digitar o nome de um produto e o programa exibe todos os detalhes daquela struct `Produto`. Se o produto não existir, exiba uma mensagem de erro.
