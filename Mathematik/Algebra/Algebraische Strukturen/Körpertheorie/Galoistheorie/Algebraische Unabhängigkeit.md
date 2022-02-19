TARGET DECK: Universität::Mathematik::Algebra

# Beschreibung


# Definition
Zahlen $a_1, a_2, ..., a_n$ werden algebraisch unabhängig über einem [[Körper]] $K$ genannt, wenn es kein Polynom $p(x_1, x_2, ..., x_n)$ gibt, für das gilt: $p(a_1, a_2, ..., a_n) = 0$


# Eigenschaften
Ist der Körper $K \subseteq \C$ abzählbar, dann gibt es abzählbar unendlich viele algebraisch unabhängige Zahlen.

**Beweis**
Zeige: Wenn $K$ abzählbar ist, dann gibt es für alle $n \in \N$  immer $n$ [[Algebraische Unabhängigkeit|Algebraisch Unabhängige Element]]

Für algebraische Unabhängigkeit dürfen keine [[Algebraisches Element|algebraischen Zahlen]] verwenden. Wären $a_1, ..., a_n$ algebraische Elemente, dann könnte man ein solches Polynom erzeugen, indem man die Minimalpolynome der oberen Zahlen miteinander multipliziert.
Noch einfacher, ist eine Zahl algebraisch, dann erfüllt sein Minimalpolynom die Bedingung.

Die Zahlen müssen also Transzendent sein.
Eine einzige Zahl $a_1$ ist automatisch algebraisch unabhängig, denn es gibt kein Polyom $p(x_1)$ mit $p(a_1) = 0$.
Wir können einfach so eine Transzendente Zahl finden, da die Menge aller Algebraischen Zahlen azählbar ist, während $\C$ überabzählbar ist

Konstruiere algebraisch unabhängie Zahlen wie folgt:
Wähle für $a_2$ eine Zahl, die in $K(a_2)$ transzendent ist. (was wir machen können, da $K(a_2)$ abzählbar und damit die Menge seiner algebraischen Zahlen ebenfalls abzählbar ist.)
Wähle dann für $a_3$ eine Zahl, die in $K(a_1, a_2)$ transzendent ist. usw.

Die daraus erhaltenen Zahlen $a_1, a_2,..., a_n$ sind algebraisch unabhängig, denn angenommen sie wären es nicht, dann gäbe es ein Polynom $p$ mit $p(a_1, a_2, ..., a_n) = 0$.
Setze alle Elemente bis auf das letzte ein: $p(a_1, a_2, ..., a_{n-1}, x_n)$ ist ein eindiensionales Polynom mit Koeffizienten aus $K(a_1, ..., a_{n-1})$. Damit ist aber $a_n$ algebraisch über $K(a_1, ..., a_{n-1})$, was im Widerspruch zur Methode steht, mit der wir die Zahlen erhalten haben.
*Anmerkung: Falls $p(a_1, a_2, ..., a_{n-1}, x_n)$ konstant ist, also nicht von $x_n$ abhängt, verwende $x_{n-1}$ für den Beweis.*

# Beispiel
## Gegenbeispiel
Die Zahlen $\pi$ und $-\pi$ sind transzendent aber nicht algebraisch unabhängig, da sie Nullstellen des Polynoms $p(x_1, x_2) = x_1 + x_2$ sind.







$\newcommand{\Q}{\mathbb Q}$
$\newcommand{\R}{\mathbb R}$
$\newcommand{\C}{\mathbb C}$
$\newcommand{\F}{\mathbb F}$
$\newcommand{\Z}{\mathbb Z}$
$\newcommand{\a}{\alpha}$


#Hadlock 