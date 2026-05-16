CreatedAt: 15-02-2026 18:47

Tags: #auth #oauth2 #token

---
## Conceito Geral
É o token gerado pelo [[Authotization Server]] para que possa ser utilizado na comunicação entre as aplicações.
Esse token pode ser do tipo [[O que é JWT|JWT]] ou um [[Token Opaco|Token Opaco]], mas independente do tipo o [[Resource Server]] deve saber o que fazer com ele, seja ler (caso especifico do [[O que é JWT|JWT]]) ou envia-lo na requisição para que o emissor do token sempre possa valida-lo.

---
## Referências
- [YT - Giuliana Bezerra](https://www.youtube.com/watch?v=68azMcqPpyo&t=1126s)