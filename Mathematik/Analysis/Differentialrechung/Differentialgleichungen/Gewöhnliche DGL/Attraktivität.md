## Beschreibung
Eine Lösung einer [[Differentialgleichung]] ist attraktiv wenn die Lösungen von kleine Änderungen des Startwert trotzdem gegen den gleichen Wert konvergieren.

## Definition
Sei $\mu: ]a, \infty[ \to \mathbb{K}^d$ eine Lösung der DGL
$$x' = f(t, x)$$

$\mu$ ist attraktiv, wenn es für alle $\tau>a \in \mathbb{R}$ ein $\nu(\varepsilon, \tau)>0$ gibt, mit:
Zu jedem Anfangswert $(\tau, \xi)$ mit $||\xi-\mu(t)||<\delta$ existiert die maximale Lösung $\lambda_{(\tau, \xi)}(t)$ und erfüllt das [[Startwertproblem]]:
$$x' = f(t, x), x(\tau) = \xi$$ für alle $t\geq\tau$ und es gilt
$$\underset{t \to \infty}{\lim} ||\lambda_{(\tau, \xi)}(t)-\mu(t)|| = 0$$

## Weitere Konzepte
### Einzugsbereich
Die Menge, aller [[Startwertproblem|Startwerte]], deren Lösungen gegen den gleichen Wert wie $\mu$ konvergieren nennt man den Einzugsbereich von $\mu$.

$$\{(\tau, \xi)\in V : ||\lambda_{(\tau, \xi)}(t)-\mu(t)|| = 0\}$$

#Mathe-IV 