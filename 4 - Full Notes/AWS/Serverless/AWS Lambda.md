CreatedAt: 27-06-2025 10:29

Tags: #serverless #cloud

---
# Conceito Geral
É uma das formas de subir aplicações [[Serverless]] que a AWS disponibiliza.
A lambda é feita para aplicações "instantâneas" assim por dizer, é para executar funções simples e de execução rápida.
Funciona da seguinte forma, o Lambda recebe um estimulo de um gatilho, por exemplo um [[API Gateway]], assim que recebe esse gatilho, ele executa o que foi programado para fazer e depois morre.
Um ponto importante para atenção é fazer um bom tratamento de sua aplicação, pois como ela escala infinitamente e é cobrado por tempo de execução, a cobrança também pode ser infinita.

---
# Referências
- [AWS](https://aws.amazon.com/pt/lambda/)