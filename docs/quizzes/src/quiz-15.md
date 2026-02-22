# Quiz 15 - Docker e Deploy 🐳

1. Qual a principal vantagem de usar Docker para uma aplicação Go?
    - [ ] Ele deixa o código Go mais rápido que o normal
    - [x] Ele empacota o binário e suas dependências de sistema em um ambiente isolado e idêntico em qualquer lugar
    - [ ] Ele converte o código Go para HTML automaticamente
    - [ ] Ele substitui a necessidade de programar
    *Explicação: Docker resolve o problema do "na minha máquina funciona".*

2. O que é o "Multi-Stage Build" em um Dockerfile?
    - [ ] Um build que roda em vários computadores ao mesmo tempo
    - [x] Uma técnica de usar um estágio para compilar o código e outro estágio (menor) apenas para rodar o binário final
    - [ ] Um comando que instala várias versões do Docker
    - [ ] Um build que troca de cor no terminal
    *Explicação: Isso permite imagens extremamente leves, na casa dos 15MB.*

3. Por que podemos usar a imagem `alpine` ou até `scratch` como base final para o Go?
    - [ ] Porque elas são grátis
    - [x] Porque binários Go são estáticos e não precisam de um sistema operacional completo para rodar
    - [ ] Porque elas têm o logo de um gopher
    - [ ] Porque elas são mais coloridas
    *Explicação: Menos arquivos na imagem significa mais segurança e menor tempo de download.*

4. Qual comando do Dockerfile define qual comando será executado quando o container subir?
    - [ ] RUN
    - [ ] COPY
    - [x] CMD
    - [ ] WORKDIR
    *Explicação: O CMD é a instrução final de execução do container.*

5. Para que serve o arquivo `docker-compose.yml`?
    - [ ] Para salvar senhas do banco de dados
    - [x] Para orquestrar e subir múltiplos containers juntos (ex: API + PostgreSQL)
    - [ ] Para traduzir o Docker para português
    - [ ] Para editar o código fonte
    *Explicação: Ele facilita muito o ambiente de desenvolvimento e testes locais.*

6. Como você passa uma variável de ambiente sensível para um container no Docker Compose?
    - [ ] Escrevendo diretamente no código Go
    - [x] Usando a seção `environment` ou um arquivo `.env`
    - [ ] Gritando para o monitor
    - [ ] Usando um comentário no Dockerfile
    *Explicação: Variáveis de ambiente mantêm segredos fora do controle de versão (Git).*

7. O que a instrução `COPY --from=builder` faz?
    - [ ] Copia o código do GitHub
    - [x] Copia arquivos de um estágio anterior do build para o estágio atual
    - [ ] Faz o download de dependências
    - [ ] Move o arquivo para a lixeira
    *Explicação: É a base do Multi-Stage Build para economizar espaço.*

8. No Go, como lemos uma variável de ambiente injetada pelo Docker?
    - [ ] env.Read("NOME")
    - [x] os.Getenv("NOME")
    - [ ] get.Environment("NOME")
    - [ ] system.Variable("NOME")
    *Explicação: O pacote `os` é o responsável por falar com o ambiente do sistema operacional.*

9. Qual comando Docker é usado para remover containers parados e liberar espaço?
    - [ ] docker remove all
    - [ ] docker clean
    - [x] docker system prune
    - [ ] docker format c:
    *Explicação: O `prune` faz uma limpeza geral de recursos não utilizados.*

10. O que significa "Orquestração de Containers"?
    - [ ] Tocar música com o computador
    - [x] Gerenciar o ciclo de vida, escalonamento e rede de vários containers (ex: Kubernetes)
    - [ ] Organizar o código por pastas
    - [ ] Baixar vários containers ao mesmo tempo
    *Explicação: Em sistemas grandes, ferramentas de orquestração automatizam o trabalho pesado de manter tudo rodando.*
