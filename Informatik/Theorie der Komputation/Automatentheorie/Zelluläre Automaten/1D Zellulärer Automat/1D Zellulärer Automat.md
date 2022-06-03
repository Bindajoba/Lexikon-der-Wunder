# Beschreibung
Ein [[Zellulärer Automat]] wird **1D-Zellulärer Automat** genannt, wenn jeder Knoten des Graphen zwei Nachbarn hat.

# Definition
Ein [[Zellulärer Automat]] wird **1D-Zellulärer Automat** genannt, wenn dessen [[Ungerichteter Graph]] [[Graphengrad]] $2$ besitzt.

Knoten werden so bezeichnet, dass jeder Knoten genau einen linken und einen rechten Nachbarn besitzt. Der Nachfolgezustand wird dann berechnet durch
$$x_{t+1}(v) = (x_t(u), x_t(v), x_t(w))$$
wobei $u$ der linke Nachbar von $v$ ist und $w$ der rechte Nachbar ist.

# Eigenschaften
## Isometrie des Graphen
Angenommen, der [[Graph|Graph]] ist zusammenhängend.
Der Graph besitzt sozusagen durch das weitergehen von einem Schritt nach rechts einen Erzeuger, mit dem alle Knoten besucht werden können. 
Man kann feststellen, dass das weitergehen von $n$ Schritten eine Gruppe bildet, die durch das gehen von einem Schritt erzeugt wird, was bedeutet, dass der Graph [[Gruppenisomorphismus|isomorph]] zum [[Cayley-Diagramm]] einer zyklischen Gruppe ist.

# Beispiel
## Endlicher Sierpinski 1D-Zellulärer Automat
Sei das Tupel $(G,f, x_S)$ gegeben durch:
![[Endlicher Sierpinski 1D-Zellulärer Automat.png]]
Dieser entwickelt sich wie folgt:
![[Entwicklung End Sierpinski 1D Zell Aut.png]]

## Unendlicher Sierpinski Automat
![[Unendlicher Sierpinski Automat.png]]

## Weitere Beispiele
![[1D Zellulärer Automat Beispiel 1.png]]





$\newcommand{\Q}{\mathbb Q}$
$\newcommand{\R}{\mathbb R}$
$\newcommand{\C}{\mathbb C}$
$\newcommand{\F}{\mathbb F}$
$\newcommand{\Z}{\mathbb Z}$
$\newcommand{\N}{\mathbb N}$
$\newcommand{\a}{\alpha}$

#Natural-Computing 
