# Beschreibung
Simulated Annealing ist ein [[Optimierungsprozess]].
Es handelt sich um eine Weiterentwicklung des [[Hill Climbing]].
Es wird ein Mechanismus eingebaut, bei dem manchmal Zustände mit einer größeren Zielfunktion gewählt werden.
Dieses Verhalten wird durch eine Funktion $A$ bestimmt. Dessen Verhalten kann sich über eine Funktion $T$ über Zeit ändern.

# Definition
Sei $T: \N \to \R$ eine Temperaturabbildung, d.h. eine eine Funktion, die eine für jeden Zeitschrit eine Temperatur ausgibt.
Sei $A: \mathcal{T} \times \mathcal{T} \times \R \to \mathbb{P}$ eine Funktion, die eine Annahmewahrscheinlichkeit für zwei Eingabewerte und eine Temperatur ausgibt.
Üblicherweise setzen wir
$$A(Q, Q', T) = e^{\frac{-(Q'-Q)}{T}}$$
für $\mathcal{T} \subseteq \R$. Sei $r \in \mathbb{P}$ eine zufällige Zahl zwischen 0 und 1. Der Prozess fährt mit **Simulated Annealing** fort, wenn $e$ die Form hat
$$e\klam{\wink{x_u}_{0 \leq u \leq t}, \tau} = x_{t+1} = \begin{cases}x_t' & \text{wenn $\tau(x_t') \leq \tau(x_t)$ oder $r \leq A(\tau(x_t), \tau(x_t'), T(t))$}\\ x_t &\text{sonst}\end{cases}$$
wobei $x_t'$ einen Zustand in der [[Umgebung (Topologie)]] von $x_t$ bezeichnet




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
