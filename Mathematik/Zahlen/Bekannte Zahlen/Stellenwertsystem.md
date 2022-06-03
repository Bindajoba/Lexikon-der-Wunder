TARGET DECK: Universität::Mathematik::Algebra

# Beschreibung
Ein Stellenwertsystem ist eine Möglichkeit, die [[Natürliche Zahlen]], [[Ganze Zahlen]], [[Rationale Zahlen]] oder [[Reelle Zahlen]] kompakt darzustellen.

# Übungen
## McEliece Übung 5-14
Stellt man $\frac{1}{7} = 0,14285714$ als Dezimalzahl dar, wiederholen sich die Nachkommastellen alle $6$ Ziffern. Bei $\frac{1}{11} = 0.090909$ wiederholen sich die Ziffern mit Periode $2$.

Zeige: Die Periode eines Bruches $\frac{k}{p}$, wobei $p$ eine [[Primzahl]] (außer $2$ und $5$) ist und $1 \leq k < p$ ist gleich der Ordnung von $10$ im [[Primer Restklassenring|Primen Restklassenring]] $\F_p$. Warum ist $5$ außergewöhnlich?

**Beweis:**
Ich denke mal, mit Ordnung ist die Ordnung in der [[Prime Restklassengruppe]] gemeint. Denn im normalen Primzahlkörper wäre die Ordnung für jede Zahl $\neq p$ gleich, was vermutlich bedeuten würde, das die Periode in jedem Stellenwertsystem gleich ist (das fühlt sich aber nicht richtig an).

Was ist die Ordnung von $10$ in $\F_7$?
- $10^1 = 3$
- $10^2 = 2$
- $10^3 = 6$
- $10^4 = 4$
- $10^5 = 5$
- $10^6 = 1$

Also ist die Ordnung von $10$ gleich $1$.
Das bedeutet, dass man $10$ mindestens $6$ mal mit sich selbst multiplizieren muss, um eine Zahl zu bekommen, die $\equiv 1\mod 7$ ist.
Das heißt $10^6 = 7q+1 \implies 10^6/7 = q\, R1 \implies \frac{1}{7} = 10^{-6}q + 10^{-6}\frac{1}{7}$

Wir verallgemeinern: Ist die Ordnung von $10$ in $\F_p$ gleich $n$, dann muss man $10$ mindestens $n$ mal mit sich selbst multiplizieren, um ein Ergebnis $\equiv_p 1$ zu bekommen.
Das heißt $10^n = pk+1 \implies 10^n/p = q + 1/p \implies \frac{1}{p} = 10^{-n}q + 10^{-n}\frac{1}{p}$

$5$ ist besonders, denn im Körper $\F_5$ wäre $10 = 0$. Es ist also egal, wie oft man es mit sich selbst multipliziert, man wird keine Zahl mit den Eigenschaften von oben Erhalten. Gleiches gilt auch für $2$.

$\newcommand{\Q}{\mathbb Q}$
$\newcommand{\R}{\mathbb R}$
$\newcommand{\C}{\mathbb C}$
$\newcommand{\F}{\mathbb F}$
$\newcommand{\Z}{\mathbb Z}$
$\newcommand{\N}{\mathbb N}$
$\newcommand{\a}{\alpha}$

#McEliece 


