TARGET DECK: Universität::Informatik::NaCo

# Beschreibung
Ein [[Optimierungsprozess]].
Er funktioniert, indem jede Iteration ein zufälliger Zustand aus der Umgebung gewählt wird dann verglichen wird, ob der aktuelle oder der gezogene Nachbarknoten kleiner ist. 

Q: Wie funktioniert Hill Climbing?
A: Jeden Optimierungsschritt wird ein zufälliger Punkt in einer Umgebung probiert. Ist dieser besser, dann wird die Optimierung damit fortgesetzt. Sonst wird die Optimierung auf dem vorherigen Punkt wiederholt.


# Definition
Sei $\mathcal D = (\mathcal X, \mathcal T, \tau, e, \wink{x_t}_{0 \leq u \leq t})$.
Ist die widerholt aufgerufene Funktion $e$ von der Form 
$$e\klam{\wink{x_u}_{0 \leq u \leq t}, \tau} = x_{t+1} = \underset{x \in \{x_t, x_t'\}}{\arg \min} \tau(x)$$
wobei $x_t' \in nachbarschaft(x_t)$ ein zufälliger Punkt in der Nachbarschaft von $x_t$ ist. 
dann nennt man den Algorithmus **Hill Climbing**

*$nachbarschaft$ muss sich nicht notwendigerweise auf [[Nachbarschaft (Graphentheorie)]] bezieht sondern allgemeiner [[Umgebung (Topologie)]] beinhalten.*





$\newcommand{\wink}[1]{\left\langle #1 \right\rangle}$
$\newcommand{\klam}[1]{\left( #1 \right)}$
$\newcommand{\Q}{\mathbb Q}$
$\newcommand{\R}{\mathbb R}$
$\newcommand{\C}{\mathbb C}$
$\newcommand{\F}{\mathbb F}$
$\newcommand{\Z}{\mathbb Z}$
$\newcommand{\N}{\mathbb N}$
$\newcommand{\a}{\alpha}$

#Natural-Computing 
