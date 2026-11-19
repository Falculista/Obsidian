---
Title: Matrizes
Data: 2025-04-23
tags:
  - Matrizes
  - Matemática
  - Álgebra
  - Estudos
---
# O que são matrizes?
Matriz é uma estrutura na qual números são organizados em linhas e colunas, sendo bem parecido com uma tabela, como podemos ver abaixo:
$$ A_{3X2} = \left[ \begin{array}{cc} 7 & 4  \\ 5 & 2  \\ -1 & 9\ \end{array} \right] $$
No caso acima, podemos ver uma matriz $3$x$2$, que nada mais é do que uma matriz com 3 linhas e 2 colunas, portanto dizemos que A é uma matriz de ordem $3$x$2$.
# De onde surgiram as matrizes?
Agora que entendemos o básico do que são matrizes, é interessante, antes de adentrar a tópicos mais profundos, explicar o surgimento delas.

Na China antiga, por volta de $200a.c$, foi escrito um livro chamado <u>"Nove Capítulos da Arte Matemática"</u>. Este livro introduziu o estudo dos chamados [[Sistemas Lineares]]. Podemos ver um exemplo de sistema linear abaixo, de acordo com a nossa notação moderna:
$$ \left\{ \begin{array}{rc} x+y=2 \\ 3x-y=2  \end{array} \right. $$
Para se resolver esse sistema, é comum somar os valores da primeira e segunda equação, para que assim um valor seja anulado (note que isso funciona somente nos casos em que um valor pode ser anulado, como é o caso do y). Fazendo isso no exemplo acima, o resultado seria: 

$$ x+3x\cancel{+y}+\cancel{(-y)}=2+2 \therefore 4x=4\therefore \frac{\cancel4x}{\cancel4}=\frac{\cancel4}{\cancel4} \therefore \boxed{x=1}$$

Porém, o sistema que eles usavam na época era diferente, funcionando da seguinte forma:

|  X  |   Y   |
| :-: | :---: |
|  I  |   I   |
| III | **I** |
| II  |  II   |
Dado um sistema linear com dois valores $x$ e $y$, como visto no exemplo de cima, para cada unidade no coeficiente (isso é, o valor antes de cada letra, sendo o 1 no caso de um espaço vazio) é adicionado um risco "I" em uma tabela, mais especificamente na coluna que representa qual valor o coeficiente está multiplicando, sendo que na última linha, os riscos representam o resultado da equação. 

No caso da primeira equação do sistema, o $x$ está sendo multiplicado por 1, portanto na tabela é adicionado um risco na coluna referente aos valores de x, e assim sucessivamente com todos os valores de x e y. 

É importante notar também que, se um valor for negativo (como é o caso do $-y$  na segunda equação), ele será representado por um risco preto, para diferenciar dos valores positivos.