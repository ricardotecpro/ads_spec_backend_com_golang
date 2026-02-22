# Aula 09 - Programação Web com net/http 🌐
## Construindo a Base do seu Próprio Servidor

---

## Agenda de Hoje 📅

1. O Pacote `net/http` { .fragment }
2. Handlers: Response vs Request { .fragment }
3. Roteamento Simples { .fragment }
4. Middlewares e Interceptação { .fragment }
5. Servindo Arquivos Estáticos { .fragment }
6. Mini-Projeto: Contador de Visitas { .fragment }

---

## 1. O Servidor Nativo 📡

- Go não precisa de Nginx ou Apache para lógica. { .fragment }
- Binário **independente** e de **alta performance**. { .fragment }

```go
http.ListenAndServe(":8080", nil)
```

---

## 2. Handlers: A Alma da Web 🏗️

```go
func Handler(w http.ResponseWriter, r *http.Request) {
    // w: Onde eu escrevo (Response)
    // r: O que eu recebo (Request)
}
```

---

## 3. Fluxo de uma Requisição 📊

```mermaid
sequenceDiagram
    Cliente->>Servidor: Request (URL, Headers, Body)
    Servidor->>Handler: Processa Lógica
    Handler-->>Servidor: Gera bytes
    Servidor-->>Cliente: Response (Status, JSON/HTML)
```

---

## 4. Middlewares 🛡️

- "Camadas de cebola" ao redor do seu código. { .fragment }
- **Aplicações**: { .fragment }
    - Logs de acesso.
    - Verificação de Autenticação.
    - Rate Limiting.

---

## 5. Arquivos Estáticos 📁

```go
fs := http.FileServer(http.Dir("./public"))
http.Handle("/", fs)
```

- Simples, direto e seguro. { .fragment }

---

## 6. Mini-Projeto: Contador de Visitas 🚀

```go
var count int
func Counter(w http.ResponseWriter, r *http.Request) {
    count++
    fmt.Fprintf(w, "Visitas: %d", count)
}
```

---

## Resumo da Aula ✅

- `net/http` é tudo que você precisa para começar. { .fragment }
- ResponseWriter envia, Request recebe. { .fragment }
- Servidores em Go são leves e portáveis. { .fragment }

---

## Próxima Aula: APIs REST Profissionais 🏗️

- Modelagem e Camadas. { .fragment }
- JSON e Verbos HTTP.

---

## Dúvidas? 🤔

> "A Web é feita de requisições e respostas. Go é o mestre de ambas."
