# Aula 02 - Fundamentos da Linguagem 🧱
## Variáveis, Tipos e Controle de Fluxo

---

## Agenda de Hoje 📅

1. Variáveis e Declaração Curta <!-- .element: class="fragment" -->
2. Tipos de Dados Primitivos <!-- .element: class="fragment" -->
3. Constantes e Iota <!-- .element: class="fragment" -->
4. Estruturas Condicionais (If/Switch) <!-- .element: class="fragment" -->
5. Repetição: O Poder do For <!-- .element: class="fragment" -->
6. Mini-Projeto: Calculadora IMC <!-- .element: class="fragment" -->

---

## 1. Declarando Variáveis 📦

- **Forma Explícita**: `var nome string = "Gopher"` <!-- .element: class="fragment" -->
- **Forma Curta**: `idade := 25` <!-- .element: class="fragment" -->
- **Zero Values**: Int (0), String (""), Bool (false). <!-- .element: class="fragment" -->

---

## 2. Tipos Primitivos 💎

- Inteiros: `int`, `int64`, `uint`. <!-- .element: class="fragment" -->
- Decimais: `float32`, `float64`. <!-- .element: class="fragment" -->
- Booleano: `bool`. <!-- .element: class="fragment" -->
- Texto: `string` (Imutável). <!-- .element: class="fragment" -->

> [!WARNING]
> Go não converte tipos automaticamente! `int + float64` causa erro.

---

## 3. Controle de Fluxo: If/Else 🚦

- Não usa parênteses. <!-- .element: class="fragment" -->
- Chaves `{}` são obrigatórias. <!-- .element: class="fragment" -->

```go
if idade >= 18 {
    fmt.Println("Adulto")
} else {
    fmt.Println("Menor")
}
```

---

## 4. O Switch "Inteligente" 💡

- Não precisa de `break`. <!-- .element: class="fragment" -->
- Pode avaliar condições complexas. <!-- .element: class="fragment" -->

```go
switch {
case nota >= 7:
    fmt.Println("Aprovado")
case nota >= 5:
    fmt.Println("Recuperação")
default:
    fmt.Println("Reprovado")
}
```

---

## 5. Estruturas de Repetição 🔁

- **O Único Loop**: `for`. <!-- .element: class="fragment" -->

```go
// Estilo C
for i := 0; i < 5; i++ { ... }

// Estilo While
for x < 10 { ... }

// Infinito
for { ... }
```

---

## 6. Diagrama de Fluxo 📊

```mermaid
graph TD
    A[Start] --> B{x > 0?}
    B -- Sim --> C[Positivo]
    B -- Não --> D[Negativo/Zero]
    C --> E[End]
    D --> E
```

---

## 7. Mini-Projeto: Calculadora IMC 🚀

```go
func main() {
    peso := 70.0
    altura := 1.75
    imc := peso / (altura * altura)
    fmt.Printf("Seu IMC é: %.2f\n", imc)
}
```

---

## Resumo da Aula ✅

- Go é estaticamente tipado e seguro. <!-- .element: class="fragment" -->
- Controle de fluxo simples e direto. <!-- .element: class="fragment" -->
- O `for` é a ferramenta universal de repetição. <!-- .element: class="fragment" -->

---

## Próxima Aula: Funções e Organização 🧩

- Múltiplos retornos. <!-- .element: class="fragment" -->
- Ponteiros (sem medo!). <!-- .element: class="fragment" -->
- Pacotes e Módulos. <!-- .element: class="fragment" -->
