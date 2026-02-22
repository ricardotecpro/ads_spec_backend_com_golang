# Exercícios: Manipulação de Arquivos e JSON 📁

!!! info "Instruções"
    Trabalhe com persistência de dados e o formato JSON.

---

### 🟢 Nível: Básico

1.  **Escrita**: Crie um programa que salve a frase "Go é incrível para Backend!" em um arquivo chamado `aprendizado.txt`.
2.  **JSON Tags**: Crie uma struct `Config` com campos `Porta` e `Debug`. Adicione struct tags para que no JSON apareçam como `app_port` e `debug_mode`.

---

### 🟡 Nível: Intermediário

3.  **Marshal/Unmarshal**: Crie uma instância de `Config`, converta para JSON e imprima a string. Depois, pegue essa string e converta de volta para uma nova struct.
4.  **Leitura de Arquivo**: Crie um programa que leia o arquivo `aprendizado.txt` e conte quantas letras existem no arquivo.

---

### 🔴 Nível: Desafio

5.  **Gerenciador de Contatos**: Crie um programa que salve um slice de structs `Contato` (Nome, Telefone) em um arquivo `agenda.json`. O programa deve ler o arquivo ao iniciar e permitir que o usuário adicione novos contatos via terminal.