# Exercícios: Interfaces e Composição 🧩

!!! info "Instruções"
    Aplique os conceitos de Polimorfismo e Composição em Go.

---

### 🟢 Nível: Básico

1.  **Interfaces**: Crie uma interface chamada `Forma` com o método `Area() float64`.
2.  **Implementação**: Crie uma struct `Quadrado` (com campo `Lado`) que implemente a interface `Forma`.

---

### 🟡 Nível: Intermediário

3.  **Múltiplas Formas**: Crie uma struct `Circulo` (com campo `Raio`) que também implemente `Forma`. Crie uma função que receba um slice de `Forma` e imprima a área de cada uma.
4.  **Composição**: Crie uma struct `Endereco` (Rua, Cidade) e uma struct `Pessoa` que contenha um `Endereco` via composição (embedding). Imprima os dados da pessoa e seu endereço.

---

### 🔴 Nível: Desafio

5.  **Simulador de Notificações**: Crie uma interface `Notificador` com o método `Enviar(mensagem string)`. Implemente dois tipos: `Email` e `SMS`. Crie uma função que receba um `Notificador` e dispare uma mensagem de "Bem-vindo" usando ambos os tipos.