CreatedAt: 18-06-2025 10:29

Tags: #cloud #architecture 

---
# Conceito Geral
Nesse caso, os microsserviços sabem se virar sozinhos inclusive, se viram para resolver erros. A comunicação é intermediada por alguma fila, nesse caso, cada serviço fica olhando a fila e buscando a informação que precisa e assim que ele pega essa informação e processa ela, lança o resultado na fila para que os outros microsserviços possam também processar o que sua parte.

---
# Referências
- [Canal Pisani da ArcH](https://www.youtube.com/watch?v=QwDY0wla13Y)
- [Canal Emerging Code](https://www.youtube.com/watch?v=K_laUuqf2fc&t=1959s)