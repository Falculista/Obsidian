---
Title: Limites
Data: 2025-07-09
tags:
  - Limites
  - Cálculo
  - Matemática
  - Estudos
---
# Definição Intuitiva
Vamos pegar um número $x$ | $x \neq 0$ e a função $f(x) = \frac{x+x³}{x}$ no gráfico abaixo:

![[f(x)=(x+x³)÷x |4000]]

Perceptivelmente, essa função possui uma intersecção em $1$. Agora perceba que, quanto mais próximo $x$ (eixo horizontal) estiver de $0$ (dizemos que x tende a zero), mais próximo o $y$ (eixo vertical) está de $1$ (dizemos que y tende a 1). Podemos ver isso na representação a seguir:

![[limite_intuição|4000]]
Matematicamente falando, dizemos que: Conforme $x \rightarrow 0$, $f(x) \rightarrow 1$ (mas que $x \neq 0$). Ou então, na notação que usaremos a partir de agora:
$$\lim_{x\to 0} f(x) = 1$$
E, de modo mais geral, definimos assim que:

![[Limite |center |800]]

#### Por que x ≠ a?
Consideramos $x \neq a$ pois, quando pegamos o limite daquela função, esperamos ver o que acontece conforme $x$ se aproxima de $a$, mas sempre sem chegar nesse valor.

Exemplo: dado uma função de $x$. Se $x \neq 0$,  $f(x) = \frac{x+x³}{x}$, mas se $x = 0$, $f(x) = 0$. Ou então:
$$f(x) = \left\{ \begin{array}{rc} \frac{x+x³}{x}| x\neq0 \\ 0|x=0  \end{array} \right.$$
O gráfico dessa função será dado por:

![[Limite no Gráfico|700 | center]]
 
 Portanto, para procurar o limite de $f(x)$ quando $x \rightarrow a$, $f$ não precisa sequer estar definida em $a$, mas apenas próximo desse valor: 
 ![[f próximo de a (Limites) |center|900]]
 Agora perceba também que, considerando um valor abaixo de $a$, estaremos diminuindo ele por algo, certo? Da mesma forma, quando consideramos um valor acima de $a$, estaremos aumentando ele. Agora, se essa diferença entre o valor aumentado e o valor diminuído for igual, isso significa que o valor usado para subtrair ou somar com $a$ é o mesmo. Definimos comumente esse valor como sendo o delta minúsculo (δ), uma letra grega muito utilizada em cálculo.
 
 Caso tenha ficado confuso, podemos ver isso usando o mesmo desenho utilizado acima:
 ![[f próximo de a 2 (Limites)|center|900]]
 Onde vemos uma parte (que é menor que $a$) sendo representado por $a - \delta$ e a outra (maior que $a$) como sendo $a + \delta$.

#### Exemplo
Dada a função:

![[Limite_Exemplo_1|center|900]]

Observamos que o gráfico está se direcionando para $0$ no eixo vertical e para $1$ no eixo horizontal, até que ele chega em $x = 1$, onde ocorre um "salto" de $y = 0$ para $y = 2$, e a partir daí o gráfico segue subindo.

O problema pede que nós avaliemos o limite de $f(x)$ para $x \rightarrow 1$, só que não é possível achar um limite único para esse caso pois haverá uma diferença entre o antes e o depois do salto ocorrer. Provaremos que isso é verdade fazendo o limite nos dois casos, ou seja, temos que ver o limite da função quando $x$ é menor que $1$ e quando $x$ for maior que 1. Começando com a parte de baixo:

![[Limite_Exemplo_1_Resolução_1|700|center]]

Nesse caso, considerando somente $x$ menor que 1, nós podemos ver que, conforme ele chega mais perto de 1, o valor de $y$ chega mais perto de $0$. Dessa forma, dizemos que o limite de $f(x)$ para $x$ tendendo a $1$, considerando somente os valores de $x$ abaixo de $1$, será igual a $0$, ou: $\lim_{x\to 1} f(x) = 0$.

O segundo passo agora é analisar o limite para os valores de $x$ maiores que $1$:

![[Limite_Exemplo_1_Resolução_2|700|center]]

Agora, para os valores de $x$ maiores que $1$, vemos que, conforme eles se aproximam de $1$, o valor de $y$ se aproxima de $2$. Dessa forma, pela mesma lógica utilizada no caso anterior, nós vimos que o limite de $f(x)$ para $x$ tendendo a 1, considerando somente os valores de $x$ maiores que $1$, será igual a 2, ou: $\lim_{x\to 1} f(x) = 2$.

Agora, sintetizando tudo, teremos que:

![[Limite_Exemplo_1_Resolução_Final|center|1000]]

Nesse caso, veja que não existe nenhum limite que satisfaça as duas condições ao mesmo tempo, pois em um caso será igual a $2$ e no outro igual a $0$. Logo, podemos afirmar que não existe $\lim_{x\to 1} f(x)$. 

Vimos então que, para o limite existir, não se pode existir dois limites ao mesmo tempo, o que ocorre caso haja algum "salto" em $y$ quando ele chega no ponto de referência, que nesse caso é o $1$, pois isso fará com que em dois casos o $f(x)$ dê valores diferentes (já que $f(x) = y$). Formalmente dizendo:

> [!info]
> Para que o limite $\lim_{x\to a}f(x)$ exista, ele não pode depender da maneira como $x$ se aproxima do ponto de referência ($a$), o que ocorrerá caso haja algum tipo de "salto" em $y$.

### Limites Laterais
O que nós fizemos de observar em cada caso o limite já foi realizar o chamado limite lateral, que é justamente sobre analisar o antes e o depois de $x$ chegar em um determinado ponto $a$. Existem então dois tipos de limites laterais:

- _**Limites à direita**_: $$\lim_{x\to a}f(x) = L$$se $f(x) \rightarrow L$ conforme $x \rightarrow a_{+}$.
  Basicamente, analisamos o limite de $f(x)$ para os casos em que $x$ tende a $a$ por valores maiores que ele. Foi o que nós fizemos quando analisamos o limite de $f(x)$ para os casos em que $x$ era maior que $1$, que naquele caso era o nosso $a$.
- _**Limites à esquerda**_: $$\lim_{x\to a} f(x) = L$$
  se $f(x) \rightarrow L$ conforme $x \rightarrow a_{-}$.
  Ao contrário do outro, nesse caso nós pegamos o limite de $f(x)$ para os casos em que $x$ tende a $a$ por valores menores que ele. Foi exatamente isso que fizemos quando analisamos o limite de $f(x)$ para os casos em que $x$ era menor que $1$ no exemplo anterior.

#### Exemplo
Dada a função:

![[Limite_Exemplo_2|center|700]]

Para calcularmos seu limite, devemos pegar o antes e o depois do salto no $y$ ocorrer. Ou seja, iremos aplicar os limites laterais.

Considerando um ponto Le (que será usado para abreviar limite à esquerda) no eixo $y$, o limite do lado esquerdo será dado usando os valores menos que $a$ (pois está do lado esquerdo a ele), representado então por $a_{-}$, como podemos ver a seguir:

![[Limite_Exemplo_2_Resolução_1 |center|800]]

E agora considerando um ponto Ld (de limite à direita) no eixo vertical, temos que o limite para o lado direito será dado usando os valores maiores que $a$ (pois estão a sua direita), representados por $a_{+}$:

![[Limite_Exemplo_2_Resolução_2|center|800]]

Concluindo assim dois limites, provando novamente que o limite depende da forma como você se aproxima do ponto $a$, e que portanto, para ter um limite bem definido, não pode haver diferença na forma como você se aproxima de $a$, seja pela direita ou pela esquerda. Dessa forma, para que haja um limite bem definido, é preciso que o limite do lado esquerdo seja igual ao do lado direito, pois isso significaria que não há diferença na forma como você se aproxima do ponto $a$. Matematicamente, definimos isso como sendo:

> [!Conclusão]
> $$\lim_{x\to a}f(x) = L \Leftrightarrow \lim_{x\to a_{-}}f(x)=\lim_{x\to a_{+}}f(x) = L$$

# Definição Formal
Há também, além da definição dada anteriormente que é mais intuitiva, uma mais formal, que será apresentada agora.

Antes de começarmos, é de extrema importância que nós entendemos o que significa a seguinte expressão: $|x-a|<k$. Que será explicada adiante.

Supondo que eu possuo um ponto $a$ em uma reta. Como já vimos anteriormente, esse ponto em si não nos interessa, somente nos é importante ver ao redor dele. Dessa forma, pegaremos dois outros pontos a uma distância $k$ de $a$ para usarmos como referência:

![[Limite_Definição_Formal_1|center|800]]

Agora, para que aquela desigualdade seja válida, se formos pegar qualquer ponto $x$ nessa reta, ele deverá estar contido nesse intervalo, pois se $|x-a| < k \implies -k < x - a < k$, logo, se somarmos $a$ dos dois lados, teremos que: $a-k<x<a+k$, provando que $x \in (a-k, a+k)$, como podemos ver a seguir:

![[Limite_Definição_Formal_2|center|800]]

Agora, indo para a definição de limites, ela será dada por:

> [!info] Definição de Limites
> Seja $f(x)$ definida num intervalo aberto contendo $a$. Podendo não estar definida em $a$. Temos: $$\lim_{x\to a}f(x)=L$$
> se para todo $\epsilon > 0$, $x\to a$ existir um $\delta >0$ tal que $|f(x)-L|<\epsilon$ sempre que $0<|x-a|<\delta$.

Confuso, não? Isso será facilmente entendido ao visualizarmos alguns gráficos:

![[Limite_Definição_Formal_3|center|600]]

Nesse caso, como podemos ver pelo ponto fechado na curva, o valor de $x=a$ está dentro da função.

Agora, aplicamos 