# Quiz 12 - Banco de Dados (GORM) 💾

1. O que significa a sigla ORM (como o GORM)?
    - [ ] Organized Recovery Manager
    - [x] Object-Relational Mapping (Mapeamento Objeto-Relacional)
    - [ ] Online Router Monitor
    - [ ] Only Ready Models
    *Explicação: ORMs transformam tabelas de banco de dados em objetos (structs) no código.*

2. Qual a principal vantagem do GORM sobre o pacote nativo `database/sql`?
    - [ ] Ele obriga o uso de cartões de crédito
    - [x] Ele automatiza tarefas repetitivas como gerar queries SQL e gerenciar tabelas
    - [ ] Ele apaga o banco caso o código esteja feio
    - [ ] Ele só funciona no Google Cloud
    *Explicação: O GORM traz alta produtividade ao abstrair o SQL complexo em funções Go.*

3. Para que serve o método `db.AutoMigrate(&MinhaStruct{})`?
    - [ ] Para migrar o código para outra linguagem
    - [x] Para criar ou atualizar automaticamente a tabela no banco conforme a estrutura da struct
    - [ ] Para deletar todos os dados do banco
    - [ ] Para salvar o banco de dados em um pendrive
    *Explicação: Migrations automáticas garantem que o banco acompanhe as mudanças do seu código.*

4. O que a struct embarcada `gorm.Model` adiciona ao seu modelo?
    - [ ] Somente o campo de nome
    - [x] ID, CreatedAt, UpdatedAt e DeletedAt (soft delete)
    - [ ] Um link para o GitHub do autor
    - [ ] A cor de fundo da tabela
    *Explicação: Facilita a criação de metadados padrão para qualquer registro no banco.*

5. Como o GORM trata a deleção de registros por padrão se o modelo tiver `gorm.Model`?
    - [ ] Exclui permanentemente do disco
    - [x] Realiza um "Soft Delete" (apenas marca como deletado, mas mantém o dado)
    - [ ] Pergunta ao administrador se ele tem certeza
    - [ ] Copia o dado para um arquivo TXT
    *Explicação: Soft delete permite recuperar dados apagados acidentalmente.*

6. Qual método é usado para inserir um novo registro no banco de dados?
    - [ ] db.Save()
    - [ ] db.Insert()
    - [x] db.Create()
    - [ ] db.Add()
    *Explicação: O `Create` recebe um ponteiro para a struct e realiza a inserção SQL.*

7. Como se faz uma busca por todos os registros de uma tabela?
    - [ ] db.ListAll(&slice)
    - [ ] db.Get(&slice)
    - [x] db.Find(&slice)
    - [ ] db.Select("*")
    *Explicação: O `Find` preenche o slice passado com todos os registros encontrados.*

8. O GORM suporta vários bancos de dados (PostgreSQL, MySQL, SQLite, SQL Server)?
    - [ ] Não, apenas SQLite
    - [x] Sim, através de "Drivers" específicos para cada banco
    - [ ] Sim, mas apenas um por projeto
    - [ ] Somente bancos de dados do Google
    *Explicação: Você pode desenvolver em SQLite localmente e subir para PostgreSQL em produção sem mudar quase nada no código.*

9. Para que servem as Tags do GORM (ex: `gorm:"primaryKey;unique"`)?
    - [ ] Para traduzir o banco de dados
    - [x] Para dar instruções específicas ao banco sobre aquela coluna (chave primária, valor único, etc.)
    - [ ] Para colorir a tabela no editor SQL
    - [ ] Para bloquear o acesso de hackers
    *Explicação: Permite configurar o banco de dados detalhadamente diretamente pela struct.*

10. O que é o "Eager Loading" (Pré-carregamento) no GORM?
    - [ ] Carregar o banco antes de ligar o computador
    - [x] Carregar dados de tabelas relacionadas (relacionamentos) em uma única consulta (usando `Preload`)
    - [ ] Aumentar a velocidade do mouse
    - [ ] Baixar o banco de dados da internet
    *Explicação: Vital para buscar um Usuário já com todos os seus Pedidos associados.*
