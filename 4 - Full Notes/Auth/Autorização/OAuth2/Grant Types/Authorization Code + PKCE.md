CreatedAt: 15-03-2026 14:11

Tags: #auth #oauth2

---
## Conceito Geral
Esse é atualmente o fluxo mais seguro do OAuth 2, ele foi pensado em autentificar de forma segura aplicações que não conseguem esconder o client_secret, no caso, aplicações que não tem um backend no servidor.
## Casos de uso
Aplicações [[SPA]] ou mobile que não tenham backend, mas pode ser implementado com backend também
## Diagrama do fluxo
``` mermaid
sequenceDiagram
actor user as Usuário
participant app as App Mobile
participant as as Authorization Server (Google)
participant rs as Resource Server (Google Calendar)

user ->> app: Clica em login com o Google
app ->> app: Cria um code_verifier
app ->> app: Cria um code_challenge
app ->> as: Envia a solicitação de login com o code_challenge e o metodo de has utilizado
as ->> as: Armazena o code_challenge
as -->> user: Redireciona para tela de login
user ->> as: Faz login com as credenciais e da consentimento
as -->> app: Devolve um autorization_code
app ->> as: Solicita o access_token utilizando o autorization_code e o code_verifier
as ->> as: Valida o autorization_code e também faz o hash do code_verifier<br/>Verifica se o hash gerado bate com o armazenado
as -->> app: Retorna access_token
app ->> rs: Solicita recurso progetido com o access_token
rs -->> app: Retorna recurso
```

---

