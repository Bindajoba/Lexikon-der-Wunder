# Definition
Sei $R$ ein Ring mit $a_1, ..., a_n \in R$. Wir sagen, ein Element $d \in R$ ist ein größter gemeinsamer Teiler (kurz ggT) von $a_1, ..., a_n$, wenn gilt
1. $d \mid a_i$ für $1 \leq i \leq n$
2. Ist $b \in R$ mit $b|a_i$ für $1 \leq i \leq n$, dann folgt $b \mid d$


# Charakterisierung

# Eigenschaften
## Reduktionsschritt
Sei $R$ ein Ring und seien $a, b, q \in R$ mit $b \neq 0$. Dann gilt die Gleichung $ggT(a, b) = ggT(a-qb, b)$

## ggT und Assoziierte Elemente
Sei $R$ ein [[Ring]] und $d \in R$ ein größter Gemeinsamer Teiler der Ringelemente $a_1, ..., a_n$. Ein weiteres Element $d' \in R$ ist genau dann ein ggT von $a_1, ..., a_n$, wenn $d$ und $d'$ zueinander assoziiert sind. Dieselbe Aussage gilt auch für das [[Kleinstes Gemeinsames Vielfaches]]



# Spezialfälle
## Natürliche Zahlen
Siehe [[Größter gemeinsamer Teiler (Natürliche Zahlen)]].

## Potenzen-1
Sei $t \in R$ und $m ,n \in \N$, dann gilt:
$$ggT(t^n-1, t^m-1) = t^{ggT(n, m)}-1$$
*Dieses Satz gibt eine Möglichkeit für spezielle große Zahlen den ggT schnell zu berechnen.*

# Übungen
## McEliece Korrolar 2.4
Zeige
$$ggT(x^{q^n}-1, x^{q^d}-x) = x^{q^{ggT(n, d)}}$$
**Beweis**:
$$\begin{align} ggT(x^{q^n}-1, x^{q^d}-x) = x^{q^{ggT(n, d)}} &= x\cdot ggT(x^{q^n-1}-1, x^{q^d-1}-1) \\ 
&= x\cdot (x^{ggT(q^n-1, q^d-1)}-1) \\
&= x\cdot (x^{q^{ggT(d, n)}-1}-1) \\
&= x^{q^{ggT(d, n)}}-x\end{align}$$
Was zu zeigen war.

$\newcommand{\Q}{\mathbb Q}$
$\newcommand{\R}{\mathbb R}$
$\newcommand{\C}{\mathbb C}$
$\newcommand{\F}{\mathbb F}$
$\newcommand{\Z}{\mathbb Z}$
$\newcommand{\N}{\mathbb N}$
$\newcommand{\a}{\alpha}$

#McEliece 
