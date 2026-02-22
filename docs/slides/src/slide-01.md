# Aula 01 - Introdução ao Go e Ecossistema 🐹
## A Linguagem do Google para a Nuvem

---

## Agenda de Hoje 📅

1. Origens e Filosofia do Go { .fragment }
2. Diferenciais com outras linguagens { .fragment }
3. Instalação e Setup { .fragment }
4. O Arquivo go.mod { .fragment }
5. "Hello World" na prática { .fragment }
6. O Ecossistema e a Comunidade { .fragment }

---

## 1. Por que o Go nasceu? 🐣

- Criado no **Google** (2007) por: { .fragment }
    - *Robert Griesemer, Rob Pike e Ken Thompson*. { .fragment }
- **Problemas reais**: { .fragment }
    - Compilação lenta (C++). { .fragment }
    - Dependências complexas. { .fragment }
    - Dificuldade com multicore (concorrência). { .fragment }

---

## 2. Filosofia: "Menos é Mais" 🧊

- Simplicidade acima de tudo. { .fragment }
- Uma única forma de fazer as coisas. { .fragment }
- Foco em **legibilidade** e **manutenibilidade**. { .fragment }
- Binários estáticos e rápidos. { .fragment }

---

## 3. Go vs Outras Linguagens 🥊

| Recurso | Go | Python | Java |
| :--- | :--- | :--- | :--- |
| Velocidade | ⚡ Alta | 🐢 Baixa | 🐎 Média |
| Tipagem | Estática | Dinâmica | Estática |
| Concorrência | Nativa | Complexa | Pesada |
| Binário | Único | Precisa Interpreter | Precisa JVM |

---

## 4. O Ecossistema Go 🐹

```mermaid
graph TD
    Tools[Go Toolchain] --> Comp[Compiler]
    Tools --> Test[Test Runner]
    Tools --> Mod[Go Modules]
    Tools --> Doc[Go Doc]
    Tools --> Fmt[Go Fmt]
    style Tools fill:#00add8,stroke:#333
```

---

## 5. Setup do Ambiente 🚀

---

## Passo a Passo:

1. Baixar em [go.dev/dl](https://go.dev/dl). { .fragment }
2. Extensão Go no **VS Code**. { .fragment }
3. Verificar versão: `go version`. { .fragment }

---

## 6. O Primeiro Programa 📝

```go
package main

import "fmt"

func main() {
    fmt.Println("Olá, Gopher! 🐹")
}
```

---

## 7. Módulos e Dependências 📂

- O arquivo `go.mod` é o coração do projeto. { .fragment }
- Comando: `go mod init meu-projeto`. { .fragment }
- Gerencia versões de bibliotecas externas de forma segura. { .fragment }

---

## 8. Termynal na Prática 💻

```termynal
$ go mod init aula01
$ go run main.go
Olá, Gopher! 🐹
$ go build main.go
$ ./main
```

---

## Resumo da Aula ✅

- Go une a eficiência do C com a simplicidade do Python. { .fragment }
- É a linguagem oficial da infraestrutura moderna (Docker, K8s). { .fragment }
- Simplicidade gera produtividade em times grandes. { .fragment }

---

## Próxima Aula: Fundamentos 🧱

- Variáveis e Tipos. { .fragment }
- Controle de Fluxo. { .fragment }
- Loops (o único `for`!). { .fragment }

---

## Dúvidas? 🤔

> "O código deve ser escrito para que humanos o leiam, e apenas incidentalmente para que máquinas o executem."
