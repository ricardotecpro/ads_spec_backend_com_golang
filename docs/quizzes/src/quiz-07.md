# Quiz 07 - Manipulação de Arquivos e JSON 📁

1. Qual pacote da biblioteca padrão é o mais utilizado para operações de entrada e saída (I/O) e arquivos em Go?
    - [ ] io/json
    - [x] os (e io/ioutil em versões legadas)
    - [ ] net/http
    - [ ] database/sql
    *Explicação: O pacote `os` fornece uma plataforma agnóstica para acessar recursos do sistema operacional.*

2. O que são as "Struct Tags" no contexto do JSON?
    - [ ] Comentários que o Go ignora
    - [x] Metadados entre crases (backticks) que dizem ao codificador JSON como mapear os campos
    - [ ] Etiquetas usadas para imprimir o código em impressoras térmicas
    - [ ] Comandos para apagar o banco de dados
    *Explicação: Tags como `json:"nome_completo"` permitem que o JSON tenha nomes diferentes da nossa struct interna.*

3. Qual a diferença entre `json.Marshal` e `json.Unmarshal`?
    - [ ] Marshal cria arquivos, Unmarshal deleta
    - [x] Marshal converte Struct para JSON; Unmarshal converte JSON para Struct
    - [ ] Marshal é para números, Unmarshal é para textos
    - [ ] Nenhuma, fazem a mesma coisa
    *Explicação: São os dois pilares da serialização em Go.*

4. Como você garante que um arquivo seja fechado corretamente após a leitura, mesmo que ocorra um erro no meio do processo?
    - [ ] Usando um loop infinito
    - [ ] Chamando Close() três vezes
    - [x] Usando o comando `defer arquivo.Close()` logo após a abertura
    - [ ] Reiniciando o computador
    *Explicação: O `defer` é a técnica padrão para gestão segura de recursos em Go.*

5. Qual formato o `json.Marshal` retorna?
    - [ ] Uma string formatada
    - [x] Um slice de bytes (`[]byte`) e um erro
    - [ ] Um número inteiro
    - [ ] Um mapa (map)
    *Explicação: Retornar bytes dá mais flexibilidade para enviar o dado pela rede ou salvar no disco.*

6. Para que serve o terceiro parâmetro numérico (ex: `0644`) na função `os.WriteFile`?
    - [ ] É o código de barras do arquivo
    - [x] São as permissões de acesso do arquivo no sistema (Unix permissions)
    - [ ] É a velocidade de escrita em KB/s
    - [ ] É a cor do ícone do arquivo
    *Explicação: Controla quem pode ler, escrever ou executar aquele arquivo.*

7. Quando você deve usar `json.NewEncoder` em vez de `json.Marshal`?
    - [ ] Quando o JSON for muito pequeno
    - [x] Quando estiver escrevendo diretamente em um fluxo (como o corpo de uma resposta HTTP ou um arquivo)
    - [ ] Somente em datas especiais
    - [ ] Quando o código for rodar em um Mac
    *Explicação: O Encoder é mais eficiente para fluxos contínuos (streams) de dados.*

8. O que acontece se uma tag JSON for definida como `json:"-"`?
    - [ ] O campo é salvo como um traço
    - [x] O campo é ignorado e não aparecerá no JSON resultante
    - [ ] O programa dá erro
    - [ ] O campo vira obrigatório
    *Explicação: Útil para esconder senhas ou dados sensíveis que não devem sair da aplicação.*

9. Go consegue ler arquivos ZIP nativamente?
    - [ ] Não, precisa de bibliotecas em C++
    - [x] Sim, através do pacote `archive/zip` da biblioteca padrão
    - [ ] Somente se o Windows permitir
    - [ ] Sim, mas apenas se o arquivo tiver menos de 1MB
    *Explicação: A biblioteca padrão do Go é riquíssima e cobre compressão, criptografia e muito mais.*

10. Como se verifica se um arquivo existe em Go sem abri-lo?
    - [ ] if exist("arquivo.txt")
    - [x] Usando `os.Stat(nome)` e verificando se o erro é `os.IsNotExist(err)`
    - [ ] Olhando pela janela
    - [ ] Usando o comando grep
    *Explicação: `os.Stat` retorna informações sobre o arquivo (metadados) sem carregar seu conteúdo.*