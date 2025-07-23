CreatedAt: 18-06-2025 13:04

Tags: #cloud #messagebroker #queue 

---
# Conceito Geral
É um componente extra que [[Message Broker|message brokers]] rebem ao usar o protocolo [[AMQP]]. Esse componente começa a receber as mensagens para rotear elas e envia-las para uma [[Queue|fila]] ou para um outro exchange.
A comunicação entre um exchange e uma [[Queue]] recebe o nome de **binding**.
Existem tipos de exchanges que são:
- **[[Fanout]]**
- **[[Topic]]**
- **[[Direct]]**
- **[[Local Random Exchange]]**
- **[[Headers Exchange]]**

---
# Referências
- [nelsonsar](https://nelsonsar.github.io/2013/10/29/AMQP-building-blocks.html)
- [RabbitMQ](https://www.rabbitmq.com/docs/exchanges#types)