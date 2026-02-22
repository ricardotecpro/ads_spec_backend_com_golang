# Exercícios: Concorrência em Go ⚡

!!! info "Instruções"
    Explore o poder das Goroutines e Channels.

---

### 🟢 Nível: Básico

1.  **Goroutine**: Crie uma função que imprima números de 1 a 10 e execute-a como uma goroutine no `main`. Verifique se o programa termina antes dela terminar (e como resolver isso com `time.Sleep`).
2.  **Canais**: Crie um canal de inteiros, envie o número 42 em uma goroutine e receba no `main`, imprimindo o valor.

---

### 🟡 Nível: Intermediário

3.  **Buffer**: Crie um canal com buffer de tamanho 2. Envie 2 mensagens sem precisar de uma goroutine consumidora imediata. O que acontece se enviar a 3ª?
4.  **Soma Concorrente**: Crie duas goroutines, cada uma calcula a soma de uma metade de um slice de números. Elas devem enviar os resultados parciais para um canal e o `main` deve somar os dois.

---

### 🔴 Nível: Desafio

5.  **Ping-Pong**: Crie duas goroutines chamadas "Ping" e "Pong". Elas devem trocar uma "bola" (um contador que incrementa) através de um canal. O programa deve parar quando o contador chegar a 10. Use o `select` para monitorar a troca.