TARGET DECK: Universität::Mathematik::Algebra

# Beschreibung


# Definition
Eine [[Isometrie]] der [[Euklidische Geometrie]] wird **Isometrie des euklidischen Raumes genannt**.




# Eigenschaften
## Charakterisierung
Jede Isometrie auf $\R^n$ ist affin, d.h. sie hat die Form
$$F(x) = Ax+p$$
für eine [[Orthogonale Matrix]] $A$ und ein $p \in \R^n$

Isometrien auf $R^2$ ([[Euklidische Geometrie]]) lassen sich wie folgt klassifizieren
1) **Verschiebungen**
   Abbildungen, die Punkte verschieben $F: \R^2 \to R^2, x \mapsto x+p$
   *Aber eine Verschiebung in der Paris-Metrik ist im allgemeinen keine Isometrie*
2) **Lineare Isometrien**
  Abbildungen der Form $F: \R^2 \to \R^2, x \mapsto Ax$
  Für eine Matrix $A$ mit $A^TA = id$ 


## Erhaltung paarweise Abstände impliziert eine Isometrie
Seien $p_1, ..., p_n$ und $q_1, ..., q_n$ Punkte in $\R^n$
Falls $d(p_i, p_j) = d(q_i, q_j)$ für alle $i, j$ dann gibt es eine Isometrie $\phi$ sodass $\phi(p_i)=q_i$


## Differenzierbarkeit
Jede Isometrie des euklidischen Raumes ist [[Differenzierbarkeit|differenzierbar]] mit der [[Jacobi-Matrix]] $A$.



## Verkettung von Spiegelungen
Seien $p_1, ..., p_k$ und $q_1, ..., q_k$ Punkte im $\R^n$ mit $d(p_i, p_j) = d(q_i, q_j)$ für alle $i, j = 1, ..., k$
Dann gibt es [[Hyperebene|Hyperebenen]] $H_1, ..., H_l, l \leq k$ sodass für $\phi := \nu_{H_1}\circ...\circ \nu_{H_l}$ gilt:
$$\phi(p_i) = q_i \forall i$$
Mit ausreichend Punkten ($n+1$) ist damit eine Isometrie eindeutig festgelegt. Das $\phi$, als Verkettung von Spiegelungen muss dann auch diese Isometrie sein.
Jede Isometrie des $\R^n$ it daher Produkt aus $\leq n+1$ Spiegelungen an Hyperebenen.

## Gruppenform
Die Menge von normalen isomorphismen bildet bereits eine Gruppe.
Da alle **Isometrien der Euklidischen Geometrie** die Form $Ax+p$ haben gilt für zwei Abbildungen: $\varphi(x) = Ax+p, \psi(x)=Bx+q$
$$\varphi \circ \psi = A(Bx+q)+p = ABx+(Ap+q)$$
Schreibt men die Funktionen in abstrakter Form erhält man
$$(A, p) \cdot (B, q) = (AB, Ap+q)$$
Das ist ein spezielles [[Semidirektes Produkt]]

Da jede Isometrie eine Verkettung von Spiegelungen ist, ist diese Gruppe aus Elementen der Ordnung $2$ erzeugt.

# Sonstiges
## Ausrichtung eines Normalvektor
Falls $v \in R^n$ ein [[Einheitsvektor]] ist, dann gibt es [[Orthogonale Matrix|orthogonales]] $A$ (d.h. $A^TA = Id$), sodass $Av = e_1$
Bildlich gibt es eine rotation, mit der ein Einheitsvektor, auf $e_1$ rotiert wird.

## Ausrichtung eines Gerade
Für jede [[(Affine) Gerade (Geometrie)]] $G$ gibt es eine Isometrie $F: \R^2 \to \R^2$, sodass $F(G)$ die erste Koordinatenachse ist, d.h $F(G) = \{(x,0, x \in \R)\}$

Das heißt, bis auf Isometrie gibt es nur eine Gerade.

# Beispiele
## Spiegelung an einer Hyperebene
Eine [[Hyperebene]] 









$\newcommand{\Q}{\mathbb Q}$
$\newcommand{\R}{\mathbb R}$
$\newcommand{\C}{\mathbb C}$
$\newcommand{\F}{\mathbb F}$
$\newcommand{\Z}{\mathbb Z}$
$\newcommand{\N}{\mathbb N}$
$\newcommand{\a}{\alpha}$

#Geometrie



