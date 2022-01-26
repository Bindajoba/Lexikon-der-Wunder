## Beschreibung
Eine Lösung einer [[Differentialgleichung]] ist stabil wenn kleine Änderungen des Startwert keine großen Änderungen der Lösung zu Folge haben.

## Definition
Sei $\mu: ]a, \infty[ \to \mathbb{K}^d$ eine Lösung der DGL
$$x' = f(t, x)$$

$\mu$ ist stabil, wenn es für alle $\varepsilon>0$ und und für alle $\tau>a \in \mathbb{R}$ ein $\delta(\varepsilon, \tau)>0$ gibt, mit:
Zu jedem Anfangswert $(\tau, \xi)$ mit $||\lambda_{(\tau, \xi)}(t)-\mu(t)||<\delta$ existiert die maximale Lösung $\lambda_{(\tau, \xi)}(t)$ und erfüllt das [[Startwertproblem]]:
$$x' = f(t, x), x(\tau) = \xi$$für alle $t\geq\tau$ und erfüllt die Abschätzung:
$$\underset{t\geq \tau}{\sup} ||\lambda_{(\tau, \xi)}(t)-\mu(t)|| < \epsilon$$

#Mathe-IV 