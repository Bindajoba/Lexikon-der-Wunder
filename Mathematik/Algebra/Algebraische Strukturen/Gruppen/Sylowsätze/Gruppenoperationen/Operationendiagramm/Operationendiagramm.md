# Beschreibung
Durch ein **Operationendiagramm** lässt sich die Auswirkung einer [[Gruppenoperation]] auf einer Menge darstellen.

# Beispiele
## Rechtecksbeispiel
Beschrifte die Ecken eines Rechtecks mit Zahlen und betrachte alle vier Konfigurationen, die man durch horizontale und vertikale Spiegelung erhält.
Zeichne die Rechtecke auf und stelle dir die [[Permutationsgruppe]] vor. Das sind die Funktionen, die die gezeichneten Rechtecke vertauschen.

Unsere Gruppenoperation $\phi$ bildet nun von der Gruppe $V_4$ auf diese [[Permutation|Permutationen]] ab.
$\phi$ ist folgendermaßen definiert:
$\phi(h) = \text{Das Rechteckpaar, dass man durch horiontales Spiegeln erhält wird getauscht}$
$\phi(v) = \text{Nicht passiert}$

Die Effekte von $\phi$ lassen sich dann so illustrieren:
![[Operationendiagramm.png]]

Die Pfeile stehen für die Bilder des erzeugendensystems der Gruppe $V_4$.

## Operation auf Untergruppen
Sei $S_3$ die [[Symmetrische Gruppe]].
Betrachte seine [[Untergruppe|Untergruppen]] $S = \{\langle e \rangle\, \langle r\rangle, \langle f\rangle, \langle rf\rangle, \langle r^2f\rangle\}$

Man kann durch einen [[Gruppenhomomorphismus]] $\tau: S_3 \to Perm(S)$ eine [[Gruppenoperation]] auf die [[Permutationsgruppe]] von $S$ definieren:

$\tau(g)= \text{ die Permutation bewegt jede Untergruppe H auf die Untergruppe }gHg^{-1}$

![[Operationendiagramm II.png]]

#Carter 