CreatedAt: 24-06-2025 09:56

Tags: #infra #cdn

---
# Conceito Geral
**Content Delivery Network** - É uma rede que visa alta disponibilidade de conteúdo estático.
Ela funciona da seguinte forma, existem diversos servidores espalhados pelo mundo, que funcionam como servidores de [[Cache|cache]] de conteúdo em localizações estratégicas para entrega de conteúdo, quando uma solicitação de conteúdo estático é feita, ela não bate direto no servidor da aplicação, nas sim em um servidor CDN que por sua ver verifica se o conteúdo existe ou não, caso não exista, vai no servidor da aplicação, obtém o conteúdo e o armazena em [[Cache|cache]].
Esse armazenamento geralmente possui uma configuração para expirar/invalidar esse arquivo depois de um tempo.
[[Fluxo de funcionamento CDN|Aqui]] está um exemplo de fluxo.
Veja as [[Vantagens de uso em ambientes cloud]].

---
# Referências
- [Canal Fernanda Kipper](https://youtu.be/pOFToA0Upek?si=WKAbtl0H3-ffQKAd)
- [Locaweb](https://www.locaweb.com.br/blog/temas/codigo-aberto/cdn/)