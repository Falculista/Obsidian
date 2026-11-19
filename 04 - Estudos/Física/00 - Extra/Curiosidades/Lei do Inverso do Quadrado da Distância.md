---
Title: Lei do Inverso do Quadrado da Distância
Data: 2025-04-25
tags:
  - Curiosidades
  - Estudos
  - Física
  - Matemática
---
Falar sobre:
- Dispersão Infinita de raios;
- Infinitos de Cantor;
- Criação dos Infinitesimais (?);
# Conceito

É muito comum em algumas fórmulas na física nos depararmos com algo do tipo:
$$ intensidade \propto \frac{1}{d^2}$$
Como a Lei da Gravitação Universal, por exemplo, que decai com o quadrado da distância de dois objetos:
$$F = G\frac{M_{1}M_{2}}{R^2}$$
Ou então na Lei de Coulomb:
$$F=K\frac{q_{1}q_{2}}{r^2}$$
Todas essas forças decaem com o quadrado da distância entre dois objetos. Agora, por quê isso acontece?

Imagine que estamos segurando uma lanterna, que, por sua vez, libera diversos feixes de luz quando ligada. Agora, imagine que colocamos uma placa metálica de área $a²$ em sua frente, a uma distancia $r$. Esta placa, por sua vez, irá "detectar" uma quantidade $n$ de feixes de luz.

Agora imaginemos que, a uma distância de $2r$ (dobro da distância da placa anterior até a lanterna) nós queiramos colocar uma placa metálica de tamanho b² tal que ela também detecte os mesmos $n$ feixes de luz percebidas pela primeira. Para que isso ocorra, b² deverá ser igual à $4\cdot a²$, portanto: $b²=4a²$.

Se continuarmos colocando placas metálicas à distâncias múltiplas de $r$, veremos que a área das placas terá uma sequência igual ao quadrado dos números naturais.

Para facilitar o entendimento, visualize a imagem à seguir:

![[Lei-do-Inverso-do-Quadrado-da-Distância.png]]

Ela nos mostra justamente o que comentamos anteriormente.

Todos os quadrados que foram formados detectam a mesma quantidade de feixes de luz, mas cada um deles as percebe em intensidades diferentes, pois os feixes se distanciaram uns dos outros, fazendo com que eles fiquem mais espalhados conforme a distância dos quadrados até a fonte aumenta. Cada quadrado, aliás, é representado usando como base o primeiro quadrado mais perto de $S$.

Dessa forma, nós "quantizamos" as forças da natureza. É como se cada quadrado de lado $a$ usado fosse uma "área fundamental" usado na sequência.

Isso nos mostra que a intensidade de quaisquer feixes propagados diminui conforme nos afastamos da fonte. 

Podemos simplificar toda essa questão para o seguinte:

Quando colocamos nossas mãos na frente de uma lanterna, vamos perceber um círculo não muito grande mas com bastante luminosidade referente a quantidade de luz emitida por ela, mas quando apontarmos a mesma lanterna para uma parede mais distante, perceberemos que a luz formará um círculo muito maior, porém será menos luminosa. Um ponto importante a se destacar antes de continuarmos é que, tanto a sua mão quanto a parede receberam a mesma quantidade de luz advinda da lanterna (desconsiderando alguns raios que foram propagados ao redor).

Isso acontece pois, ao afastar o receptor (como sua mão ou a parede) do emissor (nesse caso a lanterna), por mais que a quantidade de luz seja a mesma, a **intensidade** dela será menor. Isso é, sua densidade será muito menor, portanto os raios estarão mais distantes uns dos outros devido a suas inclinações em relação aos outros, que fez com que eles se afastassem cada vez mais.

## A fábula da pistola de manteiga

Suponha que um restaurante tenha o problema de passar manteiga em torradas. Eles querem ser muito modernos e querem passar a manteiga na torrada com uma máquina. O dono do restaurante inventa uma Pistola de Manteiga, com manteiga derretida no cabo, a qual pode ser esguichada em linhas retas.

Aqui está um pedaço de torrada, e as linhas de manteiga saem da arma e a atingem por inteiro.

![](https://cdn.kastatic.org/ka-perseus-images/93ab73645fabee343755051c8bd50eb659623df3.svg)

Agora, ao invés de uma torrada, as linhas de manteiga podem continuar e você pode posicionar a torrada mais para trás, com o _dobro_ da distância. Dois pedaços de torrada de largura e dois de altura.

![](https://cdn.kastatic.org/ka-perseus-images/b9285c665b814cd7448073409084e2a1e1de15f5.svg)

Juntos, são quatro pedaços de torrada para interceptar a manteiga. A manteiga será _um quarto_ menos espessa. Esta é a lei do inverso do quadrado (de amanteigamento).

Estendendo a ideia: no triplo da distância, você pode organizar $3$ torradas por $3$ torradas para caber dentro das linhas de pulverização, para um total de $9$ torradas, e você vai obter $\frac{1}{9}$ da espessura de manteiga, para um tratamento "econômico".

A lenda da Pistola de Manteiga foi inspirada por este maravilhoso vídeo de 3 minutos do professor de Física da Universidade de Princeton, Eric Rogers, em 1959.
https://youtu.be/HpipBkRMm8U

# A Dispersão (quase) Infinita de raios

Pensemos agora no seguinte: quando um objeto emite milhares - consideraremos aqui como sendo praticamente infinitos - de fótons, a diferença da quantidade total de fótons emitidos para as detectadas em cada quadradinho ainda seria relevante. Isso pode, aliás, ser entendido pelo mesmo conceito que rege [[Os Infinitos de Cantor]]. Cada quadradinho percebe um número $n$ que, de forma leiga, poderia até mesmo ser considerado infinito. Porém, conforme as distâncias aumentam e as dispersões vão aumentando, por mais que os quadradinhos continuem percebendo uma quantidade muito grande de fótons, essa quantidade foi reduzidas inúmeras vezes, o que faz com que os valores percebidos pelos quadradinhos $a$ ao longo da sequência vá diminuindo significativamente. 