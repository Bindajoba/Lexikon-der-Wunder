TARGET DECK: Universität::Mathematik::Algebra


$\newcommand{\Q}{\mathbb Q}$
$\newcommand{\R}{\mathbb R}$
$\newcommand{\C}{\mathbb C}$
$\newcommand{\F}{\mathbb F}$
$\newcommand{\Z}{\mathbb Z}$
$\newcommand{\N}{\mathbb N}$
$\newcommand{\a}{\alpha}$


# Aufgabe 3
Zeige $\varphi(p^n) = p^{n-1}(p-1)$.

Zeige erst $\varphi(p^2) = p(p-1)$
Es gilt $\varphi(p) = p-1$. 

$\varphi(p^2)$ gibt die Anzahl der mit $p^2$ teilerfremden kleineren Zahlen an. Die einzigen Teiler sind $1, p, p^2$.
1 muss nicht berücksichtigt werden. Offensichtlich gibt es aber $p$ Zahlen $\leq p^2$, die durch $p$ teilbar sind, nämlich $p, 2p, ..., (p-1)p, p^2$.
$p^2-p = p(p-1)$.

Das gleiche Verfahren lässt sich verallgemeinern.
Die einzigen Teiler von $p^n$ sind $1, p, p^2, ..., p^n$. Relevant ist aber nur $p$, denn ist eine Zahl durch $p^k$ teilbar, dann auch durch $p$.
Es gibt $p^{n-1}$ Zahlen zwischen $1$ und $p^n$, die durch $p$ teilbar sind.
D.h. $\phi(p^n) = p^n-p^{n-1} = p^{n-1}(p-1)$

 # Aufgabe 5
Wie viele Primitive 20te. Einheitswurzeln gibt es?
 $\varphi(20) = \varphi(4)\varphi(5) = 8$

# Aufgabe 7
Die Position der 7. Wurzeln von $1-i$.
Die Wurzeln haben den Betrag $\sqrt[7]{\sqrt 2}$ und bilden ein 7-eck, von dem eine Ecke nach $-\pi/28$ zeigt.

# Aufgabe 9
Zeige für alle $n \in \N$
$$\sum_{d|n} \varphi(d) = n$$
Beide Seiten geben die Anzahl der $n$-ten Einheitswurzel an.
Rechts ist offensichtlich. Zeige die Anzahl für Links:
Ist $a$ eine $n$-te Einheitswurzel, dann gibt es ein eindeutiges $m$, dass $n$ teilt und für das $a$ eine primitive $m$-te Einheitswurzel ist.
Für ein $m$, das $n$, teilt sich außerdem alle $m$-ten Einheitswurzeln auch $n$-te Einheitswurzeln.

Die Zahl der primitiven Einheitswurzeln berechnet sich genau durch die Eulersche Phi-Funktion, die ja durch alle Teiler von $n$ geht!









#Hadlock 