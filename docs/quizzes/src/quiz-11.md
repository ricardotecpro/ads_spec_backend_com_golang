# Quiz 11 - Framework Web Gin 🚀

1. O Gin é considerado um framework "leve" e "rápido". Qual o principal motivo dessa fama?
    - [ ] Ele usa inteligência artificial para codar
    - [x] Ele utiliza um roteador baseado em Radix Tree e tem baixíssima alocação de memória
    - [ ] Ele apaga os arquivos desnecessários do Windows
    - [ ] Ele só funciona com strings curtas
    *Explicação: O roteador do Gin é um dos mais performáticos do ecossistema Go.*

2. No Gin, qual objeto central é passado para todos os handlers para gerenciar a requisição e a resposta?
    - [ ] gin.Server
    - [x] *gin.Context
    - [ ] http.Request
    - [ ] context.Background()
    *Explicação: O `*gin.Context` encapsula tudo o que você precisa (parâmetros, JSON, resposta).*

3. Como se define uma rota com parâmetro dinâmico no Gin (ex: pegar o ID do usuário)?
    - [ ] r.GET("/user/ID")
    - [x] r.GET("/user/:id")
    - [ ] r.GET("/user/$id")
    - [ ] r.GET("/user/?id")
    *Explicação: O uso dos dois pontos `:` define um parâmetro que pode ser recuperado via `c.Param("id")`.*

4. Qual a função do método `c.ShouldBindJSON(&struct)`?
    - [ ] Deletar o JSON enviado
    - [x] Mapear automaticamente o corpo da requisição (JSON) para uma struct em Go
    - [ ] Validar a conexão com a internet
    - [ ] Transformar a struct em uma imagem
    *Explicação: O Binding economiza dezenas de linhas de tratamento manual de bytes.*

5. O que o `gin.H{}` permite que façamos?
    - [ ] Criar um loop infinito
    - [x] Escrever um JSON de forma rápida e curta no estilo chave-valor
    - [ ] Hostear o site na nuvem
    - [ ] Esconder o cabeçalho da página
    *Explicação: `gin.H` é um atalho para `map[string]interface{}`.*

6. Como você agrupa rotas que compartilham um prefixo comum (ex: `/api/v1`)?
    - [ ] Copiando e colando o prefixo em cada linha
    - [x] Usando o método `r.Group("/api/v1")`
    - [ ] Criando vários servidores diferentes
    - [ ] O Gin não permite agrupamento
    *Explicação: Grupos de rotas permitem aplicar middlewares a conjuntos específicos de endpoints.*

7. Para que serve a tag `binding:"required"` nas structs?
    - [ ] Para deixar o texto em negrito
    - [x] Para que o Gin valide automaticamente se aquele campo foi enviado no JSON
    - [ ] Para travar o banco de dados
    - [ ] Para aumentar a segurança contra hackers
    *Explicação: O Gin retorna erro automaticamente se um campo obrigatório estiver faltando.*

8. Qual o comando para iniciar o servidor Gin na porta padrão?
    - [ ] r.Start()
    - [x] r.Run()
    - [ ] r.Listen()
    - [ ] r.Serve()
    *Explicação: O `Run()` inicia o motor do framework e aguarda conexões na porta 8080.*

9. O Gin já vem com sistema de logs e recuperação de pânicos (Recovery) por padrão?
    - [ ] Não, deve ser instalado por fora
    - [x] Sim, ao usar `gin.Default()`, esses dois middlewares são ativados
    - [ ] Somente se o computador for potente
    - [ ] Somente na versão paga
    *Explicação: O Log ajuda no debug e o Recovery evita que o servidor caia por um erro inesperado.*

10. Podemos usar Middlewares personalizados no Gin?
    - [ ] Não, o Gin é fechado
    - [x] Sim, usando o método `r.Use()`
    - [ ] Sim, mas apenas para contar o tempo
    - [ ] Somente no pacote main
    *Explicação: O sistema de middlewares do Gin é extremamente modular e fácil de usar.*
