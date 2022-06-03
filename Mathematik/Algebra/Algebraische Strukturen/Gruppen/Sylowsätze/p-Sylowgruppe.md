# Beschreibung
Teile die Ordnung einer Gruppe $|G|$ in [[Teilerfremdheit|teilerfremde]] [[Primzahl|Primzahlpotenzen]] auf (die Exponenten sind dann maximal).
Eine [[P-Gruppe|p-Untergruppe]] mit der Ordnung einer solchen Primzahlprtenz wird **p-Sylowgruppe** genannt.[^1]

# Eigenschaften
## Normalteiler
Aus den [[Sylowsätze]] folgt:
Eine $p$-Sylowgruppe ist genau dann ein Normalteiler von $G$, wenn die Anzahl $\nu_p$ der $p$-Sylowgruppen von $G$ gleich $1$ ist.

## Sylowsätze
Siehe [[Sylowsätze]]


# Übungen
## Klausur 2016 Aufgabe 4
![[Klausur 2016 Aufgabe 4.png]]

### a)
Für die Anzahl der Sylowgruppen $\nu_3$ gilt $\nu_3 \mid 17$ und $\nu_3 \equiv_3 = 1 \implies \nu_3 = 1$.
Für $\nu_{17}$ gilt $\nu_{17} \mid 9 \implies \nu_3 \in \{1, 3, 9\}$ und $\nu_{17} \equiv_{17} 1 \implies \nu_{17} = 1$.

### b)
Das Komplexprodukt $UV$ ist Untergruppe von $G$. Da $U$ und $V$ die einzigen Sylowgruppen sind, sind sie Normalteiler. Desweiteren schneiden sie sich nur in $e$, denn alle Elemente vo $V$ außer $e$ haben Ordnung $17$, $U$ kann aber keine Elemente von Ordnung $17$ haben, da daraus folgen würde $17\mid 9$.
Nach Vorlesung ist $UV$ damit isomorph zum Produkt $U \times V$ und hat $|UV| = |U\times V| = |U|\cdot|V| = 9 \cdot 17 = |G|$ Elemente. Daher muss $UV = G$ sein.

### c)
Das direkte Produkt zweier abelscher Gruppen ist abelsch. $U$ ist als Gruppe von Ordnung $3^2$ (3 Primzahl) nach VL abelsch und $U$ hat Primzahlordnung, d.h. ist zyklisch und abelsch.




#Algebra 

[^1]: Gerkmann - Definition 10.3