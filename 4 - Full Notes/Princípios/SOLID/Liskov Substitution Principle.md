CreatedAt: 31-03-2026 10:23

Tags: #principle #poo #solid

---
## Conceito Geral
Esse principio diz que a classe derivada pode ser substituída pela sua classe base sem quebrar. Para ser mais claro, tudo que a classe pai faz, a filha deve fazer também, por exemplo vamos pensar em animais.
``` C#
public class Animal
{
    // Método virtual permite sobrescrita
    public virtual void EmitirSom()
    {
        Console.WriteLine("Som de animal");
    }
}

public class Cachorro : Animal
{
    // Sobrescrita do método base
    public override void EmitirSom()
    {
        Console.WriteLine("O cachorro late");
    }
    
    public void AbanarRabo()
    {
	    Console.WriteLine("O cachorro abana o rabo");
    }
}
```
Perceba que onde existir a classe animal, você pode utilizar a classe cachorro no lugar sem problemas, visto que cachorro implementa todas as ações de animal, mesmo tendo outras ações.

---