CreatedAt: 31-03-2026 09:40

Tags: #principle #poo #solid 

---
## Conceito Geral
Principio que trata que uma classe deve ter uma única responsabilidade, vamos imaginar que temos uma classe de exames.
Exemplo de erro:
``` C#
public class Exames
{
	public void Aprovar(Guid id);
	public string VerificarStatus(Guid id);
	public void EnviarNotificacao(string content);
}
```
Percebe o erro? A classe não só cuida de exames, mas também notifica, isso esta fora de escopo, a classe é somente para exames, agora vamos reescrever esse código para que o respeite o principio.
``` C#
public class Exames
{
	public void Aprovar(Guid id);
	public string VerificarStatus(Guid id);
}

public class Notificacoes
{
	public void Enviar(string content);
}
```
Agora cada um tem sua responsabilidade, inclusive os nomes dos métodos ficam menos verbosos.

---