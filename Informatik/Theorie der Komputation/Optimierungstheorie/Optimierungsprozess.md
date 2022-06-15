# Beschreibung
Das wiederholte Aufrufen einerOptimierungsfunktion.

Q: Optimierungsprozess
A: Das wiederholte Aufrufen einerOptimierungsfunktion

# Definition
Ziel ist eine Optimierung auf dem Zustandsraum $\mathcal{X}$ und auf dem Zielraum $\mathcal{T}$ und der Zielfunktion $\tau$.

Sei $e$ eine Funktion, sodass der [[Optimierungslauf]] durch das wiederholte Aufrufen von $e$ erzeugt wird. Zum Beispiel: $x_{t+1} = e \klam{\wink{x_u}_{0 \leq u \leq t, \mathcal{T}}}$ mit einem willkürlichen Anfangswert $x_0$.

Ein **Optimierungsprozess** ist ein Tupel $(\mathcal{X}, \mathcal{T}, \tau, e, \wink{x_t}_{0 \leq t \leq g})$

# Beispiel
## Zufälliges Sampling
Siehe [[Zufälliges Sampling]]

## Hill Climbing
[[Hill Climbing]]

## Simulated Annealing
[[Simulated Annealing]]

## Gradient Descent
[[Gradient Descent]]

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
