# Quiz 13 - Testes em Go ✅

1. Qual o sufixo obrigatório de um arquivo que contém testes em Go?
    - [ ] .test
    - [ ] _go_test.go
    - [x] _test.go
    - [ ] .spec.go
    *Explicação: O compilador Go ignora arquivos com este sufixo durante a compilação normal e só os usa no comando `go test`.*

2. Qual o parâmetro obrigatório de uma função de teste unitário?
    - [ ] s *sync.WaitGroup
    - [x] t *testing.T
    - [ ] err error
    - [ ] ctx context.Context
    *Explicação: O objeto `*testing.T` fornece métodos para reportar falhas e logs nos testes.*

3. De onde vem o pacote de testes do Go?
    - [ ] É preciso baixar do GitHub
    - [x] Faz parte da biblioteca padrão (`testing`)
    - [ ] É um plugin do VS Code
    - [ ] Vem junto com o Docker
    *Explicação: Go preza por ter ferramentas de qualidade embutidas na linguagem.*

4. O que é um "Table-Driven Test" (Teste de Tabela)?
    - [ ] Um teste feito no Excel
    - [x] Uma técnica de organizar vários cenários de entrada e saída em um slice para testar uma única função
    - [ ] Um teste que verifica se o banco de dados tem tabelas
    - [ ] Um teste que roda apenas em tabelas HTML
    *Explicação: É a forma mais organizada e escalável de escrever testes em Go.*

5. Qual comando gera um relatório de cobertura de testes no terminal?
    - [ ] go test -v
    - [x] go test -cover
    - [ ] go coverage
    - [ ] go check
    *Explicação: A cobertura indica quais partes do seu código foram realmente executadas pelos testes.*

6. Para que serve o pacote `httptest`?
    - [ ] Para hackear sites
    - [x] Para simular requisições e respostas HTTP sem precisar subir um servidor real
    - [ ] Para medir a velocidade da internet
    - [ ] Para criar sites bonitos
    *Explicação: Essencial para testar Handlers e Middlewares de forma isolada.*

7. Em Go, o que significa TDD (Test Driven Development)?
    - [ ] Total Data Design
    - [x] Desenvolvimento Orientado por Testes (escrever o teste antes do código)
    - [ ] Técnica De Depuração
    - [ ] Trabalho De Desenvolvedor
    *Explicação: O TDD ajuda a desenhar funções melhores e mais simples.*

8. O que acontece se uma função de teste começar com letra minúscula (ex: `func testSoma`)?
    - [ ] O Go avisa que está errado
    - [ ] O programa trava
    - [x] O `go test` irá ignorar a função (ela deve começar obrigatoriamente com `Test...`)
    - [ ] Ela vira um teste privado
    *Explicação: A ferramenta de testes só executa funções exportadas que seguem o padrão `TestXxx`.*

9. Qual o papel do método `t.Errorf`?
    - [ ] Encerrar o programa imediatamente
    - [x] Reportar que um teste falhou mas continuar a execução dos próximos testes
    - [ ] Enviar um e-mail para o desenvolvedor
    - [ ] Formatar o código
    *Explicação: Ele permite capturar múltiplos erros em uma única rodada de testes.*

10. Pode-se testar performance (benchmarks) no Go nativamente?
    - [ ] Não, precisa de ferramentas externas
    - [x] Sim, usando funções que começam com `Benchmark...` e o objeto `*testing.B`
    - [ ] Sim, mas apenas em servidores potentes
    - [ ] Somente se o código estiver em nuvem
    *Explicação: Go possui um sistema robusto para medir a velocidade e alocação de memória das suas funções.*
