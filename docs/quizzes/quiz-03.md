# Quiz 03 - Funções e Organização do Código 🧩

--8<-- "assets/quiz.html"

<div class="quiz-container">
  <div class="quiz-question">1. Como o Go permite que uma função retorne mais de um valor?</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. `func divisao(a, b int) (int, error)` é um padrão comum em Go.">Ele não permite, deve-se usar um array</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! `func divisao(a, b int) (int, error)` é um padrão comum em Go.">Basta listar os tipos de retorno entre parênteses na assinatura da função</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. `func divisao(a, b int) (int, error)` é um padrão comum em Go.">Somente se a função for iniciada com `func*`</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. `func divisao(a, b int) (int, error)` é um padrão comum em Go.">Através de variáveis globais</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">2. Para que serve o operador `&` antes de uma variável?</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. O `&` diz "onde está" o dado na memória.">Para realizar uma operação lógica "AND"</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! O `&` diz "onde está" o dado na memória.">Para obter o endereço de memória (ponteiro) daquela variável</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. O `&` diz "onde está" o dado na memória.">Para deletar a variável da memória</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. O `&` diz "onde está" o dado na memória.">Para converter um número em string</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">3. O que define se uma função ou variável é "pública" (exportada) para outros pacotes no Go?</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. Go usa a capitalização para controle de visibilidade (ex: `Fmt` vs `fmt`).">A palavra-chave `public`</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. Go usa a capitalização para controle de visibilidade (ex: `Fmt` vs `fmt`).">Se ela estiver dentro do arquivo `main.go`</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! Go usa a capitalização para controle de visibilidade (ex: `Fmt` vs `fmt`).">Se o nome dela começar com uma letra Maiúscula</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. Go usa a capitalização para controle de visibilidade (ex: `Fmt` vs `fmt`).">Se ela tiver um comentário em cima</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">4. Qual a finalidade principal de usar um Ponteiro em Go?</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. Ponteiros dão eficiência e controle sobre o estado da aplicação.">Deixar o código mais complexo e difícil de ler</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! Ponteiros dão eficiência e controle sobre o estado da aplicação.">Evitar cópias desnecessárias de dados grandes ou permitir que uma função altere o valor original</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. Ponteiros dão eficiência e controle sobre o estado da aplicação.">O Go obriga o uso de ponteiros em todas as variáveis</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. Ponteiros dão eficiência e controle sobre o estado da aplicação.">Para rodar o código em servidores antigos</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">5. O que são "Variadic Functions"?</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. O uso de `...tipo` permite passar quantos argumentos você quiser.">Funções que mudam de nome sozinhas</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! O uso de `...tipo` permite passar quantos argumentos você quiser.">Funções que aceitam um número indeterminado de argumentos do mesmo tipo</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. O uso de `...tipo` permite passar quantos argumentos você quiser.">Funções que não retornam nada</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. O uso de `...tipo` permite passar quantos argumentos você quiser.">Funções que só funcionam em variáveis do tipo bool</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">6. Como você ignora um valor de retorno que não deseja usar?</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. O `_` diz ao compilador para descartar aquele valor específico.">Deixando um espaço em branco</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! O `_` diz ao compilador para descartar aquele valor específico.">Usando o identificador em branco `_` (underscore)</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. O `_` diz ao compilador para descartar aquele valor específico.">Usando a palavra-chave `ignore`</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. O `_` diz ao compilador para descartar aquele valor específico.">O Go não permite ignorar retornos</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">7. Todo projeto Go deve ter obrigatoriamente um pacote chamado:</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. O pacote `main` informa ao compilador onde a execução do programa começa.">start</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! O pacote `main` informa ao compilador onde a execução do programa começa.">main</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. O pacote `main` informa ao compilador onde a execução do programa começa.">root</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. O pacote `main` informa ao compilador onde a execução do programa começa.">server</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">8. O que o arquivo `go.mod` gerencia?</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. Ele é a base do gerenciamento de pacotes moderno do Go.">A configuração do roteador wi-fi</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. Ele é a base do gerenciamento de pacotes moderno do Go.">O banco de dados do sistema</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! Ele é a base do gerenciamento de pacotes moderno do Go.">O nome do módulo e suas dependências externas</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. Ele é a base do gerenciamento de pacotes moderno do Go.">O estilo visual do console</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">9. Qual o operador usado para acessar o valor dentro de um ponteiro (desreferenciação)?</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. O `*` busca o "conteúdo" do endereço apontado.">&</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. O `*` busca o "conteúdo" do endereço apontado.">#</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! O `*` busca o "conteúdo" do endereço apontado.">*</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. O `*` busca o "conteúdo" do endereço apontado.">-></div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">10. Funções podem ser passadas como argumentos para outras funções em Go?</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. Isso permite padrões poderosos como middlewares e callbacks.">Não, isso é impossível</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! Isso permite padrões poderosos como middlewares e callbacks.">Sim, funções são cidadãs de primeira classe</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. Isso permite padrões poderosos como middlewares e callbacks.">Somente se forem funções matemáticas</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. Isso permite padrões poderosos como middlewares e callbacks.">Sim, mas apenas dentro do pacote `main`</div>
  <div class="quiz-feedback"></div>
</div>
