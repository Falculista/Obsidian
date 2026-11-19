---
Title: Introdução ao Modelo Computacional
Data: 2025-05-01
tags:
  - Pensamento_Computacional
  - Computação
  - Estudos
  - Fundamentos_Teóricos
---
# O que é Computação?
Antes de adentrarmos em conceitos mais complexo, é importante entender o que de fato é a computação. 

Basicamente, "computar" é o processo (também chamado de algoritmo, que veremos mais profundamente futuramente) utilizado para transformar uma informação inicial (chamado de "input") em uma final (chamado de "output"). Por exemplo, quando transformamos a equação $5+2$ em $7$, nós realizamos um processo de computação, que passou por meio de um algoritmo de soma de números.

Vimos então que o ato de "computar" (ou "computare" em Latim) é simplesmente "somar", "contar", "calcular".
# Sistemas de Numeração
Agora que vimos que "computar" é simplesmente contar, resta (para fechar os conceitos mais básicos sobre o que é computação) entender quais são os sistemas de numeração usados nessa contagem.
### Unário
Esse é o sistema mais básico de numeração, pois é contado a partir dos expoentes inteiros maiores ou iguais a 0 de 1, onde, por exemplo, cada dedo da minha mão representaria algum expoente de 1. Perceba que, de qualquer forma, cada dedo da minha mão vai representar uma unidade, pois todos os expoentes de 1 que satisfaçam as regras anteriores resultam em 1. Como vemos na figura abaixo:
![[Mão-Unário |center]]

Por exemplo, se eu precisasse contar quantas pessoas há em uma sala, eu poderia, usando os meus dedos, contar de 1 em 1 cada aluno, onde eu levanto um dedo para cada aluno contado. Porém perceba que, quando eu chegar em 10, eu não poderei mais contar, a não ser que abaixe meus dedos e comece a contar do 11, porém isso possibilita que alguns erros de contagem ocorra, pois você pode esquecer em algum momento em qual dezena está, pois nada ali te mostra se você está nos números entre 20 e 30; entre 30 e 40; etc.

Agora, é possível fazer com que eu conte mais de 10 usando somente meus dedos?
### Binário
Uma possível (e considerada a melhor) solução para o problema da contagem de 1 a 10 e suas limitações é simplesmente usar o sistema binário, onde, ao contrário do sistema anterior, nós fazemos o processo de exponenciação com a base 2. Como vemos na figura abaixo:
![[Mão-Binário |center ]]

O sistema agora pode soar um pouco estranho, pois agora o padrão de dedos levantados e abaixados será um pouco diferente, porém você verá que ele na verdade é bem simples. Usando o exemplo anterior da contagem de alunos, quando nós contarmos um aluno, levantamos o dedão; quando contarmos dois alunos, abaixamos o dedão e levantamos o indicador; quando contarmos três alunos, levantamos o indicador e o dedão juntamente; e assim sucessivamente, até o maior número, que será alcançado quando os 10 dedos estiverem levantados simultaneamente, que é o 1023.

Esse sistema é extremamente eficiente, pois você pode chegar a números muito grandes em sua contagem, desde os ímpares aos pares, usando somente os dedos da mão (como foi o nosso caso). Note que se usasse qualquer outra base, não daria certo, pois diversos números seriam deixados de fora, possibilitando que você somente conte alguns certos números. Se eu usasse um sistema de base-3 por exemplo e houvesse 8 alunos em uma sala e eu quisesse contar eles, seria impossível, pois os únicos números que poderia contar com esse sistema são: 1, 3, 4, 9, 10, 12, 13, 27 ..., 59048.

>[!info] Fontes
> - https://youtu.be/OwS9aTE2Go4?si=fEgsFMofwjglSADw
> - https://youtu.be/HjneAhCy2N4?si=rYbYYovkRjuxCHkL
> - https://youtu.be/DXvAlwMAxiA?si=xG23lfx7cb3UIxsq
> - https://youtu.be/rM9BjciBLmg?si=rSpA8uTm5REC7HaX
> - https://cs50.harvard.edu/x/2025/weeks/0/
> - https://youtu.be/IcrBqCFLHIY?si=2jFx65Kq3awTlzOi
> - https://youtu.be/sS7r7a-6SO0?si=UYX4ux_w0upuqA8y
> - https://youtu.be/OwS9aTE2Go4?si=wO37oIPBmoDl4Gez