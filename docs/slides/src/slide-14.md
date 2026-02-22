# Aula 14 - Arquitetura e Boas Práticas 🏗️
## Criando Sistemas Escaláveis e Fáceis de Manter

---

## Agenda de Hoje 📅

1. O Caos vs Organização { .fragment }
2. Clean Architecture em Go { .fragment }
3. Injeção de Dependência { .fragment }
4. Estrutura de Pastas (Padrão) { .fragment }
5. Visibilidade e o pacote `internal` { .fragment }
6. Mini-Projeto: Refatorando para DI { .fragment }

---

## 1. Clean Architecture 🧊

- **Mantra**: Independência de Framework e Banco. { .fragment }
- O código de negócio deve ser puro Go. { .fragment }

```mermaid
graph TD
    UI[Handlers] --> UC[UseCases]
    UC --> EN[Entities]
    UC --> DB[Repositories]
```

---

## 2. Injeção de Dependência (DI) 💉

- Não deixe a struct criar seu próprio Repository. { .fragment }
- **Dê** o repositório para ela (via construtor). { .fragment }

```go
func NewService(r Repository) *Service {
    return &Service{repo: r}
}
```

---

## 3. O Pacote `internal` ⚔️

- Protege o seu código de "vazar". { .fragment }
- Apenas pacotes dentro do módulo podem importá-lo. { .fragment }
- **Ideal para**: Lógica de banco e regras internas. { .fragment }

---

## 4. Estrutura de Pastas Profissional 📂

```termynal
$ tree
.
├── cmd/        # Entrypoints
├── internal/   # Core (Business)
├── pkg/        # Shared Libs
└── api/        # Docs/OpenAPI
```

---

## 5. Boas Práticas (Cringe Free) ✨

- Pacotes com nomes curtos: `user`, `auth`. { .fragment }
- Sem `utils` ou `helpers` genéricos. { .fragment }
- Retornos concretos, entradas abstratas. { .fragment }

---

## 6. Mini-Projeto: Refatorando 🚀

- Isolar a struct `Livro` em entitites. { .fragment }
- Criar interface `LivroRepository`. { .fragment }
- Fazer o Handler receber a interface. { .fragment }

---

## Resumo da Aula ✅

- Clean Arch foca no que Realmente Importa (Negócio). { .fragment }
- Injeção de Dependência facilita Testes Unitários. { .fragment }
- Estrutura de pastas reflete a maturidade do time. { .fragment }

---

## Próxima Aula: Docker e Deploy 🐳

- Indo para o mundo real.
- Containers e Infra.

---

## Dúvidas? 🤔

> "A arquitetura é o que permite que você mude de ideia depois."
