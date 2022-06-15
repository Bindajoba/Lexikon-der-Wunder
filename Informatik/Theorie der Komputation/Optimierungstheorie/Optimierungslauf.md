# Beschreibung
Ein Optimierungslauf ist eine Sequenz von Zuständen, die sich einem besseren Ergebnis annähern sollten.

Q: Optimierungslauf 
A: eine Sequenz von Zuständen, die sich einem besseren Ergebnis annähern sollten.


# Definition
Betrachte eine [[Optimierung]].
Für einen Zustandsraum $\mathcal X$ ist ein Optimierungslauf von Länge $g+1$ eine Sequenz von Zuständen $\langle x_t \rangle_{0 \leq t \leq g}$ mit $x_t \in \mathcal{X}$ für alle $t$

Ein **Optimierungslauf** 
- zeigt **Bisschen Verbesserung** (*'workin to some extend'*), wenn für $t \leq t'$ positiv mit $\tau(x_t) \leq \tau(x_{t'})$ [[Korrelation|korreliert]]
- zeigt **Strenge Verbesserung** (*'strictly improving'*), wenn für $t \leq t'$ auch $\tau(x_t) \leq \tau(x_{t'})$
- ist genau dann **Global Erfolgreich** (*'globally successful'*), wenn $\tau(x) \leq \tau(x_g)$ für alle $x \in \mathcal{X}$
  

$\newcommand{\ang}[1]{\left\langle #1 \right\rangle}$
$\newcommand{\Q}{\mathbb Q}$
$\newcommand{\R}{\mathbb R}$
$\newcommand{\C}{\mathbb C}$
$\newcommand{\F}{\mathbb F}$
$\newcommand{\Z}{\mathbb Z}$
$\newcommand{\N}{\mathbb N}$
$\newcommand{\a}{\alpha}$

#Natural-Computing 
