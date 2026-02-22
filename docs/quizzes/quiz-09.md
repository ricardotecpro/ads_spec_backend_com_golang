# Quiz 09 - Programação Web com net/http 🌐

--8<-- "assets/quiz.html"

<div class="quiz-container">
  <div class="quiz-question">1. Como o Go permite rodar um servidor HTTP sem depender de softwares como Apache ou Nginx?</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. O pacote `net/http` é robusto o suficiente para ser o próprio servidor da aplicação.">Ele se conecta via Bluetooth</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! O pacote `net/http` é robusto o suficiente para ser o próprio servidor da aplicação.">Ele possui um servidor HTTP de nível de produção embutido na biblioteca padrão (`net/http`)</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. O pacote `net/http` é robusto o suficiente para ser o próprio servidor da aplicação.">Ele usa o Internet Explorer escondido</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. O pacote `net/http` é robusto o suficiente para ser o próprio servidor da aplicação.">Ele não roda sem o Nginx</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">2. No handler `func(w http.ResponseWriter, r *http.Request)`, qual o papel do `w`?</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. O `ResponseWriter` é o canal de saída do servidor para o cliente.">Representar o Windows do servidor</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! O `ResponseWriter` é o canal de saída do servidor para o cliente.">Enviar a resposta (Headers, Body, Status) de volta para o cliente</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. O `ResponseWriter` é o canal de saída do servidor para o cliente.">Receber os dados enviados pelo navegador</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. O `ResponseWriter` é o canal de saída do servidor para o cliente.">Inverter o sentido da internet</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">3. O que o objeto `r *http.Request` contém?</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. O `Request` é o pacote completo de informações que o cliente envia para o servidor.">Apenas o endereço IP do usuário</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! O `Request` é o pacote completo de informações que o cliente envia para o servidor.">Toda a informação da requisição: Método, URL, Cabeçalhos e Corpo (Body)</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. O `Request` é o pacote completo de informações que o cliente envia para o servidor.">O código fonte do navegador do cliente</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. O `Request` é o pacote completo de informações que o cliente envia para o servidor.">A senha do administrador</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">4. Qual comando inicia o servidor e o faz escutar em uma porta específica?</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. Esta função bloqueia a execução do main e mantém o servidor ativo respondendo requisições.">http.Start(":8080")</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. Esta função bloqueia a execução do main e mantém o servidor ativo respondendo requisições.">http.Listen()</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! Esta função bloqueia a execução do main e mantém o servidor ativo respondendo requisições.">http.ListenAndServe(":8080", nil)</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. Esta função bloqueia a execução do main e mantém o servidor ativo respondendo requisições.">server.Run()</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">5. O que são "Middlewares" em uma aplicação Web?</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. Middlewares permitem adicionar camadas de lógica comuns a várias rotas.">Softwares que ficam entre o teclado e a tela</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! Middlewares permitem adicionar camadas de lógica comuns a várias rotas.">Funções que interceptam uma requisição antes que ela chegue ao handler final (ex: para logs ou login)</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. Middlewares permitem adicionar camadas de lógica comuns a várias rotas.">Cabos de rede especiais</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. Middlewares permitem adicionar camadas de lógica comuns a várias rotas.">Vírus que lentificam o servidor</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">6. Como você serve arquivos estáticos (HTML, CSS, Imagens) em Go?</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. O FileServer é uma ferramenta nativa eficiente para entregar conteúdo estático.">Copiando e colando o arquivo na tela</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! O FileServer é uma ferramenta nativa eficiente para entregar conteúdo estático.">Usando o `http.FileServer` apontando para um diretório</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. O FileServer é uma ferramenta nativa eficiente para entregar conteúdo estático.">Go não serve arquivos estáticos</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. O FileServer é uma ferramenta nativa eficiente para entregar conteúdo estático.">Usando o comando `print(arquivo)`</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">7. O que acontece se uma rota não for encontrada e você não definiu um handler padrão?</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. O roteador padrão do Go já possui tratamento básico para rotas inexistentes.">O computador explode</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! O roteador padrão do Go já possui tratamento básico para rotas inexistentes.">O servidor retorna automaticamente o erro `404 page not found`</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. O roteador padrão do Go já possui tratamento básico para rotas inexistentes.">O servidor trava</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. O roteador padrão do Go já possui tratamento básico para rotas inexistentes.">Ele escolhe uma página aleatória</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">8. No Go nativo (`net/http`), como se pega um parâmetro da Query String (ex: `?id=10`)?</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. Os parâmetros de busca ficam organizados dentro do objeto URL da requisição.">r.ID()</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! Os parâmetros de busca ficam organizados dentro do objeto URL da requisição.">r.URL.Query().Get("id")</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. Os parâmetros de busca ficam organizados dentro do objeto URL da requisição.">r.Body["id"]</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. Os parâmetros de busca ficam organizados dentro do objeto URL da requisição.">Através de um loop for</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">9. Qual o valor de retorno padrão de uma requisição bem-sucedida?</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. O código 200 é o sinal universal de que a requisição foi atendida com sucesso.">0</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. O código 200 é o sinal universal de que a requisição foi atendida com sucesso.">404</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! O código 200 é o sinal universal de que a requisição foi atendida com sucesso.">200 OK</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. O código 200 é o sinal universal de que a requisição foi atendida com sucesso.">500</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">10. É possível rodar múltiplos servidores Go em portas diferentes no mesmo binário?</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. A concorrência do Go facilita subir múltiplos micro-serviços ou painéis administrativos no mesmo processo.">Não, apenas um por vez</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! A concorrência do Go facilita subir múltiplos micro-serviços ou painéis administrativos no mesmo processo.">Sim, usando Goroutines para iniciar cada `ListenAndServe`</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. A concorrência do Go facilita subir múltiplos micro-serviços ou painéis administrativos no mesmo processo.">Somente se houver duas placas de rede</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. A concorrência do Go facilita subir múltiplos micro-serviços ou painéis administrativos no mesmo processo.">Sim, mas eles compartilham o mesmo log</div>
  <div class="quiz-feedback"></div>
</div>
