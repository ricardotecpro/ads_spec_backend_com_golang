# Quiz 08 - Concorrência em Go ⚡

1. O que é uma "Goroutine"?
    - [ ] Uma rotina de exercícios físicos para programadores
    - [x] Uma thread extremamente leve gerenciada pelo runtime do Go
    - [ ] Uma função que só roda no navegador
    - [ ] Uma ferramenta para comprimir imagens
    *Explicação: Goroutines permitem rodar milhares de tarefas simultâneas com pouquíssima memória (aprox. 2KB cada).*

2. Qual palavra-chave é usada para disparar uma função em segundo plano de forma concorrente?
    - [ ] thread
    - [ ] async
    - [x] go
    - [ ] parallel
    *Explicação: Basta um `go minhaFuncao()` para que ela execute de forma assíncrona.*

3. Segundo a filosofia do Go, como devemos gerenciar o estado entre tarefas concorrentes?
    - [ ] Usando variáveis globais e locks pesados
    - [x] Não comunique compartilhando memória; compartilhe memória comunicando (através de Canais)
    - [ ] Usando arquivos de texto temporários
    - [ ] O Go não permite compartilhar dados
    *Explicação: Canais (Channels) são a forma segura e elegante de trocar dados entre goroutines.*

4. O que acontece se você tentar ler de um canal vazio em que ninguém está enviando nada?
    - [ ] Ele retorna um erro imediatamente
    - [ ] Ele retorna zero
    - [x] A goroutine fica bloqueada (em espera) até que algo seja enviado
    - [ ] O computador reinicia
    *Explicação: O bloqueio de canais é o que permite o sincronismo natural do Go.*

5. Para que serve o comando `select`?
    - [ ] Para escolher qual banco de dados usar
    - [x] Para aguardar por múltiplas operações em canais simultâneos
    - [ ] Para selecionar texto no terminal
    - [ ] Para deletar goroutines travadas
    *Explicação: O `select` é como um `switch`, mas para operações de entrada e saída em canais.*

6. Qual a diferença entre um Canal comum e um "Buffered Channel" (Canal com Buffer)?
    - [ ] O Buffered Channel é azul
    - [x] O Buffered Channel permite enviar uma quantidade limitada de dados sem precisar de um recebedor imediato
    - [ ] O Buffered Channel é mais lento
    - [ ] Não há diferença
    *Explicação: Canais com buffer evitam bloqueios imediatos se houver espaço no "balde".*

7. O que é um "Deadlock"?
    - [ ] Um filme de ação famoso
    - [x] Uma situação onde todas as goroutines estão bloqueadas esperando umas pelas outras
    - [ ] Quando o código é apagado acidentalmente
    - [ ] Quando a internet cai durante a compilação
    *Explicação: É um erro comum de lógica em sistemas concorrentes que o Go consegue detectar em tempo de execução.*

8. Qual o tamanho médio inicial de memória que uma Goroutine consome?
    - [ ] 2 MB (como uma thread comum de SO)
    - [ ] 1 GB
    - [x] Cerca de 2 KB
    - [ ] 0 bytes
    *Explicação: Por serem tão leves, você pode rodar milhões delas em um único servidor.*

9. Para que serve o pacote `sync.WaitGroup`?
    - [ ] Para fazer o programa esperar o usuário apertar uma tecla
    - [x] Para sincronizar a conclusão de um grupo de goroutines antes de encerrar o programa
    - [ ] Para limpar o cache do computador
    - [ ] Para organizar arquivos por data
    *Explicação: O `Wait()` trava o programa principal até que todas as goroutines avisem que terminaram (`Done()`).*

10. Go utiliza paralelismo real?
    - [ ] Não, apenas simulação
    - [x] Sim, o runtime distribui as goroutines entre os diversos núcleos (cores) da CPU
    - [ ] Somente se o programador escrever código em Assembly
    - [ ] Somente em servidores Linux
    *Explicação: O escalonador do Go (scheduler) aproveita todo o poder do seu hardware multicore.*
