TARGET DECK: Universität::Mathematik::Algebra

# Beschreibung
Das [[Kreisteilungspolynom]] ist in seinem normalen Umfeld, das heißt in $\R$ ein [[Irreduzibles Polynom]]. In [[Endlicher Körper|endlichen Körpern]] ist das aber nicht zwingend der Fall.

# Sätze
## Faktorisierung 1
Sei $f(x)$ ein normiertes Polynom von Grad $n$ mit Koeffizienten aus $\F_q$.
Sei $h(x)$ ein $\F_p$-Polynom mit der Eigenschaften $h(x)^q \equiv h(x) \mod f(x)$, dann lässt sich $f(x)$ folgendermaßen faktorisieren:
$$f(x) = \prod_{s \in \F_q}ggT(f(x), h(x)-s)$$[^1]
## Anzahl der Faktoren
Die Zahl der Faktoren ist gleich der Dimension von $R(f)$, wobei $R(f)$ der Vektorraum aller Polynome $h(x) \mod f$ mit der Eigenschaft $h^q \equiv h \mod f$.

Die [[Dimension (Vektorraum)]] berechnet man, indem man ein [[Gleichungssystem (Lineare Algebra)]] aufstellt, bei dem die Koeffizienten von $h$ die Unbekennten sind. Die Lösungen des Gleichungssystems sollen die Polynomkoeffizienten sein, sodass $h$ die obere Konguenz erfüllt. Dieses Gleichungssystem hat nach den Erkenntnissen der linearen Algebra einen Vektorraum als Lösungsraum. Das ist genau $R(f)$. Die Dimension eines Lösungsraumes zu bestimmen sollte nicht allzu schwer sein.[^2]

## Faktorisierung 2
Ein Polynom $h(x) = \sum_{i=0}^{n-1}h_ix^i \in \F_q[x]$ erfüllt die Kongruenz $h^q \equiv h \mod x^n-1$ genau dann, wenn alle Koeffizientenindizes eines $q$-[[Potenzenzykel]] den gleichen Wert haben, das heißt $h_i = h_{iq} = h_{iq^2} = ...$ gilt.

Da in $\F_q[x]$ Freshmans Dream gilt und $x^i \equiv x^j \mod x^n-1 \iff i \equiv j \mod n$ muss $h$ eine Linearkombination der Potenzenzykelpolynome der $q$-Potenzenzykel in $\Z/n\Z$ sein
Ein Potenzzykelpolynom ist ein Polynom mit der Form:
$$x^{a}+ x^{aq}+x^{aq^2}+...$$
(Man erkennt durch Anwendung von Freshmans Dream, das das Polynom $h^3 \equiv h \mod x^n-1$ erfüllt)

# Beispiele
## Potenzzykelpolynome $\mod x^{20}-1$ 
Jedes Polynom $h$ mit der Eigenschaft $h^3\equiv h \mod x^{20}-1$ ist eine Linearkombination der Polyome:
- $1$
- $x+x^3+x^7+x^9$
- $x^2+x^6+x^{18}+x^{14}$
- $x^4+x^{12}+x^{16}+x^8$
- $x^5+x^{15}$
- $x^{10}$
- $x^{11}+x^{13}+x^{17}+x^{19}$


# Übungen
## McEiliece Übung 7-4
Faktorisiere die folgenden Kreisteilungspolynome in den endlichen Körpern:
- $\Phi_{17}(x)$ über $GF(2)$
- $\Phi_{11}(x)$ über $GF(3)$
  $\Phi_{11}(x) = (x^5+x^4-x^3+x^2-1)(x^5-x^3+x^2-x-1)$
- $\Phi_{13}(x)$ über $GF(5)$
  $\Phi_{15}(x) = (x^4+3x^3+3x+1)(x^4+x^3+4x^2+x+1)(x^4+2x^3+x^2+2x+1)$
- $\Phi_{19}(x)$ über $GF(7)$
  $\Phi_{19}(x) = (x^3+3x^2+3x+6)(x^4+4x^2+4x+6)(3x^3+4x^2+2x+4)$$(4x^3+2x^3+3x+3)(x^3+5x^2+6)(3x^3+6x+4)$[^3]

## McEliece Übung 7-7
Faktorisiere $x^{16}-x$ über folgende Körper:
- $\F_{16}$
  Das sind genau die Elemente des oberen Körpers, das Polynom zerfällt also in Linearfaktoren
- $\F_{2}$
  Das sind genau die Elemente des Körpers $\F_{16}$. Das Polynom zerfällt daher in die Minimalpolynome dieser Elemente, die ich zufällig bereits berechnet habe.
  $x^{16}-x = x(x-1)(x^2+x+1)(x^4+x+1)(x^4+x^3+1)(x^4+x^3+x^2+x+1)$
- $\F_{4}$
  Zufälligerweise habe ich das auch schon in [[Algebraischer Abschluss von F2]] berechnet. Das sind einfach die Polynome von oben aber die Polynome von Grad $2$ und $4$ zerfallen noch weiter.





$\newcommand{\Q}{\mathbb Q}$
$\newcommand{\R}{\mathbb R}$
$\newcommand{\C}{\mathbb C}$
$\newcommand{\F}{\mathbb F}$
$\newcommand{\Z}{\mathbb Z}$
$\newcommand{\N}{\mathbb N}$
$\newcommand{\a}{\alpha}$

#McEliece 


[^1]: McEliece - Theorem 7.3
[^2]: McEilece - Theorem 7.4
[^3]: [[Lexikon SemIV#1]]