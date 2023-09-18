## Tipos Abstratos de Dados - TAD

* Para entendermos Tipos Abstratos de Dados devemos entender os seguintes conceitos:
    * Abstração
    * Encapsulamento
    * Modularidade

1. **Abstração**
    * Abstração é um dos pilares da programação Orientada a Objetos
    * Abstração consiste em pegar um objeto e pensar e trabalhar em suas principais propriedades
    * Conseguir abstrair um item do mundo real e transformá-lo em uma classe em uma linguagem Orientada a Objetos
    * Nós pegamos todas as informações essenciais e "abstraimos" o que não é necessário
 
Exemplo:
   * Um carro possui as seguintes propriedades essenciais
       * Código da Placa
       * Cor
       * Modelo
       * Ano 
   * Construimos então uma Classe chamada Carro, onde podemos definir vários carros diferentes

2. **Encapsulamento**
   * Encapsulamento é a tecnica de manter oculto o funcionamento dos métodos de uma classe para os objetos
   * Um programa externo ou usuário só precisa saber o nome do método e não sua implementação
   * Encapsulamento é feito principalmente com métodos Publicos
   * Métodos são chamados pelo usuário, mas a sua implementação fica encapsulada

3. **Modularidade** 
   * Modularidade é quando vários componentes interagem entre si para um objetivo

#### Tipo Abstrato de Dados

* TAD é um modelo matemático de estruturas de dados que especifica
     * O tipo de dado armazenado
     * As operações definidas sobre esses dados
     * Os tipos de parâmetros dessas operações

* TAD é principalmente um conjunto de métodos apresentados em uma interface
* Para utilizar um tipo abstrato de dados, se deve implementar esses métodos da interface
* esses métodos são um conjunto da algoritmos para gerenciar operações que podem ser realizadas

### Síntese Básica de um TAD

* Exemplos de TADs:
    * Strings
    * Listas

* Cada TAD possui uma coleção de elementos linearmente organizados
* TAD oferece métodos para lidar com esses elementos
* cada tipo de TAD deve ter esses métodos da interface implementados

### Implementação da classe interface do TAD

```java
public interface TAD<E>{
   public void adicionar(E e);
   public void adicionar(int index,E e);
   public void limpar();
   public boolean contem(E e);
   public E pegar(int index);
   public int indexDe(E e);
   public boolean estaVazio();
   public boolean remover(E e);
   public E remover(int index);
   public int tamanho();
   public E definir(int index, E e);
   public void addInicio(E e);
   public E pegarInicio();
   public E pegarFim();
   public boolean removerInicio();
   public boolean removerFim();
}
```
* Glossário das variáveis

Nome | definição
-----|---------
E | tipo genérico para qualquer tipo (objeto,int,String,...)
e | variável para o elemento que deseja colocar no TAD
index | variável para o valor da posição no TAD

* Glossário dos Métodos do TAD

Método | Utilidade
-------|----------
adicionar(E e) | adiciona um elemento no TAD
adicionar(int index, E e) | adiciona um elemento em uma posição especifica
limpar() | limpa todos os elementos do TAD
contem(E e) | verifica se o elemento se encontra no TAD
pegar(int index) | retorna o elemento na posição desejada
indexDe(E e) | retorna a posição do elemento
estaVazio() | verifica se o TAD está vazio
remover(E e) | remove elemento especificado
remover(int index) | remove elemento da posição especificada
tamanho() | retorna o tamanho do TAD
definir(int index, E e) | define o tipo do dado que esta sendo armazenado
addInicio(E e) | adiciona o elemento no inicio do TAD
pegarInicio() | retorna o elemento no inicio do TAD
pegarFim() | retorna o elemento no fim do TAD
removerInicio() | remove o elemento no inicio do TAD
removerFim() | remove o elemento no final do TAD

* Nome em ingles para cada método
    * adicionar = add
    * limpar = clear
    * contem = contains
    * pegar = get
    * remover = remove
    * tamanho = size
    * definir = set
    * inicio = first
    * fim = last

O próximo assunto será sobre [Listas com TAD]()

Método | Utilidade
-------|----------
| teste | teste |
| ----- | ----- |
|       |       |