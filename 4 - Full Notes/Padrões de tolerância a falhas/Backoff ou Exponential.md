CreatedAt: 21-06-2025 18:45

Tags: #architecture #cloud #resilience #failure

---
# Conceito Geral
O tempo de espera entre as tentativas aumenta exponencialmente de acordo com o que você deseja.
Imaginando que sua requisição deu problema, se você tentar no mesmo segundo uma segunda requisição provavelmente ela não vai funcionar também, então nesse caso é interessante aumentar o intervalo (um exemplo é multiplicar por 2 o tempo a cada request mal sucedido) para que o servidor destino tenha tempo de se reestabelecer.

---
# Referências
- [Canal Douglas Mugnos](https://youtu.be/r0_hIk_tWq0?si=FxIukgPpjYstqgcZ)
- [AWS](https://aws.amazon.com/pt/builders-library/timeouts-retries-and-backoff-with-jitter/)