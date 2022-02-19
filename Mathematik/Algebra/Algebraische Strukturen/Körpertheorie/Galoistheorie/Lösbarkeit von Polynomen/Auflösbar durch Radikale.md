TARGET DECK: Universität::Mathematik::Algebra


$\newcommand{\Q}{\mathbb Q}$
$\newcommand{\R}{\mathbb R}$
$\newcommand{\C}{\mathbb C}$
$\newcommand{\F}{\mathbb F}$
$\newcommand{\Z}{\mathbb Z}$
$\newcommand{\a}{\alpha}$


# Beschreibung
Wann lassen sich Nullstellen eines [[Polynom (Ring, Körper)|Polynoms]] durch einen Term angeben, der nur Addition, Subtraktion, Multiplikation Division und das Ziehen von Wurzeln enthält?
Das soll hier beantwortet werden.

# Antwort
## Darstellbarkeit der Nullstellen
Ein Polynom heißt **durch Radikale auflösbar**, wenn jede Nullstelle durch Radikale darstellbar ist.
Eine Zahl $a$ wird in $\Q$ durch Radikale darstellbar genannt, wenn sie Teil einer endlichen Kette von [[Radikalerweiterung|Radikalerweiterungen]] ist:
$$\Q \subset K_1 \subset K_2 \subset ... \subset K_n$$
mit $q \in K_n$-

*Diese Kette gleicht sehr der Kette für [[Konstruierbare Zahlen]] und der [[Normalreihe]]*

## Darstellbarkeit mit Zerfällungskörper
Ein Polynom heißt durch **Radikale auflösbar**, wenn sein [[Zerfällungskörper]] $V$ durch eine endliche Reihe von Radikalerweiterungen dartellbar ist:
$$\Q \subset K_1 \subset K_2 \subset ... \subset K_n = V$$
## Endantwort
Ein Polynom ist durch Radikale auflösbar, wenn seine [[Galoisgruppe eines Polynoms|Galois-Gruppe]] [[Auflösbare Gruppe|auflösbar]] ist.

## Satz von Abel
Es gibt Polynome von Grad $\geq 5$, die nicht lösbar sind. 
Diese Polynome sind die Polynome mit Grad größer $5$ die die [[Symmetrische Gruppe]] als [[Galoisgruppe eines Polynoms|Galoisgruppe]] haben.

## Alle oder keine Nullstelle darstellbar.
Sei $f$ ein irreduzibles $\Q$-Polynom. Ist eine Nullstelle durch Radikale darstellbar, dann auch alle anderen 

# Aufgaben
## Symmetrische Gruppe
Finde ein [[Irreduzibles Polynom]] der Form $f(x) = x^5+ax+b$, welches nicht auflösbar ist.
$f$ ist nicht auflösbar, wenn seine Galoisgruppe $S_5$ ist. Das gilt, wenn $f$ drei reelle und zwei nicht-reelle Nullstellen hat.
Suche also mit GeoGebra nach Polynomen von Grad 5, die 3 einfache Nullstellen haben.
- Erste Beobachtung: $a$ muss negativ sein, sonst gibt es nur eine Nullstelle.
- $b=-1$ führt nur zu lösbaren Polynomen
- $b=-2$ genauso
- $f(x) = x^5-3x+1$ sieht gut aus. Es ist nicht in $\Q$ reduzibel. Wäre es reduzibel, dann müsste es die Nullstellen $1$ oder $-1$ haben.


#Hadlock 
[^1]: 