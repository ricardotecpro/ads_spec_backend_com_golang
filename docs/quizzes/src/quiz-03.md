# Quiz 03 - Funções e Organização do Código 🧩

1. Como o Go permite que uma função retorne mais de um valor?
    - [ ] Ele não permite, deve-se usar um array
    - [x] Basta listar os tipos de retorno entre parênteses na assinatura da função
    - [ ] Somente se a função for iniciada com `func*`
    - [ ] Através de variáveis globais
    *Explicação: `func divisao(a, b int) (int, error)` é um padrão comum em Go.*

2. Para que serve o operador `&` antes de uma variável?
    - [ ] Para realizar uma operação lógica "AND"
    - [x] Para obter o endereço de memória (ponteiro) daquela variável
    - [ ] Para deletar a variável da memória
    - [ ] Para converter um número em string
    *Explicação: O `&` diz "onde está" o dado na memória.*

3. O que define se uma função ou variável é "pública" (exportada) para outros pacotes no Go?
    - [ ] A palavra-chave `public`
    - [ ] Se ela estiver dentro do arquivo `main.go`
    - [x] Se o nome dela começar com uma letra Maiúscula
    - [ ] Se ela tiver um comentário em cima
    *Explicação: Go usa a capitalização para controle de visibilidade (ex: `Fmt` vs `fmt`).*

4. Qual a finalidade principal de usar um Ponteiro em Go?
    - [ ] Deixar o código mais complexo e difícil de ler
    - [x] Evitar cópias desnecessárias de dados grandes ou permitir que uma função altere o valor original
    - [ ] O Go obriga o uso de ponteiros em todas as variáveis
    - [ ] Para rodar o código em servidores antigos
    *Explicação: Ponteiros dão eficiência e controle sobre o estado da aplicação.*

5. O que são "Variadic Functions"?
    - [ ] Funções que mudam de nome sozinhas
    - [x] Funções que aceitam um número indeterminado de argumentos do mesmo tipo
    - [ ] Funções que não retornam nada
    - [ ] Funções que só funcionam em variáveis do tipo bool
    *Explicação: O uso de `...tipo` permite passar quantos argumentos você quiser.*

6. Como você ignora um valor de retorno que não deseja usar?
    - [ ] Deixando um espaço em branco
    - [x] Usando o identificador em branco `_` (underscore)
    - [ ] Usando a palavra-chave `ignore`
    - [ ] O Go não permite ignorar retornos
    *Explicação: O `_` diz ao compilador para descartar aquele valor específico.*

7. Todo projeto Go deve ter obrigatoriamente um pacote chamado:
    - [ ] start
    - [x] main
    - [ ] root
    - [ ] server
    *Explicação: O pacote `main` informa ao compilador onde a execução do programa começa.*

8. O que o arquivo `go.mod` gerencia?
    - [ ] A configuração do roteador wi-fi
    - [ ] O banco de dados do sistema
    - [x] O nome do módulo e suas dependências externas
    - [ ] O estilo visual do console
    *Explicação: Ele é a base do gerenciamento de pacotes moderno do Go.*

9. Qual o operador usado para acessar o valor dentro de um ponteiro (desreferenciação)?
    - [ ] &
    - [ ] #
    - [x] *
    - [ ] ->
    *Explicação: O `*` busca o "conteúdo" do endereço apontado.*

10. Funções podem ser passadas como argumentos para outras funções em Go?
    - [ ] Não, isso é impossível
    - [x] Sim, funções são cidadãs de primeira classe
    - [ ] Somente se forem funções matemáticas
    - [ ] Sim, mas apenas dentro do pacote `main`
    *Explicação: Isso permite padrões poderosos como middlewares e callbacks.*
