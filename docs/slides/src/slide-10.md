# Aula 10 - Construindo APIs REST 🏗️
## Arquitetura Profissional e Design de Recursos

---

## Agenda de Hoje 📅

1. O que é REST na Prática? { .fragment }
2. Verbos HTTP e Semântica { .fragment }
3. Organização por Camadas (Pattern) { .fragment }
4. Status Codes: A Linguagem da Resposta { .fragment }
5. JSON como Contrato { .fragment }
6. Mini-Projeto: API de Livros { .fragment }

---

## 1. REST: Representational State Transfer 🧊

- É um estilo de arquitetura para sistemas distribuídos. { .fragment }
- **Recurso**: Tudo o que é Nomeável (Substantivo). { .fragment }
- **URI**: O Identificador único (ex: `/usuarios/1`). { .fragment }

---

## 2. Verbos HTTP: As Ações 🎬

| Verbo | Ação | Ideal para... |
| :--- | :--- | :--- |
| **GET** | Ler | Listar ou buscar um item. |
| **POST** | Criar | Inserir novo dado. |
| **PUT/PATCH** | Atualizar | Alterar dados existentes. |
| **DELETE** | Remover | Apagar um recurso. |

---

## 3. Organização Profissional 📂

> "Separe quem recebe o dado de quem decide o que fazer com ele." { .fragment }

- **Handlers**: Tratam o HTTP. { .fragment }
- **Services**: Regras de Negócio. { .fragment }
- **Models/Entity**: A cara do dado. { .fragment }
- **Repository**: Acesso ao Banco de Dados. { .fragment }

---

## 4. Diagrama de Camadas 📊

```mermaid
graph TD
    Client[Browser/Postman] --> Handler[Handler/Controller]
    Handler --> Service[Service/Business]
    Service --> Repo[Repository/DB]
    Repo --> Data[(Banco de Dados)]
```

---

## 5. Status Codes: O Feedback 🚦

- **2xx**: Sucesso (200 OK, 201 Created). { .fragment }
- **4xx**: Erro do Cliente (400 Bad Request, 404 Not Found). { .fragment }
- **5xx**: Erro do Servidor (500 Internal Error). { .fragment }

---

## 6. Mini-Projeto: API de Livros 🚀

- Criar estrutura de pastas. { .fragment }
- Implementar Listagem e Cadastro. { .fragment }
- Separar Structs em um pacote `models`. { .fragment }

---

## Resumo da Aula ✅

- REST usa o protocolo HTTP de forma inteligente. { .fragment }
- Camadas facilitam a manutenção e testes. { .fragment }
- URIs devem ser substantivos, não verbos. { .fragment }

---

## Próxima Aula: Framework Gin 🚀

- Desenvolvimento ultra-rápido. { .fragment }
- Validação automática de JSON.

---

## Dúvidas? 🤔

> "Uma boa API é aquela que se explica sozinha."