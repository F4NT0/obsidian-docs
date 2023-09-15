## $$\sf Criando \space Titulos \space Avançados$$

Um título avançado em uma documentação é utilizando o símbolo **#** mais estruturas vindo do KateX dentro de um bloco especial.

Um bloco especial no Github são informações que ficam entre **$**.

`$$texto$$` faz com que o texto fique centralizado na página.

`$texto$` faz com que a palavra no texto fique em um formato diferente.

Para mais informações, leia a página [Utilizando KateX no markdown](Advanced/KateX).

---

Quando criamos um bloco especial em KateX, devemos separar cada palavra usando o comando _\space_ para dar um espaço separando cada uma.

`ris:Markdown``ris:Markdown`<table align="center">
    <tr>
        <td><img src="images/bloco-titulos.png"></td>
    </tr>
</table>

Compilando o exemplo acima:

$$Exemplo sem o uso do space$$

$$Exemplo \space com \space o \space uso \space do \space space$$

---

Podemos colocar esse bloco junto com um **#** para determinar como título.

<table align="center">
    <tr>
        <td><img src="images/Titulo-avanc1.png"></td>
    </tr>
</table>

Compilando o exemplo acima:

# $$Título \space Avançado$$

---

Podemos melhorar esse título usando uma fonte e colocar dentro de um box.

Para mudar a fonte podemos escolher entre o `\sf` e o `\frac`, existem outros mas estes dois foram os que achei mais bonito.

Para colocar um box no texto, colocamos todo o título dentro de um `\boxed{}`

Dentro de um box:

<table align="center">
    <tr>
        <td><img src="images/titulo-boxed.png"></td>
    </tr>
</table>

# $$\boxed{Título \space Avançado}$$

Dentro de um box usando a fonte `\sf`:

<table align="center">
    <tr>
        <td><img src="images/titulo-sf.png"></td>
    </tr>
</table>

# $$\boxed{\sf Título \space Avançado}$$

Dentro de um box usando a fonte `\frak`:

<table align="center">
    <tr>
        <td><img src="images/titulo-frak.png"></td>
    </tr>
</table>

# $$\boxed{\frak{Título \space Avançado}}$$

Podemos colorir, para isso leia mais sobre na página [Cores no Markdown](Advanced/Colors).

Mudando a cor do título para vermelho:

<table align="center">
    <tr>
        <td><img src="images/titulo-red.png"></td>
    </tr>
</table>

# $$\boxed{\sf \color{red} Título \space Avançado}$$

Mudando a cor do box e do texto para azul:

<table align="center">
    <tr>
        <td><img src="images/titulo-boxblue.png"></td>
    </tr>
</table>

# $$\color{blue} \boxed{\sf Título \space Avançado}$$
