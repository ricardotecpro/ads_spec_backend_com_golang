# Quiz 12 - Banco de Dados (GORM) 💾

--8<-- "assets/quiz.html"

<div class="quiz-container">
  <div class="quiz-question">1. O que significa a sigla ORM (como o GORM)?</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. ORMs transformam tabelas de banco de dados em objetos (structs) no código.">Organized Recovery Manager</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! ORMs transformam tabelas de banco de dados em objetos (structs) no código.">Object-Relational Mapping (Mapeamento Objeto-Relacional)</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. ORMs transformam tabelas de banco de dados em objetos (structs) no código.">Online Router Monitor</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. ORMs transformam tabelas de banco de dados em objetos (structs) no código.">Only Ready Models</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">2. Qual a principal vantagem do GORM sobre o pacote nativo `database/sql`?</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. O GORM traz alta produtividade ao abstrair o SQL complexo em funções Go.">Ele obriga o uso de cartões de crédito</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! O GORM traz alta produtividade ao abstrair o SQL complexo em funções Go.">Ele automatiza tarefas repetitivas como gerar queries SQL e gerenciar tabelas</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. O GORM traz alta produtividade ao abstrair o SQL complexo em funções Go.">Ele apaga o banco caso o código esteja feio</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. O GORM traz alta produtividade ao abstrair o SQL complexo em funções Go.">Ele só funciona no Google Cloud</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">3. Para que serve o método `db.AutoMigrate(&MinhaStruct{})`?</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. Migrations automáticas garantem que o banco acompanhe as mudanças do seu código.">Para migrar o código para outra linguagem</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! Migrations automáticas garantem que o banco acompanhe as mudanças do seu código.">Para criar ou atualizar automaticamente a tabela no banco conforme a estrutura da struct</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. Migrations automáticas garantem que o banco acompanhe as mudanças do seu código.">Para deletar todos os dados do banco</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. Migrations automáticas garantem que o banco acompanhe as mudanças do seu código.">Para salvar o banco de dados em um pendrive</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">4. O que a struct embarcada `gorm.Model` adiciona ao seu modelo?</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. Facilita a criação de metadados padrão para qualquer registro no banco.">Somente o campo de nome</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! Facilita a criação de metadados padrão para qualquer registro no banco.">ID, CreatedAt, UpdatedAt e DeletedAt (soft delete)</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. Facilita a criação de metadados padrão para qualquer registro no banco.">Um link para o GitHub do autor</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. Facilita a criação de metadados padrão para qualquer registro no banco.">A cor de fundo da tabela</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">5. Como o GORM trata a deleção de registros por padrão se o modelo tiver `gorm.Model`?</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. Soft delete permite recuperar dados apagados acidentalmente.">Exclui permanentemente do disco</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! Soft delete permite recuperar dados apagados acidentalmente.">Realiza um "Soft Delete" (apenas marca como deletado, mas mantém o dado)</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. Soft delete permite recuperar dados apagados acidentalmente.">Pergunta ao administrador se ele tem certeza</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. Soft delete permite recuperar dados apagados acidentalmente.">Copia o dado para um arquivo TXT</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">6. Qual método é usado para inserir um novo registro no banco de dados?</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. O `Create` recebe um ponteiro para a struct e realiza a inserção SQL.">db.Save()</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. O `Create` recebe um ponteiro para a struct e realiza a inserção SQL.">db.Insert()</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! O `Create` recebe um ponteiro para a struct e realiza a inserção SQL.">db.Create()</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. O `Create` recebe um ponteiro para a struct e realiza a inserção SQL.">db.Add()</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">7. Como se faz uma busca por todos os registros de uma tabela?</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. O `Find` preenche o slice passado com todos os registros encontrados.">db.ListAll(&slice)</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. O `Find` preenche o slice passado com todos os registros encontrados.">db.Get(&slice)</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! O `Find` preenche o slice passado com todos os registros encontrados.">db.Find(&slice)</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. O `Find` preenche o slice passado com todos os registros encontrados.">db.Select("*")</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">8. O GORM suporta vários bancos de dados (PostgreSQL, MySQL, SQLite, SQL Server)?</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. Você pode desenvolver em SQLite localmente e subir para PostgreSQL em produção sem mudar quase nada no código.">Não, apenas SQLite</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! Você pode desenvolver em SQLite localmente e subir para PostgreSQL em produção sem mudar quase nada no código.">Sim, através de "Drivers" específicos para cada banco</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. Você pode desenvolver em SQLite localmente e subir para PostgreSQL em produção sem mudar quase nada no código.">Sim, mas apenas um por projeto</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. Você pode desenvolver em SQLite localmente e subir para PostgreSQL em produção sem mudar quase nada no código.">Somente bancos de dados do Google</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">9. Para que servem as Tags do GORM (ex: `gorm:"primaryKey;unique"`)?</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. Permite configurar o banco de dados detalhadamente diretamente pela struct.">Para traduzir o banco de dados</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! Permite configurar o banco de dados detalhadamente diretamente pela struct.">Para dar instruções específicas ao banco sobre aquela coluna (chave primária, valor único, etc.)</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. Permite configurar o banco de dados detalhadamente diretamente pela struct.">Para colorir a tabela no editor SQL</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. Permite configurar o banco de dados detalhadamente diretamente pela struct.">Para bloquear o acesso de hackers</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">10. O que é o "Eager Loading" (Pré-carregamento) no GORM?</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. Vital para buscar um Usuário já com todos os seus Pedidos associados.">Carregar o banco antes de ligar o computador</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! Vital para buscar um Usuário já com todos os seus Pedidos associados.">Carregar dados de tabelas relacionadas (relacionamentos) em uma única consulta (usando `Preload`)</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. Vital para buscar um Usuário já com todos os seus Pedidos associados.">Aumentar a velocidade do mouse</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. Vital para buscar um Usuário já com todos os seus Pedidos associados.">Baixar o banco de dados da internet</div>
  <div class="quiz-feedback"></div>
</div>
