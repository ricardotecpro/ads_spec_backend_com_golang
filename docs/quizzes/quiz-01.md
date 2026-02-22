# Quiz 01 - Introdução ao Go e Ecossistema 🐹

--8<-- "assets/quiz.html"

<div class="quiz-container">
  <div class="quiz-question">1. Em que ano a linguagem Go foi lançada publicamente como open source?</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. O Google iniciou o projeto em 2007, mas o lançamento oficial como open source foi em 2009.">2005</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. O Google iniciou o projeto em 2007, mas o lançamento oficial como open source foi em 2009.">2007</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! O Google iniciou o projeto em 2007, mas o lançamento oficial como open source foi em 2009.">2009</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. O Google iniciou o projeto em 2007, mas o lançamento oficial como open source foi em 2009.">2012</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">2. Quem são os três criadores originais do Go?</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. Estes três engenheiros do Google uniram forças para criar uma linguagem que resolvesse problemas de escala.">Steve Jobs, Bill Gates e Mark Zuckerberg</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! Estes três engenheiros do Google uniram forças para criar uma linguagem que resolvesse problemas de escala.">Robert Griesemer, Rob Pike e Ken Thompson</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. Estes três engenheiros do Google uniram forças para criar uma linguagem que resolvesse problemas de escala.">Linus Torvalds, Guido van Rossum e Bjarne Stroustrup</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. Estes três engenheiros do Google uniram forças para criar uma linguagem que resolvesse problemas de escala.">James Gosling, Brendan Eich e Anders Hejlsberg</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">3. Qual a principal filosofia de design da linguagem Go?</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. Go preza pelo "menos é mais", removendo recursos complexos que dificultam a leitura do código.">Complexidade máxima para maior controle</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. Go preza pelo "menos é mais", removendo recursos complexos que dificultam a leitura do código.">Suporte exagerado a herança de classes</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! Go preza pelo "menos é mais", removendo recursos complexos que dificultam a leitura do código.">Simplicidade, clareza e eficiência</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. Go preza pelo "menos é mais", removendo recursos complexos que dificultam a leitura do código.">Ser uma linguagem puramente funcional</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">4. O Go é uma linguagem compilada ou interpretada?</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! Go gera binários estáticos que rodam diretamente no sistema operacional, o que garante alta performance.">Compilada diretamente para código de máquina</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. Go gera binários estáticos que rodam diretamente no sistema operacional, o que garante alta performance.">Interpretada como Python ou Ruby</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. Go gera binários estáticos que rodam diretamente no sistema operacional, o que garante alta performance.">Roda em uma máquina virtual (como Java JVM)</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. Go gera binários estáticos que rodam diretamente no sistema operacional, o que garante alta performance.">Transpilada para JavaScript</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">5. O que o comando `go run main.go` faz?</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. É o comando ideal para testes rápidos durante o desenvolvimento.">Apenas gera o executável no disco</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. É o comando ideal para testes rápidos durante o desenvolvimento.">Formata o código fonte</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! É o comando ideal para testes rápidos durante o desenvolvimento.">Compila e executa o programa em um passo temporário</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. É o comando ideal para testes rápidos durante o desenvolvimento.">Instala dependências externas</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">6. Qual comando é usado para inicializar um novo projeto (módulo) em Go?</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. O `go mod init <nome>` cria o arquivo go.mod, essencial para gerenciar dependências modernas.">go init</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. O `go mod init <nome>` cria o arquivo go.mod, essencial para gerenciar dependências modernas.">go start</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! O `go mod init <nome>` cria o arquivo go.mod, essencial para gerenciar dependências modernas.">go mod init</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. O `go mod init <nome>` cria o arquivo go.mod, essencial para gerenciar dependências modernas.">go create module</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">7. O Go possui Coletor de Lixo (Garbage Collector)?</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. O GC do Go é altamente otimizado para baixa latência, facilitando o trabalho do desenvolvedor.">Não, a memória é manual como em C</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! O GC do Go é altamente otimizado para baixa latência, facilitando o trabalho do desenvolvedor.">Sim, ele gerencia a memória automaticamente</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. O GC do Go é altamente otimizado para baixa latência, facilitando o trabalho do desenvolvedor.">Apenas se você instalar um plugin externo</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. O GC do Go é altamente otimizado para baixa latência, facilitando o trabalho do desenvolvedor.">Sim, mas ele apaga o código fonte também</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">8. Qual o nome da mascote oficial do Go?</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. O Gopher foi desenhado por Renee French e se tornou o símbolo da comunidade.">The Go Cat</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. O Gopher foi desenhado por Renee French e se tornou o símbolo da comunidade.">Gofer the Rabbit</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! O Gopher foi desenhado por Renee French e se tornou o símbolo da comunidade.">The Gopher</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. O Gopher foi desenhado por Renee French e se tornou o símbolo da comunidade.">Rusty the Crab</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. O Gopher foi desenhado por Renee French e se tornou o símbolo da comunidade.">Gopher é um esquilo-da-mongólia.</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">9. O que significa dizer que o Go gera "Binários Estáticos"?</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. Isso facilita muito o deploy, pois você só precisa enviar um único arquivo para o servidor.">Que o programa não pode ser alterado depois de pronto</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. Isso facilita muito o deploy, pois você só precisa enviar um único arquivo para o servidor.">Que ele só roda em computadores parados (estáticos)</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! Isso facilita muito o deploy, pois você só precisa enviar um único arquivo para o servidor.">Que o executável contém todas as dependências necessárias para rodar</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. Isso facilita muito o deploy, pois você só precisa enviar um único arquivo para o servidor.">Que a tela do programa nunca se move</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">10. Qual empresa criou e mantém o Go?</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. O Go nasceu dentro do Google para resolver desafios de infraestrutura da própria empresa.">Microsoft</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. O Go nasceu dentro do Google para resolver desafios de infraestrutura da própria empresa.">Facebook (Meta)</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! O Go nasceu dentro do Google para resolver desafios de infraestrutura da própria empresa.">Google</div>
  <div class="quiz-option" data-correct="false" data-feedback="❌ Incorreto. O Go nasceu dentro do Google para resolver desafios de infraestrutura da própria empresa.">Amazon</div>
  <div class="quiz-feedback"></div>
</div>
