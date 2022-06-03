# Beschreibung
Kombiniert man die Methoden des [[Simulated Annealing]] und des [[Gradient Descent]], dann erhält man eine Verbesserung der beiden.

# Definition
Sei $\mathcal{D} = (\mathcal{X}, \mathcal{T}, \tau, e_\mathcal{D}, \wink{x_t}_{0 \leq u \leq t})$ ein [[Optimierungsprozess]], welches [[Simulated Annealing]] verwendet.
Sei $\mathcal{F} = (\mathcal{X}, \mathcal{T}, \tau, e_\mathcal{F}, \wink{x_{t+v}}_{0 \leq v \leq t})$ ein [[Optimierungsprozess]], welches [[Gradient Descent]] verwendet.

Der Prozess $\mathcal{E} = (\mathcal{X}, \mathcal{T}, \tau, e_\mathcal{E}, \wink{x_u}_{0 \leq u \leq t})$ ist ein [[Optimierungsprozess]], welches genau dann Simulated Annealing mit $n$ Schritten Local Gradient ist, wenn $e_\mathcal{E}$ von der Form 
$$e_{\mathcal{E}} \klam{\wink{x_u}_{0 \leq u \leq t, \tau}} = x_{t+1} = \begin{cases}\mathcal{F}^*(x_t') & \text{wenn }\mathcal{F}^*(x_t') \leq \tau(x_t) \\
& \text{oder } r \leq A(\tau(x_t), \tau(\mathcal{F}^*(x_t')), T(t)), \\
x_t & \text{sonst }\end{cases}
$$
wobei $\mathcal{F}^*(x_t') = \underset{0 \leq v \leq n }{\underset{x_{t+v}}{\arg \min}} (x_{t+v})$
die beste Lösung ist, die $\mathcal{F}$ gefunden hat.




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
