# Quiz 05 - Interfaces e Composição 🧩

1. Por que as interfaces em Go são chamadas de "Duck Typing" implícito?
    - [ ] Porque elas têm um desenho de pato no ícone
    - [x] Porque você não precisa declarar que "implementa" uma interface; basta ter os métodos necessários
    - [ ] Porque elas só funcionam com nomes de animais
    - [ ] Porque são muito lentas para rodar
    *Explicação: "Se caminha como pato e faz quack como pato, é um pato". Go detecta a implementação automaticamente.*

2. O que acontece se uma interface definir 3 métodos e uma struct implementar apenas 2?
    - [ ] O Go tenta adivinhar o terceiro
    - [x] A struct NÃO implementa a interface (erro de tipo)
    - [ ] A struct implementa a interface parcialmente
    - [ ] O programa roda mas dá erro se chamar o método faltante
    *Explicação: Para implementar uma interface, a satisfação dos métodos deve ser total.*

3. Qual a principal vantagem da Composição sobre a Herança em Go?
    - [ ] Deixa o código mais colorido
    - [x] Evita hierarquias complexas e rígidas, promovendo o desacoplamento
    - [ ] Permite que o código rode mais rápido no Windows
    - [ ] Nenhuma, herança é sempre melhor
    *Explicação: A composição permite montar tipos complexos como "peças de Lego".*

4. Para que serve a "Interface Vazia" `interface{}` (ou `any` nas versões mais novas)?
    - [ ] Para indicar que o programa não faz nada
    - [x] Para representar um valor de qualquer tipo
    - [ ] Para deletar variáveis da memória
    - [ ] Para criar um loop que nunca termina
    *Explicação: Ela é a base para funções que precisam aceitar qualquer tipo de dado.*

5. O que significa "Aceite Interfaces, Retorne Structs"?
    - [ ] É uma regra de etiqueta do Google
    - [x] É uma boa prática que dá flexibilidade a quem chama a função e clareza no retorno
    - [ ] Significa que o código deve ser escrito apenas com interfaces
    - [ ] É um padrão para banco de dados
    *Explicação: Aceitar interfaces torna sua função genérica; retornar structs dá rapidez e precisão no uso.*

6. Como você faz o "Type Assertion" para descobrir o tipo real por trás de uma interface?
    - [ ] var x = interface.(tipo)
    - [ ] interface.as(tipo)
    - [x] valor, ok := interface.(tipo)
    - [ ] check(interface == tipo)
    *Explicação: O padrão `v, ok := i.(T)` permite verificar o tipo de forma segura.*

7. Em Go, podemos anexar métodos a tipos básicos (como `int`)?
    - [ ] Não, apenas a structs
    - [x] Sim, desde que você defina um novo tipo (ex: `type MeuInt int`)
    - [ ] Sim, basta usar a extensão .go
    - [ ] Somente se o computador for de 64 bits
    *Explicação: Criar novos tipos permite estender funcionalidades até de tipos primitivos.*

8. Qual o limite de métodos que uma interface pode ter?
    - [ ] No máximo 10
    - [ ] Apenas 1
    - [x] Não há limite técnico, mas interfaces pequenas (1 ou 2 métodos) são preferíveis
    - [ ] Elas devem ter sempre um número par de métodos
    *Explicação: Interfaces pequenas são mais fáceis de implementar e reutilizar.*

9. O que é "Embedding" (Embutimento) na Composição?
    - [ ] Colocar o computador dentro de uma caixa
    - [ ] Copiar e colar código de um arquivo no outro
    - [x] Colocar uma struct dentro de outra sem dar um nome ao campo, herdando seus métodos
    - [ ] Salvar o código no banco de dados
    *Explicação: O embedding faz com que a struct externa "ganhe" os métodos da interna automaticamente.*

10. Go suporta Polimorfismo?
    - [ ] Não, Go é funcional
    - [x] Sim, através do uso de Interfaces
    - [ ] Somente se usar o pacote `poly`
    - [ ] Não, Go é procedural e não tem objetos
    *Explicação: O polimorfismo em Go é limpo e focado no comportamento, não na identidade.*