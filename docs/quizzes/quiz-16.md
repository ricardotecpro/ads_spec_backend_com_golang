# Quiz 16 - Revisão Geral e Projeto Final 🏆

--8<-- "assets/quiz.html"

<div class="quiz-container">
  <div class="quiz-question">1. Qual o principal diferencial do Go em relação à concorrência?</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. Concorrência de baixo custo é o "superpoder" do Go.">Ela tem as cores mais bonitas</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! Concorrência de baixo custo é o "superpoder" do Go.">O modelo de concorrência nativo (CSP) com Goroutines e Channels</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. Concorrência de baixo custo é o "superpoder" do Go.">Ela permite programar apenas com o mouse</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. Concorrência de baixo custo é o "superpoder" do Go.">Ela não usa internet para compilar</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">2. Na organização por camadas, onde ficam as validações de campos obrigatórios?</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. Validar na entrada evita que dados sujos poluam o sistema.">No banco de dados</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! Validar na entrada evita que dados sujos poluam o sistema.">Na camada de Handler (via Binding) ou no Service (Regras de Negócio)</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. Validar na entrada evita que dados sujos poluam o sistema.">No manual do usuário</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. Validar na entrada evita que dados sujos poluam o sistema.">Em um arquivo de imagem</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">3. O que garante que o binário de produção seja pequeno e seguro?</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. Imagens Alpine com apenas o binário são o padrão da indústria.">Usar um computador novo</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! Imagens Alpine com apenas o binário são o padrão da indústria.">Multi-Stage Builds no Docker e compilação estática do Go</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. Imagens Alpine com apenas o binário são o padrão da indústria.">Deletar o código fonte antes de rodar</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. Imagens Alpine com apenas o binário são o padrão da indústria.">Comprimir o arquivo com WinRAR</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">4. Qual o comando usado para atualizar todas as dependências do projeto?</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. O `go mod tidy` limpa o arquivo, mas o `get -u` busca novas versões.">go clean</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! O `go mod tidy` limpa o arquivo, mas o `get -u` busca novas versões.">go get -u ./...</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. O `go mod tidy` limpa o arquivo, mas o `get -u` busca novas versões.">go mod tidy</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. O `go mod tidy` limpa o arquivo, mas o `get -u` busca novas versões.">go update</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">5. O que define que uma struct em Go "implementa" uma interface?</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. O mapeamento é implícito e automático.">Ela deve ter um comentário dizendo isso</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! O mapeamento é implícito e automático.">Ela deve possuir as assinaturas exatas de todos os métodos da interface</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. O mapeamento é implícito e automático.">Ela deve herdar de uma classe base</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. O mapeamento é implícito e automático.">Ela deve estar no mesmo arquivo da interface</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">6. Qual a função do arquivo `.env` em um projeto profissional?</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. Segurança em primeiro lugar.">Enviar e-mails automaticamente</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! Segurança em primeiro lugar.">Armazenar configurações e segredos específicos do ambiente que não devem ir para o Git</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. Segurança em primeiro lugar.">Decorar o terminal</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. Segurança em primeiro lugar.">Aumentar o brilho da tela</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">7. Em um sistema de biblioteca, "Empréstimo" seria melhor modelado como:</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. Relacionamentos n-pra-n ou com metadados exigem estruturas próprias.">Um campo dentro da struct Usuário</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! Relacionamentos n-pra-n ou com metadados exigem estruturas próprias.">Uma entidade/struct separada que relaciona Usuário e Livro</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. Relacionamentos n-pra-n ou com metadados exigem estruturas próprias.">Um comentário no código</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. Relacionamentos n-pra-n ou com metadados exigem estruturas próprias.">Um arquivo de texto separado</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">8. O que acontece se chamarmos `db.AutoMigrate` e a tabela já existir?</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. É uma migração incremental e segura na maioria dos casos.">O banco de dados é apagado</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! É uma migração incremental e segura na maioria dos casos.">O GORM altera a tabela para incluir novas colunas (se houver), mas mantém os dados existentes</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. É uma migração incremental e segura na maioria dos casos.">O programa trava com erro</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. É uma migração incremental e segura na maioria dos casos.">Ele cria uma cópia da tabela</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">9. Qual ferramenta é usada para simular múltiplos usuários acessando a API ao mesmo tempo em testes?</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. Go é a melhor ferramenta para testar o próprio Go sob carga.">Um browser aberto 100 vezes</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! Go é a melhor ferramenta para testar o próprio Go sob carga.">Goroutines em um loop de teste</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. Go é a melhor ferramenta para testar o próprio Go sob carga.">O cronômetro do celular</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. Go é a melhor ferramenta para testar o próprio Go sob carga.">O comando ping</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">10. Qual a melhor maneira de continuar aprendendo Go após este curso?</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. Programação é uma prática constante. Mão na massa!">Parar de programar e só ler livros</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! Programação é uma prática constante. Mão na massa!">Construir projetos reais, ler a biblioteca padrão e participar da comunidade</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. Programação é uma prática constante. Mão na massa!">Esperar o Google lançar uma nova versão</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. Programação é uma prática constante. Mão na massa!">Decorar o dicionário de funções</div>
  <div class="quiz-feedback"></div>
</div>
