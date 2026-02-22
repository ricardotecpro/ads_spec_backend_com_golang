# Quiz 04 - Estruturas de Dados Avançadas 🗄️

--8<-- "assets/quiz.html"

<div class="quiz-container">
  <div class="quiz-question">1. Qual a principal diferença entre um Array e um Slice em Go?</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. Slices são abstrações poderosas sobre arrays que permitem crescer conforme a necessidade.">O Array é mais rápido que o Slice</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! Slices são abstrações poderosas sobre arrays que permitem crescer conforme a necessidade.">O Array tem tamanho fixo e o Slice tem tamanho dinâmico</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. Slices são abstrações poderosas sobre arrays que permitem crescer conforme a necessidade.">O Slice só aceita strings</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. Slices são abstrações poderosas sobre arrays que permitem crescer conforme a necessidade.">Não há diferença, são nomes diferentes para a mesma coisa</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">2. Como você adiciona um elemento a um Slice?</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. O `append` é a função nativa para gerenciar o crescimento de slices.">slice.Add(valor)</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. O `append` é a função nativa para gerenciar o crescimento de slices.">slice.Push(valor)</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! O `append` é a função nativa para gerenciar o crescimento de slices.">slice = append(slice, valor)</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. O `append` é a função nativa para gerenciar o crescimento de slices.">slice[last] = valor</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">3. O que é um "Map" em Go?</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. Maps permitem buscas extremamente rápidas baseadas em chaves únicas.">Um mapa geográfico para navegação</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! Maps permitem buscas extremamente rápidas baseadas em chaves únicas.">Uma coleção desordenada de pares chave-valor</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. Maps permitem buscas extremamente rápidas baseadas em chaves únicas.">Um slice que contém apenas números</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. Maps permitem buscas extremamente rápidas baseadas em chaves únicas.">Uma ferramenta para desenhar diagramas</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">4. Qual a função usada para inicializar um Map ou um Slice com capacidade prévia?</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. O `make` aloca a memória necessária para estas estruturas.">create()</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. O `make` aloca a memória necessária para estas estruturas.">init()</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! O `make` aloca a memória necessária para estas estruturas.">make()</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. O `make` aloca a memória necessária para estas estruturas.">build()</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">5. O que acontece se você tentar acessar uma chave que não existe em um Map?</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. Go é seguro e evita crashes, retornando o valor padrão do tipo.">O programa sofre um crash imediatamente</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. Go é seguro e evita crashes, retornando o valor padrão do tipo.">Ele retorna null</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! Go é seguro e evita crashes, retornando o valor padrão do tipo.">Ele retorna o "zero value" do tipo do valor (ex: 0 para int)</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. Go é seguro e evita crashes, retornando o valor padrão do tipo.">Ele pergunta ao usuário o que fazer</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">6. Como você define uma "Struct" em Go?</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. Structs são agrupamentos de campos que formam um novo tipo de dado.">class Pessoa { ... }</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. Structs são agrupamentos de campos que formam um novo tipo de dado.">struct Pessoa { ... }</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! Structs são agrupamentos de campos que formam um novo tipo de dado.">type Pessoa struct { ... }</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. Structs são agrupamentos de campos que formam um novo tipo de dado.">define Pessoa struct { ... }</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">7. Go possui herança de classes como em Java ou C#?</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. A composição é considerada mais flexível e menos propensa a erros que a herança clássica.">Sim, através de extends</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! A composição é considerada mais flexível e menos propensa a erros que a herança clássica.">Não, Go usa Composição (Embedding) em vez de herança</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. A composição é considerada mais flexível e menos propensa a erros que a herança clássica.">Sim, mas apenas no pacote main</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. A composição é considerada mais flexível e menos propensa a erros que a herança clássica.">Sim, mas é considerada má prática</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">8. O que é um "Método" no contexto de uma Struct?</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. Métodos permitem que tipos tenham comportamentos associados (ex: `p.Saudacao()`).">Uma função global que não pertence a ninguém</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! Métodos permitem que tipos tenham comportamentos associados (ex: `p.Saudacao()`).">Uma função que possui um "receiver" (destinatário), anexando-a a um tipo</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. Métodos permitem que tipos tenham comportamentos associados (ex: `p.Saudacao()`).">O nome técnico para uma variável dentro da struct</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. Métodos permitem que tipos tenham comportamentos associados (ex: `p.Saudacao()`).">Um comentário especial</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">9. Ao fatiar um slice como `sub := lista[1:3]`, quais índices são incluídos?</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. O padrão do Go (e de muitas linguagens) é `[inclusive:exclusive]`.">1 e 3</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! O padrão do Go (e de muitas linguagens) é `[inclusive:exclusive]`.">1 e 2 (o limite superior é exclusivo)</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. O padrão do Go (e de muitas linguagens) é `[inclusive:exclusive]`.">1, 2 e 3</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. O padrão do Go (e de muitas linguagens) é `[inclusive:exclusive]`.">Apenas o 1</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">10. Como se remove uma chave de um Map?</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. A função `delete` remove a entrada do mapa de forma eficiente.">map.Remove(chave)</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. A função `delete` remove a entrada do mapa de forma eficiente.">map[chave] = nil</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! A função `delete` remove a entrada do mapa de forma eficiente.">delete(map, chave)</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. A função `delete` remove a entrada do mapa de forma eficiente.">discard(map, chave)</div>
  <div class="quiz-feedback"></div>
</div>
