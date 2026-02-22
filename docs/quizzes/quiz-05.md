# Quiz 05 - Interfaces e Composição 🧩

--8<-- "assets/quiz.html"

<div class="quiz-container">
  <div class="quiz-question">1. Por que as interfaces em Go são chamadas de "Duck Typing" implícito?</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. "Se caminha como pato e faz quack como pato, é um pato". Go detecta a implementação automaticamente.">Porque elas têm um desenho de pato no ícone</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! "Se caminha como pato e faz quack como pato, é um pato". Go detecta a implementação automaticamente.">Porque você não precisa declarar que "implementa" uma interface; basta ter os métodos necessários</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. "Se caminha como pato e faz quack como pato, é um pato". Go detecta a implementação automaticamente.">Porque elas só funcionam com nomes de animais</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. "Se caminha como pato e faz quack como pato, é um pato". Go detecta a implementação automaticamente.">Porque são muito lentas para rodar</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">2. O que acontece se uma interface definir 3 métodos e uma struct implementar apenas 2?</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. Para implementar uma interface, a satisfação dos métodos deve ser total.">O Go tenta adivinhar o terceiro</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! Para implementar uma interface, a satisfação dos métodos deve ser total.">A struct NÃO implementa a interface (erro de tipo)</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. Para implementar uma interface, a satisfação dos métodos deve ser total.">A struct implementa a interface parcialmente</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. Para implementar uma interface, a satisfação dos métodos deve ser total.">O programa roda mas dá erro se chamar o método faltante</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">3. Qual a principal vantagem da Composição sobre a Herança em Go?</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. A composição permite montar tipos complexos como "peças de Lego".">Deixa o código mais colorido</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! A composição permite montar tipos complexos como "peças de Lego".">Evita hierarquias complexas e rígidas, promovendo o desacoplamento</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. A composição permite montar tipos complexos como "peças de Lego".">Permite que o código rode mais rápido no Windows</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. A composição permite montar tipos complexos como "peças de Lego".">Nenhuma, herança é sempre melhor</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">4. Para que serve a "Interface Vazia" `interface{}` (ou `any` nas versões mais novas)?</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. Ela é a base para funções que precisam aceitar qualquer tipo de dado.">Para indicar que o programa não faz nada</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! Ela é a base para funções que precisam aceitar qualquer tipo de dado.">Para representar um valor de qualquer tipo</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. Ela é a base para funções que precisam aceitar qualquer tipo de dado.">Para deletar variáveis da memória</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. Ela é a base para funções que precisam aceitar qualquer tipo de dado.">Para criar um loop que nunca termina</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">5. O que significa "Aceite Interfaces, Retorne Structs"?</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. Aceitar interfaces torna sua função genérica; retornar structs dá rapidez e precisão no uso.">É uma regra de etiqueta do Google</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! Aceitar interfaces torna sua função genérica; retornar structs dá rapidez e precisão no uso.">É uma boa prática que dá flexibilidade a quem chama a função e clareza no retorno</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. Aceitar interfaces torna sua função genérica; retornar structs dá rapidez e precisão no uso.">Significa que o código deve ser escrito apenas com interfaces</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. Aceitar interfaces torna sua função genérica; retornar structs dá rapidez e precisão no uso.">É um padrão para banco de dados</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">6. Como você faz o "Type Assertion" para descobrir o tipo real por trás de uma interface?</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. O padrão `v, ok := i.(T)` permite verificar o tipo de forma segura.">var x = interface.(tipo)</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. O padrão `v, ok := i.(T)` permite verificar o tipo de forma segura.">interface.as(tipo)</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! O padrão `v, ok := i.(T)` permite verificar o tipo de forma segura.">valor, ok := interface.(tipo)</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. O padrão `v, ok := i.(T)` permite verificar o tipo de forma segura.">check(interface == tipo)</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">7. Em Go, podemos anexar métodos a tipos básicos (como `int`)?</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. Criar novos tipos permite estender funcionalidades até de tipos primitivos.">Não, apenas a structs</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! Criar novos tipos permite estender funcionalidades até de tipos primitivos.">Sim, desde que você defina um novo tipo (ex: `type MeuInt int`)</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. Criar novos tipos permite estender funcionalidades até de tipos primitivos.">Sim, basta usar a extensão .go</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. Criar novos tipos permite estender funcionalidades até de tipos primitivos.">Somente se o computador for de 64 bits</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">8. Qual o limite de métodos que uma interface pode ter?</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. Interfaces pequenas são mais fáceis de implementar e reutilizar.">No máximo 10</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. Interfaces pequenas são mais fáceis de implementar e reutilizar.">Apenas 1</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! Interfaces pequenas são mais fáceis de implementar e reutilizar.">Não há limite técnico, mas interfaces pequenas (1 ou 2 métodos) são preferíveis</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. Interfaces pequenas são mais fáceis de implementar e reutilizar.">Elas devem ter sempre um número par de métodos</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">9. O que é "Embedding" (Embutimento) na Composição?</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. O embedding faz com que a struct externa "ganhe" os métodos da interna automaticamente.">Colocar o computador dentro de uma caixa</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. O embedding faz com que a struct externa "ganhe" os métodos da interna automaticamente.">Copiar e colar código de um arquivo no outro</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! O embedding faz com que a struct externa "ganhe" os métodos da interna automaticamente.">Colocar uma struct dentro de outra sem dar um nome ao campo, herdando seus métodos</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. O embedding faz com que a struct externa "ganhe" os métodos da interna automaticamente.">Salvar o código no banco de dados</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">10. Go suporta Polimorfismo?</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. O polimorfismo em Go é limpo e focado no comportamento, não na identidade.">Não, Go é funcional</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! O polimorfismo em Go é limpo e focado no comportamento, não na identidade.">Sim, através do uso de Interfaces</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. O polimorfismo em Go é limpo e focado no comportamento, não na identidade.">Somente se usar o pacote `poly`</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. O polimorfismo em Go é limpo e focado no comportamento, não na identidade.">Não, Go é procedural e não tem objetos</div>
  <div class="quiz-feedback"></div>
</div>
