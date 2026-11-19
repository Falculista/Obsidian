---
Title: Soma dos Ângulos Internos de um Polígono
Data: 2025-08-19
tags:
  - Matemática
  - Estudos
  - Geometria
  - Geometria_Plana
  - Polígonos
---
Sabemos que os polígonos possuem em cada abertura entre duas arestas um ângulo, mas seria interessante se, ao sabermos a soma de todos os ângulos internos dele, pudéssemos determinar a quantidade de arestas (ou vértices, pois o número de vértices é igual ao de arestas) dele, e vice-versa.
# Ângulos Internos de um Triângulo
Sabemos que a soma dos ângulos internos de um triângulo é igual a $180\textdegree$ como foi demonstrado em [[02 - Ângulos de um Triângulo]].

![[Soma_Angulos_Internos_Ex1|center|500]]
O interessante disso, que você verá na próxima parte, é que para saber a soma dos ângulos internos de qualquer outro polígono, basta sabermos a do triângulo, por isso começamos definindo isso para depois avançarmos em outros polígonos.
# Ângulos Internos de um Polígono Qualquer
Vejamos, inicialmente, um quadrilátero qualquer:
![[Soma_Angulos_Internos_Ex2|center|500]]

Para determinar a soma dos ângulos internos deste (e de qualquer outro) quadrilátero, podemos colocar ele em função de triângulos, pois como sabemos a soma dos ângulos internos de um triângulo, ao transformarmos um quadrilátero em triângulos nós saberemos quais são seus ângulos internos. 

Só que observe que o nosso objetivo principal nessa parte aqui é determinar qual é a soma dos ângulos internos para um polígono qualquer, ou seja, somente com seu número de vértices (ou arestas) obter essa informação. Por essa razão, vamos analisar isso a partir do ponto de vista de um único vértice, e não do polígono inteiro. Isso significa que formaremos triângulos em um polígono usando somente $1$ vértice, para depois conseguirmos observar um padrão e generalizar para um polígono de $n$ vértices. Segue abaixo essa ideia em um quadrilátero:

![[Soma_Angulos_Internos_Ex3|center|500]]

Então, a partir do ponto de vista do vértice em destaque, conseguimos traçar somente uma diagonal no polígono, dividindo o quadrilátero em $2$ triângulos. Porém, nós sabemos que

![[Soma_Angulos_Internos_Ex4|center|800]]

portanto, somando no sistema:

![[Soma_Angulos_Internos_Ex5|center|800]]

Conclui-se então que um quadrilátero possui $360\textdegree$ como soma de seus ângulos internos. Agora note que $360$ é o dobro de $180$, que é a soma dos ângulos de um triângulo, e isso não é coincidência, pois quando dividimos o quadrilátero em $2$ triângulos, é intuitivo que, por cada um possuir $180\textdegree$, o quadrilátero possuiria então $360\textdegree$. Podemos escrever então que, para um quadrilátero, a seguinte conta é válida:$$\boxed{S_i=180\textdegree \cdot 2}$$
sendo $S_i$ a soma dos ângulos internos e $2$ o total de triângulos formados na figura.

Para