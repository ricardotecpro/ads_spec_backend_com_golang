# Aula 07 - Manipulação de Arquivos e JSON 📁
## Persistindo Dados e Comunicando-se com o Mundo

---

## Agenda de Hoje 📅

1. O Pacote `os` e o Sistema de Arquivos { .fragment }
2. Leitura e Escrita de Arquivos { .fragment }
3. Permissões de Acesso (Chmod) { .fragment }
4. Serialização com JSON { .fragment }
5. Struct Tags e Mapeamento { .fragment }
6. Mini-Projeto: CLI To-Do com JSON { .fragment }

---

## 1. Falando com o SO 🖥️

- Go é excelente para ferramentas de linha de comando. { .fragment }
- Pacote `os` abstrai a diferença entre Windows/Linux. { .fragment }

---

## 2. Escrita Simplificada ✍️

```go
texto := "Dados do sistema"
err := os.WriteFile("log.txt", []byte(texto), 0644)
```

- **0644**: Permissão de leitura/escrita padrão. { .fragment }

---

## 3. JSON: A Língua do Backend 🏗️

- Go possui suporte nativo via `encoding/json`. { .fragment }
- **Marshal**: Struct -> JSON. { .fragment }
- **Unmarshal**: JSON -> Struct. { .fragment }

---

## 4. O Poder das Struct Tags 🏷️

- Permite renomear chaves no JSON. { .fragment }

```go
type User struct {
    Nome  string `json:"full_name"`
    Senha string `json:"-"` // Oculta no JSON
}
```

---

## 5. Fluxo de Dados JSON 📊

```mermaid
graph LR
    A[Struct em Memória] -->|json.Marshal| B[Slice de Bytes]
    B -->|os.WriteFile| C[(Arquivo config.json)]
    C -->|os.ReadFile| B
    B -->|json.Unmarshal| A
```

---

## 6. Mini-Projeto: To-Do List CLI 🚀

- Uma struct `Tarefa` (ID, Texto, Status). { .fragment }
- Salvar um slice de tarefas em `tarefas.json`. { .fragment }
- Ler e exibir ao abrir o programa. { .fragment }

---

## Resumo da Aula ✅

- Go trata arquivos de forma binária (`[]byte`). { .fragment }
- JSON é mapeado diretamente para structs via Tags. { .fragment }
- Defer é vital para liberar o arquivo após o uso. { .fragment }

---

## Próxima Aula: Concorrência ⚡

- Goroutines: Rodando em paralelo. { .fragment }
- Channels: A comunicação segura. { .fragment }

---

## Dúvidas? 🤔

> "Dados são o novo petróleo, mas o JSON é o oleoduto."
