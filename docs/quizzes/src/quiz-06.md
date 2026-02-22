# Quiz 06 - Tratamento de Erros ⚠️

1. Qual o padrão idiomático para tratar erros em Go?
    - [ ] Usar blocos try/catch/finally
    - [x] Verificar se o retorno do tipo `error` é diferente de `nil`
    - [ ] Ignorar todos os erros e torcer para o melhor
    - [ ] Usar somente o comando panic
    *Explicação: Go trata erros como valores comuns, forçando o desenvolvedor a lidar com eles no momento em que ocorrem.*

2. O que é o tipo `error` em Go?
    - [ ] Uma palavra-chave do sistema operacional
    - [x] Uma interface nativa com o método `Error() string`
    - [ ] Um número inteiro que indica o código do erro
    - [ ] Um booleano (true ou false)
    *Explicação: Por ser uma interface, qualquer tipo que implemente o método `Error()` pode ser usado como erro.*

3. Quando se deve usar a função `panic`?
    - [ ] Em qualquer erro de validação de formulário
    - [x] Apenas para erros críticos e irrecuperáveis que impedem o programa de continuar
    - [ ] Para retornar mensagens de sucesso
    - [ ] Para fechar o programa voluntariamente
    *Explicação: O panic é agressivo e deve ser reservado para falhas catastróficas (ex: falta de memória).*

4. Qual a função do comando `defer`?
    - [ ] Deletar uma variável
    - [x] Adiar a execução de uma função até o final da função atual (mesmo em caso de erro)
    - [ ] Aumentar a velocidade do loop for
    - [ ] Esconder o erro do usuário
    *Explicação: Essencial para garantir o fechamento de arquivos e conexões de rede.*

5. Para que serve o comando `recover`?
    - [ ] Para recuperar arquivos deletados
    - [x] Para capturar um panic em execução e evitar o encerramento do programa
    - [ ] Para restaurar o banco de dados
    - [ ] Para atualizar a versão do Go
    *Explicação: O recover só funciona dentro de uma função chamada via `defer`.*

6. Qual a diferença entre `errors.New` e `fmt.Errorf`?
    - [ ] Nenhuma, são sinônimos
    - [ ] `errors.New` é mais rápido no Linux
    - [x] `fmt.Errorf` permite formatar a mensagem com variáveis (estilo Printf)
    - [ ] `errors.New` apaga o log automaticamente
    *Explicação: `fmt.Errorf` é ideal para adicionar contexto dinâmico ao erro.*

7. Por que Go não utiliza exceções (try/catch)?
    - [ ] Porque os criadores esqueceram de implementar
    - [x] Para manter o fluxo de controle visível, simples e evitar "saltos" mágicos no código
    - [ ] Porque exceções consomem muita bateria
    - [ ] Porque Go é uma linguagem para crianças
    *Explicação: O tratamento explícito torna o código mais previsível e fácil de debugar.*

8. O que acontece se você declarar um erro e não verificá-lo (usar `_`)?
    - [ ] O Go avisa o usuário na tela
    - [ ] O programa fica mais rápido
    - [x] Você corre o risco de ignorar falhas graves, gerando bugs difíceis de encontrar
    - [ ] O compilador deleta o arquivo fonte
    *Explicação: Ignorar erros é considerado um dos maiores "pecados" de um desenvolvedor Go.*

9. Onde o comando `defer` costuma ser colocado?
    - [ ] Sempre no final da função
    - [x] Logo após a declaração bem-sucedida do recurso (ex: após abrir um arquivo)
    - [ ] Apenas dentro do pacote main
    - [ ] Em um arquivo separado de configuração
    *Explicação: Colocá-lo logo após o recurso evita o esquecimento de fechá-lo.*

10. Pode-se retornar um valor e um erro ao mesmo tempo?
    - [ ] Não, é proibido
    - [x] Sim, é o padrão recomendado em Go
    - [ ] Somente se o valor for uma string
    - [ ] Apenas em funções que usam ponteiros
    *Explicação: `return resultado, nil` ou `return nil, erro` é a base da robustez do Go.*
