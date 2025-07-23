CreatedAt: 16-06-2025 18:38

Tags: #cloud #storage #s3

---
# Conceito Geral
Qualquer coisa salva no S3 é um objeto com as seguintes propriedades:
- Key - Nome do arquivo
- Value - Os binários do arquivo
- Version - Versão do arquivo (isso é utilizado pelo [[Versionamento]])
- Metadata - Informações extras que todo arquivo tem como data, local, tag, etc.
- **[[ACL]]** - Permissão do arquivo

---
# Referências
- [AWS](https://docs.aws.amazon.com/pt_br/AmazonS3/latest/userguide/UsingObjects.html)