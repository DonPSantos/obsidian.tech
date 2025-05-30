CreatedAt: 27-05-2025 09:13

Tags: #cloud 

---
# Conceito Geral
- **OnDemand** - paga-se de acordo com o uso, é instantâneo e de acordo com o solicitado, mas em contra partida é o mais caro.
- **Savings Plans** - Você solicita a maquina por um contrato de 1 a 3 anos pago de forma antecipada, nesse caso é para uma aplicação estável, não é recomendado para Auto Scaling, visto que tem que ter previsão total de uso dessa maquina, essas maquinas são mais baratas que OnDemand, podendo chegar a uma economia de 72%.
- **Spot** - São instancias que podem cair a qualquer momento, pois utilizam o recurso que está ocioso do EC2, se alguma instancia OnDemand ou Saving Plan solicitar esse recurso, sua maquina será desativada. Nesse caso, a economia chega a 90%.

---
# Referências
- [AWS Modelo de pagamento EC2](https://aws.amazon.com/pt/ec2/pricing/)