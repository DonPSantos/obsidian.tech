CreatedAt: 15-03-2026 18:48

Tags: #auth #authentication

---
## Conceito Geral
**Security Assertion Markup Language** é um padrão de código aberto utilizado para **autenticação** [[O que é SSO|SSO]] em aplicações, principalmente no meio empresarial,. Ele utiliza o XML por debaixo dos panos.
## Exemplo de fluxo
``` mermaid
sequenceDiagram
actor user as Usuário
participant app as WebApp
participant idp as IDP

user ->> app: Solicita login
app ->> idp: Direciona o login para um IDP que sabe resolver
idp -->> user: Solicita as credenciais
user ->> idp: Insere as credenciais
idp -->> app: Retorna um XML que contém informações do usuário<br/>e grupos e funções do mesmo
app ->> app: Verifica assinatura do XML
app -->> user: Concede acesso
```

---