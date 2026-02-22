# Quiz 13 - Testes em Go ✅

--8<-- "assets/quiz.html"

<div class="quiz-container">
  <div class="quiz-question">1. Qual o sufixo obrigatório de um arquivo que contém testes em Go?</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. O compilador Go ignora arquivos com este sufixo durante a compilação normal e só os usa no comando `go test`.">.test</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. O compilador Go ignora arquivos com este sufixo durante a compilação normal e só os usa no comando `go test`.">_go_test.go</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! O compilador Go ignora arquivos com este sufixo durante a compilação normal e só os usa no comando `go test`.">_test.go</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. O compilador Go ignora arquivos com este sufixo durante a compilação normal e só os usa no comando `go test`.">.spec.go</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">2. Qual o parâmetro obrigatório de uma função de teste unitário?</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. O objeto `*testing.T` fornece métodos para reportar falhas e logs nos testes.">s *sync.WaitGroup</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! O objeto `*testing.T` fornece métodos para reportar falhas e logs nos testes.">t *testing.T</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. O objeto `*testing.T` fornece métodos para reportar falhas e logs nos testes.">err error</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. O objeto `*testing.T` fornece métodos para reportar falhas e logs nos testes.">ctx context.Context</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">3. De onde vem o pacote de testes do Go?</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. Go preza por ter ferramentas de qualidade embutidas na linguagem.">É preciso baixar do GitHub</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! Go preza por ter ferramentas de qualidade embutidas na linguagem.">Faz parte da biblioteca padrão (`testing`)</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. Go preza por ter ferramentas de qualidade embutidas na linguagem.">É um plugin do VS Code</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. Go preza por ter ferramentas de qualidade embutidas na linguagem.">Vem junto com o Docker</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">4. O que é um "Table-Driven Test" (Teste de Tabela)?</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. É a forma mais organizada e escalável de escrever testes em Go.">Um teste feito no Excel</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! É a forma mais organizada e escalável de escrever testes em Go.">Uma técnica de organizar vários cenários de entrada e saída em um slice para testar uma única função</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. É a forma mais organizada e escalável de escrever testes em Go.">Um teste que verifica se o banco de dados tem tabelas</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. É a forma mais organizada e escalável de escrever testes em Go.">Um teste que roda apenas em tabelas HTML</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">5. Qual comando gera um relatório de cobertura de testes no terminal?</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. A cobertura indica quais partes do seu código foram realmente executadas pelos testes.">go test -v</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! A cobertura indica quais partes do seu código foram realmente executadas pelos testes.">go test -cover</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. A cobertura indica quais partes do seu código foram realmente executadas pelos testes.">go coverage</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. A cobertura indica quais partes do seu código foram realmente executadas pelos testes.">go check</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">6. Para que serve o pacote `httptest`?</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. Essencial para testar Handlers e Middlewares de forma isolada.">Para hackear sites</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! Essencial para testar Handlers e Middlewares de forma isolada.">Para simular requisições e respostas HTTP sem precisar subir um servidor real</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. Essencial para testar Handlers e Middlewares de forma isolada.">Para medir a velocidade da internet</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. Essencial para testar Handlers e Middlewares de forma isolada.">Para criar sites bonitos</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">7. Em Go, o que significa TDD (Test Driven Development)?</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. O TDD ajuda a desenhar funções melhores e mais simples.">Total Data Design</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! O TDD ajuda a desenhar funções melhores e mais simples.">Desenvolvimento Orientado por Testes (escrever o teste antes do código)</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. O TDD ajuda a desenhar funções melhores e mais simples.">Técnica De Depuração</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. O TDD ajuda a desenhar funções melhores e mais simples.">Trabalho De Desenvolvedor</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">8. O que acontece se uma função de teste começar com letra minúscula (ex: `func testSoma`)?</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. A ferramenta de testes só executa funções exportadas que seguem o padrão `TestXxx`.">O Go avisa que está errado</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. A ferramenta de testes só executa funções exportadas que seguem o padrão `TestXxx`.">O programa trava</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! A ferramenta de testes só executa funções exportadas que seguem o padrão `TestXxx`.">O `go test` irá ignorar a função (ela deve começar obrigatoriamente com `Test...`)</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. A ferramenta de testes só executa funções exportadas que seguem o padrão `TestXxx`.">Ela vira um teste privado</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">9. Qual o papel do método `t.Errorf`?</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. Ele permite capturar múltiplos erros em uma única rodada de testes.">Encerrar o programa imediatamente</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! Ele permite capturar múltiplos erros em uma única rodada de testes.">Reportar que um teste falhou mas continuar a execução dos próximos testes</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. Ele permite capturar múltiplos erros em uma única rodada de testes.">Enviar um e-mail para o desenvolvedor</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. Ele permite capturar múltiplos erros em uma única rodada de testes.">Formatar o código</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">10. Pode-se testar performance (benchmarks) no Go nativamente?</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. Go possui um sistema robusto para medir a velocidade e alocação de memória das suas funções.">Não, precisa de ferramentas externas</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! Go possui um sistema robusto para medir a velocidade e alocação de memória das suas funções.">Sim, usando funções que começam com `Benchmark...` e o objeto `*testing.B`</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. Go possui um sistema robusto para medir a velocidade e alocação de memória das suas funções.">Sim, mas apenas em servidores potentes</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. Go possui um sistema robusto para medir a velocidade e alocação de memória das suas funções.">Somente se o código estiver em nuvem</div>
  <div class="quiz-feedback"></div>
</div>
