CreatedAt: 18-06-2025 15:59

Tags: #queue #messagebroker #cloud 

---
# Conceito Geral
Muito semelhante ao [[Direct|Direct Exchange]] a diferença é que aqui temos uma funcionalidade a mais, podemos adicionar * e # para servirem como coringas na keys, por exemplo:
Temos 3 filas:
- Q1 (logs de acesso): apache.access
- Q2 (logs de erro): apache.error
- Q3 (logs de erro): apache.\*
Então, se eu receber uma mensagem com uma key apache.access tanto a fila Q1 quanto a fila Q3 receberão as mensagens porque o padrão (como se fosse uma regex) bate. O mesmo vale se eu receber uma mensagem com a key apache.error, a diferença é que a fila Q2 receberá mensagem ao invés da fila Q1.

---
# Referências
- [nelsonsar](https://nelsonsar.github.io/2013/11/07/RabbitMQ-exchange-types.html)