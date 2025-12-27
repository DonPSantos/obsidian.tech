CreatedAt: 27-05-2025 09:24

Tags: #cloud #auth

---
# Conceito Geral
Users da AWS se dividem em 2 tipos basicamente
- **Programmatic Access** - Acesso geralmente utilizado por aplicações para que elas efetuem login na AWS, nesse você recebe um **access key ID** e um **secret access key**
- **AWS Management Console Access** - Acesso ao console da AWS, geralmente utilizado por pessoas, nesse aqui você loga direto na plataforma da AWS, pode ser com senha ou login federado
Uma recomendação é não tratar permissões direto no usuario, o melhor caminho é criar os [[AWS Groups|grupos]] e atribuir os usuários aos [[AWS Groups|grupos]].

---
# Referências
- [AWS Users](https://docs.aws.amazon.com/IAM/latest/UserGuide/id_users.html)
