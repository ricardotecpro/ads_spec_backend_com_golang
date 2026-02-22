# Exercícios: Docker e Deploy 🐳

!!! info "Instruções"
    Prepare sua aplicação para o mundo real usando containers.

---

### 🟢 Nível: Básico

1.  **Dockerfile**: Crie um arquivo `Dockerfile` simples para um "Hello World" em Go.
2.  **Imagens**: Use o comando `docker build` para criar a imagem e `docker images` para verificar o tamanho dela.

---

### 🟡 Nível: Intermediário

3.  **Multi-Stage**: Refatore seu Dockerfile para usar Multi-Stage Build e compare a diferença de tamanho entre a imagem de build e a imagem final.
4.  **Execução**: Suba um container rodando sua aplicação na porta 9000 e verifique se consegue acessá-la de fora do container.

---

### 🔴 Nível: Desafio

5.  **Compose Completo**: Crie um arquivo `docker-compose.yml` que suba sua API (da aula 12) e um banco de dados PostgreSQL. Garante que a API espere o banco de dados estar pronto antes de tentar conectar.