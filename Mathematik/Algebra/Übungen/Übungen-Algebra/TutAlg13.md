TARGET DECK: Universität::Mathematik::Algebra

$\newcommand{\Q}{\mathbb Q}$
$\newcommand{\R}{\mathbb R}$
$\newcommand{\C}{\mathbb C}$
$\newcommand{\F}{\mathbb F}$
$\newcommand{\Z}{\mathbb Z}$
$\newcommand{\a}{\alpha}$
![[blatt13.pdf]]

# Aufgabe 0
## a)
Erw. $L|K$ ist normal und separabel

## b)
Zwischen der Menge der Untergruppen von $Gal(L|K)$ und der Menge der Zwischenkörper von $L|K$.

## c)
Eine endliche sep. Erw. $L|K$ hat nur endlich viele Zwishcenkörper Zwischenkörper. Für endl. Galois-Erw. $L|K$ gilt $Gal(L|K) = [L:K]$

## d)
$K$-Autom. $\sigma$ sind durch die Bilder $\sigma(\a), \sigma(\beta), \sigma(\gamma)$ eindeutig festgelegt $\implies \sigma \in G=Gal(L|K)$ reicht diese Bilder anzugeben.

## e)
Nullst. auf Nullst.: $\sigma \in G$, dann kann $\sigma$ die Nst. $\a$ von $\mu_{K, \a}$ nur auf eine Nst. von $\mu_{K, \a}$. Das Polynom $\mu_{K, \a}$ hat nur endlich viele Nullstellen also gibt es nur endlich viele Möglichkeiten für das Bild.

# Aufgabe 1
![[blatt13.pdf]]

## a)
$\zeta$ ist aus der Einheitengruppe und hat Ordnung $5$. D.h. $\zeta^5 = 1$. Damit ist $\zeta$ eine Nullstelle von $f :=x^5 -  1= (x-1)(x^4+x^3+x^2+x^1+1)$

$g:=x^4+x^3+x^2+x^1+1$ ist ein normiertes Polynom von Grad $4$ mit $\zeta$ als Nullstelle und ist damit sein Minimalpolynom.

Durch Potenzieren von $\zeta$ erhalten wir $3$ neue Elemente: $1, \zeta, \zeta^2, \zeta^3, \zeta^4$ sind eine Basis von $K$ als $\Q$-Vektorraum und sind damit Linear unabhängig. Desweiteren sind sie eine Nullstelle $f$, wie man durch einsetzen und feststellt.
Damit liegen alle $5$ Nullstellen von $f$ in $K$.

Wir haben $\zeta$ als beliebige Nullstelle von $x^4+x^3+x^2+x^1+1$ definiert. Obere Eigenschaft gilt damit auch für die anderen Nullstellen $\zeta^2, \zeta^3,  \zeta^4$.

Durch Adjunktion von einer Nullstelle sind damit auch alle anderen Nullstellen Teil der Körpererweiterung, d.h. $f$ ist separabel. $\Q$ hat Charakteristik $0$ und ist damit normal.

## b)
$\Q$-Homomorphismen sind durch die Bilder der Erzeuger eindeutig definiert. $K$ entsteht durch Adjunktion von $\zeta$.
Wegen Nst. auf Nst. muss $\zeta$ auf eine andere Nullstelle des Minimalpolynoms $g$ abbilden.
Für jedes Bild gibt es einen eindeutigen $K$-Homomorphismus. Dieser Homomorphismus bildet von $K$ auf $K$ ab und ist damit auch ein Automorphismus.
Es gibt also $4$ $\Q$-Automorphismen.

## d)
- $\sigma_1(\zeta) := \zeta$
- $\sigma_2(\zeta) = \zeta^2$
- $\sigma_3(\zeta) = \zeta^3$
- $\sigma_4(\zeta) = \zeta^4$

| $\circ$    | $\sigma_1$ | $\sigma_2$ | $\sigma_3$ | $\sigma_4$ |
| ---------- | ---------- | ---------- | ---------- | ---------- |
| $\sigma_1$ | $\sigma_1$ | $\sigma_2$ | $\sigma_3$ | $\sigma_4$ |
| $\sigma_2$ | $\sigma_2$ | $\sigma_4$ | $\sigma_1$ | $\sigma_1$ |
| $\sigma_3$ | $\sigma_3$ | $\sigma_1$ | $\sigma_4$ | $\sigma_2$ |
| $\sigma_4$ | $\sigma_4$ | $\sigma_3$ | $\sigma_2$ | $\sigma_1$ |

Die Tabelle sieht aus wie die von $\Z/4\Z$.

![[blatt13.pdf]]
# Aufgabe 2
## a)
Ist $M$ ein Zwischenkörper und $U = Gal(L|K)$ die zugehörige Untergruppe, dann gilt $[L:M] = |U|$ und $[M:K] = (G:U)$
Gesucht sind also Gruppen der Ordnung $2$, die Untergruppen von $\Z/4\Z \times \Z/4\Z$
Siehe dazu unten. 

## b)
$\Z/4\Z \times \Z/2\Z$ hat Ordnung $4$ und damit die Möglichen Untergruppen der Ordnung $1, 2, 4, 8$.
Gebe alle Untergruppen an:
- $1:  \{(0, 0)\}$
- $8: \Z/4\Z \times \Z/2\Z$
- $2:$ ist eine Primzahl. Damit sind alle Gruppen dieser Ordnung zyklisch und werden nur durch ein Element erzeugt. Probiere alle Elemente durch und wir erhalten $(0, 1)$, $(2, 0)$ und $(2, 1)$.
- $4$: Die Einzigen Gruppen der Ordnung $4$ sind $\Z/4\Z$ und $\Z/2\Z \times \Z/2\Z$.
$\Z/4\Z$ ist zyklisch und wird durch ein Element erzeugt. Probieren aller Elemente ergibt $(0, 1), (0, 3), (1, 1), (1, 3)$. Entfernt man Gruppen, sodass keine gleiche Untergruppe doppelt erzeugt wird, erhält man. $(0, 1), (1, 1)$ 
- $\Z/2\Z \times \Z/2\Z$ wird durch zwei Elemente der Ordnung $2$ erzeugt, sofern sie sich nur im neutralen Element $(0, 0)$ schneiden. Zwei Untergruppen der Ordnung 2, die durch unterschiedliche Elemente erzeugt werden, schneiden sich immer im Neutralelement, da es nur ein Element gibt, aus dem sie erzeugt werden können. Durch Kombination der oberen drei Elemente von Ordnung $2$ erhält man $3$ Untergruppen. Diese drei Untergruppen sind aber gleich, nämlich $(0, 0), (2, 0), (0, 1), (2, 1)$. Also gibt es nur eine soche Untergruppe. 





#Algebra 


