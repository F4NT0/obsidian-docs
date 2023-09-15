## Listas Lineares

* Listas lineares é um [TAD](https://github.com/F4NT0/Algoritmos_Estrutura_Dados/wiki/TAD)

* Lista linear agrupa informações referentes a um conjunto de elementos que possuem uma relação de ordem linear entre eles

* Conjunto de Nodos n > 0 tais que suas propriedades estruturais decorrem da posição relativa dos Nodos dentro de uma sequencia linear, ou seja, um Nodo possui a informação do Nodo anterior e do proximo

* Em uma lista linear deve ser armazenado a referência do primeiro e ultimo nodo da lista, tendo os seguintes nomes:
    * primeiro nodo da lista: **HEAD**
    * ultimo nodo da lista: **TAILS**

* Os métodos das Listas lineares são a implementação dos métodos existentes na interface TAD, para isso se deve fazer o seguinte na classe java:

```java
public class ListasLineares implements TAD{
   //Implementação dos métodos da interface TAD
}
```

**Todos os códigos implementados se encontram no diretório TAD**

### Aplicações

* Aplicações com listas de alocação sequencial são mais limitadas, mas são bastante utilizadas
* Sua aplicação não é recomendada quando não se sabe exatamente quantos elementos deverão ser armazenadas ou se forem muitos elementos

### Alocações

* Existem dois tipos de alocações em uma Lista
    * Alocações Estáticas
    * Alocações Dinâmicas

* **Alocação Estática**
    * Possui um tamanho fixo
    * Funciona como um Vetor
    * Problemas:
        * Custo muito grande em inserção e remoção
        * Tem que ter uma estimativa de tamanho máximo
    * Utilidade:
        * Quando é necessário otimizar o uso da memória

1 | 2 | 3 | 4 | 5 | 6 
-|-|-|-|-|-|

* **Alocação Dinâmica**
    * Aumenta e diminui em tempo de execução
    * Estrutura encadeada onde se usa Nodos que são ligados entre si para indicar a relação de ordem existente entre os itens
    * Utilidade:
        * Quando não é possivel prever o número de entradas de dados
        * Quando uma operação necessita de uma estrutura encadeada

![nodo1](https://github.com/F4NT0/Algoritmos_Estrutura_Dados/wiki/lista/nodo1.png)


## Listas Encadeadas

* Consiste de um determinado número de Nodos, cada um com uma referência para o proximo
* A inserção e remoção de elementos no meio de uma lista encadeada é uma operação prática
* Possui duas representações diferentes:
    * Encadeamento simples
        * Constitui de que necessita somente da referencia ao proximo nodo
    * Encadeamento duplo
        * Constitui que o Nodo possui uma referencia ao proximo e ao anterior

![nodo2](https://github.com/F4NT0/Algoritmos_Estrutura_Dados/wiki/lista/nodo2.png)

* A organização dos Nodos é a seguinte:
   * Nodos conectados por links
   * Acesso direto ao primeiro elemento é obrigatório
   * Acesso direto ao ultimo não é obrigatório
   * Outros nodos podem ser acessados a partir dos links

![nodo3](https://github.com/F4NT0/Algoritmos_Estrutura_Dados/wiki/lista/nodo3.png)

#### Implementação da Classe Nodo

* Exemplo de uma classe Nodo Genérico

```java
private class Nodo<T>{
    private T elemento;
    private Nodo<T> proximo;
    public Nodo(E e){}
    public void definirElemento(T e){}
    public T pegarElemento(){}
    public void definirProximo(Nodo<T> n){}
    public Nodo<T> pegarProximo(){}
}
```
* Glossário da Classe Nodo

Nome | Definição
-----|----------
**T** | tipo genérico, onde podemos usar classes
**elemento** ou **e** | nome da variavel genérica do elemento do Nodo
**n** | variavel de entrada de um Nodo
definirElemento(T e) | método para definir o tipo de elemento do Nodo
pegarElemento() | Método para retornar o elemento
definirProximo(Nodo<T> n) | Método para definir qual nodo será o proximo do atual
pegarProximo() | Método para retornar o proximo Nodo


* Tem que ser definido e implementado esses métodos para se poder usar em um TAD lista

* Para alocar um nodo em Java se usa o operador **new** para criar um novo nodo

```java
Nodo<Classe> novoNodo = new Nodo<Classe>(elemento);
```

* Como os objetos Nodo devem ser acessados apenas pela classe de Lista, a classe Nodo pode ser declarada como uma **classe Interna**

* Classes internar são classes declaradas dentro de outras classes e que são visíveis apenas dentro do contexto da classe onde estão definidas
