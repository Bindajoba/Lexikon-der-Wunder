TARGET DECK: Universität::Mathematik::Algebra

# Aufgabe 1
Zeige: Die [[Galoisgruppe]] von $f = (x^p-1)/(x-1)$ ist [[Zyklische Gruppe|zyklisch]], und hat [[Ordnung (Gruppe)|Ordnung]] $p-1$.

Siehe [[Galoisgruppe]]

# Aufgabe 2
Bestimme die [[Galoisgruppe]] von $\Q(\sqrt 2, \sqrt 3)$.

Siehe [[Galoisgruppe]]

# Aufgabe 4
Gibt es ein Polynom in $\Q[x]$, sodass $\Q(\sqrt[3] 2)$ sein [[Zerfällungskörper]] ist?

Siehe [[Zerfällungskörper]]


# Aufgabe 5
Sei $\phi \in Gal(L|K)$ wobei die Erweiterung [[Endliche Körpererweiterung|endlich]] ist. Sei $M$ ein Zwischenkörper.

Zeige: Der [[Fixkörper]] $M^{\phi} = \{\phi(a) = a: a \in M\}$ ist ein [[Zwischenkörper]]. 
Zeige außerdem: $[M:K] = [\phi(M):K]$.

$\phi(1) = 1$. Für $a, b \in M^\phi: \phi(a+b) = \phi(a) + \phi(b) = a+b$. Multiplikation analog und so.
Und offensichtlich gilt $M^\phi \subseteq M \subseteq L$

$M|K$ induziert einen Vektorraum. Mit einer Basis von $M$ kann man jedes Element in $\phi(M)$ durch die Bilder der Basen beschreiben. Umgekehrt, da $\phi$ bijektiv ist, lässt sich jedes Element aus $M$ durch die Uhrbilder der Basis von $\phi(M)$ beschreiben. Das muss aber bedeuten, dass die Basen gleich groß sind.

# Aufgabe 6
Zeige: Wenn $K$ abzählbar ist, dann gibt es für alle $n \in \N$  immer $n$ [[Algebraische Unabhängigkeit|Algebraisch Unabhängige Element]]

Für algebraische Unabhängigkeit dürfen keine [[Algebraisches Element|algebraischen Zahlen]] verwenden. Wären $a_1, ..., a_n$ algebraische Elemente, dann könnte man ein solches Polynom erzeugen, indem man die Minimalpolynome der oberen Zahlen miteinander multipliziert.
Noch einfacher, ist eine Zahl algebraisch, dann erfüllt sein Minimalpolynom die Bedingung.

Die Zahlen müssen also Transzendent sein.
Eine einzige Zahl $a_1$ ist automatisch algebraisch unabhängig, denn es gibt kein Polyom $p(x_1)$ mit $p(a_1) = 0$.

Konstruiere algebraisch unabhängie Zahlen wie folgt:
Wähle für $a_2$ eine Zahl, die in $K(a_2)$ transzendent ist.
Wähle dann für $a_3$ eine Zahl, die in $K(a_1, a_2)$ transzendent ist.

Die daraus erhaltenen Zahlen $a_1, a_2,..., a_n$ sind algebraisch unabhängig, denn angenommen sie wären es nicht, dann gäbe es ein Polynom $p$ mit $p(a_1, a_2, ..., a_n) = 0$.
Setze alle Elemente bis auf das letzte ein: $p(a_1, a_2, ..., a_{n-1}, x_n)$ ist ein eindiensionales Polynom mit Koeffizienten aus $K(a_1, ..., a_{n-1})$. Damit ist aber $a_n$ algebraisch über $K(a_1, ..., a_{n-1})$, was im Widerspruch zur Methode steht, mit der wir die Zahlen erhalten haben.
*Anmerkung: Falls $p(a_1, a_2, ..., a_{n-1}, x_n)$ konstant ist, also nicht von $x_n$ abhängt, verwende $x_{n-1}$ für den Beweis.*

# Aufgabe 7
Zu Zeigen: Sei $K(a_1, ..., a_n)$ eine Erweiterung algebraisch unabhängiger Zahlen. Für jede Permutation dieser Zahlen, gibt es einen $K$-[[Körperautomorphismus]], der den Effekt hat auf die gleiche Weise die Zahlen $\{a_1, ..., a_n\}$ zu permutieren.

Sei $\phi$ eine Funktion, die $\{a_1, ..., a_n\}$ im Sinne einer bestimmten Permutation vertauscht



$\newcommand{\Q}{\mathbb Q}$
$\newcommand{\R}{\mathbb R}$
$\newcommand{\C}{\mathbb C}$
$\newcommand{\F}{\mathbb F}$
$\newcommand{\Z}{\mathbb Z}$
$\newcommand{\a}{\alpha}$


#Hadlock 