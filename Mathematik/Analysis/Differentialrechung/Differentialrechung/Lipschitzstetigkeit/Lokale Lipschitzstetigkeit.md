## Beschreibung
Für eine lipschitzstetige Funktion existiert ein Doppelkegel, dessen Ursprung entlang des Graphen bewegt werden kann, sodass ein Teilgraph, einer Umgebung um den Ursprung stets außerhalb des Doppelkegels bleibt



## Definition
Seien
- $k, m, n \in \mathbb{N}$
$k$ ist die Dimension von der $t$-Komponente
$n$ ist die Dimension von der $x$-Komponente
$m$ ist die Dimension der Bildmenge von $g$
- $D \subseteq \mathbb{R}^k \times \mathbb{K}^n$, sodass $t \in \mathbb{R}^k$ und $x\in \mathbb{K}^n$
- $g: \begin{array}{rcl} D & \to & \mathbb{K}^m \\ (t, x) & \mapsto & g(t, x) \end{array}$

$g$ heißt **Lokal Lipschitzstetig** auf $D$ bezüglich $x$, wenn es zu jedem $(t, x) \in D$ eine Umgebung U gibt, sodass $f|_{U\cap D}$ [[Globale Lipschitzstetigkeit|Global Lipschitzstetig]] auf $U\cap D$ bezüglich $x$ ist.

Ist g unabhängig von t, dann muss man bezüglich $t$ natürlich nicht sagen.[^1]

## Satz I 
Seien
- $k, m, n \in \mathbb{N}$
$k$ ist die Dimension von der $t$-Komponente
$n$ ist die Dimension von der $x$-Komponente
$m$ ist die Dimension der Bildmenge von $g$
- $V \subseteq \mathbb{R}^k \times \mathbb{K}^n$ ein [[Gebiet]]
- $g: \begin{array}{rcl} V & \to & \mathbb{K}^m \\ (t, x) & \mapsto & g(t, x) \end{array}$

Ist die partielle Ableitung nach der 2. Variable (also $x$)
$$D_2g:\begin{array}{rcl} V & \to & L(\mathbb{K}^n, \mathbb{K}^m) \\ (t, x) & \mapsto & (D_2g)(t, x) \end{array}$$ stetig, dann ist $g$ lokal Lipschitzstetig.[^2]

## Eigenschaften
Auf einem Gebiet ist die Summe/Produkt **bzgl. $x$ lokal lipschitzstetiger** Funktionen wieder lokal lipschitzstetig bzgl. $x$[^3]


#Mathe-IV 

[^1]: Zenk - Definition 18.2.4
[^2]: Zenk - Satz 18.2.3
[^3]: Zenk - Bemerkung 18.2.4-5