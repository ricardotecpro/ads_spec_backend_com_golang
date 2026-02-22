# Quiz 08 - Concorrência em Go ⚡

--8<-- "assets/quiz.html"

<div class="quiz-container">
  <div class="quiz-question">1. O que é uma "Goroutine"?</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. Goroutines permitem rodar milhares de tarefas simultâneas com pouquíssima memória (aprox. 2KB cada).">Uma rotina de exercícios físicos para programadores</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! Goroutines permitem rodar milhares de tarefas simultâneas com pouquíssima memória (aprox. 2KB cada).">Uma thread extremamente leve gerenciada pelo runtime do Go</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. Goroutines permitem rodar milhares de tarefas simultâneas com pouquíssima memória (aprox. 2KB cada).">Uma função que só roda no navegador</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. Goroutines permitem rodar milhares de tarefas simultâneas com pouquíssima memória (aprox. 2KB cada).">Uma ferramenta para comprimir imagens</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">2. Qual palavra-chave é usada para disparar uma função em segundo plano de forma concorrente?</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. Basta um `go minhaFuncao()` para que ela execute de forma assíncrona.">thread</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. Basta um `go minhaFuncao()` para que ela execute de forma assíncrona.">async</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! Basta um `go minhaFuncao()` para que ela execute de forma assíncrona.">go</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. Basta um `go minhaFuncao()` para que ela execute de forma assíncrona.">parallel</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">3. Segundo a filosofia do Go, como devemos gerenciar o estado entre tarefas concorrentes?</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. Canais (Channels) são a forma segura e elegante de trocar dados entre goroutines.">Usando variáveis globais e locks pesados</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! Canais (Channels) são a forma segura e elegante de trocar dados entre goroutines.">Não comunique compartilhando memória; compartilhe memória comunicando (através de Canais)</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. Canais (Channels) são a forma segura e elegante de trocar dados entre goroutines.">Usando arquivos de texto temporários</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. Canais (Channels) são a forma segura e elegante de trocar dados entre goroutines.">O Go não permite compartilhar dados</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">4. O que acontece se você tentar ler de um canal vazio em que ninguém está enviando nada?</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. O bloqueio de canais é o que permite o sincronismo natural do Go.">Ele retorna um erro imediatamente</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. O bloqueio de canais é o que permite o sincronismo natural do Go.">Ele retorna zero</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! O bloqueio de canais é o que permite o sincronismo natural do Go.">A goroutine fica bloqueada (em espera) até que algo seja enviado</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. O bloqueio de canais é o que permite o sincronismo natural do Go.">O computador reinicia</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">5. Para que serve o comando `select`?</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. O `select` é como um `switch`, mas para operações de entrada e saída em canais.">Para escolher qual banco de dados usar</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! O `select` é como um `switch`, mas para operações de entrada e saída em canais.">Para aguardar por múltiplas operações em canais simultâneos</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. O `select` é como um `switch`, mas para operações de entrada e saída em canais.">Para selecionar texto no terminal</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. O `select` é como um `switch`, mas para operações de entrada e saída em canais.">Para deletar goroutines travadas</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">6. Qual a diferença entre um Canal comum e um "Buffered Channel" (Canal com Buffer)?</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. Canais com buffer evitam bloqueios imediatos se houver espaço no "balde".">O Buffered Channel é azul</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! Canais com buffer evitam bloqueios imediatos se houver espaço no "balde".">O Buffered Channel permite enviar uma quantidade limitada de dados sem precisar de um recebedor imediato</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. Canais com buffer evitam bloqueios imediatos se houver espaço no "balde".">O Buffered Channel é mais lento</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. Canais com buffer evitam bloqueios imediatos se houver espaço no "balde".">Não há diferença</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">7. O que é um "Deadlock"?</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. É um erro comum de lógica em sistemas concorrentes que o Go consegue detectar em tempo de execução.">Um filme de ação famoso</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! É um erro comum de lógica em sistemas concorrentes que o Go consegue detectar em tempo de execução.">Uma situação onde todas as goroutines estão bloqueadas esperando umas pelas outras</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. É um erro comum de lógica em sistemas concorrentes que o Go consegue detectar em tempo de execução.">Quando o código é apagado acidentalmente</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. É um erro comum de lógica em sistemas concorrentes que o Go consegue detectar em tempo de execução.">Quando a internet cai durante a compilação</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">8. Qual o tamanho médio inicial de memória que uma Goroutine consome?</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. Por serem tão leves, você pode rodar milhões delas em um único servidor.">2 MB (como uma thread comum de SO)</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. Por serem tão leves, você pode rodar milhões delas em um único servidor.">1 GB</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! Por serem tão leves, você pode rodar milhões delas em um único servidor.">Cerca de 2 KB</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. Por serem tão leves, você pode rodar milhões delas em um único servidor.">0 bytes</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">9. Para que serve o pacote `sync.WaitGroup`?</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. O `Wait()` trava o programa principal até que todas as goroutines avisem que terminaram (`Done()`).">Para fazer o programa esperar o usuário apertar uma tecla</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! O `Wait()` trava o programa principal até que todas as goroutines avisem que terminaram (`Done()`).">Para sincronizar a conclusão de um grupo de goroutines antes de encerrar o programa</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. O `Wait()` trava o programa principal até que todas as goroutines avisem que terminaram (`Done()`).">Para limpar o cache do computador</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. O `Wait()` trava o programa principal até que todas as goroutines avisem que terminaram (`Done()`).">Para organizar arquivos por data</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">10. Go utiliza paralelismo real?</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. O escalonador do Go (scheduler) aproveita todo o poder do seu hardware multicore.">Não, apenas simulação</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! O escalonador do Go (scheduler) aproveita todo o poder do seu hardware multicore.">Sim, o runtime distribui as goroutines entre os diversos núcleos (cores) da CPU</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. O escalonador do Go (scheduler) aproveita todo o poder do seu hardware multicore.">Somente se o programador escrever código em Assembly</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. O escalonador do Go (scheduler) aproveita todo o poder do seu hardware multicore.">Somente em servidores Linux</div>
  <div class="quiz-feedback"></div>
</div>
