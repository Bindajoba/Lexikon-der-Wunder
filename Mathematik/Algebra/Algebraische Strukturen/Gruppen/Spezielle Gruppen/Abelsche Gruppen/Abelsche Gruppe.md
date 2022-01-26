## Beschreibung
Eine **Abelsche Gruppe** (auch **kommutative Gruppe**) ist eine [[Gruppe]], bei der es egal ist, in welcher Reihenfolge man die [[Transformation|Transformationen]] anwendet

Die Operation in einer abelschen Gruppe wird üblicherweise mit $+$ beziechnet.

## Definition
Eine Gruppe $G$ ist kommutativ, wenn für alle Elemente $f, g \in G$ gilt
$$fg=gf$$
Die Operation in einer abelschen Gruppe wird üblicherweise mit $+$ bezeichnet.

## Eigenschaften
In **Abelschen Gruppen** gilt
$$(g*h)^n = g^n*h^n$$

### Multiplikationstafel
Die [[Multiplikationstafel]] einer Abelschen Gruppe ist immer an der Diagonalen symmetrisch.

### Cayley Diagramm
Eine Gruppe ist abelsch wenn $AB = BA$ gilt.
Folgt man ein einem Cayley-Diagramm erst einem roten und dann einem blauen Pfeil, sollte man beim gleichen Knoten herauskommen, wie wenn man erst einem blauen und dann einem roten Pfeil folgt.

### Produkt aus Zyklischen Gruppen
Carter impliziert, dass Abelsche Gruppen immer eine [[Zyklische Gruppe]] oder ein Produkt einer Zyklischen Gruppe ist

### Lemma 6.6
Sei $G$ eine abelsche Gruppe, seien $s \in \mathbb{N}_0, m_1, ..., m_s \in \mathbb{N}$ und $g_1, ..., g_s \in G$ mit $ord(g_i) | m$ für $1 \leq i \leq s$ Sei $U = \langle g_1, ..., g_s\rangle$. Dann gibt es einen surjektiven Gruppenhomomorphismus $\phi: \mathbb{Z} / m_1\mathbb{Z} \times ... \times \mathbb{Z} / m_s\mathbb{Z} \to U$ mit
$$\phi(\bar a_1, ..., \bar a_s) = a_1g_1 + ... + a_sg_s \text{ für alle } a_1, ..., a_s \in \mathbb{Z}$$

Ist $G$ eine abelsche Gruppe mit $G[p] = G$, dann gibt es eine Abbildung $\cdot: \mathbb{F}_p \times G \to G$ mit $\bar a \cdot g = ag$ für alle $a \in\mathbb{Z}$ und $g \in G$. Mit dieser Abbildung wir auf $G$ die Struktur eines $\mathbb{F}_p$-Vektorraums definiert

*Ich denke, dieses Lemma ist dazu du um Angst zu machen. Ich lese mir nicht alles durch, was da steht. Für so etwas sind aber anscheinend Lemmata da.*



## Beispiele
Die Gruppe aller Verschiebungen auf der rellen Achse ist abelsch, da es egal ist, in welcher Reihenfolge ich Verschiebungen durchnehmen soll.


#Arnold #Algebra #Carter 