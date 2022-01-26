## Definition
Sei $a \in U$ oder $a$ eine [[Isolierte Singularität|isolierte Singularität]] von $f$.
$f(z) = \sum\limits_{k \in \mathbb{Z}} c_k(z-a)^k$ die Laurentreihenentwicklung von der [[Analytische Funktion|analytischen Funktion]] $f$ um $a$

Dann heißt
$$\omega(f, a):= \begin{cases} -\infty & \text{falls } a \text{ wesentliche Singularität}\\ n & \text{falls } c_n \neq 0 \text{ und } c_k = 0 \text{ für } k \in \mathbb{Z}, k < n\\ \infty & \text{falls } f \text{ die Nullfunktion in einer Umgebung von } a \text{ ist} \end{cases}$$ die Ordnung von $f$ in $a$.[^1]

*Die Ordnung ist sowas wie der Grad aber von unten. Es ist die kleinste Potenz in einem [[Rationale Funktion|gebrochen-rationalen Polynom]]*

## Eigenschaften
- Ist $\omega(f, a) > 0$, dann hat $f$ in $a$ eine $n$-fache Nullstelle
- Ist $\omega(f, a) \geq 0$, dann ist $f$ in $a$ holomorph (fortsetzbar) und $Res(f, a) = 0$
- Ist $\omega(f, a) = 0$, dann ist $f$ in $a$ holomorph (fortsetzbar) und $f(a) \neq 0$
- Ist $\omega(f, a) < 0$, dann hat $f$ in $a$ einen Pol $n$-ter Ordnung