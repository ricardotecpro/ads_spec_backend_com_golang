# Quiz 10 - Construindo APIs REST 🏗️

1. No design de APIs REST, o que representa um "Recurso"?
    - [ ] O código fonte do servidor
    - [x] Qualquer entidade ou dado nomeável (ex: /usuarios, /produtos)
    - [ ] A velocidade da CPU
    - [ ] O manual de instruções
    *Explicação: REST foca na manipulação de recursos através de identificadores únicos (URIs).*

2. Qual a principal vantagem de organizar o projeto em Camadas (MVC/Serviços)?
    - [ ] O código fica mais bonito no editor
    - [x] Facilita a manutenção, testes e a troca de tecnologias (ex: mudar o banco de dados)
    - [ ] O programa compila mais rápido
    - [ ] Impede que hackers vejam o código
    *Explicação: Separar lógica de negócio, acesso a dados e handlers HTTP garante um sistema escalável.*

3. Qual verbo HTTP deve ser usado para CRIAR um novo recurso?
    - [ ] GET
    - [x] POST
    - [ ] PUT
    - [ ] DELETE
    *Explicação: O POST é o método padrão para submissão de novos dados para o servidor.*

4. O que a camada "Repository" deve fazer?
    - [ ] Validar o e-mail do usuário
    - [x] Lidar puramente com a persistência e busca de dados (Banco de Dados/Arquivos)
    - [ ] Desenhar o JSON de resposta
    - [ ] Controlar as rotas da API
    *Explicação: O Repository abstrai como e onde os dados são salvos.*

5. Qual o código de status HTTP recomendado ao se criar um recurso com sucesso?
    - [ ] 200 OK
    - [x] 201 Created
    - [ ] 400 Bad Request
    - [ ] 500
    *Explicação: O 201 informa explicitamente que algo novo nasceu no sistema.*

6. No REST profissional, devemos usar verbos nas URLs (ex: `/deletar_item/123`)?
    - [ ] Sim, deixa mais claro
    - [x] Não, devemos usar substantivos e deixar a ação para o Verbo HTTP (ex: `DELETE /items/123`)
    - [ ] Depende do humor do desenvolvedor
    - [ ] Somente se o projeto for pequeno
    *Explicação: APIs RESTful usam os métodos HTTP para definir a ação sem poluir a URL.*

7. Para que serve o método `PATCH`?
    - [ ] Para deletar tudo
    - [x] Para atualizar apenas parte de um recurso (ex: mudar só o preço de um produto)
    - [ ] Para enviar mensagens secretas
    - [ ] Para instalar atualizações no servidor
    *Explicação: Diferente do PUT (substituição total), o PATCH é cirúrgico.*

8. O que é "Idempotência"?
    - [ ] Um tipo de bateria de longa duração
    - [x] A propriedade de uma requisição que, se repetida, produz o mesmo resultado no servidor sem efeitos colaterais extras
    - [ ] Uma função que gera números aleatórios
    - [ ] A velocidade de resposta da internet
    *Explicação: GET, PUT e DELETE são idempotentes; POST geralmente não é.*

9. Onde costuma ficar a "Regra de Negócio" na organização por camadas?
    - [ ] No arquivo main.go
    - [x] Na camada de Service (Serviços)
    - [ ] Dentro do banco de dados
    - [ ] No frontend
    *Explicação: A camada de serviço é o "cérebro" que toma decisões baseadas nos dados.*

10. Qual ferramenta é o padrão para documentar e testar contratos de APIs REST?
    - [ ] Microsoft Word
    - [x] Swagger (OpenAPI)
    - [ ] Paint
    - [ ] Notepad++
    *Explicação: O Swagger gera uma documentação viva e interativa da sua API.*
