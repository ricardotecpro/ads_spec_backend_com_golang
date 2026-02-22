# Aula 12 - Banco de Dados (GORM) 💾
## Persistência de Dados Profissional em Go

---

## Agenda de Hoje 📅

1. SQL Puro vs ORM <!-- .element: class="fragment" -->
2. Introdução ao GORM <!-- .element: class="fragment" -->
3. Models e Auto-Migrations <!-- .element: class="fragment" -->
4. Operações de CRUD <!-- .element: class="fragment" -->
5. Relacionamentos (Has One, Has Many) <!-- .element: class="fragment" -->
6. Mini-Projeto: API com Banco Real <!-- .element: class="fragment" -->

---

## 1. O que é um ORM? 🗺️

- **Object-Relational Mapping**. <!-- .element: class="fragment" -->
- Traduz Tabelas ↔ Structs. <!-- .element: class="fragment" -->
- Abstrai o SQL para funções Go. <!-- .element: class="fragment" -->

---

## 2. Definindo Modelos 🏗️

```go
type Produto struct {
    gorm.Model // ID, Created, Updated, Deleted
    Nome  string `gorm:"size:100;not null"`
    Preco float64
}
```

- Tags controlam o comportamento do SQL. <!-- .element: class="fragment" -->

---

## 3. Auto-Migrations 📈

- Não escreva `CREATE TABLE` manual! <!-- .element: class="fragment" -->

```go
db.AutoMigrate(&Produto{})
```

- O GORM sincroniza seu código com o banco. <!-- .element: class="fragment" -->

---

## 4. O Ciclo do CRUD 📝

- **Create**: `db.Create(&p)`. <!-- .element: class="fragment" -->
- **Read**: `db.First(&p, 1)` ou `db.Find(&lista)`. <!-- .element: class="fragment" -->
- **Update**: `db.Model(&p).Update("Preco", 100)`. <!-- .element: class="fragment" -->
- **Delete**: `db.Delete(&p)`. <!-- .element: class="fragment" -->

---

## 5. Arquitetura DB 📊

```mermaid
graph LR
    App[Código Go] -->|Struct| ORM[GORM]
    ORM -->|SQL| Driver[SQLite Driver]
    Driver -->|Disk| File[(test.db)]
```

---

## 6. Mini-Projeto: API Persistente 🚀

- Integrar Gin + GORM. <!-- .element: class="fragment" -->
- Salvar dados enviados pelo Postman no SQLite. <!-- .element: class="fragment" -->
- Garantir que dados existam após reiniciar. <!-- .element: class="fragment" -->

---

## Resumo da Aula ✅

- GORM traz velocidade e segurança ao lidar com SQL. <!-- .element: class="fragment" -->
- `gorm.Model` padroniza seus registros. <!-- .element: class="fragment" -->
- Migrations automáticas eliminam erros de script manuais. <!-- .element: class="fragment" -->

---

## Próxima Aula: Testes em Go ✅

- Garantindo que a API não quebre.
- Testes Unitários e Table-Driven.

---

## Dúvidas? 🤔

> "Quem não persiste, não existe. No banco de dados e na vida."