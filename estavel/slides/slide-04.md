# Aula 04 - Estruturas de Dados Avançadas 🗄️
## Gerenciando Coleções e Tipos Customizados

---

## Agenda de Hoje 📅

1. Arrays vs Slices <!-- .element: class="fragment" -->
2. Manipulação de Slices (Append/Slice) <!-- .element: class="fragment" -->
3. Maps: Chave e Valor <!-- .element: class="fragment" -->
4. Structs: O Coração dos Dados <!-- .element: class="fragment" -->
5. Métodos e Comportamento <!-- .element: class="fragment" -->
6. Mini-Projeto: Escola de Gophers <!-- .element: class="fragment" -->

---

## 1. Arrays vs Slices 🍕

- **Arrays**: Rígidos, tamanho faz parte do tipo. <!-- .element: class="fragment" -->
- **Slices**: Flexíveis, dinâmicos. O "padrão" do Go. <!-- .element: class="fragment" -->

```go
// Array
var a [2]string

// Slice
s := []string{"A", "B"}
s = append(s, "C")
```

---

## 2. Anatomia de um Slice 🔍

```mermaid
graph LR
    subgraph "Capacidade (Reservado)"
        D3[Elemento 3]
        D4[Vazio]
    end
    subgraph "Slice (Existente)"
        D1[Elemento 1]
        D2[Elemento 2]
    end
    Ptr[Ponteiro] --> D1
```

---

## 3. Maps: O Dicionário Veloz 🗝️

- Coleção de pares chave-valor. <!-- .element: class="fragment" -->
- Chaves devem ser comparáveis. <!-- .element: class="fragment" -->

```go
estoque := make(map[string]int)
estoque["teclado"] = 50

valor, existe := estoque["mouse"]
```

---

## 4. Structs: Seus Próprios Tipos 🏗️

- Go não tem classes, tem Structs. <!-- .element: class="fragment" -->
- Agrupam dados de tipos diferentes. <!-- .element: class="fragment" -->

```go
type Aluno struct {
    Nome  string
    Idade int
    Notas []float64
}
```

---

## 5. Adicionando Comportamento (Métodos) ⚡

- Funções "anexadas" a um tipo. <!-- .element: class="fragment" -->

```go
func (a Aluno) Media() float64 {
    total := 0.0
    for _, n := range a.Notas {
        total += n
    }
    return total / float64(len(a.Notas))
}
```

---

## 6. Mini-Projeto: Escola de Gophers 🚀

- Criar um sistema que armazena alunos em um `map`. <!-- .element: class="fragment" -->
- Cada aluno é uma `struct`. <!-- .element: class="fragment" -->
- Calcular e exibir médias. <!-- .element: class="fragment" -->

---

## Resumo da Aula ✅

- Slices são extensões dinâmicas de memória. <!-- .element: class="fragment" -->
- Maps oferecem performance em buscas por chaves. <!-- .element: class="fragment" -->
- Structs modelam o domínio do seu negócio. <!-- .element: class="fragment" -->

---

## Próxima Aula: Interfaces e Flexibilidade 🧩

- O segredo do Polimorfismo em Go. <!-- .element: class="fragment" -->
- Programação baseada em Composição. <!-- .element: class="fragment" -->

---

## Dúvidas? 🤔

> "A estrutura de dados correta resolve metade do problema."
