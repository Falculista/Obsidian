---
Title: 01 - Conceito e Representação Genérica
Data: 2025-11-25
tags:
  - Matrizes
  - Estudos
  - Matemática
  - Álgebra
  - Universo_Narrado
---
# $$\text{Matrizes}$$
Iniciando um novo módulo sobre matrizes e determinantes, começaremos por definir o que de fato são as matrizes.

Basicamente, matriz é uma estrutura na qual números são organizados em linhas e colunas. Visualmente, matriz é uma tabela. 

Veja o exemplo a seguir: 
$$
A =
\begin{bmatrix}
7 & 4 
\\
5 & 2
\\
-1 & 9
\end{bmatrix}
$$

Esta é uma matriz com $2$ colunas e $3$ linhas. Portanto, nós a chamamos de matriz $A_{3X2}$, conforme a imagem a seguir mostra:

![[Matriz_3x2|center|600]]

Note também que comumente nos referimos ao nome de uma matriz com uma letra maiúscula, enquanto que os elementos nela presente são referenciados com letras minúsculas.

Imagine agora uma matriz com $m$ linhas e $n$ colunas, sua representação genérica (isto é, uma representação "abstrata", não complexa, para fins didáticos, onde elementos são substituídos por letras por exemplo) será dada por:

![[Matriz_MXN|center|1000]]

>[!Observação]
>Na lista acima, pode-se cometer o erro de ler o número ao lado dos elementos da matriz como sendo algarismos de uma dezena. Exemplo: $a_{11}$ "'a' onze". Porém, note que os números, embora não espaçados, não estão juntos e são escritos próximos uns aos outros por convenção. Logo, para o elemento usado anteriormente, leríamos "'a' um um" ou ainda - na forma correta - "elemento 'a' linha um coluna um".

Além de representar uma matriz, podemos também montá-la com base em um sistema linear, afinal as matrizes são conjuntos de sistemas lineares (veremos isso com mais profundidade mais pra frente).

Supondo o seguinte sistema:
$$
A_{3X2} \rightarrow a_{ij} =
\begin{cases}
i^2+j \space ; \space i > j
\\
i^2-j \space ; \space i \leq j
\end{cases}
$$
Neste caso, para uma matriz $A_{3X2}$, o elemento $a$ presente na linha $i$ coluna $j$ terá as seguintes condições:

- Se $i$ for maior que $j$, o elemento $a_{ij}$ será igual a: $i^2+j$.
- Se $i$ for menor ou igual a $j$, o elemento $a_{ij}$ será igual a: $i^2-j$.

Montando a matriz:

![[Montagem de matriz|center|800]]

Então nós concluímos que, ao achar a expressão de uma matriz, nós podemos facilmente montá-la com base nas definições dadas.

---
# $$\text{Exercícios}$$
Agora que já estudamos o básico de matrizes, faremos alguns exercícios de fixação:

# Exemplo 1

Considerando a matriz abaixo, identifique: 

$$
A =
\begin{bmatrix}
1 & 2 & 1 & 4 
\\
4 & 8 & 7 & 6
\\
8 & 5 & 1 & -4 
\\
7 & 0 & 9 & 0
\end{bmatrix}
$$

- Ordem da matriz:
- Elementos:
	- $a_{12}=$
	- $a_{43}=$
	- $a_{33}=$
	- $a_{14}=$
# Exemplo 2

Construa a matriz de ordem $2X3$ dada por:

$$
a_{ij} =
\begin{cases}
2i+j^2 \space ; \space i \geq j
\\
i-j \space ; \space i < j
\end{cases}
$$
# $$\text{Resolução}$$
Passados os exercícios, resolveremos eles:
# Exemplo 1

Considerando a matriz abaixo, identifique: 

$$
A =
\begin{bmatrix}
1 & 2 & 1 & 4 
\\
4 & 8 & 7 & 6
\\
8 & 5 & 1 & -4 
\\
7 & 0 & 9 & 0
\end{bmatrix}
$$

- Ordem da matriz: $\color{yellow}4X4$
- Elementos:
	- $a_{12}=$ $\color{yellow}2$
	- $a_{43}=$ $\color{yellow}9$
	- $a_{33}=$ $\color{yellow}1$
	- $a_{14}=$ $\color{yellow}4$

# Exemplo 2

Construa a matriz de ordem $2X3$ dada por:

$$
a_{ij} =
\begin{cases}
2i+j^2 \space ; \space i \geq j
\\
i-j \space ; \space i < j
\end{cases}
$$

$$
\color{yellow}
A_{2X3} =
\begin{bmatrix}
a_{11} & a_{12} & a_{13}
\\
a_{21} & a_{22} & a_{23}
\end{bmatrix}
=
A_{2X3} =
\begin{bmatrix}
2\cdot1+1^2 & 1-2 & 1-3
\\
2\cdot2+1^2 & 2\cdot2+2^2 & 2-3
\end{bmatrix}
$$
$$
\color{yellow}
=
A_{2X3} =
\boxed{
\begin{bmatrix}
3 & -1 & -2
\\
5 & 8 & -1
\end{bmatrix}
}
$$
