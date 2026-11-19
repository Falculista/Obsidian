---
Title: Nº de Diagonais de Polígonos
Data: 2025-08-17
tags:
  - Polígonos
  - Matemática
  - Geometria
  - Geometria_Plana
  - Estudos
---
# O que é diagonal?
A diagonal é o segmento que liga dois vértices passando por dentro do polígono convexo. Exemplo:
![[Diagonal_de_Polígonos_1|center|700]]
No exemplo acima, percebemos que o triângulo não possui diagonais, pois todas as linhas que conectam dois vértices não passam por dentro do polígono, pois para quaisquer três pontos, só existe uma possibilidade de conectar eles. Em outras palavras, o triângulo em si já é a única conexão que pode haver entre seus pontos, e não existe outra forma de conectá-los sem que isso forme arestas e não diagonais. Concluímos assim que, para haver diagonais em um polígono, é preciso que haja no mínimo $4$ vértices no polígono.

Analisando agora a segunda figura, que aliás é um hexágono, ela possui:
- $6$ vértices ($6V$);
- $6$ arestas ($9A$);
- $9$ diagonais ($9d$).

Vendo agora isso para os principais tipos de polígonos, temos:

| Nome do Polígono | Nº de Vértices | Nº de Diagonais |
| ---------------- | -------------- | --------------- |
| Triângulo        | 3              | (não possui)    |
| Quadrilátero     | 4              | 2               |
| Pentágono        | 5              | 5               |
| Hexágono         | 6              | 9               |
| Heptágono        | 7              | 14              |
| Octágono         | 8              | 20              |
| Eneágono         | 9              | 27              |
| Decágono         | 10             | 35              |
| Undecágono       | 11             | 44              |
| Dodecágono       | 12             | 54              |
| Icoságono        | 20             | 170             |

# Número de diagonais
O nº de diagonais de um polígono é facilmente deduzível se você souber quantas diagonais somente $1$ vértice tem e quantos vértices existem na figura. No caso do hexágono, pense o seguinte: cada vértice de um hexágono possuirá $3$ diagonais; seu número de vértices é igual a $6$; aqui talvez você pense que basta multiplicar esses números e achamos a quantidade de diagonais, porém ao multiplicar esses números você está contando tanto com a "ida" de cada diagonal de um vértice para outro (isto é, do vértice $A$ para $B$ por exemplo) quanto com a "volta" (de $B$ para $A$), portanto para achar o número real de diagonais você deve, ao final da multiplicação, dividir o valor dela por $2$, considerando assim uma diagonal como sendo somente uma diagonal, e não duas (considerando ida e volta). Fazendo a conta: $$nº \space diagonais \space  do  \space hexágono=\frac{6\cdot3}{2}=\frac{18}{2}=9$$
Porém esse método de achar diagonais não é muito robusto, pois precisaríamos saber antes quantas diagonais cada vértice tem, e no caso de um polígono de $n$ vértices isso é impossível. Pensando nisso, vamos tentar formar uma fórmula mais robusta.

Se nós queremos saber quantas diagonais um polígono qualquer possui, a forma mais óbvia de se fazer isso é analisar quantas diagonais cada vértice forma e, a partir disso, generalizar para todos os $n$ vértices dele.

Cada vértice de um polígono, independente de qual seja, NÃO pode formar diagonais consigo mesmo e nem com os dois vértices ao seu lado, pois não há como se conectar em si mesmo e a conexão entre vértices colineares forma uma aresta e não uma diagonal. Portanto para cada vértice, sua conexão com outro vértice (tirando ele mesmo e os outros dois ao seu lado) forma uma diagonal, e se o número de vértices de um polígono é igual a $n$, cada vértice também não poderá fazer uma conexão somente com $3$ vértices, e a quantidade de diagonais que um vértice pode formar então é vista como sendo a quantidade de vértices que o polígono possui (pois para cada $1$ vértice é formado mais uma $1$ diagonal) menos esses $3$ que são desconsiderados, sendo que podemos resumir tudo isso como sendo: $(n-3)$. E ainda em um polígono de $n$ vértices, é intuitivo que isso se repetirá $n$ vezes, ou seja: $n\cdot(n-3)$, bastando agora aplicarmos a lógica que usamos anteriormente de desconsiderar a "ida" e "volta" como coisas distintas, e isso pode ser visto na fórmula a partir de uma divisão por dois. Concluímos então que:$$\boxed{nº \space de \space diagonais = \frac{n\cdot(n-3)}{2}}$$
sendo $n$ o número de vértices do polígono.
# Exercícios
Aqui iremos desde exercícios muito básicos alguns avançados. Os mais básicos serão para **_fixação_**, uns um pouco mais avançados serão de **_embasamento_** e depois, para os mais avançados ainda terão os exercícios de **_aprofundamento_**.
#### Fixação
1) Calcule o nº de diagonais de um quadrilátero convexo.
2) Calcule o nº de diagonais de um pentágono convexo.
3) Calcule o nº de diagonais de um hexágono convexo.
4) Calcule o nº de diagonais de um icoságono convexo.
5) Quantas diagonais partem de cada vértice de um octógono convexo?
6) Em uma região existem $10$ cidades, todas ˜ sobre uma circunferência imaginária. Deseja-se construir estradas em linha reta ligando todos estas cidades entre si. Quantas serão as estradas?
7) Qual polígono convexo possui $5$ diagonais?
#### Embasamento
1) Determine o polígono convexo cujo número de diagonais é o dobro do número de lados.
2) O numero de lados de dois polígonos convexos são dois números consecutivos. Se a diferença entre o número de diagonais é $8$, quais são esses polígonos? 
3) Existe um polígono convexo cujo número de diagonais é o triplo do número de lados?
4) Seja um octógono convexo $ABCDEFGH$. Quantas são as diagonais que não contêm os vértices $A$ nem $D$?
#### Aprofundamento
1) Dado dois polígonos convexos, sendo que um tem $6$ lados e $39$ diagonais a mais que o outro, determine a soma total do número de vértices e de diagonais dos dois polígonos.
2) Unindo-se três a três os vértices de um polígono regular, obtém-se $220$ triângulos. Quantas diagonais possui esse polígono?
3) A diferença entre o número de diagonais de dois polígonos convexos é 85 e o número de lados de um é o triplo do número de lados do outro. Quais são estes polígonos?
4) A soma do número de diagonais de dois polígonos convexos é $142$ e a diferença entre o número de lados é $1$. Quantos lados têm estes polígonos?
# Resolução dos Exercícios