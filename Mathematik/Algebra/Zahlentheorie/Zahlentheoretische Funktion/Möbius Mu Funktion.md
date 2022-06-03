TARGET DECK: Universität::Mathematik::Algebra

# Beschreibung
Die Möbius Mu Funktion ist eine spezielle [[Multiplikative Zahlentheoretische Funktion]].

# Definition
Sei $n = p_1^{e_1}...p_m^{e_m}$ eine natürliche Zahl in Primzaktorenzerlegung.
Dann ist die Möbius $\mu$-Funktion wie folgt definiert:
$$\mu(n) = \begin{cases}0, &\text{wenn } n \text{ nicht quadratfrei} \\
					(-1)^m &\text{wenn } n \end{cases}$$
*Das sieht verdächtig nach dem [[Quadratisches Reziprozitätsgesetz]], bzw. das [[Legendre-Symbol]].*
Siehe [[Quadratfreie Zahl]]
# Eigenschaften
## Summatorische Funktion
Die [[Summatorische Funktion]] ist:
$$\sum_{d \mid n}\mu(d) = \begin{cases} 1 &\text{ für }n=1, \\ 0 &\text{ sonst}\end{cases}$$


## McEliece 6-4
Zeige:
$$\sum_{d^2 \mid n}\mu(d) = |\mu(n)|$$
Führe eine Fallunterscheidung durch je nachdem, ob $n$ Quadratfrei ist oder nicht.
- $n$ ist quadratfrei.
  Dann ist $\sum_{d^2\mid n}\mu(d) = \mu(1) = 1$
  Außerdem isr $\mu(n) =  \pm 1$
- $n$ ist nicht quadratfrei
  Dann ist $\mu(n) = 0$ und alle Quadrate, die $n$ teilen lassen sich als Produkt von Primzahlquadratpotenzen schreiben, $n$ teilen: $p_1^{2e_1}, ..., p_m^{2e_m}$ mit den zugehörigen Primzahlen $p_1^{e_1}, ..., p_m^{e_m}$.
  $$\sum_{d^2 \mid n}\mu(d)$$
Das ist Summe der mu-Funktionen aller möglichen Kombinationen der Multiplikation der oberen Primzahlen (Wobei jede Primzahl $p_j$ einen Exponenten haben muss, der kleiner ist als $e_j$). Gilt dabei für ein $e_i$ einer Zahl $k = p_1^{e_1} ... p_m^{e_m}$ auch $e_i\geq 2$, dann ist $\mu(k) = 0$, verschwinden also.
Damit sind nur Kombinationen der Zahlen $p_1, ..., p_m$ relevant anzusehen.
Jetzt stellt sich die Frage: Wie viele Möglichkeiten gibt es eine geradzahlige Anzahl von Primzahlen aus den oberen zu wählen und wie viele Möglichkeiten gibt es eine ungeradezahlige Art zu wählen. Das will ich nicht ausrechnen aber wahrscheinlich kommt die gleiche Anzahl heraus. Subtrahiert man also die Anzahlen erhält man $0$, was der Methode entspricht, alle Zahlen für die $\mu(k) = 1$ bzw. $\mu(k) = -1$ zu trennen zu zählen und dann zusammenaddieren.

## McEliece 6-5
Berechne $\sum_{d \mid n} |\mu(d)|$.
Sei $n = p_1^{e_1}...p_m^{e_m}$
Oberer Ausdruck beschreibt die Summe von $\mu(d)$ für alle Teiler von $n$. $|\mu(d)| = 0$, wenn $d$ nicht quadratfrei und $1$ wenn $d$ quadratfrei ist. Der obere Ausdruck ist also die Summe aller quadratfreier Teiler von $n$. Die quadratfreie Teiler sind genau die Zahlen der Form $p_1^{f_1}...p_m^{f_m}$ mit $f_i \in \{0, 1\}$.
Damit gibt es also $2^m$ verschiedene quadratfreie Zahlen, die $n$ teilen.


$\newcommand{\Q}{\mathbb Q}$
$\newcommand{\R}{\mathbb R}$
$\newcommand{\C}{\mathbb C}$
$\newcommand{\F}{\mathbb F}$
$\newcommand{\Z}{\mathbb Z}$
$\newcommand{\N}{\mathbb N}$
$\newcommand{\a}{\alpha}$

#McEliece 


