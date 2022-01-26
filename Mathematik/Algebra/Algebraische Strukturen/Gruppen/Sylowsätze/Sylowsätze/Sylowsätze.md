# Sätze
## "0-ter Sylowsatz"
Sei $G$ eine [[Endliche Gruppe]], $p$ eine [[Primzahl]] und $k \in \mathbb{N}_0$ derart, dass $p^k$ ein Teiler des [[Ordnung (Gruppe)|Gruppenordnung]] $|G|$ ist. Dann gibt es in $G$ eine Untergruppe der Ordnung $p^k$[^1]

Außerdem ist jede Untergruppe der Ordnung $p^k$ eine Untergruppe einer Untergruppe der Ordnung $p^{k+1}$
*Obacht: Nur weil es Untergruppen von Ordnung $p^k$ gibt, heißt das nicht, dass es en Element dieser Ordnung gibt.*


Dieser Satz ist eine Verallgemeinerung vom [[Satz von Cauchy]]

### Beweis
Nach dem Satz von Cauchy hat jede Gruppe, deren Ordnung durch $p$ teilbar ist, eine Untergruppe $U$ der Ordnung $p$.
Erzeuge nun die Faktorgruppe $G/U$. Alle Instanzen von $U$ werden zu einem Element der Faktorgruppe zusammengefasst.
Diese Gruppe ist jetzt aber wieder durch $p$ teilbar. Der Satz von Cauchy lässt sich erneut, nun auf die Faktorgruppe anwenden.

Im Rückschluss musste aber die ursprüngliche Gruppe eine Untergruppe der Ordnung $p^2$ haben. induktiv kann man den Beweis dann fortführen

![[Sylowsätze Bewis Sat 0.png]]

### Anwendung
200 ist durch 5, 2, 4 und 8 teilbar, und muss daher diese Untergruppen enthalten
![[Sylowsätze Anwendung I.png]]

## 1-ter Sylowsatz
Jede Untergruppe von $G$ ist in einer $p$-Sylowgruppe enthalten


## 2-ter Sylowsatz
Je zwei [[p-Sylowgruppe]] sind zueinander [[Konjugationsklasse|konjugiert]] und daher [[Isomorphismus|isomorph]].
Eine Sylowgruppe ist genau dann ein Normalteiler, wenn die Anzahl der Sylovgruppen $\nu_p$ 1 ist.

## 3-ter Sylowsatz
Sei $|G| = mp^r$, wobei $m$ und $p^r$ teilerfremd sind.

Für die Anzahl $\nu_p$ der Sylowgruppen gilt $\nu_p \equiv_p 1$ und $\nu_p | m$

*Carter verwendet statt der zweiten Bedingung $\nu$ teilt $|G|$. Gerkmanns Aussage ist also etwas stärker, denke ich.*

### Beweis
Sei $H$ eine $p$-Sylowgruppe. Aus dem zweiten Sylowsatz folgt, dass alle anderen $p$-Sylowgruppen zu $H$ [[Konjugation (Untergruppen)|konjugiert]] sind.
D.h. die Menge der $p$-Sylowgruppen ist der [[Orbit (Gruppenoperation)|Bahn]] der Konjugationsoperation auf der Menge der $p$-Sylowgruppen. Nach dem [[Orbit-Stabilisator-Satz]] teilt der Orbit die Gruppengröße.

Damit wurde Carters Behauptung gezeigt.

Zeige nun $\nu_p \equiv_p 1$:
Sei $S$ die Gruppe der $p$-Sylowgruppen.
Sei $H$ eine $p$-Sylowgruppe, die auf $S$ durch [[Konjugation (Untergruppen)|Konjugation]] operiert.

Zeige, dass es nur ein [[Stabiles Element]] bezüglich der Konjugation gibt.
EIne $p$-Sylowgruppe $K$ ist stabil, wenn $hKh^{-1} = K$ für alle $h \in H$.
Offensichtlich ist $hHh^{-1} = H$ stabil.

Angenommen $K$ ist stabil und die Gleichung $hKh^{-1} = K$ für alle $h \in H$ gilt.
Dann gilt $H \subseteq N_G(K)$
$N_G(K)$ ist selbst eine Gruppe, daher sind die $p$-Sylowgruppen $G$ und $H$ zueinander konjugiert.
$K$ ist aber in $N_G(K)$ [[Normalteiler|normal]] und ist nur zu sich selbst konjugiert. Daher müssen $K$ und $H$ die gleiche Gruppe sein.

Da $H$ eine $p$-Gruppe ist, die auf $G$ operiert, ist $|S| \equiv_p$ Menge der stabilen Elemente von $S = 1$ 

#Algebra 

[^1]: Gerkmann - Satz 10.1