# Quiz 16 - Revisão Geral e Projeto Final 🏆

1. Qual o principal diferencial do Go em relação à concorrência?
    - [ ] Ela tem as cores mais bonitas
    - [x] O modelo de concorrência nativo (CSP) com Goroutines e Channels
    - [ ] Ela permite programar apenas com o mouse
    - [ ] Ela não usa internet para compilar
    *Explicação: Concorrência de baixo custo é o "superpoder" do Go.*

2. Na organização por camadas, onde ficam as validações de campos obrigatórios?
    - [ ] No banco de dados
    - [x] Na camada de Handler (via Binding) ou no Service (Regras de Negócio)
    - [ ] No manual do usuário
    - [ ] Em um arquivo de imagem
    *Explicação: Validar na entrada evita que dados sujos poluam o sistema.*

3. O que garante que o binário de produção seja pequeno e seguro?
    - [ ] Usar um computador novo
    - [x] Multi-Stage Builds no Docker e compilação estática do Go
    - [ ] Deletar o código fonte antes de rodar
    - [ ] Comprimir o arquivo com WinRAR
    *Explicação: Imagens Alpine com apenas o binário são o padrão da indústria.*

4. Qual o comando usado para atualizar todas as dependências do projeto?
    - [ ] go clean
    - [x] go get -u ./...
    - [ ] go mod tidy
    - [ ] go update
    *Explicação: O `go mod tidy` limpa o arquivo, mas o `get -u` busca novas versões.*

5. O que define que uma struct em Go "implementa" uma interface?
    - [ ] Ela deve ter um comentário dizendo isso
    - [x] Ela deve possuir as assinaturas exatas de todos os métodos da interface
    - [ ] Ela deve herdar de uma classe base
    - [ ] Ela deve estar no mesmo arquivo da interface
    *Explicação: O mapeamento é implícito e automático.*

6. Qual a função do arquivo `.env` em um projeto profissional?
    - [ ] Enviar e-mails automaticamente
    - [x] Armazenar configurações e segredos específicos do ambiente que não devem ir para o Git
    - [ ] Decorar o terminal
    - [ ] Aumentar o brilho da tela
    *Explicação: Segurança em primeiro lugar.*

7. Em um sistema de biblioteca, "Empréstimo" seria melhor modelado como:
    - [ ] Um campo dentro da struct Usuário
    - [x] Uma entidade/struct separada que relaciona Usuário e Livro
    - [ ] Um comentário no código
    - [ ] Um arquivo de texto separado
    *Explicação: Relacionamentos n-pra-n ou com metadados exigem estruturas próprias.*

8. O que acontece se chamarmos `db.AutoMigrate` e a tabela já existir?
    - [ ] O banco de dados é apagado
    - [x] O GORM altera a tabela para incluir novas colunas (se houver), mas mantém os dados existentes
    - [ ] O programa trava com erro
    - [ ] Ele cria uma cópia da tabela
    *Explicação: É uma migração incremental e segura na maioria dos casos.*

9. Qual ferramenta é usada para simular múltiplos usuários acessando a API ao mesmo tempo em testes?
    - [ ] Um browser aberto 100 vezes
    - [x] Goroutines em um loop de teste
    - [ ] O cronômetro do celular
    - [ ] O comando ping
    *Explicação: Go é a melhor ferramenta para testar o próprio Go sob carga.*

10. Qual a melhor maneira de continuar aprendendo Go após este curso?
    - [ ] Parar de programar e só ler livros
    - [x] Construir projetos reais, ler a biblioteca padrão e participar da comunidade
    - [ ] Esperar o Google lançar uma nova versão
    - [ ] Decorar o dicionário de funções
    *Explicação: Programação é uma prática constante. Mão na massa!*