---
Title: Introdução a Joins em SQL
Data: 2025-09-02
tags:
  - SQL
  - Banco_de_Dados
  - Estudos
  - Computação
---
# O que é e pra quê serve o Join?
Em um banco de dados nós temos diversas tabelas com diferentes funções. Por exemplo, observe o caso abaixo:
![[Banco_de_Dados_JOIN_EX1|center|800]]
Onde nós temos um banco de dados com três tabelas dentro: "Clientes", "Pedidos" e "Produtos". Se um cliente (chamaremos aqui de Cliente_exemplo) fizer um pedido (Pedido_exemplo) com um produto (Produto_exemplo), teremos a seguinte relação:
![[Banco_de_Dados_JOIN_EX2|center|800]]

Agora, se você quiser saber quais produtos o clienteExemplo comprou, você precisará "juntar" (JOIN) as tabelas. Sem essa junção, seria muito mais difícil realizar a análise desses dados, evitando a redundância.
# Conjuntos
Como nós iremos juntar tabelas, ou seja, faremos um conjunto delas, podemos também deduzir que a Teoria dos Conjuntos será válida para essa junção. Portanto, para entendermos melhor como o JOIN funciona, precisamos também entender essa área da matemática.

Imagine dois conjuntos, como os abaixo:
![[Conjunto_JOIN_EX1|center|400]]

Cada conjunto possui seus elementos. Agora imagine que alguns elementos do conjunto $A$ também estão presentes no conjunto $B$ (ou interagem entre si), então nós podemos simplificar as coisas simplesmente juntando esses conjuntos de modo que esses elementos estejam presentes nos dois de forma concomitantemente. Representamos então a junção desses dois conjuntos por:
![[Conjunto_JOIN_EX2|center|330]]
Agora observe que há diferentes modos de analisar os elementos dessa junção. As possibilidades são:
- Elementos que somente estão em $A$;
- Elementos que somente estão em $B$;
- Elementos que estão em $A$ e $B$, mas não-concomitante a eles;
-  Elementos que estão em $A$ e $B$, mas concomitante a eles;

Os comandos do JOIN são basicamente permutações de intersecções entre dois conjuntos. Facilitando: pense que nós temos de juntar
