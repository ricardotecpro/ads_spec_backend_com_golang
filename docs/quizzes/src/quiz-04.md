# Quiz 04 - Estruturas de Dados Avançadas 🗄️

1. Qual a principal diferença entre um Array e um Slice em Go?
    - [ ] O Array é mais rápido que o Slice
    - [x] O Array tem tamanho fixo e o Slice tem tamanho dinâmico
    - [ ] O Slice só aceita strings
    - [ ] Não há diferença, são nomes diferentes para a mesma coisa
    *Explicação: Slices são abstrações poderosas sobre arrays que permitem crescer conforme a necessidade.*

2. Como você adiciona um elemento a um Slice?
    - [ ] slice.Add(valor)
    - [ ] slice.Push(valor)
    - [x] slice = append(slice, valor)
    - [ ] slice[last] = valor
    *Explicação: O `append` é a função nativa para gerenciar o crescimento de slices.*

3. O que é um "Map" em Go?
    - [ ] Um mapa geográfico para navegação
    - [x] Uma coleção desordenada de pares chave-valor
    - [ ] Um slice que contém apenas números
    - [ ] Uma ferramenta para desenhar diagramas
    *Explicação: Maps permitem buscas extremamente rápidas baseadas em chaves únicas.*

4. Qual a função usada para inicializar um Map ou um Slice com capacidade prévia?
    - [ ] create()
    - [ ] init()
    - [x] make()
    - [ ] build()
    *Explicação: O `make` aloca a memória necessária para estas estruturas.*

5. O que acontece se você tentar acessar uma chave que não existe em um Map?
    - [ ] O programa sofre um crash imediatamente
    - [ ] Ele retorna null
    - [x] Ele retorna o "zero value" do tipo do valor (ex: 0 para int)
    - [ ] Ele pergunta ao usuário o que fazer
    *Explicação: Go é seguro e evita crashes, retornando o valor padrão do tipo.*

6. Como você define uma "Struct" em Go?
    - [ ] class Pessoa { ... }
    - [ ] struct Pessoa { ... }
    - [x] type Pessoa struct { ... }
    - [ ] define Pessoa struct { ... }
    *Explicação: Structs são agrupamentos de campos que formam um novo tipo de dado.*

7. Go possui herança de classes como em Java ou C#?
    - [ ] Sim, através de extends
    - [x] Não, Go usa Composição (Embedding) em vez de herança
    - [ ] Sim, mas apenas no pacote main
    - [ ] Sim, mas é considerada má prática
    *Explicação: A composição é considerada mais flexível e menos propensa a erros que a herança clássica.*

8. O que é um "Método" no contexto de uma Struct?
    - [ ] Uma função global que não pertence a ninguém
    - [x] Uma função que possui um "receiver" (destinatário), anexando-a a um tipo
    - [ ] O nome técnico para uma variável dentro da struct
    - [ ] Um comentário especial
    *Explicação: Métodos permitem que tipos tenham comportamentos associados (ex: `p.Saudacao()`).*

9. Ao fatiar um slice como `sub := lista[1:3]`, quais índices são incluídos?
    - [ ] 1 e 3
    - [x] 1 e 2 (o limite superior é exclusivo)
    - [ ] 1, 2 e 3
    - [ ] Apenas o 1
    *Explicação: O padrão do Go (e de muitas linguagens) é `[inclusive:exclusive]`.*

10. Como se remove uma chave de um Map?
    - [ ] map.Remove(chave)
    - [ ] map[chave] = nil
    - [x] delete(map, chave)
    - [ ] discard(map, chave)
    *Explicação: A função `delete` remove a entrada do mapa de forma eficiente.*
