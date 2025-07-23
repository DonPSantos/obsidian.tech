CreatedAt: 21-06-2025 18:48

Tags: #architecture #cloud #resilience #failure

---
# Conceito Geral
O tempo entre um retry e outro é calculado de forma randômica, essa estratégia além de dar um tempo para o servidor se recuperar, ele também evita que os requests tenham conflito por conta de tempo, essa estratégia pode ser utilizada junto com o [[Backoff ou Exponential]].

---
# Referências
- [Canal Douglas Mugnos](https://youtu.be/r0_hIk_tWq0?si=FxIukgPpjYstqgcZ)
- [AWS](https://aws.amazon.com/pt/builders-library/timeouts-retries-and-backoff-with-jitter/)