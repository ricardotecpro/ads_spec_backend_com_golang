# Quiz 02 - Fundamentos da Linguagem 🧱

--8<-- "assets/quiz.html"

<div class="quiz-container">
  <div class="quiz-question">1. Qual a diferença entre declarar uma variável com `var` e usar o operador curto `:=`?</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. O operador curto é uma conveniência para declarar e inicializar variáveis locais.">Não há diferença, ambos funcionam igual em qualquer lugar</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! O operador curto é uma conveniência para declarar e inicializar variáveis locais.">O `:=` só pode ser usado dentro de funções e detecta o tipo automaticamente</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. O operador curto é uma conveniência para declarar e inicializar variáveis locais.">O `var` é para constantes e o `:=` para variáveis</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. O operador curto é uma conveniência para declarar e inicializar variáveis locais.">O `:=` é mais lento que o `var`</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">2. O que acontece se você somar um `int` com um `int64` sem conversão explícita?</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. Go é extremamente rígido com tipos para evitar bugs silenciosos.">O Go faz a conversão automática (coerção)</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! Go é extremamente rígido com tipos para evitar bugs silenciosos.">Ocorrerá um erro de compilação (tipos incompatíveis)</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. Go é extremamente rígido com tipos para evitar bugs silenciosos.">O resultado será sempre zero</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. Go é extremamente rígido com tipos para evitar bugs silenciosos.">O Go converte tudo para string</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">3. Quantas estruturas de loop existem em Go?</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. A simplicidade do Go remove o `while` e o `do-while`, usando o `for` para tudo.">Três: for, while e do-while</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! A simplicidade do Go remove o `while` e o `do-while`, usando o `for` para tudo.">Apenas uma: for (que assume várias formas)</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. A simplicidade do Go remove o `while` e o `do-while`, usando o `for` para tudo.">Nenhuma, Go usa apenas recursão</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. A simplicidade do Go remove o `while` e o `do-while`, usando o `for` para tudo.">Duas: for e foreach</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">4. Como se escreve um teste de condição `if` em Go corretamente?</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. Em Go, os parênteses no `if` são desnecessários e não recomendados.">if (x > 10) { ... }</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! Em Go, os parênteses no `if` são desnecessários e não recomendados.">if x > 10 { ... }</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. Em Go, os parênteses no `if` são desnecessários e não recomendados.">if x > 10 then ...</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. Em Go, os parênteses no `if` são desnecessários e não recomendados.">if [ x -gt 10 ]; then ...</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">5. Para que serve a palavra-chave `const`?</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. Constantes são usadas para valores como o PI ou mensagens de erro padronizadas.">Para declarar variáveis que mudam o tempo todo</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! Constantes são usadas para valores como o PI ou mensagens de erro padronizadas.">Para declarar valores fixos que não podem ser alterados durante a execução</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. Constantes são usadas para valores como o PI ou mensagens de erro padronizadas.">Para importar pacotes de outros arquivos</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. Constantes são usadas para valores como o PI ou mensagens de erro padronizadas.">Para definir o nome do autor do código</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">6. Qual o valor padrão (zero value) de um tipo `string` em Go?</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. Em Go, toda variável nasce com um valor padrão seguro.">"null"</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. Em Go, toda variável nasce com um valor padrão seguro.">"undefined"</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! Em Go, toda variável nasce com um valor padrão seguro.">"" (string vazia)</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. Em Go, toda variável nasce com um valor padrão seguro.">"Zero"</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">7. No comando `switch`, é necessário usar `break` no final de cada `case`?</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. Isso remove uma das maiores fontes de erros do C e Java.">Sim, senão ele executa o próximo caso</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! Isso remove uma das maiores fontes de erros do C e Java.">Não, o Go para automaticamente no final do caso (não tem fallthrough por padrão)</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. Isso remove uma das maiores fontes de erros do C e Java.">Sim, mas apenas se o caso for numérico</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. Isso remove uma das maiores fontes de erros do C e Java.">O switch do Go não aceita `case`</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">8. O que é "Inferência de Tipo" em Go?</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. `x := 10` faz o compilador entender que `x` é um `int`.">É quando o programador precisa adivinhar o tipo da variável</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! `x := 10` faz o compilador entender que `x` é um `int`.">É quando o compilador descobre o tipo da variável baseando-se no valor atribuído</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. `x := 10` faz o compilador entender que `x` é um `int`.">É um erro onde o tipo se perde durante a execução</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. `x := 10` faz o compilador entender que `x` é um `int`.">É uma função que converte strings em números</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">9. Qual tipo de dado deve ser usado para valores decimais de alta precisão?</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. O `float64` é o padrão para números de ponto flutuante em Go.">int</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. O `float64` é o padrão para números de ponto flutuante em Go.">bool</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! O `float64` é o padrão para números de ponto flutuante em Go.">float64</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. O `float64` é o padrão para números de ponto flutuante em Go.">string</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">10. Como se cria um loop infinito em Go?</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. Um `for` sem condições roda para sempre até ser interrompido.">for true { }</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. Um `for` sem condições roda para sempre até ser interrompido.">while(true) { }</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! Um `for` sem condições roda para sempre até ser interrompido.">for { }</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. Um `for` sem condições roda para sempre até ser interrompido.">loop { }</div>
  <div class="quiz-feedback"></div>
</div>
