CreatedAt: 21-06-2025 17:21

Tags: #architecture #cloud #resilience #failure

---
# Conceito Geral
É uma estratégia utilizada para que uma requisição seja reexecutada/feita uma nova tentativa de forma automática de forma que seja agnóstica ao usuario. Para implementar essa estratégia é bom ter domínio de aplicações [[Idempotência|idempotentes]] pois você precisa garantir que vários requests não terão efeitos colaterais.
Os retries no geral tem duas variáveis, o **tempo de espera entre tentativas** e o **numero máximo de tentativas**.
Também é um excelente pratica configurar um timeout dos requests, para que você mesmo não ajude a sobrecarregar o servidor.
Essa arquitetura de resiliência se subdivide em três tipos.
- **[[Retry Simples]]**
- **[[Backoff ou Exponential]]**
- **[[Jitter]]**

---
# Referências
- [Canal Douglas Mugnos](https://youtu.be/r0_hIk_tWq0?si=FxIukgPpjYstqgcZ)
- [AWS](https://aws.amazon.com/pt/builders-library/timeouts-retries-and-backoff-with-jitter/)