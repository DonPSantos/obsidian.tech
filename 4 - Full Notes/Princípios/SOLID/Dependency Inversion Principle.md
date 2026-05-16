CreatedAt: 31-03-2026 11:14

Tags: #principle #poo #solid

---
## Conceito Geral
Esse é o principio mais comum para quem trabalha com .NET, onde diz que você não vai utilizar uma implementação diretamente, você vai utilizar uma abstração (interface) para tornar o código mais flexível.
Primeiro o exemplo errado:
``` C#
public class PedidoService {
    private PedidoRepository repository;
    public PedidoService() {
        this.repository = new PedidoRepository();
    }
    public void ProcessarPedido(Pedido pedido) {
        // Lógica de processamento do pedido
        repository.salvarPedido(pedido);
    }
}
```
Aquele **new** representa que vocês está utilizando diretamente a classe, o que acaba gerando um alto acoplamento, por exemplo, seria muito complicado implementar o exemplo do [[Open-Closed Principle]] mas se implementando da forma correta, fica bem mais simples, vamos ao exemplo correto agora.
``` C#
public interface IPedidoRepository {
    void SalvarPedido(Pedido pedido);
}

public class PedidoService {
    private IPedidoRepository repository;
    public PedidoService(IPedidoRepository repository) {
        this.repository = repository;
    }
    public void processarPedido(Pedido pedido) {
        // Lógica de processamento do pedido
        repository.SalvarPedido(pedido);
    }
}
```
Perceba que agora você só conhece a interface, pouco importa a implementação, agora fica muito mais simples alterar a implementação se necessário, ou até mesmo aplicar o [[Open-Closed Principle]]. 

---