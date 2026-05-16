CreatedAt: 15-02-2026 18:52

Tags: #auth #token #jwt

---
## Conceito Geral
**Json Web Token** é um padrão aberto de gerar tokens que pode ser lido de forma fácil tem até um site para isso, o [jwt.io](https://www.jwt.io/) o que não faz dele menos seguro, muito pelo contrario, esse padrão é provavelmente o mais utilizado no mundo.
O JWT é dividido em 3 partes sem decodificar, essas partes são divididas por . e decodificado, cada uma é um objeto json, essas partes são:
* [[JWT Header|Header]]
* [[JWT Payload|Payload]]
* [[JWT Signature|Signature]]
Exemplo de token encoded:
eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJzdWIiOiIxMjM0NTY3ODkwIiwibmFtZSI6IkpvaG4gRG9lIiwiYWRtaW4iOnRydWUsImlhdCI6MTUxNjIzOTAyMn0.KMUFsIDTnFmyG3nMiGM6H9FNFUROf3wh7SmqJp-QV30

---
## Referências
- [YT - Código Fonte TV](https://www.youtube.com/watch?v=Gyq-yeot8qM)