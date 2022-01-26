# Beschreibung
Die **Faktorgruppe** oder **Quotientengruppe** ist die Gruppe die man erhält, wenn man eine Gruppe durch einen seiner [[Normalteiler]] teilt.

Diese Operation ist das Gegenstück zum [[Äußeres Direktes Produkt (Gruppe)|Direkten Produkt]], vielleicht zum [[Inneres Direktes Produkt (Gruppe)|Inneren Direkten Produkt]] und zum [[Semidirektes Produkt|Semidirektes Produkt]]

# Definition
Sei $G$ eine [[Gruppe]] und $N$ ein [[Normalteiler]], Dann ist die Menge $G/N$ der [[Nebenklasse|Linksnebenklassen]] mit der [[Verknüpfung auf Nebenklassen (Gruppe)|Verknüpfung]] $gN \cdot hN = (gh)N$ eine Gruppe, die sogenannte **Faktorgruppe** von $G$ modulo $N$.[^1]


## Kanonischer Epimorphismus
Siehe [[Kanonischer Epimorphismus (Gruppe)]]

# Intuition
Die **Faktorgruppe** heißt Wahrscheinlich so, weil sie ein Faktor beim Produkt zweier Gruppen ist.
Hintergrund ist die Tatsache, dass die Gruppe in [[Nebenklasse|Nebenklasse]] einer [[Untergruppe]] zerlegbar ist. Sind die Rechts- und Linksnebenklassen gleich, d.h. die Untergruppe ist ein [[Normalteiler]], so bilden die Nebenklassen eine Gruppe.

![[Faktorgruppe Intuition.png]]
Im oberen Bild ist klar die [[Zyklische Gruppe]] $C_3$ erkennbar.

# Eigenschaften
## Isomorphiesätze
Sei $G$ eine [[Gruppe]] $N \trianglelefteq G$ und $U$ eine [[Untergruppe]] von $G$
1. Dann ist $N \cap U$ ein [[Normalteiler]] von $U$, und es gilt $U/(N\cap U ) \cong (UN)/N$
2. Ist auch $U \triangleleft G$ und gilt $U \supseteq N$, dann gilt $G/U \cong (G/N)/(U/N)$[^2]

Siehe [[Gruppenisomorphismus]]


#Algebra 

[^1]: Gerkmann - Satz 5.9
[^2]: Gerkmann - Satz 4.24