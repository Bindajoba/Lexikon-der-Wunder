# Koncret
Ich wurde gefragt, wie viele Gruppen mit Ordnung $2022$ gibt. Da ich mich als einen Gruppenexperten bezeichnen würde, denke ich, dass ich der Frage gewachsen bin.

Bezeichne die zu untersuchende Gruppe mit $G$.

# Sylowgruppen
$2022$ zerfällt in die Primfaktoren $2, 3, 337$.
Damit gibt es eine Untergruppen der Ordnung $2, 3, 337$.
Relevant ist aber vorerst $337$. Wir wollen zeigen, dass es nur eine einzige solche Gruppe gibt.

# 337 Normalteiler 
Es gilt $2022 = 6 \cdot 337$. Nach dem 3ten Sylowsatz gilt für die Anzahl $\nu_{377}$ der $337$-Sylowgruppen:
$\nu_{377} \equiv_{377} 1$ und $\nu_{377} \mid 6$
Also gibt es nur eine Untergruppe der Ordnung $377$. Diese Untergruppe, nennen wir sie $N_{377}$ ist damit Normalteiler von $G$.

Unsere Gruppen mit Normalteiler haben eine spezielle Eigenschaft. Sie wird in $6$ Nebenklassen mit $337$ Elementen aufgeteilt. Diese Nebenklassen bilden eine Faktorgruppe, die isomorph zu einer Gruppe der Ordnung $6$ ist.
Die Gruppe hat also diese grobe Struktur:
![[Gruppe 2022 Calyey I.png]]
*Es sind noch keine Beziehungen zwischen den Nebenklassen eingezeichnet, darum kümmern wir uns jetzt.*

# Erster Versuch mit direkten Produkten Gruppen zu finden
Wir nehmen an, jede Nebenklasse ist eine exakte Kopie von $N$. Damit meine ich, dass man beim Anwenden des Gruppeneements, dass das oberen Pinke Element auf das obere Blaue Element alle anderen Elemente genauso abbildet, sodass diese netten Parallen entstehen.  
![[Gruppe 2022 Cayley.png]]
Diese Voraussetzung muss nämlich nicht unbedingt erfüllt sein. Wir wollen uns aber zuerst auf diese unkomplizierte Gruppen beschränken. Die Gruppen mit der oberen Eigenschaft sind genau die Gruppen, die aus dem direkten Produkt entstehen.
Es gibt $2$ Gruppen der Ordnung $6$: $C_6 = C_2 \times C_3$ und $S_3$ (Die Diedergruppe ist gleich der Symmetrischen Gruppe)

## Verwenden der Zyklischen Gruppe $C_6$
In dem Fall verbinden sich die $6$ Nebenklassen wie folgt:
![[Gruppe 2022 Zyklisch Cayley.png]]
Wir erhalten die Gruppe $C_6 \times C_{377} = C_{2022}$. 

## Verwenden der Symmetrischen Gruppe $S_3$
Die $6$ Nebenklassen verbinden sich zu:
![[Grupp 2022 S3 Cayley.png]]
Wir erhalten die Gruppe $S_3 \times C_{337}$

# Mit Semidirekten Produkten Gruppen finden
Die andere Möglichkeit mehr Gruppen zu erzeugen, ist das Semidirekte Produkt zu verwenden.
Dafür ist die Automorphismengruppe von $N = C_{337}$ wichtig.

Jeder Automorphismus $\phi$ einer Gruppe wird durch den Erzeuger dieser eindeutig definiert. Sei $g \in C_{337}$ ein solcher Erzeuger.
Damit gibt es für jedes mögliche Bild $\phi(g) \in C_{377}$ maximal einen Automorphismus.
Bezeichne die möglichen Automorphismen mit $\phi_1, ..., \phi_{377}$ und es gelte $\phi_i(g) = g^i$.
Offensichtlich ist $\phi_{377}$ kein Automorphismus, da $\phi_{377}(g) = e$, was bedeutet $\phi_{337}(C_{337}) = \{e\}$ (womit $\phi_{377}$ nicht bijektiv ist).
Alle anderen $\phi_i$ sind aber bijektiv, da $\phi_i(g) = g^i$ mit $i \in \{1, ..., 336\}$ ein Erzeuger von $C_{337}$ ist. 
Durch das Potenzieren der Eingabe $\phi_i(g^j) = (g^i)^j$ erhält man jedes Element der Gruppe $C_{337}$.

Welche Struktur hat aber die Automorphismengruppe?
Betrachte dazu folgendes Analogon. Die Menge $C_{337}$ ist isomorph zu $\Z/337\Z$, was ein Körper ist.
Das Analogon der Gleichung $\phi_i(g) = g^i$ ist in $\Z/337\Z$ die Gleichung $i \cdot 1 = i$. Die Automorphismengruppe von $C_{377}$ ist daher isomorph zur Multiplikationsgruppe von $\Z/337\Z$. Dieser ist zyklisch und von der Ordnung $336$.

Führe schon mal die Primfaktorenzerlegung durch, die wird vermutlich später wichtig: $336 = 2\cdot 168 = 2^4 \cdot 21 = 2^4 \cdot 3 \cdot 7$

Sei $U_6$ eine noch nicht näher definierte Gruppe von Ordnung $6$. Ein Semidirektes Produkt $N\rtimes_\psi U_6$ benutzt einen Homomorphismus $\psi$, der von $U$ in $Aut(C_{337}) \cong C_{336}$ abbildet.
$U_6$ ist als Gruppe mit Ordnung $6$ isomorph zu $C_6$ oder $S_3$. Gehe beide Fälle ab:

## $U_6$ ist zyklisch $C_6$ 
Finde alle Homomorphismen $\psi: C_6 \to Aut(C_{337})$.
Wie vorhin können wir die Tatsache ausnutzen, dass $C_6$ durch ein Element, nennen wir es $g$ erzeugt wird. Ein Homomorphismus ist durch das Bild von $g$ eindeutig.
Ein Homomorphismus $\psi$ muss die Eigenschaft $\psi(g)^6 = \psi(g^6) = \psi(e) = id$ erfüllen.
Damit muss der Automorphismus $\psi(g)$ von Ordnung $6, 3, 2, 1$ sein.

Bestimme nun alle möglichen Bilder von $g$, klassifiziert nach Ordnung $1, 2, 3, 6$.
- Ordnung $1$:
$\psi(g)^1 = id \iff \psi(g) = id$
- Ordnung $2$
$Aut(C_{337}) \cong C_{336}$ hat $\varphi(2) = 1$ Element von Ordnung $2$.
Wendet man die obere Analogie mit der Multiplikationsgruppe an und löst der Gleichung $n^2 \equiv_{337} 1$ mit Processing, dann erhält man die zwei Lösungen $1$ und $336$. Somit ist $\phi^{336}$ der einzige Automorphismus der Ordnung $2$.
- Ordnung $3$
Das gleiche Verfahren für Ordnung $3$ gibt uns $2$ Automorphismen $\phi^{128}, \phi^{208}$
- Ordnung $6$
Das gleiche Verfahren für Ordnung $6$ gibt uns $2$ weitere Automorphismen $\phi^{129}, \phi^{209}$


Wir erhalten damit die beiden Semidirekte Produkte $C_{337}\rtimes_{\psi_{56}} C_6$ und $C_{337}\rtimes_{\psi_{280}} C_6$. (Ich habe die Befürchtung, die beiden Semidirekten Produkte ergeben isomorphe Gruppen).

### Das Semidirekte Produkt $C_{337}\rtimes_{\psi_{128}} C_6$
Wie sieht der Cayley-Graph eines Semidirekten Produkts aus? Das ist gar nicht so kompliziert. Wir nehmen alle Elemente des Normalteilers $C_{377}$ und kopieren sie auf $6$ Nebenklassen. 
Wobei, um zu erklären, wie Nebenklassen in Cayley-Diagramme funktionieren, bräuchte ich vermutlich noch einige Stunden mehr.
Hier, so sieht das Produkt aus:
![[Gruppe6.png]]
*Jeder Kreis sieht anders aus, da $\psi_{129}$ Ordnung $6$ hat und daher erst ab $\psi^6 = id$*.

## Das Semidirekte Produkt $C_{337}\rtimes_{\psi_{128}} C_6$

*Besteht im Gegensatz zum oberen Bild nur aus $3$ gleichen Mustern.*

## Das Semidirekte Produkt $C_{337}\rtimes_{\psi_{336}} C_6$
![[Gruppe2.png]]
*Sehr langweilig, aber leicht zu verstehen!*

# $U_6$ ist die Symmetrische Gruppe $S_3$
Wie gerade können wir den Automorphismus eindeutig bestimmen, indem wir die Bilder des Erzeugers von $S_3$ definieren. Einen Erzeuger erhalten wir durch einen $3$-Zykel $g$ und einen $2$-Zykel $h$.
Wie vorhin gibt es aber Einschränkungen bezüglich der Automorphismen, auf die wir $g, h$ abbilden können. Das Bild von $g$ muss Ordnung $1, 3$ haben, das Bild von $h$ hingegen $1, 2$.

Ich kürze ab.
Ich behaupte, dass es nicht möglich ist, $g$ auf einen $3$ Zykel und $h$ auf einen $2$-Zykel abzubilden. Denn dann gäbe es einen Isomorphismus in eine Untergruppe der Form $C_3 \times C_2 \cong C:6$ womit, aber $S_3 \cong C_6$, was ein Widerspruch ist.



## Der Automorphismus $\psi(g) = \phi_{128}, \psi(h) = id$
Wir erhalten einen Widerspruch, da $\phi_{208} = \psi(hg^2h)=\psi(g) = \phi_{128}$.
Der Widerspruch kommt vermutlich daher, dass $C_2$ kein Normalteiler von $S_3$ ist.

## Der Automorphismus $\psi(g) = id, \psi(h) = \phi_{336}$
Diesmal klappt alles und wir bekommen die Gruppe:
![[GruppeS3.png]]
*Man muss noch Pfeile wie bei der Symmetrischen Gruppe üblich eintragen.*