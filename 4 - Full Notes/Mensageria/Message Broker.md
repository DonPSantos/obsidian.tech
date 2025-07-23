CreatedAt: 18-06-2025 11:25

Tags: #cloud #messagebroker #queue 

---
# Conceito Geral
São aplicações core de um sistema com [[O que é uma mensageria|mensageria]], eles são os responsáveis por gerenciar a [[Queue|fila]] e garantir integridade das mensagens, nisso estamos falando de garantir que as mensagens estão sendo entregues, que os [[Consumer|consumidores]] estão corretos, que as mensagens não serão duplicadas ou ignoradas, dentre outras coisas.
Os message brokers mais famosos são:
- **[[Apache Kafka]]**
- **[[RabbitMQ]]**
- **[[Amazon SQS]]**
Alguns message brokers utilizam o protocolo [[AMQP]] para se comunicar, e isso adiciona uma funcionalidade nova, as [[Exchanges]] que passam a receber as mensagens dos [[Producer|producers]].

---
# Referências
- [IBM](https://www.ibm.com/br-pt/topics/message-brokers)
- [RabbitMQ](https://www.rabbitmq.com/docs/exchanges)
- [nelsonsar](https://nelsonsar.github.io/2013/10/29/AMQP-building-blocks.html)
