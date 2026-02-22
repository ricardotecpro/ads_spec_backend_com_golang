# Aula 03 - Funções e Organização do Código 🧩
## Estruturando Projetos de Forma Profissional

---

## Agenda de Hoje 📅

1. Anatomia de uma Função <!-- .element: class="fragment" -->
2. Retornos Múltiplos e Variádicos <!-- .element: class="fragment" -->
3. Ponteiros: Endereços vs Valores <!-- .element: class="fragment" -->
4. Visibilidade (Exportação) <!-- .element: class="fragment" -->
5. Módulos e Gestão de Pacotes <!-- .element: class="fragment" -->
6. Mini-Projeto: Conversos Modular <!-- .element: class="fragment" -->

---

## 1. Funções em Go ⚙️

- Funções são blocos independentes. <!-- .element: class="fragment" -->
- **Cidadãs de 1ª Classe**: Podem ser variáveis e argumentos. <!-- .element: class="fragment" -->

```go
func somar(a int, b int) int {
    return a + b
}
```

---

## 2. O Diferencial: Retornos Múltiplos 🔄

- Útil para retornar o dado e o erro simultaneamente. <!-- .element: class="fragment" -->

```go
func dividir(a, b float64) (float64, error) {
    if b == 0 {
        return 0, errors.New("não pode dividir por 0")
    }
    return a / b, nil
}
```

---

## 3. Ponteiros: O Guia Definitivo 📍

- **Endereço (`&`)**: Onde o dado mora. <!-- .element: class="fragment" -->
- **Valor (`*`)**: O que tem dentro da casa. <!-- .element: class="fragment" -->

```go
func dobrar(n *int) {
    *n = *n * 2
}
```

> "Ponteiros economizam memória ao evitar cópias de objetos grandes." <!-- .element: class="fragment" -->

---

## 4. Organizando a Casa: Pacotes 📂

- Pastas = Pacotes. <!-- .element: class="fragment" -->
- **Exportação Camuflada**: <!-- .element: class="fragment" -->
    - `Calcular` (Maiúsculo) -> Público. <!-- .element: class="fragment" -->
    - `calcular` (Minúsculo) -> Privado do pacote. <!-- .element: class="fragment" -->

---

## 5. Estrutura de Projeto 🏗️

```termynal
$ tree
.
├── go.mod
├── main.go
└── conversor/
    └── temperatura.go
```

---

## 6. Diagrama de Módulo 📊

```mermaid
graph LR
    Main[main.go] -->|import| P1[Package 1]
    Main -->|import| P2[Package 2]
    P1 -->|internal| F1[Func Privada]
    P1 -->|exported| F2[Func Pública]
```

---

## Resumo da Aula ✅

- Go força uma organização clara por pastas. <!-- .element: class="fragment" -->
- Múltiplos retornos eliminam a necessidade de exceções globais. <!-- .element: class="fragment" -->
- Ponteiros dão controle total sobre a performance. <!-- .element: class="fragment" -->

---

## Próxima Aula: Estruturas de Dados 🗄️

- Slices: Arrays dinâmicos. <!-- .element: class="fragment" -->
- Maps: O dicionário do Go. <!-- .element: class="fragment" -->
- Structs: Criando seus tipos. <!-- .element: class="fragment" -->

---

## Dúvidas? 🤔

> "Um código bom é um código organizado."