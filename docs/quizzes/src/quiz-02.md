# Quiz 02 - Fundamentos da Linguagem 🧱

1. Qual a diferença entre declarar uma variável com `var` e usar o operador curto `:=`?
    - [ ] Não há diferença, ambos funcionam igual em qualquer lugar
    - [x] O `:=` só pode ser usado dentro de funções e detecta o tipo automaticamente
    - [ ] O `var` é para constantes e o `:=` para variáveis
    - [ ] O `:=` é mais lento que o `var`
    *Explicação: O operador curto é uma conveniência para declarar e inicializar variáveis locais.*

2. O que acontece se você somar um `int` com um `int64` sem conversão explícita?
    - [ ] O Go faz a conversão automática (coerção)
    - [x] Ocorrerá um erro de compilação (tipos incompatíveis)
    - [ ] O resultado será sempre zero
    - [ ] O Go converte tudo para string
    *Explicação: Go é extremamente rígido com tipos para evitar bugs silenciosos.*

3. Quantas estruturas de loop existem em Go?
    - [ ] Três: for, while e do-while
    - [x] Apenas uma: for (que assume várias formas)
    - [ ] Nenhuma, Go usa apenas recursão
    - [ ] Duas: for e foreach
    *Explicação: A simplicidade do Go remove o `while` e o `do-while`, usando o `for` para tudo.*

4. Como se escreve um teste de condição `if` em Go corretamente?
    - [ ] if (x > 10) { ... }
    - [x] if x > 10 { ... }
    - [ ] if x > 10 then ...
    - [ ] if [ x -gt 10 ]; then ...
    *Explicação: Em Go, os parênteses no `if` são desnecessários e não recomendados.*

5. Para que serve a palavra-chave `const`?
    - [ ] Para declarar variáveis que mudam o tempo todo
    - [x] Para declarar valores fixos que não podem ser alterados durante a execução
    - [ ] Para importar pacotes de outros arquivos
    - [ ] Para definir o nome do autor do código
    *Explicação: Constantes são usadas para valores como o PI ou mensagens de erro padronizadas.*

6. Qual o valor padrão (zero value) de um tipo `string` em Go?
    - [ ] "null"
    - [ ] "undefined"
    - [x] "" (string vazia)
    - [ ] "Zero"
    *Explicação: Em Go, toda variável nasce com um valor padrão seguro.*

7. No comando `switch`, é necessário usar `break` no final de cada `case`?
    - [ ] Sim, senão ele executa o próximo caso
    - [x] Não, o Go para automaticamente no final do caso (não tem fallthrough por padrão)
    - [ ] Sim, mas apenas se o caso for numérico
    - [ ] O switch do Go não aceita `case`
    *Explicação: Isso remove uma das maiores fontes de erros do C e Java.*

8. O que é "Inferência de Tipo" em Go?
    - [ ] É quando o programador precisa adivinhar o tipo da variável
    - [x] É quando o compilador descobre o tipo da variável baseando-se no valor atribuído
    - [ ] É um erro onde o tipo se perde durante a execução
    - [ ] É uma função que converte strings em números
    *Explicação: `x := 10` faz o compilador entender que `x` é um `int`.*

9. Qual tipo de dado deve ser usado para valores decimais de alta precisão?
    - [ ] int
    - [ ] bool
    - [x] float64
    - [ ] string
    *Explicação: O `float64` é o padrão para números de ponto flutuante em Go.*

10. Como se cria um loop infinito em Go?
    - [ ] for true { }
    - [ ] while(true) { }
    - [x] for { }
    - [ ] loop { }
    *Explicação: Um `for` sem condições roda para sempre até ser interrompido.*
