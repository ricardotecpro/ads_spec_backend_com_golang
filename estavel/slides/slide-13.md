# Aula 13 - Testes em Go ✅
## Garantindo a Qualidade e Estabilidade do seu Código

---

## Agenda de Hoje 📅

1. Por que testar é vital? <!-- .element: class="fragment" -->
2. O comando `go test` <!-- .element: class="fragment" -->
3. Testes Unitários Básicos <!-- .element: class="fragment" -->
4. Table-Driven Tests (Idiomático) <!-- .element: class="fragment" -->
5. Cobertura e Performance <!-- .element: class="fragment" -->
6. Mini-Projeto: TDD na Prática <!-- .element: class="fragment" -->

---

## 1. O Suporte Nativo 🧪

- Go não precisa de frameworks externos (como Jest ou JUnit). <!-- .element: class="fragment" -->
- Pacote `testing` e comando `go test` fazem tudo. <!-- .element: class="fragment" -->
- Sufixo obrigatório: `_test.go`. <!-- .element: class="fragment" -->

---

## 2. Testes de Tabela (Professional) 📊

- Teste múltiplos cenários com um único loop. <!-- .element: class="fragment" -->

```go
tests := []struct {
    a, b, want int
}{
    {1, 1, 2},
    {2, 2, 4},
    {-1, 1, 0},
}
```

---

## 3. Cobertura de Testes 📈

- Quanto do seu código está realmente protegido? <!-- .element: class="fragment" -->

```termynal
$ go test -cover
coverage: 87.5%
```

- Gere relatórios HTML visuais para análise. <!-- .element: class="fragment" -->

---

## 4. Mocking de API 🎭

- Teste Handlers sem subir o servidor. <!-- .element: class="fragment" -->
- Pacote `net/http/httptest`. <!-- .element: class="fragment" -->

```mermaid
graph LR
    Test[Test Code] -->|Fake Req| Handler[Handler]
    Handler -->|Record| res[ResponseRecorder]
    res -->|Verify| Test
```

---

## 5. Benchmarks: Medindo Velocidade ⚡

- Teste o tempo de execução e alocação de memória. <!-- .element: class="fragment" -->

```go
func BenchmarkProcesso(b *testing.B) {
    for i := 0; i < b.N; i++ {
        Processo()
    }
}
```

---

## 6. Mini-Projeto: TDD na Prática 🚀

- Inverter uma string. <!-- .element: class="fragment" -->
- Passo 1: Criar o teste (FAIL). <!-- .element: class="fragment" -->
- Passo 2: Codar a função. <!-- .element: class="fragment" -->
- Passo 3: Testar novamente (PASS). <!-- .element: class="fragment" -->

---

## Resumo da Aula ✅

- Testes em Go são simples e rápidos. <!-- .element: class="fragment" -->
- Table-driven tests evitam duplicação de lógica. <!-- .element: class="fragment" -->
- Cobertura alta = Dormir tranquilo. <!-- .element: class="fragment" -->

---

## Próxima Aula: Arquitetura Limpa 🏗️

- Injeção de Dependência.
- Organizando grandes projetos.

---

## Dúvidas? 🤔

> "Testes não evitam bugs, eles evitam que os mesmos bugs voltem."
