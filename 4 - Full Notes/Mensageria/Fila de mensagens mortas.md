CreatedAt: 19-06-2025 14:56

Tags: #queue #messagebroker

---
# Conceito Geral
Nada mais é que uma [[Queue|fila]] que recepta as mensagens de um [[Message Broker]] que tiveram algum erro durante o processo, essas mensagens ficam salvas para que a equipe responsável pelo sistema fique ciente das falhas e também possa analisar todas elas e tomar medidas necessárias para evitar novos erros, principalmente recorrentes.
Os motivos de falha de uma mensagem podem ser:
- A mensagem é enviada para uma [[Queue|fila]]que não existe.
- O comprimento máximo da [[Queue|fila]] foi excedido.
- A mensagem excede o limite de tamanho.
- A mensagem expira porque atingiu o [[TTL]].
- A mensagem é rejeitada por outra troca de [[Queue|fila]].
- A mensagem foi lida e rejeitada muitas vezes.

---
# Referências
