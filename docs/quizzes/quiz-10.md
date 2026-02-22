# Quiz 10 - Construindo APIs REST 🏗️

--8<-- "assets/quiz.html"

<div class="quiz-container">
  <div class="quiz-question">1. No design de APIs REST, o que representa um "Recurso"?</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. REST foca na manipulação de recursos através de identificadores únicos (URIs).">O código fonte do servidor</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! REST foca na manipulação de recursos através de identificadores únicos (URIs).">Qualquer entidade ou dado nomeável (ex: /usuarios, /produtos)</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. REST foca na manipulação de recursos através de identificadores únicos (URIs).">A velocidade da CPU</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. REST foca na manipulação de recursos através de identificadores únicos (URIs).">O manual de instruções</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">2. Qual a principal vantagem de organizar o projeto em Camadas (MVC/Serviços)?</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. Separar lógica de negócio, acesso a dados e handlers HTTP garante um sistema escalável.">O código fica mais bonito no editor</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! Separar lógica de negócio, acesso a dados e handlers HTTP garante um sistema escalável.">Facilita a manutenção, testes e a troca de tecnologias (ex: mudar o banco de dados)</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. Separar lógica de negócio, acesso a dados e handlers HTTP garante um sistema escalável.">O programa compila mais rápido</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. Separar lógica de negócio, acesso a dados e handlers HTTP garante um sistema escalável.">Impede que hackers vejam o código</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">3. Qual verbo HTTP deve ser usado para CRIAR um novo recurso?</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. O POST é o método padrão para submissão de novos dados para o servidor.">GET</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! O POST é o método padrão para submissão de novos dados para o servidor.">POST</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. O POST é o método padrão para submissão de novos dados para o servidor.">PUT</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. O POST é o método padrão para submissão de novos dados para o servidor.">DELETE</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">4. O que a camada "Repository" deve fazer?</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. O Repository abstrai como e onde os dados são salvos.">Validar o e-mail do usuário</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! O Repository abstrai como e onde os dados são salvos.">Lidar puramente com a persistência e busca de dados (Banco de Dados/Arquivos)</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. O Repository abstrai como e onde os dados são salvos.">Desenhar o JSON de resposta</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. O Repository abstrai como e onde os dados são salvos.">Controlar as rotas da API</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">5. Qual o código de status HTTP recomendado ao se criar um recurso com sucesso?</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. O 201 informa explicitamente que algo novo nasceu no sistema.">200 OK</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! O 201 informa explicitamente que algo novo nasceu no sistema.">201 Created</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. O 201 informa explicitamente que algo novo nasceu no sistema.">400 Bad Request</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. O 201 informa explicitamente que algo novo nasceu no sistema.">500</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">6. No REST profissional, devemos usar verbos nas URLs (ex: `/deletar_item/123`)?</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. APIs RESTful usam os métodos HTTP para definir a ação sem poluir a URL.">Sim, deixa mais claro</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! APIs RESTful usam os métodos HTTP para definir a ação sem poluir a URL.">Não, devemos usar substantivos e deixar a ação para o Verbo HTTP (ex: `DELETE /items/123`)</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. APIs RESTful usam os métodos HTTP para definir a ação sem poluir a URL.">Depende do humor do desenvolvedor</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. APIs RESTful usam os métodos HTTP para definir a ação sem poluir a URL.">Somente se o projeto for pequeno</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">7. Para que serve o método `PATCH`?</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. Diferente do PUT (substituição total), o PATCH é cirúrgico.">Para deletar tudo</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! Diferente do PUT (substituição total), o PATCH é cirúrgico.">Para atualizar apenas parte de um recurso (ex: mudar só o preço de um produto)</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. Diferente do PUT (substituição total), o PATCH é cirúrgico.">Para enviar mensagens secretas</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. Diferente do PUT (substituição total), o PATCH é cirúrgico.">Para instalar atualizações no servidor</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">8. O que é "Idempotência"?</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. GET, PUT e DELETE são idempotentes; POST geralmente não é.">Um tipo de bateria de longa duração</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! GET, PUT e DELETE são idempotentes; POST geralmente não é.">A propriedade de uma requisição que, se repetida, produz o mesmo resultado no servidor sem efeitos colaterais extras</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. GET, PUT e DELETE são idempotentes; POST geralmente não é.">Uma função que gera números aleatórios</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. GET, PUT e DELETE são idempotentes; POST geralmente não é.">A velocidade de resposta da internet</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">9. Onde costuma ficar a "Regra de Negócio" na organização por camadas?</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. A camada de serviço é o "cérebro" que toma decisões baseadas nos dados.">No arquivo main.go</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! A camada de serviço é o "cérebro" que toma decisões baseadas nos dados.">Na camada de Service (Serviços)</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. A camada de serviço é o "cérebro" que toma decisões baseadas nos dados.">Dentro do banco de dados</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. A camada de serviço é o "cérebro" que toma decisões baseadas nos dados.">No frontend</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">10. Qual ferramenta é o padrão para documentar e testar contratos de APIs REST?</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. O Swagger gera uma documentação viva e interativa da sua API.">Microsoft Word</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! O Swagger gera uma documentação viva e interativa da sua API.">Swagger (OpenAPI)</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. O Swagger gera uma documentação viva e interativa da sua API.">Paint</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. O Swagger gera uma documentação viva e interativa da sua API.">Notepad++</div>
  <div class="quiz-feedback"></div>
</div>
