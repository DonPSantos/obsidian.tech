CreatedAt: 18-06-2025 11:02

Tags: #cloud #queue #messagebroker #architecture

---
# Conceito Geral
É uma forma de comunicação entre sistemas, os sistemas para de se comunicar diretamente e passam a utilizar um [[Message Broker]] que intermedia as comunicações, apesar de aumentar a complexibilidade, se bem utilizado deixa o sistema resiliente a falhas, também deixa o sistema extremamente desacoplado e com grande capacidade de escalabilidade.
O processo de mensageria possui os seguintes componentes (de forma simplista):
- **[[Producer]]**
- **[[Message Broker]]**
- **[[Consumer]]**
- **[[Queue]]**

---
# Referências
- Gemini
- [DEV](https://dev.to/matheushchaves/conhecendo-mensageria-491d)