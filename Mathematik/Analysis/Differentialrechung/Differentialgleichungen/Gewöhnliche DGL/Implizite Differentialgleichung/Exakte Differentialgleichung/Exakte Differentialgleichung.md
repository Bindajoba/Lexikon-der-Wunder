## Definition
Seien
- $U \subseteq \mathbb{R}^2$ ein [[Gebiet]]
- $f: U \to \mathbb{R}$ [[Stetigkeit|stetig]]
- $g: U \to \mathbb{R}$ [[Stetigkeit|stetig]]

Eine [[Implizite Differentialgleichung]]
$$f(t, x) + g(t, x)x' = 0$$ heißt **exakt**, wenn es eine stetig differenzierbare Funktion $F:U \to \mathbb{R}$ gibt mit 
$$(grad F)(t, x)= \begin{pmatrix}f(t, x) \\ g(t, x)  \end{pmatrix} \text{ für alle }(t, x)\in U \tag{1}$$
In diesem Fall heißt F [[Stammfunktion|Stammfunktion]] für $(1)$[^1]

## Äquivalente Definition I
Seien
- $U \subseteq \mathbb{R}^2$ eine [[Sternförmige Menge]]
- $f: U \to \mathbb{R}$ [[Stetigkeit|stetig]] [[Partielle Differenzierbarkeit|partiell differenzierbar]]
- $g: U \to \mathbb{R}$ [[Stetigkeit|stetig]] [[Partielle Differenzierbarkeit|partiell differenzierbar]]

gilt
$$\frac{\partial g}{\partial t} = \frac{\partial f}{\partial x}$$ dann heißt 
$$f(t, x) + g(t, x)x' = 0$$ **exakt**[^3]

## Lösung
Seien
- $U \subseteq \mathbb{R}^2$ ein [[Gebiet]]
- $f: U \to \mathbb{R}$ [[Stetigkeit|stetig]]
- $g: U \to \mathbb{R}$ [[Stetigkeit|stetig]]

Sei
- $I \subseteq \mathbb{R}$ ein Intervall mit nichtleerem Inneren

Eine Funktion $\lambda: I \to \mathbb{R}$ ist genau dann eine Lösung von $(1)$, wenn
1. $\lambda$ ist stetig differenzierbar
2. $F(t, \lambda(t)) = c \in \mathbb{R}$ für jedes $t \in I$[^2]

### Startwertproblem
Sei $(t_0, x_0) \in U$ ein Startzustand einer **Exakten Differentialgleichung**

Gilt $g(t_0, x_0) \neq 0$, dann hat das [[Startwertproblem]] $x(t_0) = x_0$ eine lokal eindeutige Lösung $\lambda: ]t_0-\beta, t_ß + \beta[$, die sich durch Auflösen von 
$$F(t, \lambda(t)) = F(t_0, x_0)$$ bekommen lässt.

#Mathe-IV 
[^1]: Zenk - Definition 17.3.1
[^2]: Zenk - Satz 17.3.2
[^3]: Zenk - Bemerkung 17.3.5