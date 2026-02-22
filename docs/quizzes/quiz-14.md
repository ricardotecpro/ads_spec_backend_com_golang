# Quiz 14 - Arquitetura e Boas Práticas 🏗️

--8<-- "assets/quiz.html"

<div class="quiz-container">
  <div class="quiz-question">1. Qual o maior objetivo da "Clean Architecture"?</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. A arquitetura limpa permite que o "coração" do sistema seja testável e imune a trocas de tecnologia externa.">Fazer com que o código rode em computadores antigos</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! A arquitetura limpa permite que o "coração" do sistema seja testável e imune a trocas de tecnologia externa.">Isolar a lógica de negócio de detalhes externos como banco de dados, UI e frameworks</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. A arquitetura limpa permite que o "coração" do sistema seja testável e imune a trocas de tecnologia externa.">Exigir que o programador tome banho antes de codar</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. A arquitetura limpa permite que o "coração" do sistema seja testável e imune a trocas de tecnologia externa.">Diminuir o espaço em disco do projeto</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">2. Em Go, o que define a camada de "Entidade"?</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. Entidades são o nível mais alto e estável da arquitetura.">A conexão com o banco de dados</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! Entidades são o nível mais alto e estável da arquitetura.">As structs que representam o domínio do negócio e suas regras fundamentais</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. Entidades são o nível mais alto e estável da arquitetura.">Os scripts de deploy</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. Entidades são o nível mais alto e estável da arquitetura.">A interface visual do site</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">3. O que é "Injeção de Dependência" (DI)?</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. A DI permite desacoplar componentes, facilitando o uso de Mocks nos testes.">Colocar vírus no código de terceiros</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! A DI permite desacoplar componentes, facilitando o uso de Mocks nos testes.">Passar as dependências de um objeto (como um repositório) via construtor ou interface, em vez de criá-las internamente</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. A DI permite desacoplar componentes, facilitando o uso de Mocks nos testes.">Uma vacina para erros de sintaxe</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. A DI permite desacoplar componentes, facilitando o uso de Mocks nos testes.">Formatar o computador via terminal</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">4. Por que a pasta `internal/` é especial em Go?</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. É a forma do Go garantir o encapsulamento e privacidade de módulos internos.">Porque ela é escondida por padrão</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! É a forma do Go garantir o encapsulamento e privacidade de módulos internos.">Porque o compilador impede que pacotes fora do projeto importem o código que está dentro dela</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. É a forma do Go garantir o encapsulamento e privacidade de módulos internos.">Porque ela acelera o processamento de imagens</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. É a forma do Go garantir o encapsulamento e privacidade de módulos internos.">Porque só o administrador pode editá-la</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">5. Qual a recomendação para nomenclatura de pacotes em Go?</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. Nomes simples facilitam a leitura e o import do código.">Usar nomes complexos e técnicos (ex: `BusinessLogicImplementation`)</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! Nomes simples facilitam a leitura e o import do código.">Usar substantivos curtos, simples e em minúsculo (ex: `user`, `auth`, `order`)</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. Nomes simples facilitam a leitura e o import do código.">Usar apenas números</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. Nomes simples facilitam a leitura e o import do código.">Usar o nome do desenvolvedor</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">6. O que significa a frase "Retorne structs, aceite interfaces"?</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. Essa prática maximiza o polimorfismo mantendo a facilidade de uso do retorno.">É uma tradução errada de um livro</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! Essa prática maximiza o polimorfismo mantendo a facilidade de uso do retorno.">Que suas funções devem aceitar abstrações (interfaces) para serem flexíveis, mas retornar dados concretos para serem rápidas</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. Essa prática maximiza o polimorfismo mantendo a facilidade de uso do retorno.">Que o programa deve ter apenas 10 arquivos</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. Essa prática maximiza o polimorfismo mantendo a facilidade de uso do retorno.">Que não devemos usar variáveis</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">7. Na Clean Architecture, quem pode conhecer quem?</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. A regra de dependência aponta sempre para dentro (para o Core).">Todos podem conhecer todos</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! A regra de dependência aponta sempre para dentro (para o Core).">As camadas externas podem conhecer as internas, mas as internas nunca conhecem as externas</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. A regra de dependência aponta sempre para dentro (para o Core).">Somente o banco de dados conhece o resto</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. A regra de dependência aponta sempre para dentro (para o Core).">As camadas são secretas</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">8. Qual o papel do arquivo `main.go` em um projeto bem arquitetado?</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. O main deve ser magro, servindo apenas para o bootstrapping da aplicação.">Conter toda a lógica do sistema</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! O main deve ser magro, servindo apenas para o bootstrapping da aplicação.">Atuar como o "fio de ligação", instanciando as dependências e iniciando o servidor</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. O main deve ser magro, servindo apenas para o bootstrapping da aplicação.">Ser o manual de instruções</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. O main deve ser magro, servindo apenas para o bootstrapping da aplicação.">O projeto não precisa de um main.go</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">9. Go prefere Composição ou Herança?</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. A composição é considerada mais robusta e simples de manter em Go.">Herança pesada com várias camadas</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! A composição é considerada mais robusta e simples de manter em Go.">Composição (Embedding)</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. A composição é considerada mais robusta e simples de manter em Go.">Go não permite nenhum dos dois</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. A composição é considerada mais robusta e simples de manter em Go.">Depende do sistema operacional</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">10. Onde deve ficar a lógica de "Como salvar no banco de dados"?</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. O Repository é o especialista em persistência, protegendo o resto do sistema dos detalhes do SQL.">Na camada de Service</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. O Repository é o especialista em persistência, protegendo o resto do sistema dos detalhes do SQL.">No arquivo main</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! O Repository é o especialista em persistência, protegendo o resto do sistema dos detalhes do SQL.">Na camada de Repository</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. O Repository é o especialista em persistência, protegendo o resto do sistema dos detalhes do SQL.">Directamente no Handler</div>
  <div class="quiz-feedback"></div>
</div>
