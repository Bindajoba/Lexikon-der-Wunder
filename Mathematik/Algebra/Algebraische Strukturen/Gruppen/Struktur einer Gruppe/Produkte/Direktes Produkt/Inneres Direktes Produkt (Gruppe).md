# Definition
Sei $G$ eine Gruppe und seien $U,N$ Untergruppen von $G$. Wir bezeichnen das [[Komplexprodukt]] $G$ als **inneres direktes Produkt** von $U$ und $V$, wenn $U$ und $N$ beides [[Normalteiler]] von $G$ sind und $G = UN$ sowie $U \cap N = \{e\}$ gilt.

*Das Produkt ist inner, weil das Ergbnis wieder in $G$ liegt. Es ergibt aber das gleiche Ergebnis wie [[Äußeres Direktes Produkt (Gruppe)]].*

# Eigenschaft
## Eindeutige Zerlegung
Sei $g \in UN$. Dann gibt es nur ein $u \in U$ und ein $n \in N$ sodass $g = un$

## Isomorphie zum Äußeren Produkt
Existiert ein Inneres Produkt, so ist dies Isomorph zum [[Äußeres Direktes Produkt (Gruppe)|Äußeren Produkt]]:
$$UN \simeq  U\times N$$
# Aufgaben
## Klausur 2019 Aufgabe 4
Sei $G$ eine Gruppe der Ordnung $33$, $P$ eine Normalteiler der Ordnung $3$ und $Q$ ein Normalteiler der Ordnung $11$.

Weisen Sie nach, dass $G$ ein inneres Produkt aus $P$ und $Q$ ist.
$P, Q$ sind Normalteiler von $G$, also gilt $PQ = QP$ und $PQ$ ist eine Untergruppe von $G$.
Die Gruppen haben Primzahlordnung und sind damit zyklisch. Es gilt $ggT(3, 11) = 1$ und damit $P \cap Q = \{e\}$. 
Desweiteren sind $P, Q$ Normalteiler von $G$ und damit auch von der Untergruppe $PQ \supseteq P, Q$. 
Das Komplexprodukt $PQ$ ist damit ein inneres dir. Produkt von $P$ und $Q$ und Untergruppe von $G$.
Als direktes Produkt, (welches isomorph zum äußeren Produkt ist, welches auf der Gruppe des kartesischen Produkts von $P, G$) ist $|PQ| = 3 \cdot 11 = 33 = |G|$, d.h. $PQ = G$.





#Algebra 