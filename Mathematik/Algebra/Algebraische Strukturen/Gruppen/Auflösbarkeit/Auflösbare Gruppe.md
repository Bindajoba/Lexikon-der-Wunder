# Beschreibung
Die Bildung von [[Kommutatorgruppe|Kommutatorgruppen]] lässt sich iterieren. Man bezeichnet mit $G^{(2)}$ die Kommutatorgruppe von $G'$.  

# Definition
Eine Gruppe $G$ heißt **auflösbar**, wenn $G^{(n)} = \{e\}$ für ein $n \in \mathbb{N}_0$ gilt.

*$G^{(n)}$ bezeichnet die [[Kommutatorgruppe]]*

# Charakterisierungen
Eine endliche Gruppe $G$ ist genau dann [[Auflösbare Gruppe|auflösbar]], wenn sie eine [[Abelsche Normalreihe]] besitzt

## Auflösbarkeit durch Normalteiler
Sind $G/N$ und $N$ auflösbar, genau dann ist auch $G$ auflösbar.

# Eigenschaften
## Auflösbarkeit von Untergruppen
Jede [[Untergruppe]] einer **auflösbaren Gruppe** ist **auflösbar**.




# Beispiel
## Abelsche Gruppe
Offenbar sind abelsche Gruppen auflösbar, denn $[g, h] = e$

## p-Gruppen
Jede [[P-Gruppe]] ist auflösbar..[^1]

**Beweis**:
Eine $p$-Gruppe ist [[Abelsche Gruppe|abelsch]] oder hat einen nicht-triviales [[Zentrum (Gruppe)|Zentrum]]. Durch das Dividieren der Gruppe durch das Zentrum erhält man eine kleinere $p$-Gruppe

# Übungen
## Klausur 2018 Aufgabe 4
![[Klausur 2018 Aufgabe 4.png]]
### a)
$40 = 8 \cdot 5$.

Bestimme die Anzahl $\nu_5$ von $5$-Sylowgruppen:
Nach VL gilt $\nu_5 \equiv_5 1$ und $\nu_5 \mid 8$, kann also nur $\nu_5 = 1$ sein. Die $5$-Sylowgruppe ist einzig also Normalteiler. Nenne die Gruppe $N$. $N$ ist zyklisch also abelsch, also auflösbar.

Damit existiert die Faktorgruppe $G/N$ und hat die Ordnung $40/5 = 8$. 
Diese Faktorgruppe ist eine p-Gruppe und damit auflösbar.

Ist die Faktorgruppe und der Normalteiler auflösbar, dann auch $G$.

### b)
$C_{2} \times C_{20}$ ist abelsch aber nicht zyklisch. Wäre es der Fall, dann müsste es $40$ Elemente und ein Element der Ordnung $40$ haben. Die Elemente in $C_{2} \times C_{20}$ haben die Form $(a, b)$ und es gilt $20 \cdot (a, b) = (20a, 20b) = (0, 0)$. Die Elemente von $C_{2} \times C_{20}$ haben also maximal Ordnung 20.







[^1]: Gerkmann - Satz 9.17