CreatedAt: 06-07-2025 15:11

Tags: #desig-pattner #behavioral-pattner #distributed-systems

---
# Conceito Geral
Esse pattern é geralmente utilizando para lidar com um fluxo que exija o consumo de vários [[Microsserviços]], aqui você tem um processo que pode levar ate mesmo dias, divididos em vários passos que caso um deles tenha falha, você pode programar o rollback de todos os [[Microsserviços]] que já foram executados durante esse fluxo.
O SAGA Pattern pode ser implementado utilizando os conceitos de [[Microsserviços orquestrados]] ou [[Microsserviços coreografados]].

---
# Referências
- [Canal Douglas Mugnos](https://www.youtube.com/watch?v=FEXtev8rEYM)
- [Microsservices.io](https://microservices.io/patterns/data/saga.html)
- [dev](https://dev.to/thiagosilva95/saga-pattern-para-microservices-2pb6)
