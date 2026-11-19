---
Title: Postulados da Geometria de Posição
Data: 2025-08-07
tags:
  - Geometria_Espacial
  - Estudos
  - Matemática
---
# O que é Geometria de Posição?
Geometria de posição é a área da matemática que estuda as posições relativas entre formas geométricas no espaço. Abandonaremos então, nesse momento, nossos estudos de Geometria Plana, cuja principal função era estudar unicamente tudo aquilo que possui somente duas dimensões. Agora, nos estudos de Geometria Espacial, abordaremos três dimensões.
# Conceitos Primitivos

- **_Pontos_**:

```tikz
\begin{document}
\begin{tikzpicture}

	\filldraw[thick] (0,1) circle (2pt) node[anchor=north] {a};
\end{tikzpicture}
\end{document}
```

Um ponto é algo sem comprimento, largura ou profundidade. Se você der um zoom em um ponto, não verá ele aumentando, pois isso significaria que ele possui um tamanho definido e que, portanto, ao mudar o ponto de vista sobre ele, ele aumentaria ou diminuiria de tamanho.


- **_Retas_**:

  ```tikz
\begin{document}
\begin{tikzpicture}
	\draw [thick][<->] (-3,1) -- (7,1);
		\filldraw (0,1) circle (2pt) node[anchor=south] {A};
		\filldraw (4,1) circle (2pt) node[anchor=south] {B};
\end{tikzpicture}
\end{document}
``` 

Uma reta é um conjunto de pontos alinhados. A partir da reta (que possui tamanho infinito), conseguimos formar os _segmentos de reta_, que são "pedaços" da reta. No caso acima, vimos um segmento de reta entre $A$ e $B$, os conectando. Portanto, define-se o segmento de reta como sendo aquilo que conecta dois pontos. Há também as _semirretas_, que são infinitas somente para um lado, o outro possui um início, como podemos ver abaixo:

  ```tikz
\begin{document}
\begin{tikzpicture}
	\draw [thick][->] (0,1) -- (10,1);
		\filldraw (0,1) circle (2pt) node[anchor=south] {A};
\end{tikzpicture}
\end{document}
``` 
 

- **_Plano_**:
```tikz
\begin{document}
\begin{tikzpicture}

% --- Definimos aqui nomes para determinadas posições, não é necessário, mas ajuda no caso de ter de usá-las novamente por alguma razão ---
	\coordinate (A) at (-2,2);
	\coordinate (B) at (4,2);
	\coordinate (C) at (-3,0);
	\coordinate (D) at (3,0);
	
% --- Aqui, nós criamos uma figura que será pintada 70% de cinza e possuirá uma borda preta, tendo seus vértices as posições definidas acima ---	
	\filldraw[fill=gray!70,draw=black]
	(C) -- (D) -- (B) -- (A) -- cycle;

% --- Abaixo, nós criamos 4 pontos definidos nos pontos cartesianos que nós criamos anteriormente. Cada ponto terá uma letra o acompanhando, que foi criada com \node sendo que a posição da letra em relação ponto foi definido nos colchetes ---

	\fill (A) circle (2pt);
	\node[left] at (A) {A};
	
	\fill (B) circle (2pt);
	\node[right] at (B) {B};
	
	\fill (C) circle (2pt);
	\node[left] at (C) {C};
	
	\fill (D) circle (2pt);
	\node[right] at (D) {D};
	
\end{tikzpicture}
\end{document}
``` 

Um plano, assim como uma reta, também é um conjunto de pontos, porém agora não mais alinhados em uma só direção, mas em duas. Ou seja, um plano nada mais é do que um conjunto de pontos que forma uma superfície.
# Postulados
Dado os conceitos primitivos, conseguimos definir os postulados, que são conceitos completamente intuitivos e que não necessitam de uma demonstração, sendo que tudo se baseia neles, ou seja, são os fundamentos de todo o assunto (que no caso é Geometria Espacial). Existem alguns tipos de postulados, trataremos de todos eles abaixo.
### Postulados - Existência
O primeiro será os postulados referentes a existências, ou seja, dos que dizem respeito ao que existe no assunto. São eles:

1. Existem infinitos pontos.
2. Existem infinitas retas. Em cada uma, assim como fora dela, existem infinitos pontos.
3. Existem infinitos planos. Em cada um, assim como fora dele, existem infinitos pontos.
### Postulados - Determinação
No caso dos postulados da existência, apenas falamos sobre o que existe. Agora, abordaremos os postulados que determinam certas coisas com base nos conceitos primitivos. São eles:

1. Dois pontos distintos determinam uma única reta.
2. Três pontos não colineares determinam um único ponto.
### Postulados - Inclusão
Determinado as existências de certos conceitos axiomáticos e visto determinações com base nos conceitos primitivos, veremos agora o postulado referente a inclusão, ou seja, sobre o que está contido em quê. É ele:

1. Se uma reta contém dois pontos distintos de um plano, então a reta está contida no plano.
### Postulados - Separação
Agora analisaremos casos de separações. São elas:

1. Um ponto separa uma reta em duas semirretas.
2. Uma reta separa um plano em dois semiplanos.
3. Um plano separa um **_espaço_** em dois semiespaços.
### Postulado das Paralelas
Agora, para fechar os postulados, analisaremos o caso de paralelas. É ele:

1. Por um ponto passa uma única reta paralela a uma reta dada.

Esse, inclusive, é o famoso quinto postulado de Euclides, que, com base nele, foi formulado a geometria não euclidiana.