CreatedAt: 18-06-2025 21:53

Tags: #messagebroker #queue #cloud 

---
# Conceito Geral
Esse exchange funciona de forma local, diferente dos outros que a fila pode residir em um nó diferente.
O uso desse exchange é para uma baixa latência e entrega super rápida, caso exista alguma fila ativa ou até mesmo mais de uma, a entrega será feita de forma aleatótia.

---
# Referências
- [RabbitMQ](https://www.rabbitmq.com/docs/local-random-exchange)