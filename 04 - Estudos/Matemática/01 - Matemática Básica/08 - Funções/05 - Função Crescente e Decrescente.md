---
Title: Função Crescente/Decrescente
Data: 2025-10-06
tags:
  - Função
  - Estudos
  - Matemática
  - Matemática_Básica
  - Universo_Narrado
---
# $$\text{Introdução}$$
Agora que nós já entendemos o comportamento de uma função, é importante também entender algumas de suas classificações: as funções crescentes e descrentes. 

As funções crescentes, como o próprio nome já sugere, são as que, dado um valor $x$, a função $f(x)$ retorna um valor maior conforme $x$ aumenta.

As funções decrescentes, ao contrário das crescentes, são as que, dado um valor de $x$, a função $f(x)$ retorna um valor menor conforme $x$ aumenta.
# $$\text{Função Crescente}$$
Para começar a entender como uma função crescente funciona, vamos analisar um gráfico primeiro:

![[Função_Crescente_1|center|500]]

Neste caso, é possível observar que, conforme o $x$ aumenta, seu valor correspondente em $y$ também aumenta, e como a função $f(x)$ é igual ao $y$, então, supondo que você pegue dois valores $x_1$ e $x_2$, sendo que o valor $x_1$ é maior do que o $x_2$, a função de $f(x_1)$ também será maior do que a função de $f(x_2)$, pois o $x$ aumentou e, portanto, o $y$ também aumentou. Concluímos assim que esta é uma <u>função crescente</u>.

Podemos ver isso melhor abaixo:

![[Função_Crescente_2|center|800]]
 
Portanto, podemos definir a função crescente como sendo:

>[!Função Crescente]
>A função $f:A \rightarrow B$ (ou seja, a função que relaciona um valor do domínio $A$ com o contradomínio $B$) é crescente se, para todo $x_2$ e $x_1$ em $A$, com $x_1>x_2$, temos:
>$$f(x_1)>f(x_2)$$
# $$\text{Função Decrescente}$$
Agora, é intuitivo que a função decrescente será somente o inverso da função crescente. Vejamos o seguinte exemplo:

![[Função_Decrescente_1|center|500]]

Neste caso, nós podemos ver que, conforme o $x$ aumenta, o $y$ diminui, o que significa que essa é uma <u>função decrescente</u>. Nós podemos provar isso ao observar que, ao pegarmos dois valores aleatórios nessa função $x_1$ e $x_2$, tal que $x_1$ seja maior do que $x_2$, o valor de $y$ correspondente a $x_1$ será menor do que o valor de $y$ correspondente ao $x_2$, mesmo que $x_1$ seja maior do que $x_2$, o que indica que o $y$ diminuiu conforme o $x$ aumentou, e como $f(x)$ é igual a $y$, então $f(x_2)>f(x_1)$, ou ainda $f(x_1)<f(x_2)$. 

Podemos ver isso abaixo:

![[Função_Decrescente_2|center|800]]

Portanto, podemos definir que:

>[!Função decrescente]
>A função $f:A \rightarrow B$ (ou seja, a função que relaciona um valor do domínio $A$ com o contradomínio $B$) é decrescente se, para todo $x_1$ e $x_2$ em $A$, com $x_1>x_2$ temos: $$f(x_2)>f(x_1)$$ 

Então, em suma, vimos que:

- <u>Função Crescente</u>: conforme $x$ aumenta, o $y$ aumenta junto;
- <u>Função Decrescente</u>: conforme $x$ aumenta, o $y$ diminui.

--------------------------------------------------------------------------------------------
# $$\text{Exemplo}$$
Agora, vejamos um exemplo um tanto quanto especial:

![[Função_Crescente_Decrescente_1|center|800]]

>[!Observação]
>A figura acima não está proporcional e, se houver uma análise meticulosa, será percebido alguns erros nas informações que serão passadas e alguns casos reais. Sabendo disso, avalie as informações a seguir considerando o que ocorre em grande parte da função, desconsiderando comportamentos anômalos em determinadas regiões. 
>
>Não abordarei os erros no gráfico aqui, porém fica como exercício mental tentar encontrar e solucionar eles.

Neste caso, nós temos que entender como $f(x)$ varia conforme o $x$ muda em diferentes locais. Portanto, antes de concluirmos qualquer coisa, devemos quebrar o problema em partes inicialmente para que depois analisemos cada uma dessas partes. Então vamos determinar quais serão os locais a serem estudados para depois analisá-los separadamente:

![[Função_Crescente_Decrescente_2|center|800]]

Dessa forma, nós temos de analisar as seguintes partes de $x$: depois de $0$ mas antes de $3$; depois de $3$ mas antes de $7$; e, por último, depois de $7$.
#### Caso (a)
No caso **(a)** ($0 < x < 3$), nós vemos que, conforme o $x$ aumenta, o $y$ diminui, o que significa que, dados dois pontos $x_1$ e $x_2$ quaisquer neste intervalo, tal que $x_2$ seja maior do que $x_1$, nós veremos que o $y$ em $x_2$ será menor do que em $x_1$, o que significa que $f(x_1)>f(x_2)$ essa é uma <u>função decrescente</u>.
#### Caso (b)
No caso **(b)** ($3<x<7$), temos que, conforme o $x$ aumenta, o $y$ também aumenta, o que significa que, dados dois pontos $x_1$ e $x_2$ quaisquer neste intervalo, tal que $x_2$ seja maior do que $x_1$, nós veremos que o $y$ em $x_2$ será maior do que em $x_1$, o que significa que $f(x_2)>f(x_1)$ essa é uma <u>função crescente</u>.
#### Caso (c)
No caso **(c)** ($x>7$), temos que, conforme o $x$ aumenta, o $y$ diminui, sendo o mesmo do **Caso (a)**. Para evitar redundância, podemos somente concluir que $f(x_1)>f(x_2)$, sendo, portanto, uma <u>função decrescente</u>.

Assim, vimos que:
- $f_\text{a}: A\rightarrow B = \text{decrescente}\space |\space 0<x<3$;
- $f_\text{b}: A\rightarrow B = \text{crescente}\space |\space 3<x<7$;
- $f_\text{c}: A\rightarrow B = \text{decrescente}\space |\space x>7$.

![[Função_Crescente_Decrescente_3|center|800]]

Podemos concluir assim que, a depender do local onde você observa o problema, ele se comportará de uma determinada maneira. Newton, ao formular as derivadas e integrais (assunto que será abordado muito mais à frente), já trazia essa visão de que, antes de qualquer coisa ao abordarmos um problema, devemos quebrar ele em minúsculas partes para analisá-las individualmente, para posteriormente, sintetizar tudo em uma generalização. Somente assim se pode chegar ao verdadeiro e mais valioso conhecimento, aquele em quê se entende e não somente se memoriza.

--------------------------------------------------------------------------------------------

