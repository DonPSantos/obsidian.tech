CreatedAt: 31-03-2026 09:58

Tags: #principle #poo #solid

---
## Conceito Geral
Esse conceito diz que uma classe deve ser fechada para alteração e aberta para expansão, vamos para o exemplo de uma classe de exames.
Exemplo errado:
``` C#
public class AprovaExame 
{ 
	public void aprovarSolicitacaoExame(Exame exame)
	{ 
		if(exame.tipo == SANGUE){ 
			if(VerificaCondicoesExameSangue(exame)) 
				Console.WriteLine("Exame sanguíneo aprovado!"); 
		} else if(exame.tipo == RAIOX) 
		{ 
			if (VerificaCondicoesRaioX(exame)) 
				Console.WriteLine("Raio X aprovado!"); 
		} 
	} 
	private boolean VerificaCondicoesExameSangue()
	{ 
	//.... 
	} 
	private boolean VerificaCondicoesRaioX(){ 
	//....
	} 
}
```
Observe esse exemplo e pense na adição de um novo exame por exemplo uma endoscopia, teria de adicionar mais um IF e mais um método privado, agora vamos reescrever seguindo o principio.
Primeiro, vamos criar uma interface que vai servir para todos os exames.
``` C#
public interface IAprovaExame
{ 
	void aprovarSolicitacaoExame(Exame exame); 
	bool verificaCondicoesExame(Exame exame); 
}
```
Com essa interface, sempre que quisermos implementar um novo exame, criaremos uma classe que implementa essa interface.
``` C#
public class AprovaExameSangue: IAprovaExame
{ 
	public void aprovarSolicitacaoExame(Exame exame)
	{ 
		if(VerificaCondicoesExame(exame)) 
			Console.WriteLine("Exame sanguíneo aprovado!");  
	}
	
	bool VerificaCondicoesExame(Exame exame)
	{ 
	//.... 
	} 
}

public class AprovaRaioX: IAprovaExame
{  
	public void AprovarSolicitacaoExame(Exame exame)
	{ 
		if(VerificaCondicoesExame(exame)) 
			Console.WriteLine("Raio X aprovado!");
	} 
	
	bool VerificaCondicoesExame(Exame exame)
	{ 
	//.... 
	} 
}
```
Agora as regras dos exames estão totalmente isoladas, cada um em sua classe, uma observação importante, esse principio não acaba com os IFs, eles vão para uma outra camada a qual não tenha regra de negocio, apenas orquestração de fluxo.
Outro ponto a se relacionar é que aplicando e esse principio ele se relaciona com o [[Single Responsability Principle]].

---