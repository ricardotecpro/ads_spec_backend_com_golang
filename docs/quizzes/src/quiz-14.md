# Quiz 14 - Arquitetura e Boas Práticas 🏗️

1. Qual o maior objetivo da "Clean Architecture"?
    - [ ] Fazer com que o código rode em computadores antigos
    - [x] Isolar a lógica de negócio de detalhes externos como banco de dados, UI e frameworks
    - [ ] Exigir que o programador tome banho antes de codar
    - [ ] Diminuir o espaço em disco do projeto
    *Explicação: A arquitetura limpa permite que o "coração" do sistema seja testável e imune a trocas de tecnologia externa.*

2. Em Go, o que define a camada de "Entidade"?
    - [ ] A conexão com o banco de dados
    - [x] As structs que representam o domínio do negócio e suas regras fundamentais
    - [ ] Os scripts de deploy
    - [ ] A interface visual do site
    *Explicação: Entidades são o nível mais alto e estável da arquitetura.*

3. O que é "Injeção de Dependência" (DI)?
    - [ ] Colocar vírus no código de terceiros
    - [x] Passar as dependências de um objeto (como um repositório) via construtor ou interface, em vez de criá-las internamente
    - [ ] Uma vacina para erros de sintaxe
    - [ ] Formatar o computador via terminal
    *Explicação: A DI permite desacoplar componentes, facilitando o uso de Mocks nos testes.*

4. Por que a pasta `internal/` é especial em Go?
    - [ ] Porque ela é escondida por padrão
    - [x] Porque o compilador impede que pacotes fora do projeto importem o código que está dentro dela
    - [ ] Porque ela acelera o processamento de imagens
    - [ ] Porque só o administrador pode editá-la
    *Explicação: É a forma do Go garantir o encapsulamento e privacidade de módulos internos.*

5. Qual a recomendação para nomenclatura de pacotes em Go?
    - [ ] Usar nomes complexos e técnicos (ex: `BusinessLogicImplementation`)
    - [x] Usar substantivos curtos, simples e em minúsculo (ex: `user`, `auth`, `order`)
    - [ ] Usar apenas números
    - [ ] Usar o nome do desenvolvedor
    *Explicação: Nomes simples facilitam a leitura e o import do código.*

6. O que significa a frase "Retorne structs, aceite interfaces"?
    - [ ] É uma tradução errada de um livro
    - [x] Que suas funções devem aceitar abstrações (interfaces) para serem flexíveis, mas retornar dados concretos para serem rápidas
    - [ ] Que o programa deve ter apenas 10 arquivos
    - [ ] Que não devemos usar variáveis
    *Explicação: Essa prática maximiza o polimorfismo mantendo a facilidade de uso do retorno.*

7. Na Clean Architecture, quem pode conhecer quem?
    - [ ] Todos podem conhecer todos
    - [x] As camadas externas podem conhecer as internas, mas as internas nunca conhecem as externas
    - [ ] Somente o banco de dados conhece o resto
    - [ ] As camadas são secretas
    *Explicação: A regra de dependência aponta sempre para dentro (para o Core).*

8. Qual o papel do arquivo `main.go` em um projeto bem arquitetado?
    - [ ] Conter toda a lógica do sistema
    - [x] Atuar como o "fio de ligação", instanciando as dependências e iniciando o servidor
    - [ ] Ser o manual de instruções
    - [ ] O projeto não precisa de um main.go
    *Explicação: O main deve ser magro, servindo apenas para o bootstrapping da aplicação.*

9. Go prefere Composição ou Herança?
    - [ ] Herança pesada com várias camadas
    - [x] Composição (Embedding)
    - [ ] Go não permite nenhum dos dois
    - [ ] Depende do sistema operacional
    *Explicação: A composição é considerada mais robusta e simples de manter em Go.*

10. Onde deve ficar a lógica de "Como salvar no banco de dados"?
    - [ ] Na camada de Service
    - [ ] No arquivo main
    - [x] Na camada de Repository
    - [ ] Directamente no Handler
    *Explicação: O Repository é o especialista em persistência, protegendo o resto do sistema dos detalhes do SQL.*
