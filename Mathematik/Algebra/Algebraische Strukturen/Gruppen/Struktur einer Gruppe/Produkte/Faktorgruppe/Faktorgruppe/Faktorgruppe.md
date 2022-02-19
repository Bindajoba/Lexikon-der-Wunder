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


# Übungen
## Klausur 2018 Aufgabe 3
![[Klausur 2018 Aufgabe 3.png]]

### a)
$N$ ist eine abelsche Untergruppe und ist damit ein Normalteiler von $G$.
$N$ hat Ordnung $10/2 = 5$.
Es gilt damit die Gleichung 
$$|G|=|G/N||N| \implies 10 = |G/N|5 \implies |G/N| = 2$$
$eN = \{e, g^2, g^4, g^6, g^8 \}$ verschieden zur Nebenklasse $gN = \{g, g^3, g^5, g^7, g^9\}$, was die zwei Elemente der Faktorgruppe sind.

### b)
Sei $\phi (\Z \times \Z) \to \Z/2\Z \times \Z/3\Z, (a, b)\mapsto (a +2\Z, b+ 3\Z)$
Zeige mit dem [[Homomorphiesatz für Gruppen]]
- $\phi$ ist ein [[Gruppenhomomorphismus|Homomorphismus]]
- $\phi$ ist surjektiv.
- $kern(\phi) = 2\Z\times3\Z$

1. $\phi((a,b)+(c,d)) = \phi(a+c, b+d) = (a+c+2\Z, b+d+3\Z) = (a+2\Z, b+3\Z)+(c+2\Z, d+3\Z)$$= \phi((a, b))+\phi((c, d))$
2. Sei $(a+2\Z, b+3\Z) \in\Z/2\Z \times \Z/3\Z$, dann gilt $\phi((a, b)) =(a+2\Z, b+3\Z)$
3. $\phi((a, b)) = 0 \iff (a+2\Z, b+3\Z) = (2\Z, 3\Z) \iff a \in 2\Z, b\in 3\Z \iff (a, b) \in 2\Z\times3\Z$

Also sind nach dem Homomorphiesatz obere Gruppen isomorph.



 
#Algebra 

[^1]: Gerkmann - Satz 5.9
[^2]: Gerkmann - Satz 4.24