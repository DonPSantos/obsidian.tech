CreatedAt: 16-02-2026 14:24

Tags: #auth #token #jwt

---
## Conceito Geral
Nessa parte estão as claims do token, são as informações que o token transporta que podem ser informações default do padrão JWT ou adicionadas pelo IDP que o gerou, essas claims se subdividem em 3 tipos:
- [[Registered Claims]]
- [[Public Claims]]
- [[Private Claims]]
Um exemplo de estrutura desse payload
``` JSON
{
  "sub": "1234567890", //claim redistered 
  "name": "John Doe", //claim que pode ser publica ou privada
  "admin": true, //claim que pode ser publica ou privada
  "iat": 1516239022 //claim redistered 
}
```

---
## Referências
- [YT - Código Fonte TV](https://www.youtube.com/watch?v=Gyq-yeot8qM)