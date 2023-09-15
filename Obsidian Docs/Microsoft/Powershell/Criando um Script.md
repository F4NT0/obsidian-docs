## Comandos básicos de Powershell

Um `cmdlet` (pronuncia-se "command-let") é um comando compilado. Um **cmdlet** pode ser desenvolvido no .NET ou no .NET Core e invocado como um comando no PowerShell. Milhares de cmdlets estão disponíveis na sua instalação do PowerShell. O desafio está em descobrir o que eles são e o que eles podem fazer por você.

Comando|Para que serve
|---|---|
`$PSVersionTable`|Verifica a instalação do Powershell
`get-verb`|Apresenta todos os comandos possíveis
`Get-Command -Verb Get -Noun File*`|Encontrar os comandos que possuem Get no nome
`New-Item`| Cria um novo arquivo


## Criando um Arquivo Script de Powershell

* Primeiro criamos um arquivo com a extensão `.ps1` que são de Scripts Powershell

```powershell
New-Item example.ps1
```

* Depois abrimos esse arquivo em um editor de códigos, como o Visual Studio Code

```powershell
code helloworld.ps1
```

* Para enviar uma mensagem para o console pelo script iremos usar o comando $\color{lightblue}\cal{Write-Output}$

```powershell
Write-Output 'Hello World!'
```

* Para receber mensagens externas para o arquivo, usamos o comando $\color{lightblue}\cal{Read-Host}$
* Para enviar um texto para o console usamos o $\color{lightgreen}\cal{-Prompt}$
* Salvamos os dados em uma variável começando com `$` que recebe o texto de entrada

```powershell
$name = Read-Host -Prompt "Please enter your name"
```

* Para pegar a info dessa variável, chamamos o nome dela com o `$` dentro de uma String

```powershell
Write-Output "Congratulations $name! You have written your first code with PowerShell!"
```

## Rodando o primeiro Script

* Para rodar um projeto no Powershell, precisa abrir um Powershell como administrador e colocar o seguinte comando:

```powershell
Set-ExecutionPolicy RemoteSigned
```

* Depois feche o Powershell como administrador e abra um Powershell normal e rode o arquivo somente chamando o nome dele

```powershell
.\helloworld.ps1
```

