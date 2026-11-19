---
Title: Noções e Proposições Primitivas de Geometria - FME9
Data: 2025-05-16
tags:
  - Geometria
  - Matemática
  - Estudos
---
# Postulados

> [!info] Postulado 1
> "Fique postulado traçar uma reta a partir de todo ponto até todo ponto."

Esse postulado diz basicamente que, dado dois pontos, eu posso traçar uma reta de um até o outro, como podemos ver nas figuras abaixo:

```tikz 
\begin{document} \begin{tikzpicture}[domain=0:4] \draw[very thin,color=gray] (-0.1,-1.1) grid (3.9,3.9); \draw[->] (-0.2,0) -- (4.2,0) node[right] {$x$}; \draw[->] (0,-1.2) -- (0,4.2) node[above] {$f(x)$}; \draw[color=red] plot (\x,\x) node[right] {$f(x) =x$}; \draw[color=blue] plot (\x,{sin(\x r)}) node[right] {$f(x) = \sin x$}; \draw[color=orange] plot (\x,{0.05*exp(\x)}) node[right] {$f(x) = \frac{1}{20} \mathrm e^x$}; \end{tikzpicture} \end{document} ```
```tikz
\begin{document}
\begin{tikzpicture}
  \draw [thick] (0,0) -- (3,2);
	  \filldraw (0,0) circle (2pt) node[anchor=north] {A};
	  \filldraw (3,2) circle (2pt) node[anchor=west] {B};
   \draw [thick] (4,0) -- (8,1);
	   \filldraw (4,0) circle (2pt) node[anchor=north] {x};
	   \filldraw (8,1) circle (2pt) node[anchor=west] {y};
\end{tikzpicture}
\end{document}
```

>[!info] Postulado 2
>"Também prolongar uma reta limitada, continuamente, sobre uma reta."

Isso é: dado uma reta qualquer, eu posso estender ela o quanto eu quiser.


```tikz
\begin{document}
\begin{tikzpicture}
	\draw [thick][<->] (-3,1) -- (7,1);
		\filldraw (0,1) circle (2pt) node[anchor=south] {A};
		\filldraw (4,1) circle (2pt) node[anchor=south] {B};
\end{tikzpicture}
\end{document}
``` 


>[!info] Postulado 3
>"E, com todo centro e distância, descrever um círculo."

Dado um ponto central e uma certa distância à esse ponto, você pode descrever diversos pontos que, a essa distância do centro, formam um círculo.

```tikz
\begin{document}
\begin{tikzpicture}

	\filldraw[thick] (0,1) circle (2pt) node[anchor=north] {a};
\end{tikzpicture}
\end{document}
```
