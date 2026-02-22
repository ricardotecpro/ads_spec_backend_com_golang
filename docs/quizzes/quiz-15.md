# Quiz 15 - Docker e Deploy 🐳

--8<-- "assets/quiz.html"

<div class="quiz-container">
  <div class="quiz-question">1. Qual a principal vantagem de usar Docker para uma aplicação Go?</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. Docker resolve o problema do "na minha máquina funciona".">Ele deixa o código Go mais rápido que o normal</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! Docker resolve o problema do "na minha máquina funciona".">Ele empacota o binário e suas dependências de sistema em um ambiente isolado e idêntico em qualquer lugar</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. Docker resolve o problema do "na minha máquina funciona".">Ele converte o código Go para HTML automaticamente</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. Docker resolve o problema do "na minha máquina funciona".">Ele substitui a necessidade de programar</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">2. O que é o "Multi-Stage Build" em um Dockerfile?</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. Isso permite imagens extremamente leves, na casa dos 15MB.">Um build que roda em vários computadores ao mesmo tempo</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! Isso permite imagens extremamente leves, na casa dos 15MB.">Uma técnica de usar um estágio para compilar o código e outro estágio (menor) apenas para rodar o binário final</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. Isso permite imagens extremamente leves, na casa dos 15MB.">Um comando que instala várias versões do Docker</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. Isso permite imagens extremamente leves, na casa dos 15MB.">Um build que troca de cor no terminal</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">3. Por que podemos usar a imagem `alpine` ou até `scratch` como base final para o Go?</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. Menos arquivos na imagem significa mais segurança e menor tempo de download.">Porque elas são grátis</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! Menos arquivos na imagem significa mais segurança e menor tempo de download.">Porque binários Go são estáticos e não precisam de um sistema operacional completo para rodar</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. Menos arquivos na imagem significa mais segurança e menor tempo de download.">Porque elas têm o logo de um gopher</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. Menos arquivos na imagem significa mais segurança e menor tempo de download.">Porque elas são mais coloridas</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">4. Qual comando do Dockerfile define qual comando será executado quando o container subir?</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. O CMD é a instrução final de execução do container.">RUN</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. O CMD é a instrução final de execução do container.">COPY</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! O CMD é a instrução final de execução do container.">CMD</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. O CMD é a instrução final de execução do container.">WORKDIR</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">5. Para que serve o arquivo `docker-compose.yml`?</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. Ele facilita muito o ambiente de desenvolvimento e testes locais.">Para salvar senhas do banco de dados</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! Ele facilita muito o ambiente de desenvolvimento e testes locais.">Para orquestrar e subir múltiplos containers juntos (ex: API + PostgreSQL)</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. Ele facilita muito o ambiente de desenvolvimento e testes locais.">Para traduzir o Docker para português</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. Ele facilita muito o ambiente de desenvolvimento e testes locais.">Para editar o código fonte</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">6. Como você passa uma variável de ambiente sensível para um container no Docker Compose?</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. Variáveis de ambiente mantêm segredos fora do controle de versão (Git).">Escrevendo diretamente no código Go</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! Variáveis de ambiente mantêm segredos fora do controle de versão (Git).">Usando a seção `environment` ou um arquivo `.env`</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. Variáveis de ambiente mantêm segredos fora do controle de versão (Git).">Gritando para o monitor</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. Variáveis de ambiente mantêm segredos fora do controle de versão (Git).">Usando um comentário no Dockerfile</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">7. O que a instrução `COPY --from=builder` faz?</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. É a base do Multi-Stage Build para economizar espaço.">Copia o código do GitHub</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! É a base do Multi-Stage Build para economizar espaço.">Copia arquivos de um estágio anterior do build para o estágio atual</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. É a base do Multi-Stage Build para economizar espaço.">Faz o download de dependências</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. É a base do Multi-Stage Build para economizar espaço.">Move o arquivo para a lixeira</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">8. No Go, como lemos uma variável de ambiente injetada pelo Docker?</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. O pacote `os` é o responsável por falar com o ambiente do sistema operacional.">env.Read("NOME")</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! O pacote `os` é o responsável por falar com o ambiente do sistema operacional.">os.Getenv("NOME")</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. O pacote `os` é o responsável por falar com o ambiente do sistema operacional.">get.Environment("NOME")</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. O pacote `os` é o responsável por falar com o ambiente do sistema operacional.">system.Variable("NOME")</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">9. Qual comando Docker é usado para remover containers parados e liberar espaço?</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. O `prune` faz uma limpeza geral de recursos não utilizados.">docker remove all</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. O `prune` faz uma limpeza geral de recursos não utilizados.">docker clean</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! O `prune` faz uma limpeza geral de recursos não utilizados.">docker system prune</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. O `prune` faz uma limpeza geral de recursos não utilizados.">docker format c:</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">10. O que significa "Orquestração de Containers"?</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. Em sistemas grandes, ferramentas de orquestração automatizam o trabalho pesado de manter tudo rodando.">Tocar música com o computador</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! Em sistemas grandes, ferramentas de orquestração automatizam o trabalho pesado de manter tudo rodando.">Gerenciar o ciclo de vida, escalonamento e rede de vários containers (ex: Kubernetes)</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. Em sistemas grandes, ferramentas de orquestração automatizam o trabalho pesado de manter tudo rodando.">Organizar o código por pastas</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. Em sistemas grandes, ferramentas de orquestração automatizam o trabalho pesado de manter tudo rodando.">Baixar vários containers ao mesmo tempo</div>
  <div class="quiz-feedback"></div>
</div>
