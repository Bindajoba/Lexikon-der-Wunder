# Definition
Sei $R$ ein [[Ring]]. Dann gibt es einen [[Erweiterungsring|Erweiterungsring]] $R[x] \supseteq R$ und ein Element $x \in R[x]$ mit der Eigenschaft, dass für jedes Element $f \in R[x] \backslash \{0_R\}$ ein eindeutig bestimmtes $n \in \mathbb{N}_0$ und eindeutig bestimmte $a_0, ..., a_n \in R$ existieren, so dass $a_n \neq 0$ ist und $f$ in der Form
$$f = a_nx^n + a_{n-1}x^{n-1}+...+a_1x+a_0$$
dargestellt werden kann.

*$x$ sollte nicht als beliebige Zahl aufgefasst werden. Es ist vielmehr irgendein formaler Ausdruck. Die Struktur der Polynome entsteht dadurch, dass Ringe über Addition und Multiplikation abgeschlossen sind.*

## Polynomring
Der Ring $R[x]$ wird Polynomring genannt. Dessen Elemente heißen [[Polynom (Komplexe Analysis)|Polynome]]

## Grad
Man bezeichnet die Zahl $n = grad(f)$ als Grad des Polynoms $f$

## Leitterm
Das Polynom $a_nx^n$ ist der Leitterm, das Element $a_n \in R$ der Leitkoeffizient.

# Eigenschaften
## Universelle Eigenschaft des Polynomsrings
Für jeden [[Ringhomomorphismus]] $\phi: R \to S$ und jedes $a \in S$ gibt es einen eindeutig bestimmten Ringhomorphismus $\hat \phi: R[x] \to S$ mit $\hat|_R = \phi$ und $\hat \phi(x) = a$

*Bedeutet das, dass man $a$ in $x$ einsetzt? Ja, so in der Art.*

## Eindeutigkeit
Je zwei Polynomring über einem Ring $R$ sind bis auf Isomorphie gleich.

## Proposition
Sei $R$ ein Ring und $R[x]$ ein Polynomring über $R$

Sind $0_R \neq f,g \in R[x]$ und gilt auch $f+g \neq 0_R$, dann folgt 
$$grad(f+g) \leq \max\{grad(f), grad(g)\}$$
und 
$$grad(fg) \leq grad(f)+grad(g)$$

Ist $R$ ein Integritätsbereich, dann gilt dasselbe auch für den Ring $R[x]$. In diesem Fall gilt sogar $grad(fg) = grad(f) + grad(g)$ für alle $f, g \neq 0_R$[^1]

## Gleiche Einheitengruppe wie bei Grundmenge
Sei $R$ ein [[Integritätsbereich]]. Dann gilt $R[x]^\times = R^\times$, d.h. die [[Einheitengruppe]] des Polynomrings $R[x]$ stimmt mit der Einheitengruppe des Grundrings $R$ überein.[^2]




#Zahlentheorie 

[^1]: Gerkmann - Proposition 4.6
[^2]: Gerkmann - Folgerung 4.8