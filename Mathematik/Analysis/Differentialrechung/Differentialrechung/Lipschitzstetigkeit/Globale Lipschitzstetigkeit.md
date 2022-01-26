## Beschreibung
Für eine lipschitzstetige Funktion existiert ein Doppelkegel, dessen Ursprung entlang des Graphen bewegt werden kann, sodass dieser stets außerhalb des Doppelkegels bleibt[^1]

Eine Funktion ist global lipschitzstetig, wenn sie [[Differenzierbarkeit|differenzierbar]] ist und die Ableitung der Funktion einen Maximalen Wert annimmt. 

Globale Lipschitzstetigkeit ist stärker als [[Gleichmäßige Stetigkeit]].
Insbseondere ist jede global lipschitzstetige Funktion [[Lokale Lipschitzstetigkeit|lokal lipschitzstetig]]
## Definition
Seien
- $k, m, n \in \mathbb{N}$
$k$ ist die Dimension von der $t$-Komponente
$n$ ist die Dimension von der $x$-Komponente
$m$ ist die Dimension der Bildmenge von $g$
- $D \subseteq \mathbb{R}^k \times \mathbb{K}^n$, sodass $t \in \mathbb{R}^k$ und $x\in \mathbb{K}^n$
- $g: \begin{array}{rcl} D & \to & \mathbb{K}^m \\ (t, x) & \mapsto & g(t, x) \end{array}$

$g$ heißt **Global Lipschitzstetig** auf $D$ bezüglich $x$, wenn es $L>0$ gibt, sodass
$$||g(t, x)-g(t, y)|| \leq L||x-y|| \text{ für alle } (t, x), (t, y) \in D$$

Ist g unabhängig von t, dann muss man bezüglich $t$ natürlich nicht sagen.

#Mathe-IV 
[^1]:  Wikipedia - https://de.wikipedia.org/wiki/Lipschitzstetigkeit