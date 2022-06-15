TARGET DECK: Universität::Mathematik::Geometrie

# Beschreibung
Eine [[Folge|Funktionenfolge]] heißt **gleichmäßig konvergent**, wenn die Geschwindigkeit mit der die Funktion punktweise gegen einen Grenzwert konvergiert nicht vom Funktionswert abhängt.

Das ist gegeben, wenn man die Funktion durch eine Funktionenfolge abschätzen kann, die überall gleich ist.

# Definition
Die Folge $(f_n)_{n \in \N}$ konvergiert genau dann gleichmäßg gegen $f$, wenn
$$\underset{n \to \infty}{\lim} \sup{x \in D_f}|f_n(x)-f(x)| = 0$$
Das ist genau dann gegeben, wenn
$$\forall \varepsilon > 0: \exists N \in \N: \forall n \geq N: |f_n(x)-f(x)|<\varepsilon$$


# Eigenschaften


# Beispiel
## Punktweise aber keine gleichmäßge Konvergenz
![[Beispiel Gleichmäßige Konvergenz.png]]
 Die Funktionenfolge $x \mapsto x^{2n}$ konvergiert punktweise gegen eine Funktion, die überall $0$ ist außer bei $\pm 1$, wo sie $1$ ist. Das Supremum oben konvergiert nicht gleichmäßig gegen $0$. Da es in einer Umgebung um $x_0=1$ immer ein $x$ gibt, bei dem $f_n(x) \approx 1$.


#Geometrie



