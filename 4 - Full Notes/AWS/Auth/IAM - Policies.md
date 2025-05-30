CreatedAt: 26-05-2025 17:36

Tags: #cloud #auth

---
# Conceito Geral
As policies definem de forma granular o que cada recurso na AWS pode acessar e fazer dentro da própria AWS, essas regras são fixas no recurso ao qual forem atribuídas.
Policies podem ser atreladas diretamente a [[IAM - Users|usuários]], [[AWS Groups|grupos]], [[IAM - Roles|roles]] ou recursos.
Exemplos de usos de Policies:
- Permitir que o [[EC2 |EC2]] que tenha uma API consiga se comunicar com um [[RDS |RDS]].
- Criar uma [[IAM - Roles|role]] que permita listar [[S3|buckets]].
- Dar para um grupo destinado a analistas de BI acesso ao [[Amazon QuickSight]].

---
# Referências
- [AWS IAM Policies](https://docs.aws.amazon.com/IAM/latest/UserGuide/access_policies.html)