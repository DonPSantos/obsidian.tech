CreatedAt: 31-03-2026 11:02

Tags: #principle #poo #solid 

---
## Conceito Geral
Aqui é tratado que diversas interfaces é melhor que uma única interface genérica gigantesca.
Para o exemplo errado, vamos pensar em um funcionário, e criar uma interface para ele:
``` C#
public interface IFuncionario 
{ 
	public decimal Salario(); 
	public decimal GerarComissao(); 
}
```
Agora temos dois tipos de funcionários especializados:
``` C#
public class Vendedor: IFuncionario 
{ 
	public decimal Salario() 
	{ 
		//Código
	} 
	public decimal GerarComissao() 
	{ 
		//Código
	} 
}

public class Recepcionista: IFuncionario
{ 
	public decimal Salario() 
	{ 
		//Código
	}  
	public decimal GerarComissao() 
	{ 
		//Código
	} 
}
```
Percebe o problema? Uma recepcionista podendo gerar comissão? Não faz sentido, o melhor seria ter mais interfaces de forma especifica, vamos reescrever da forma correta agora.
``` C#
//Interface base se mantém, mas removemos o metodo de gerar comissão
public interface IFuncionario 
{ 
	public decimal Salario();
}
// Movemos o metodo para outra interface
public interface IComissionavel
{ 
	public decimal GerarComissao(); 
}

//O vendedor implementa as duas interfaces pois precisa de ambos os metodos.
public class Vendedor: IFuncionario, IComissionavel
{ 
	public decimal Salario() 
	{ 
		//Código
	} 
	public decimal GerarComissao() 
	{ 
		//Código
	} 
}

//A recepcionista implementa apenas a funcionario que contém apenas o que ela precisa saber fazer.
public class Recepcionista: IFuncionario
{ 
	public decimal Salario() 
	{ 
		//Código
	}
}
```


---