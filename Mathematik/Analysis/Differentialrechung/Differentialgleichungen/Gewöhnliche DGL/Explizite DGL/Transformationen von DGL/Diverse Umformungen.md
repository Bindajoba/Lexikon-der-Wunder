## Besschreibung
Hier werden diverse Möglichkeiten aufgelistet, eine [[Explizite Differentialgleichung]] umzuformen.

## Umformung I
Seien
- $V \subseteq \mathbb{R} \times \mathbb{K}^d$ ein [[Gebiet]]
V ist das Gebiet, in dem wir Lösungen suchen werden
- $g:V \to \mathbb{K}^d$ [[Stetigkeit|stetig]]
- $I \in \mathbb{R}$ ein Intervall mit nichtleerem Inneren
$I$ ist ein Definitionsbereich einer Lösung
I muss so klein sein, dass gilt $\{(t, \lambda(t)): t \in I\} \subseteq V$
*D.h. Die Lösungskurve liegt in $V$*
- $(t_0, x_0) \in V$ ein Startwert

Sei eine [[Explizite Differentialgleichung]] mit [[Startwertproblem]]
$$x' = f(t, x), x(t_0) = x_0 \tag{1}$$

$\lambda: I \to \mathbb{K}^d$ ist genau dann eine Lösung von $(1)$, wenn

$\lambda$ ist stetig und für jedes $t\in I$ gilt
$$\lambda(t) = x_0 + \int\limits_{t_0}^t f(s, \lambda(s)) \,ds$$[^1]

*Der Satz ist ziemlich fundamental.
Inegriert man beginnend zum Zeitpunkt $t_0$ entlang aller Steigungen einer Lösung, so erhält man genau die Lösung zurück.*


#Mathe-IV 

[^1]: Zenk - Satz 18.1.2