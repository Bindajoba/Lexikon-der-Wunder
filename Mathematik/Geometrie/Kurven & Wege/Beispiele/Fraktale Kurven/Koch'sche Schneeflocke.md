TARGET DECK: Universität::Mathematik::Geometrie

# Beschreibung
Eines der einfachsten Fraktale, um zu zeigen, dass [[Kurve|stetige Kurven]] [[Rektifizierbarkeit|nicht rektifizierbar]] sein können.


# Konstruktion
![Bild](https://upload.wikimedia.org/wikipedia/commons/thumb/6/6f/How_to_make_Koch_curve.svg/1050px-How_to_make_Koch_curve.svg.png)

![](https://upload.wikimedia.org/wikipedia/commons/b/b8/Kochkurve.png)

# Definition
Baue Kurve $f_1: [0, 1] \to \R$, sodass
- $f_0$ Gerade
- $f_i$ ist Geradesegment auf jedem Teilintervall $I = \eck{\frac{j}{q^i}, \frac{j+1}{q^i}}$ für alle $j \in \N$
- Um $f_{i+1}$ auf $f_{i}$ zu erhalten ersetzee in jede Teilintervall $I$ das Geradensegment $f|_I$ durch Verkettung $a \circ b \circ c \circ d$, wobei 
	- $a$ Anfangssegment von $f_{i}|_I$ der Länge $\frac{1}{3}l(f_i|_I)$
	- $d$ Endsegment von "-"
	- $b, c$ Seiten des gleichschenkligen Dreiecks mit Basis beim mittleren Drittel von $f_i|_I$


# Eigenschaften
Der Grenzwert der Konstruktion oben hat folgende Eigenschaften:

## Stetigkeit
Die Koch'sche Schneeflocke ist stetig, dass kann man mit dem $\delta$-$\varepsilon$-Kriterium prüfen.

## Nicht rektifizierbar
Die Länge der Flocke ist nicht rektifizierbar.

**Beweis Stetigkeit und Nichtrektifizierbarkeit:**
Wir beobachten:
1) $f_{i+1}\klam{\frac{j}{4^i}} = f_i\klam{\frac{j}{4^i}}$
   *Alte Ecken bleiben Ecken*
2) $\sum_{j=0}^{4^i-1}\|f_i\klam{\frac{j+1}{4^i}}-f_i\klam{\frac{j}{4^i}}\| = l(f_i)$
3) $l(f_i+1) = \frac{4}{3}l(f_i)$
4) $\|f_{i+1}(t)-f_i(t)\| \leq \frac{1}{3^{i+1}}l(f_0)$
   *Besagt durch Majorisierung, dass die $f_i(t)$ Cauchyfolgen sind. Also existiert für jedes $t$ der Grenzwert $\lim_{i \to \infty} f_i(t) = f(t)$*

Punkt 4) besagt sogar, dass $f_i(t)$ gleichmäßig konvergiert. (Die Geschwnidigkeit des Konvergierens hängt nicht von $t$ ab). Der Grenzwert eienr [[Gleichmäßige Konvergenz|gleichmäßig konvergierenden Folge]] von Stetigen Funktionen ist wieder stetig. 
Zusammen mit b) gilt:
$$l(f) \geq l(f_i) = \klam {\frac{4}{3}}^il(f_0)\, \forall i$$
$\implies l(f) = \infty$.



#Geometrie



$\newcommand{\eck}[1]{\left[ #1 \right]}$
$\newcommand{\ges}[1]{\left\{ #1 \right\}}$
$\newcommand{\wink}[1]{\left\langle #1 \right\rangle}$
$\newcommand{\klam}[1]{\left( #1 \right)}$
$\newcommand{\Q}{\mathbb Q}$
$\newcommand{\R}{\mathbb R}$
$\newcommand{\C}{\mathbb C}$
$\newcommand{\F}{\mathbb F}$
$\newcommand{\Z}{\mathbb Z}$
$\newcommand{\N}{\mathbb N}$
$\newcommand{\a}{\alpha}$


