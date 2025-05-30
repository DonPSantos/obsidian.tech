CreatedAt: 26-05-2025 23:53

Tags: #cloud #auth

---
# Conceito Geral
É uma identidade que não está diretamente atrelada a nada, mas pode ser consumida por basicamente tudo, inclusive uma outra conta AWS.
Elas expiram com o tempo, são utilizadas geralmente para delegar acesso entre recursos AWS.
Um ponto importante é que além delas não terem uma longa duração, quem for consumir as roles não precisa de nenhum tipo de credencial, pois a role consegue resolver isso automaticamente com credenciais temporárias.

---
# Referências
- [AWS Roles](https://docs.aws.amazon.com/IAM/latest/UserGuide/id_roles.html)