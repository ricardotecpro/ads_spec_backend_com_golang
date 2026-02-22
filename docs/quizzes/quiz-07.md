# Quiz 07 - Manipulação de Arquivos e JSON 📁

--8<-- "assets/quiz.html"

<div class="quiz-container">
  <div class="quiz-question">1. Qual pacote da biblioteca padrão é o mais utilizado para operações de entrada e saída (I/O) e arquivos em Go?</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. O pacote `os` fornece uma plataforma agnóstica para acessar recursos do sistema operacional.">io/json</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! O pacote `os` fornece uma plataforma agnóstica para acessar recursos do sistema operacional.">os (e io/ioutil em versões legadas)</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. O pacote `os` fornece uma plataforma agnóstica para acessar recursos do sistema operacional.">net/http</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. O pacote `os` fornece uma plataforma agnóstica para acessar recursos do sistema operacional.">database/sql</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">2. O que são as "Struct Tags" no contexto do JSON?</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. Tags como `json:"nome_completo"` permitem que o JSON tenha nomes diferentes da nossa struct interna.">Comentários que o Go ignora</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! Tags como `json:"nome_completo"` permitem que o JSON tenha nomes diferentes da nossa struct interna.">Metadados entre crases (backticks) que dizem ao codificador JSON como mapear os campos</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. Tags como `json:"nome_completo"` permitem que o JSON tenha nomes diferentes da nossa struct interna.">Etiquetas usadas para imprimir o código em impressoras térmicas</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. Tags como `json:"nome_completo"` permitem que o JSON tenha nomes diferentes da nossa struct interna.">Comandos para apagar o banco de dados</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">3. Qual a diferença entre `json.Marshal` e `json.Unmarshal`?</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. São os dois pilares da serialização em Go.">Marshal cria arquivos, Unmarshal deleta</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! São os dois pilares da serialização em Go.">Marshal converte Struct para JSON; Unmarshal converte JSON para Struct</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. São os dois pilares da serialização em Go.">Marshal é para números, Unmarshal é para textos</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. São os dois pilares da serialização em Go.">Nenhuma, fazem a mesma coisa</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">4. Como você garante que um arquivo seja fechado corretamente após a leitura, mesmo que ocorra um erro no meio do processo?</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. O `defer` é a técnica padrão para gestão segura de recursos em Go.">Usando um loop infinito</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. O `defer` é a técnica padrão para gestão segura de recursos em Go.">Chamando Close() três vezes</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! O `defer` é a técnica padrão para gestão segura de recursos em Go.">Usando o comando `defer arquivo.Close()` logo após a abertura</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. O `defer` é a técnica padrão para gestão segura de recursos em Go.">Reiniciando o computador</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">5. Qual formato o `json.Marshal` retorna?</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. Retornar bytes dá mais flexibilidade para enviar o dado pela rede ou salvar no disco.">Uma string formatada</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! Retornar bytes dá mais flexibilidade para enviar o dado pela rede ou salvar no disco.">Um slice de bytes (`[]byte`) e um erro</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. Retornar bytes dá mais flexibilidade para enviar o dado pela rede ou salvar no disco.">Um número inteiro</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. Retornar bytes dá mais flexibilidade para enviar o dado pela rede ou salvar no disco.">Um mapa (map)</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">6. Para que serve o terceiro parâmetro numérico (ex: `0644`) na função `os.WriteFile`?</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. Controla quem pode ler, escrever ou executar aquele arquivo.">É o código de barras do arquivo</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! Controla quem pode ler, escrever ou executar aquele arquivo.">São as permissões de acesso do arquivo no sistema (Unix permissions)</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. Controla quem pode ler, escrever ou executar aquele arquivo.">É a velocidade de escrita em KB/s</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. Controla quem pode ler, escrever ou executar aquele arquivo.">É a cor do ícone do arquivo</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">7. Quando você deve usar `json.NewEncoder` em vez de `json.Marshal`?</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. O Encoder é mais eficiente para fluxos contínuos (streams) de dados.">Quando o JSON for muito pequeno</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! O Encoder é mais eficiente para fluxos contínuos (streams) de dados.">Quando estiver escrevendo diretamente em um fluxo (como o corpo de uma resposta HTTP ou um arquivo)</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. O Encoder é mais eficiente para fluxos contínuos (streams) de dados.">Somente em datas especiais</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. O Encoder é mais eficiente para fluxos contínuos (streams) de dados.">Quando o código for rodar em um Mac</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">8. O que acontece se uma tag JSON for definida como `json:"-"`?</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. Útil para esconder senhas ou dados sensíveis que não devem sair da aplicação.">O campo é salvo como um traço</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! Útil para esconder senhas ou dados sensíveis que não devem sair da aplicação.">O campo é ignorado e não aparecerá no JSON resultante</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. Útil para esconder senhas ou dados sensíveis que não devem sair da aplicação.">O programa dá erro</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. Útil para esconder senhas ou dados sensíveis que não devem sair da aplicação.">O campo vira obrigatório</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">9. Go consegue ler arquivos ZIP nativamente?</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. A biblioteca padrão do Go é riquíssima e cobre compressão, criptografia e muito mais.">Não, precisa de bibliotecas em C++</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! A biblioteca padrão do Go é riquíssima e cobre compressão, criptografia e muito mais.">Sim, através do pacote `archive/zip` da biblioteca padrão</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. A biblioteca padrão do Go é riquíssima e cobre compressão, criptografia e muito mais.">Somente se o Windows permitir</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. A biblioteca padrão do Go é riquíssima e cobre compressão, criptografia e muito mais.">Sim, mas apenas se o arquivo tiver menos de 1MB</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">10. Como se verifica se um arquivo existe em Go sem abri-lo?</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. `os.Stat` retorna informações sobre o arquivo (metadados) sem carregar seu conteúdo.">if exist("arquivo.txt")</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! `os.Stat` retorna informações sobre o arquivo (metadados) sem carregar seu conteúdo.">Usando `os.Stat(nome)` e verificando se o erro é `os.IsNotExist(err)`</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. `os.Stat` retorna informações sobre o arquivo (metadados) sem carregar seu conteúdo.">Olhando pela janela</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. `os.Stat` retorna informações sobre o arquivo (metadados) sem carregar seu conteúdo.">Usando o comando grep</div>
  <div class="quiz-feedback"></div>
</div>
