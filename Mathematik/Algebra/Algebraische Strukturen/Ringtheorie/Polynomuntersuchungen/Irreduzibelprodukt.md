TARGET DECK: Universität::Mathematik::Algebra

# Beschreibung
Ein Irreduzibelprodukt $n$-ten Grades beschreibt das Polynom, dass man durch das Produkt aller [[Irreduzibles Polynom|Irreduziblen Polynome]] $n$-ten Grades erhält.

# Definition
Sei $K$ ein [[Endlicher Körper]] (oder vielleicht sogar etwas allgemeineres).
Das Produkt aller in $K$ irreduziblen Polynome $n$-ten Grades wird mit $V_n$ bezeichnet.

# Eigenschaften
## Spezielle Eigenschaft bei endlichen Körpern
Es gilt die Eigenschaft:
$$x^{q^n}-x = \prod_{d \mid n}V_d(x)$$
**Beweis:**
Nach Übungsaufgabe, ist $x^{q^n}-x$ das Produkt aller irreduziblen Polynome, deren Grad $n$ teilt. Das Produkt aller Polynome vom Grad $d$ werden in $V_d(x)$ zusammengefasst, wodurch obere Gleichungs selbstverständlich ist.

## Berechnung
Man kann sich die obere Gleichung mit dem [[Möbiusscher Umkehrsatz]] zu nutze machen und eine Formel für die Berechnung von $V_d(x)$ erhalten, nämlich:
$$V_n(x) = \prod_{d \mid n} (x^{q^d}-x)^{\mu(n/d)}$$
**Beweis:**
$x^{q^n}-x = \prod_{d \mid n}V_d(x)$ ist die [[Summatorische Funktion]] von $V_d(x)$, das Additionssymbol wurde aber durch ein Produktsymbol ersetzt. Durch den Umkehrsatz erhalten wir die obere Formel.

$\newcommand{\Q}{\mathbb Q}$
$\newcommand{\R}{\mathbb R}$
$\newcommand{\C}{\mathbb C}$
$\newcommand{\F}{\mathbb F}$
$\newcommand{\Z}{\mathbb Z}$
$\newcommand{\N}{\mathbb N}$
$\newcommand{\a}{\alpha}$

#McEliece 


