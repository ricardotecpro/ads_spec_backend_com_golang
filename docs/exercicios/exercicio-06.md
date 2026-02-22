# Exercícios: Tratamento de Erros ⚠️

!!! info "Instruções"
    Pratique a captura e criação de erros em Go.

---

### 🟢 Nível: Básico

1.  **Check de Erro**: Escreva uma função que leia o nome de um arquivo do terminal e tente abri-lo usando `os.Open`. Trate o erro caso o arquivo não exista.
2.  **Panic**: Crie uma função que cause um `panic` propositalmente (ex: divisão por zero ou acesso a índice inexistente em slice).

---

### 🟡 Nível: Intermediário

3.  **Recover**: Use o `recover` para capturar o panic do exercício anterior e imprimir uma mensagem amigável sem derrubar o programa.
4.  **Custom Error**: Defina uma variável de erro `ErrIdadeInvalida` e use-a em uma função `VerificarIdade(idade int)`.

---

### 🔴 Nível: Desafio

5.  **Calculadora Segura**: Crie uma função `Dividir(a, b float64) (float64, error)`. Se `b` for 0, retorne um erro detalhado usando `fmt.Errorf` incluindo os valores de `a` e `b`. No `main`, execute essa função e trate o erro exibindo-o no console.