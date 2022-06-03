TARGET DECK: Universität::Mathematik::Algebra

# Beschreibung
Eine einfache Radikale Erweiterung ist eine [[Radikalerweiterung]], die nur durch eine Element erzeugt wird. (Es darf also kein Turm sein.)

# Eigenschaften
## Bedingungen für Isomorpie
Sei $n \in \N$ mit $n \geq 2$ und $K = K'(\zeta_n)$ ein Körper mit $char(K) \nmid n$.
Wir setzen voraus, dass $K$ eine primitive $n$- te [[Primitive Einheitswurzel|Einheitswurzel]] $\zeta_n$ enthält.

Sei $\alpha \in L$ eine n-te Wurzel von $a = \alpha^n \in K^\times$. 
Dann gilt:
- Die Erweiterung $K(\alpha)|K$ ist eine [[Galois-Erweiterung]]
- $Gal(K(\alpha)|K) \cong \Z/d\Z$, wobei $d$ ein Teiler von $n$ ist
- Es gilt $G \cong \Z/N\Z$ genau dann, wenn $f = x^n-a$ über $K$ [[Irreduzibles Polynom|irreduzibel]] ist

# Übungen
## Checkliste Gerkmann
### Aufgabe 1
Wieviele Untergruppen hat die Galoisgruppe der Erweiterung $\Q(\sqrt[8]2, \zeta_{8})|\Q$, wobei $\zeta_8$ eine primitive $8$-te Einheitswurzel ist.

$\Q(\zeta_8)$ ist ein Körper, der die achte Einheitswurzel enthält. Demzufolge gilt der Satz oben und $Gal(\Q(\sqrt[8]2, \zeta_{8})|\Q(\zeta_8)) \cong \Z/d\Z$ mit $d \in \{1, 2, 4, 8\}$
Ich denke aber, dass $x^8-2$ irreduzibel über $\Q(\zeta_8)$ ist.

$x^8-2 = (x-\sqrt[8]2)(x-\zeta_8\sqrt[8]2)(x-\zeta_8^2\sqrt[8]2)(x-\zeta_8^3\sqrt[8]2)...$
Eine beliebiges Produkt dieser Linearfaktoren hätte den Konstanten Term $\zeta_8^n\sqrt[8]2^m$, wobei $m$ die Anzahl der Linearen Faktoren ist, die man zusammenmultipliziert hat.
Angenommen $x^8-2$ ist reduzibel, dann muss ein Produkt von ( nicht allen) Linearfaktoren ein $\Q(\zeta_8)[x]$ Polynom sein. Das bedeutet, dass es ein $n \in \N$ und $m \in \{1, ..., 7\}$ gibt, sodass $\zeta_8^n\sqrt[8]2^m \in \Q(\zeta_8)$.
Das gilt genau dann, wenn $\zeta_8^n\sqrt[8]2 / \zeta_8^n \in \sqrt[8]2^m \in \Q(\zeta_8)$.
Ich glaube aber $\sqrt 2 \in \Q(\zeta_8)$ da $\sqrt 2 = \zeta_8 + \zeta_8^7$.
$$x^8-2 = (x^4+\sqrt 2)(x^4-\sqrt 2)$$
$x^8-2$ ist also gar nicht das Minimalpolynom von $\sqrt[8]2$, $x^4-\sqrt 2$ ist kleiner!




$\newcommand{\Q}{\mathbb Q}$
$\newcommand{\R}{\mathbb R}$
$\newcommand{\C}{\mathbb C}$
$\newcommand{\F}{\mathbb F}$
$\newcommand{\Z}{\mathbb Z}$
$\newcommand{\N}{\mathbb N}$
$\newcommand{\a}{\alpha}$

#Algebra 


