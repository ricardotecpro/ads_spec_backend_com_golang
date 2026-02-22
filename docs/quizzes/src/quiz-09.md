# Quiz 09 - Programação Web com net/http 🌐

1. Como o Go permite rodar um servidor HTTP sem depender de softwares como Apache ou Nginx?
    - [ ] Ele se conecta via Bluetooth
    - [x] Ele possui um servidor HTTP de nível de produção embutido na biblioteca padrão (`net/http`)
    - [ ] Ele usa o Internet Explorer escondido
    - [ ] Ele não roda sem o Nginx
    *Explicação: O pacote `net/http` é robusto o suficiente para ser o próprio servidor da aplicação.*

2. No handler `func(w http.ResponseWriter, r *http.Request)`, qual o papel do `w`?
    - [ ] Representar o Windows do servidor
    - [x] Enviar a resposta (Headers, Body, Status) de volta para o cliente
    - [ ] Receber os dados enviados pelo navegador
    - [ ] Inverter o sentido da internet
    *Explicação: O `ResponseWriter` é o canal de saída do servidor para o cliente.*

3. O que o objeto `r *http.Request` contém?
    - [ ] Apenas o endereço IP do usuário
    - [x] Toda a informação da requisição: Método, URL, Cabeçalhos e Corpo (Body)
    - [ ] O código fonte do navegador do cliente
    - [ ] A senha do administrador
    *Explicação: O `Request` é o pacote completo de informações que o cliente envia para o servidor.*

4. Qual comando inicia o servidor e o faz escutar em uma porta específica?
    - [ ] http.Start(":8080")
    - [ ] http.Listen()
    - [x] http.ListenAndServe(":8080", nil)
    - [ ] server.Run()
    *Explicação: Esta função bloqueia a execução do main e mantém o servidor ativo respondendo requisições.*

5. O que são "Middlewares" em uma aplicação Web?
    - [ ] Softwares que ficam entre o teclado e a tela
    - [x] Funções que interceptam uma requisição antes que ela chegue ao handler final (ex: para logs ou login)
    - [ ] Cabos de rede especiais
    - [ ] Vírus que lentificam o servidor
    *Explicação: Middlewares permitem adicionar camadas de lógica comuns a várias rotas.*

6. Como você serve arquivos estáticos (HTML, CSS, Imagens) em Go?
    - [ ] Copiando e colando o arquivo na tela
    - [x] Usando o `http.FileServer` apontando para um diretório
    - [ ] Go não serve arquivos estáticos
    - [ ] Usando o comando `print(arquivo)`
    *Explicação: O FileServer é uma ferramenta nativa eficiente para entregar conteúdo estático.*

7. O que acontece se uma rota não for encontrada e você não definiu um handler padrão?
    - [ ] O computador explode
    - [x] O servidor retorna automaticamente o erro `404 page not found`
    - [ ] O servidor trava
    - [ ] Ele escolhe uma página aleatória
    *Explicação: O roteador padrão do Go já possui tratamento básico para rotas inexistentes.*

8. No Go nativo (`net/http`), como se pega um parâmetro da Query String (ex: `?id=10`)?
    - [ ] r.ID()
    - [x] r.URL.Query().Get("id")
    - [ ] r.Body["id"]
    - [ ] Através de um loop for
    *Explicação: Os parâmetros de busca ficam organizados dentro do objeto URL da requisição.*

9. Qual o valor de retorno padrão de uma requisição bem-sucedida?
    - [ ] 0
    - [ ] 404
    - [x] 200 OK
    - [ ] 500
    *Explicação: O código 200 é o sinal universal de que a requisição foi atendida com sucesso.*

10. É possível rodar múltiplos servidores Go em portas diferentes no mesmo binário?
    - [ ] Não, apenas um por vez
    - [x] Sim, usando Goroutines para iniciar cada `ListenAndServe`
    - [ ] Somente se houver duas placas de rede
    - [ ] Sim, mas eles compartilham o mesmo log
    *Explicação: A concorrência do Go facilita subir múltiplos micro-serviços ou painéis administrativos no mesmo processo.*