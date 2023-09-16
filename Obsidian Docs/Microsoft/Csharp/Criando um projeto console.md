Para rodar programas C# é necessário criar um projeto .NET pelo Visual Studio (Forma mais fácil).

Existe um tipo de projeto no Visual Studio chamado `Console App` onde ele vai iniciar o projeto pelo console de vez de abrir um Swagger.

Esse tipo de projeto serve para testar programas simples de C# sem se preocupar em configurar ambiente, só vai precisar do seguinte:

1. Baixar o Visual Studio Community ou Enterprise
2. Baixar o JDK do .NET pelo site oficial
3. Criar um projeto console e colocar o que quer no arquivo chamado `Program.cs`

Vídeo que eu fiz para explicar todo o processo de criação de um projeto console:

<iframe width="711" height="400" src="https://www.youtube.com/embed/YcW7CLAQJjQ" title="Como criar um projeto console para testes em C#" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
## Passo a Passo

---

### Criando uma Solução vazia (Blank Solution)

---

- Com uma Solução, podemos criar projetos C# dentro dela.

1. Abra o Visual Studio e selecione a opção `Create a new project`

![[1.png]]

1. Vai mostrar uma tela com diferentes templates de projetos, nós vamos escolher a opção `Blank Solution` que vai nos deixar construir qualquer tipo de projeto, ele vai criar um projeto inicial somente com um arquivo `.sln` (Todo projeto .NET é uma Solução).

![[2.png]]

1. Coloque o nome da Solução seguindo o exemplo CamelCase e selecione a opção `Create`

![[3.png]]
### Criando um Projeto Console (Console App)

---

- Abra a solução e no canto direito tem a aba chamada `Solution Explorer`

![[4.png]]

- Clique com o botão direito do mouse no nome da Solução .NET

![[5.png]]

- Procure pela opção `Add > New Project...`

![[6.png]]- Procure pelo tipo de projeto chamado Console App e clique em Next
![[7.png]]

- Coloque um nome para a Solução seguindo o estilo _CamelCase_ onde a primeira letra de cada palavra é maiuscula.
- O local do projeto deve ser o mesmo da solução.
- Após verificado essas informações, clique em `Next`

![[8.png]]

- Por fim, coloque a versão do .NET que você esteja usando e clique em `Create`

![[9.png]]
- Após isso o Visual Studio vai criar o Projeto dentro da Solução e vai automaticamente abrir o arquivo `Program.cs` que é onde vamos colocar o código C# que o Visual Studio vai rodar para nós quando compilarmos.

![[10.png]]

### Executando o Projeto

---

- Para executar o projeto devemos definir ele como o principal para ser executado, onde vamos clicar com o botão direito em cima dele e escolher a opção `Set as Startup Project`

![[11.png]]

- Com isso agora vai mostrar o nome do nosso projeto na área de Runner do Visual Studio:

![[12.png]]

- Podemos usar o atalho de teclado `Ctrl` + `Shift` + `B` para compilar o projeto.
- Quando compilamos, vai abrir um console de `Output` dentro do Visual Studio

![[13.png]]
- Agora que o projeto foi compilado, podemos clicar no botão de `Run` do projeto e vai ser aberto um console (no meu caso o Powershell) com o resultado da compilação do arquivo `Program.cs`

![[14.png]]
## Conclusão

---

Com isso, agora podemos construir qualquer programa simples de C# para podermos testar a linguagem e entender melhor Programação Orientado a Objetos, onde o Visual Studio nos auxilia com as configurações iniciais para só nos preocuparmos com o desenvolvimento do projeto.

Agora você está apto a testar programas básicos de C#, caso queiria desenvolver uma API REST ou um projeto Desktop tem outros tipos de projetos que já lhe auxiliam no desenvolvimento muito mais rápido e já possuindo as regras básicas, mas como queremos somente compilar e testar programas em C# simples, o Projeto do tipo console já é excelente.