CreatedAt: 15-03-2026 14:10

Tags: #auth #oauth2

---
## Conceito Geral
Esse fluxo já foi o padrão, mas atualmente está sendo substituído pelo [[Authorization Code + PKCE]] mas ainda é seguro em determinados casos de uso.
## Casos de uso
Esse fluxo é melhor utilizado quando você tem um front que roda no servidor e não no navegador, o que possibilita guardar o client_secret de forma mais segura.
## Diagrama do fluxo
``` mermaid
sequenceDiagram
actor user as Usuário
participant ua as Browser
participant client as Client (API)
participant as as Authorization Server (Google)
participant rs as Resource Server (Google Calendar)

user ->> ua: Clica em login com o Google
ua ->> client: Envia a solicitação
client ->> as: Redireciona o navegador para o IDP passando client_id, scopes e redirect_uri
as -->> ua: Solicita consentimento
ua -->> user: Monstra um botão para consentir
user ->> ua: Confirma consentimento
ua ->> as: Retorna consentimento
as -->> client: Envia o authorization_code para a redirect_uri
client ->> as: Envia o authorization_code e client_secret da API
as -->> client: Retorna o access_token
client ->> rs: Enviar o access_token para solicitar os dados protegidos
rs -->> client: Retorna os dados protegidos
```

---
