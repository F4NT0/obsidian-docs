### Árvores

* Árvores são estruturas de dados que caracterizam uma relação de hierarquia entre os dados que a compõem, ou seja, para se conectar com um dado, deve passar por um dado que esteja conectado com ele anteriormente
* Normalmente uma árvore é caracterizadas como bolinhas que se conectam uma com as outras, como mostrado abaixo:
![exemplo_arvore](imagens_arvores/arvore.png)
* Cada bolinha de uma árvore é um Nodo, onde uma árvore em si possui um ou mais Nodos

#### Terminologias

* O primeiro Nodo da árvore(a ponta bem acima) é chamado de **raiz** da árvore, porque estamos vendo uma árvore de cabeça para baixo
* Todo o resto da árvore é uma **Sub-árvore** da árvore total, tendo sua própria raiz internamente dessa sub-árvore, ou seja, cada Nodo da árvore é raiz de uma sub-árvore
![raiz_subarvore](imagens_arvores/raiz.png)
* **Pai,irmãos e filhos**:
    * o Nodo raiz de uma árvore é chamada de **Pai** e todos os Nodos que estiverem ligados a ele são **filhos**
    * Quando tem dois Nodos, um do lado do outro, são chamados de **Irmãos**
![pai_filhos](imagens_arvores/pai_filho.png)

* **Grau e Nível**
    * **Grau** é o número de subárvores de um Nodo, ou seja, quantos Nodos estão conectados ao Nodo visto
    * Quando o grau é zero, o nodo não possui filhos, ele é denominado **Folha** ou **Terminal**
    * **Nível** é o número de linhas que liga o Nodo á raiz, e a raiz em sí é o Nível zero
    * Graus da Imagem abaixo:
        * Grau do Nodo A: 2
        * Grau do Nodo B: 2
        * Grau do Nodo C: 1
        * Grau do Nodo D: 1
        * Grau do Nodo E: 1
        * Grau do Nodo F: 2
        * Grau do Nodo G: 0(**Nodo Folha**)
        * Grau do Nodo H: 0(**Nodo Folha**)
        * Grau do Nodo I: 0(**Nodo Folha**)
        * Grau do Nodo J: 0(**Nodo Folha**)
![grau_nivel](imagens_arvores/grau_nivel.png)
* **Altura da Árvore**:
    * Altura é o tamanho total da árvore, sendo que a raiz da árvore é contado como zero
    * Altura total da árvore é a altura das folhas da árvore
    * Altura da árvore abaixo: 2
![altura](imagens_arvores/altura.png)

* **Revisão das Nomenclaturas**
    * O primeiro Nodo mais acima é a **Raiz**
    * Os Nodos internos da árvore são os **Nodos internos** ou  **Galhos**
    * Se retiramos o Nodo Raiz de uma árvore, teremos várias outras árvores, que chamamos nesse momento de **Floresta**

![definicao](imagens_arvores/Definicao.png)