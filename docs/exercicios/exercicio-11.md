# Exercícios: Framework Web Gin 🚀

!!! info "Instruções"
    Explore as facilidades do Gin para criar APIs robustas.

---

### 🟢 Nível: Básico

1.  **Instalação**: Inicialize um módulo Go e instale o Gin usando `go get -u github.com/gin-gonic/gin`.
2.  **Primeira Rota**: Crie um servidor Gin que responda com um JSON de boas-vindas na rota raiz `/`.

---

### 🟡 Nível: Intermediário

3.  **Parâmetros**: Crie uma rota `/ola/:nome` que responda "Olá, [nome]" tanto em texto puro quanto em um campo JSON.
4.  **Grupos**: Crie um grupo de rotas `/api/v1` e coloque dentro dele uma rota de `status` que retorne a versão da API.

---

### 🔴 Nível: Desafio

5.  **Validação de Cadastro**: Crie uma struct `Usuario` com campos `Email` (obrigatório) e `Senha` (obrigatório e mínimo de 6 caracteres - pesquise sobre a tag `binding`). Implemente uma rota `POST /cadastro` que valide esses dados e retorne um erro amigável caso a validação falhe.