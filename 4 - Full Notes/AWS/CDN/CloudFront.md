CreatedAt: 24-06-2025 10:46

Tags: #cloud #infra #cdn 

---
# Conceito Geral
É o [[CDN]] da AWS. Ele pode trabalhar com conjunto com outra soluções da AWS como [[AWS Shield]], [[AWS Web Application Firewall (WAF)]] e [[Amazon Route 53]]. 
Também da para integrar ele com o [[AWS Certificate Manager (ACM)]] para adicionar certificado [[SSL]].
Outra coisa que é possível fazer é o controle de autorização, como exemplo você pode fazer com que um bucket [[S3]] seja acessível apenas pelo CloudFront e controlar quem pode ou não ter esse acesso.
O CloudFront pode ser configurado para conectar com um endpoint ou um [[OAC]].

---
# Referências
- [AWS](https://docs.aws.amazon.com/pt_br/AmazonCloudFront/latest/DeveloperGuide/getting-started-secure-static-website-cloudformation-template.html)
- [AWS](https://aws.amazon.com/pt/cloudfront/getting-started/?nc=sn&loc=4)
