# Quiz 06 - Tratamento de Erros ⚠️

--8<-- "assets/quiz.html"

<div class="quiz-container">
  <div class="quiz-question">1. Qual o padrão idiomático para tratar erros em Go?</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. Go trata erros como valores comuns, forçando o desenvolvedor a lidar com eles no momento em que ocorrem.">Usar blocos try/catch/finally</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! Go trata erros como valores comuns, forçando o desenvolvedor a lidar com eles no momento em que ocorrem.">Verificar se o retorno do tipo `error` é diferente de `nil`</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. Go trata erros como valores comuns, forçando o desenvolvedor a lidar com eles no momento em que ocorrem.">Ignorar todos os erros e torcer para o melhor</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. Go trata erros como valores comuns, forçando o desenvolvedor a lidar com eles no momento em que ocorrem.">Usar somente o comando panic</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">2. O que é o tipo `error` em Go?</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. Por ser uma interface, qualquer tipo que implemente o método `Error()` pode ser usado como erro.">Uma palavra-chave do sistema operacional</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! Por ser uma interface, qualquer tipo que implemente o método `Error()` pode ser usado como erro.">Uma interface nativa com o método `Error() string`</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. Por ser uma interface, qualquer tipo que implemente o método `Error()` pode ser usado como erro.">Um número inteiro que indica o código do erro</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. Por ser uma interface, qualquer tipo que implemente o método `Error()` pode ser usado como erro.">Um booleano (true ou false)</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">3. Quando se deve usar a função `panic`?</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. O panic é agressivo e deve ser reservado para falhas catastróficas (ex: falta de memória).">Em qualquer erro de validação de formulário</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! O panic é agressivo e deve ser reservado para falhas catastróficas (ex: falta de memória).">Apenas para erros críticos e irrecuperáveis que impedem o programa de continuar</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. O panic é agressivo e deve ser reservado para falhas catastróficas (ex: falta de memória).">Para retornar mensagens de sucesso</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. O panic é agressivo e deve ser reservado para falhas catastróficas (ex: falta de memória).">Para fechar o programa voluntariamente</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">4. Qual a função do comando `defer`?</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. Essencial para garantir o fechamento de arquivos e conexões de rede.">Deletar uma variável</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! Essencial para garantir o fechamento de arquivos e conexões de rede.">Adiar a execução de uma função até o final da função atual (mesmo em caso de erro)</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. Essencial para garantir o fechamento de arquivos e conexões de rede.">Aumentar a velocidade do loop for</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. Essencial para garantir o fechamento de arquivos e conexões de rede.">Esconder o erro do usuário</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">5. Para que serve o comando `recover`?</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. O recover só funciona dentro de uma função chamada via `defer`.">Para recuperar arquivos deletados</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! O recover só funciona dentro de uma função chamada via `defer`.">Para capturar um panic em execução e evitar o encerramento do programa</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. O recover só funciona dentro de uma função chamada via `defer`.">Para restaurar o banco de dados</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. O recover só funciona dentro de uma função chamada via `defer`.">Para atualizar a versão do Go</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">6. Qual a diferença entre `errors.New` e `fmt.Errorf`?</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. `fmt.Errorf` é ideal para adicionar contexto dinâmico ao erro.">Nenhuma, são sinônimos</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. `fmt.Errorf` é ideal para adicionar contexto dinâmico ao erro.">`errors.New` é mais rápido no Linux</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! `fmt.Errorf` é ideal para adicionar contexto dinâmico ao erro.">`fmt.Errorf` permite formatar a mensagem com variáveis (estilo Printf)</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. `fmt.Errorf` é ideal para adicionar contexto dinâmico ao erro.">`errors.New` apaga o log automaticamente</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">7. Por que Go não utiliza exceções (try/catch)?</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. O tratamento explícito torna o código mais previsível e fácil de debugar.">Porque os criadores esqueceram de implementar</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! O tratamento explícito torna o código mais previsível e fácil de debugar.">Para manter o fluxo de controle visível, simples e evitar "saltos" mágicos no código</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. O tratamento explícito torna o código mais previsível e fácil de debugar.">Porque exceções consomem muita bateria</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. O tratamento explícito torna o código mais previsível e fácil de debugar.">Porque Go é uma linguagem para crianças</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">8. O que acontece se você declarar um erro e não verificá-lo (usar `_`)?</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. Ignorar erros é considerado um dos maiores "pecados" de um desenvolvedor Go.">O Go avisa o usuário na tela</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. Ignorar erros é considerado um dos maiores "pecados" de um desenvolvedor Go.">O programa fica mais rápido</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! Ignorar erros é considerado um dos maiores "pecados" de um desenvolvedor Go.">Você corre o risco de ignorar falhas graves, gerando bugs difíceis de encontrar</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. Ignorar erros é considerado um dos maiores "pecados" de um desenvolvedor Go.">O compilador deleta o arquivo fonte</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">9. Onde o comando `defer` costuma ser colocado?</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. Colocá-lo logo após o recurso evita o esquecimento de fechá-lo.">Sempre no final da função</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! Colocá-lo logo após o recurso evita o esquecimento de fechá-lo.">Logo após a declaração bem-sucedida do recurso (ex: após abrir um arquivo)</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. Colocá-lo logo após o recurso evita o esquecimento de fechá-lo.">Apenas dentro do pacote main</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. Colocá-lo logo após o recurso evita o esquecimento de fechá-lo.">Em um arquivo separado de configuração</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">10. Pode-se retornar um valor e um erro ao mesmo tempo?</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. `return resultado, nil` ou `return nil, erro` é a base da robustez do Go.">Não, é proibido</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! `return resultado, nil` ou `return nil, erro` é a base da robustez do Go.">Sim, é o padrão recomendado em Go</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. `return resultado, nil` ou `return nil, erro` é a base da robustez do Go.">Somente se o valor for uma string</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. `return resultado, nil` ou `return nil, erro` é a base da robustez do Go.">Apenas em funções que usam ponteiros</div>
  <div class="quiz-feedback"></div>
</div>
