CreatedAt: 15-03-2026 19:42

Tags: #auth #authentication #oauth2

---
## Conceito Geral
**OpenID Connect** - É a camada de [[Autenticação|autenticação]] [[O que é SSO|SSO]] construída sobre o [[O que é o OAuth2|OAuth 2]], o OIDC adiciona mais um objeto ao [[O que é o OAuth2|OAuth 2]], o ID Token, que diferente do [[Access Token]] é necessariamente um [[O que é JWT|JWT]] que contém as informações do usuário, como por exemplo nome, e-mail, url de foto, etc.
**ID Token**: É lido pelo front para montar a tela customizada pelo usuário
[[Access Token]]: É passado para o backend nas requisições para poder ter acesso aos recursos restritos.

---