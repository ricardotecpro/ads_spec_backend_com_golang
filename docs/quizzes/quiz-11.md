# Quiz 11 - Framework Web Gin 🚀

--8<-- "assets/quiz.html"

<div class="quiz-container">
  <div class="quiz-question">1. O Gin é considerado um framework "leve" e "rápido". Qual o principal motivo dessa fama?</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. O roteador do Gin é um dos mais performáticos do ecossistema Go.">Ele usa inteligência artificial para codar</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! O roteador do Gin é um dos mais performáticos do ecossistema Go.">Ele utiliza um roteador baseado em Radix Tree e tem baixíssima alocação de memória</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. O roteador do Gin é um dos mais performáticos do ecossistema Go.">Ele apaga os arquivos desnecessários do Windows</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. O roteador do Gin é um dos mais performáticos do ecossistema Go.">Ele só funciona com strings curtas</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">2. No Gin, qual objeto central é passado para todos os handlers para gerenciar a requisição e a resposta?</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. O `*gin.Context` encapsula tudo o que você precisa (parâmetros, JSON, resposta).">gin.Server</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! O `*gin.Context` encapsula tudo o que você precisa (parâmetros, JSON, resposta).">*gin.Context</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. O `*gin.Context` encapsula tudo o que você precisa (parâmetros, JSON, resposta).">http.Request</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. O `*gin.Context` encapsula tudo o que você precisa (parâmetros, JSON, resposta).">context.Background()</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">3. Como se define uma rota com parâmetro dinâmico no Gin (ex: pegar o ID do usuário)?</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. O uso dos dois pontos `:` define um parâmetro que pode ser recuperado via `c.Param("id")`.">r.GET("/user/ID")</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! O uso dos dois pontos `:` define um parâmetro que pode ser recuperado via `c.Param("id")`.">r.GET("/user/:id")</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. O uso dos dois pontos `:` define um parâmetro que pode ser recuperado via `c.Param("id")`.">r.GET("/user/$id")</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. O uso dos dois pontos `:` define um parâmetro que pode ser recuperado via `c.Param("id")`.">r.GET("/user/?id")</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">4. Qual a função do método `c.ShouldBindJSON(&struct)`?</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. O Binding economiza dezenas de linhas de tratamento manual de bytes.">Deletar o JSON enviado</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! O Binding economiza dezenas de linhas de tratamento manual de bytes.">Mapear automaticamente o corpo da requisição (JSON) para uma struct em Go</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. O Binding economiza dezenas de linhas de tratamento manual de bytes.">Validar a conexão com a internet</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. O Binding economiza dezenas de linhas de tratamento manual de bytes.">Transformar a struct em uma imagem</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">5. O que o `gin.H{}` permite que façamos?</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. `gin.H` é um atalho para `map[string]interface{}`.">Criar um loop infinito</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! `gin.H` é um atalho para `map[string]interface{}`.">Escrever um JSON de forma rápida e curta no estilo chave-valor</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. `gin.H` é um atalho para `map[string]interface{}`.">Hostear o site na nuvem</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. `gin.H` é um atalho para `map[string]interface{}`.">Esconder o cabeçalho da página</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">6. Como você agrupa rotas que compartilham um prefixo comum (ex: `/api/v1`)?</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. Grupos de rotas permitem aplicar middlewares a conjuntos específicos de endpoints.">Copiando e colando o prefixo em cada linha</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! Grupos de rotas permitem aplicar middlewares a conjuntos específicos de endpoints.">Usando o método `r.Group("/api/v1")`</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. Grupos de rotas permitem aplicar middlewares a conjuntos específicos de endpoints.">Criando vários servidores diferentes</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. Grupos de rotas permitem aplicar middlewares a conjuntos específicos de endpoints.">O Gin não permite agrupamento</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">7. Para que serve a tag `binding:"required"` nas structs?</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. O Gin retorna erro automaticamente se um campo obrigatório estiver faltando.">Para deixar o texto em negrito</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! O Gin retorna erro automaticamente se um campo obrigatório estiver faltando.">Para que o Gin valide automaticamente se aquele campo foi enviado no JSON</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. O Gin retorna erro automaticamente se um campo obrigatório estiver faltando.">Para travar o banco de dados</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. O Gin retorna erro automaticamente se um campo obrigatório estiver faltando.">Para aumentar a segurança contra hackers</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">8. Qual o comando para iniciar o servidor Gin na porta padrão?</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. O `Run()` inicia o motor do framework e aguarda conexões na porta 8080.">r.Start()</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! O `Run()` inicia o motor do framework e aguarda conexões na porta 8080.">r.Run()</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. O `Run()` inicia o motor do framework e aguarda conexões na porta 8080.">r.Listen()</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. O `Run()` inicia o motor do framework e aguarda conexões na porta 8080.">r.Serve()</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">9. O Gin já vem com sistema de logs e recuperação de pânicos (Recovery) por padrão?</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. O Log ajuda no debug e o Recovery evita que o servidor caia por um erro inesperado.">Não, deve ser instalado por fora</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! O Log ajuda no debug e o Recovery evita que o servidor caia por um erro inesperado.">Sim, ao usar `gin.Default()`, esses dois middlewares são ativados</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. O Log ajuda no debug e o Recovery evita que o servidor caia por um erro inesperado.">Somente se o computador for potente</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. O Log ajuda no debug e o Recovery evita que o servidor caia por um erro inesperado.">Somente na versão paga</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">10. Podemos usar Middlewares personalizados no Gin?</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. O sistema de middlewares do Gin é extremamente modular e fácil de usar.">Não, o Gin é fechado</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! O sistema de middlewares do Gin é extremamente modular e fácil de usar.">Sim, usando o método `r.Use()`</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. O sistema de middlewares do Gin é extremamente modular e fácil de usar.">Sim, mas apenas para contar o tempo</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. O sistema de middlewares do Gin é extremamente modular e fácil de usar.">Somente no pacote main</div>
  <div class="quiz-feedback"></div>
</div>
