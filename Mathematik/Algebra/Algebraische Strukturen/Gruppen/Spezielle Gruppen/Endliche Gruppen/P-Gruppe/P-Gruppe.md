# Beschreibung
Eine $p$-Gruppe ist eine [[Gruppe]] mit [[Primzahl]]potenz[[Ordnung (Gruppe)|ordnung]] $p^n$


# Eigenschaften
## Anzahl von Stabilen Elementen
Wenn eine Gruppe $G$ der Ordung $p$ auf einer Menge $S$ operiert, dann gilt
$$|S| \equiv_p \text{ Anzahl stabiler Elemente in } S$$
Es besteht also eine [[Kongruenz (Ganze Zahlen)]].

**Beweis:** Nach dem [[Orbit-Stabilisator-Satz]] ist die Größe jedes Orbits ein Faktor von $|G| = p$. Da $p$ eine [[Primzahl]] ist, sind die einzigen Faktoren entweder $1$ oder $p$.
Jeder Orbit ist also entweder ein [[Stabiles Element]] oder ein Knäuel von $p$ Elementen aus $S$. ($p$ ist eine Primzahl. Das Knäuel ist daher sogar ein Zykel)

![[P-Gruppe Kongruenzsatz.png]]

Daraus ergibt sich die einfache Gleichung
$$\text{Zahl der Stabilen Elemente } + \text{ Zahl der nichtstabilen Elemente in p-Knäuel } = |G|$$
Die Zahl der nichtstabilen Elemente tauchen in $p$-Knäuel und sind demnach ein vielfaches von 7.

*Eine Verallgemeinerung weitet oberen Satz auf alle p-Gruppen, d.h. auch auf Gruppen von Primzahlordnung aus. Der Beweis verläuft sehr ähnlich.*

## Kongruenz des Index
Für eine [[Untergruppe]] $H$ einer $p$-Gruppe $G$ gilt
$$[N_G(H) : H] \equiv_p [G:H]$$
wobei $[G:H]$ sich auf den Index, also die Anzahl von [[Nebenklasse|Nebenklassen]] bezieht. 

## Nichttriviales Zentrum
Sei $G$ eine nichttriviale $p$-Gruppe. Dann ist das [[Zentrum]] $Z(G)$ von $G$ ebenfalls nichttrivial, besteht also aus mindestens $p$ Elementen.[^1]

**Beweis:**
Wir stellen die Klassengleichung auf. Sei $R$ ein Repräsentantensystem der Konjugationsklassen von $G$, die aus mehr als einem Element bestehen. Die [[Klassengleichung]] hat dann die Form
$$|G| = |Z(G)|+ \sum_{g \in R}(G:C_G(g))$$
$|G|$ ist durch $p$ teilbar. Die $(G:C_G(g))$ teilen $|G|$ und sind größer als $1$, sind also auch durch $p$ teilbar. In Folge muss $|Z(G)|$ auch größer $1$ und durch $p$ teilbar sein.
Damit ist $Z(G)$ nicht-trivial.



## Klassifikation von $p^2$
Sei $p$ eine Primzahl. Dann ist jede Gruppe der Ordnung $p^2$ [[Abelsche Gruppe|abelsch]]. 

## Auflösbarkeit
Jede $p$-Gruppe ist [[Auflösbare Gruppe|auflösbar]][^2]

#Carter #Algebra 

[^1]: Gerkmann - Satz 9.14
[^2]: Gerkmann - Satz 9.17