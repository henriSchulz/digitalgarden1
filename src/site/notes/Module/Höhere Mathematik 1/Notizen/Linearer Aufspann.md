---
{"dg-publish":true,"permalink":"/module/hoehere-mathematik-1/notizen/linearer-aufspann/","tags":["Mathematik","Lineare-Algebra","HM1","gardenEntry","gardenEntry","gardenEntry","gardenEntry"]}
---


## Linearer Aufspann
Ist $M \subseteq V$ mit $M = \emptyset$, dann $\text{lin}(\textcolor{green}{ M }) = \{\underbrace{  \alpha_{1}  \cdot\vec{v_{1}} + \dots+ \alpha_{n}  \cdot\vec{v_{n}} ,\alpha_{1}, \dots, \alpha_{n} \in K, \vec{v_{1}},\dots,\vec{v_{n}} \in \textcolor{green}{ M } }_{ \text{Alle Linearkombinationen aller Vektoren von M} }\}$
$\text{lin}(\textcolor{green}{ M })$ (linearer Aufspann von $\textcolor{green}{ M }$) ist immer ein Unterraum von $V$

#### Illustration warum $\text{lin} \{ (1,1), (1,-1) \}$ ein Unterraum von $\mathbb{R}^2$ ist.

z.B.:
$$
\begin{array}
\vec{v_{1}} = \alpha_{1}(1,1) + \alpha_{2}(1,-1) \\
\vec{v_{2}} = \beta_{1}(1,1) + \beta_{2}(1,-1)
\end{array} \implies  \vec{v_{1}} + \vec{v_{2}} = (\alpha_{1} + \beta_{1})(1,1) + (\alpha_{2} + \beta_{2})(1,-1)
$$
#### Beispiel 2
Ist $M = \{ (1,1), (1,-1) \}$ dann $\text{lin}(M) = \mathbb{R}^2$
d.h.alle Vektoren in $\mathbb{R}^2$ sind Linearkombinationen von $(1,1), (1,-1)$

**Beweis**: Sei $(x,y) \in \mathbb{R}^2$. Wir suchen $\alpha_{1}, \alpha_{2}$ mit $(x,y) = \alpha_{1}(1,1) + \alpha_{2}(1,-1)$
$$
\Leftrightarrow (x,y) = (\alpha_{1},\alpha_{1}) + (\alpha_{2},-\alpha_{2}) \Leftrightarrow (x,y) = (\alpha_{1}+\alpha_{2}, \alpha_{1}-\alpha_{2}) \Leftrightarrow\begin{cases} 
\alpha_{1}+\alpha_{2} = x \;\;\;(1)\\
\alpha_{1}-\alpha_{2} = y \;\;\;(2)
\end{cases}
$$
$$
(1) + (2) \implies 2\alpha_{1} = x+y \implies \alpha_{1} = \frac{x+y}{2}
$$
$$
(1) - (2) \implies 2\alpha_{2}  = x-y \implies \alpha_{2} = \frac{x-y}{2}
$$
Also $(x,y) \in \text{lin}(M)$. Also $\mathbb{R}^2 \subseteq \text{lin}(M) \implies \text{lin}(M) = \mathbb{R}^2$
#### Beispiel 3
Sein $\vec{v_{1}} = \begin{pmatrix}1\\0\\1\end{pmatrix}$ und $\vec{v_{2}} = \begin{pmatrix}1\\1\\0\end{pmatrix}$, dann gilt
$$
\begin{pmatrix}2\\1\\1\end{pmatrix} = \vec{v_{1}} + \vec{v_{2}} \implies \begin{pmatrix}
2 \\
1 \\
1
\end{pmatrix} \in \text{lin} \{ \vec{v_{1}}, \vec{v_{2}} \}
$$
aber $\begin{pmatrix}1\\1\\1\end{pmatrix} \not\in \text{lin} \{ \vec{v_{1}}, \vec{v_{2}} \}$ sonst gäbe es $\alpha_{1}, \alpha_{2}$ mit $\begin{pmatrix}1\\1\\1\end{pmatrix} = \alpha \begin{pmatrix}1\\0\\0\end{pmatrix} + \alpha_{2} \begin{pmatrix}1\\1\\0\end{pmatrix}$

$$
\begin{pmatrix}1\\1\\1\end{pmatrix} = \begin{pmatrix}
\alpha_{1}+\alpha_{2} \\
\alpha_{2} \\
\alpha_{1}
\end{pmatrix} \implies \textcolor{red}{ \text{Wiederspruch} }
$$
Wenn $\vec{v} \neq 0$: Der lineare Aufspann ist die Gerade, die $\vec{v}$ bildet
Wenn $\vec{v}$ und $\vec{w}$ nicht parallel sind, ist der lineare Aufspann die Ebene, die $\vec{v}$ und $\vec{w}$ bilden