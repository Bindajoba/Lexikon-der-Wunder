TARGET DECK: Universität::Informatik::NaCo

# Beschreibung
Ein [[Optimierungsprozess]]. Der nächstbessere Wert wird gefunden, indem dem Gradienten gefolgt wird.

Q: Wie findet der Optimierungsprozess Gradient Descent den Optimalen Wert?
A: In dem dem Gradienten, d.h. der am stärksten abfallenden Richtung gefolgt wird.

# Definition
Sei $\mathcal{T}$ kontinuierlich und $\tau'$ die [[Abbildung|Ableitung]] von $\tau$.

Der Prozess $\mathcal{D}$ fährt mit **Gradient Descent** (mit update Rate $\alpha \in \R^+$) fort, wenn $e$ von der Form
$$e\klam{\wink{x_u}_{0 \leq u \leq t}, \tau} = x_{t+1} = x_t-\alpha\cdot \tau'(x_t)$$
Wenn $\tau$ [[Stochastische Funktion|stochastisch]] ist, dann heißt der Prozess **stochastic gradient descent (SGD)**.





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
