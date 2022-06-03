# Beschreibung
Das Zufällige Sampling ist ein [[Optimierungsprozess]]
Es wird ein jede Iteration ein neuer Zufallswert gewählt und mit dem aktuellen Wert verglichen.

# Definition
Sei $\mathcal{D} = (\mathcal{X}, \mathcal T, \tau, e, \wink {x_t}_{0 \leq u \leq t})$ ein Optimierungsprozess
Sei $X \subseteq \mathcal{X}$ eine Menge von $n \in \N$ zufällig ausgewählten Elementen.

Der Prozess $\mathcal{D}$ verwendet Zufälliges Sampling, wenn $e$ von der Form ist:
$$e\klam{\wink{x_u}_{0 \leq u \leq t}, \tau} = x_{t+1} = \underset{x \in \{x_t \cup X\}}{\arg \min} \tau(x)$$




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
