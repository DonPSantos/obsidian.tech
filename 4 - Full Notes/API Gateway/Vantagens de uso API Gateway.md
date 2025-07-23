CreatedAt: 26-06-2025 23:43

Tags: #cloud #auth #api #auth 

---
## Segurança
Com um API Gateway você pode implementar nele mesmo a validação de autenticação e autorização aos seus [[Microsserviços]], também é possível implementar apenas nele o certificado [[SSL]] e deixando seus [[Microsserviços]] em uma rede completamente privada. Também lhe proporciona uma forma segura de export uma documentação de consumo de seus serviços.
## Controle e transformação do trafego
Pode ser utilizado para rotear requests, transformar a requisição em um outro [[Protocolos de APIs|protocolo de API]] ou até mesmo configurar um [[Load Balancing]], esse funcionando apenas na [[7 - Aplicação|camada 7]].
## Performance
Outro ponto extremamente importante é que é possível configurar [[Cache]] para que você não precise fica fazendo consultas nos [[Microsserviços]], podendo assim gerar economia no ambiente cloud.

---
# Referências
- [Kong](https://konghq.com/blog/learning-center/what-is-an-api-gateway)