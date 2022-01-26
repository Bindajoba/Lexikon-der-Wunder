## Beschreibung
Die **n-te Zyklische Gruppe** ist die Menge aller Kongruenzrotationen eines [[Regelmäßiges Polygon|regelmäßigen n-Ecks]].

Sie wird manchmal mit $C_n$ und manchmal mit $\mathbb{Z}_n$ beschrieben.

Sie Elelemte der zyklischen Gruppe werden durch Potenzen von $a$ geschrieben:
$$C_n = \{e, a, ..., a^n\}$$[^1]

## Definition
### Definition Gerkmann
Wird eine [[Gruppe]] von einem Element [[Erzeugendensystem|erzeugt]], wird sie Zyklisch genannt.

Eine endliche zyklische Gruppe besteht aus den Elementen
$$e_G, g, g^2, ..., g^{n-1}$$

### Unendliche zyklische Gruppe
Siehe [[Unendliche Zyklische Gruppe]]

### Endliche zyklische Gruppe
Siehe [[Endliche Zyklische Gruppe]]

## Eigenschaften
### Inverse
Für ein Element $a^k$ ist das Inverse $(a^k)^{-1} = a^{n-k}$

### Untergruppe
Jede [[Untergruppe]] einer Zyklischen Gruppe ist zyklisch.
 

Genauer: Hat die zyklische Gruppe $G$ eine Ordnung von $n$, dann ist jede Untergruppe entweder $\{e\}$ oder hat die Ordnung $m$, wobei $m$ ein Teiler von $n$ ist.[^2]

## Homomorphismen
Sei $G$ eine zyklische Gruppe, $g\in G$ ein erzeugendes Element, $H$ eine weitere Gruppe und $h \in H$
Ist $ord(g) = \infty$ oder $ord(g)$ endlich und ein Vielfaches von $ord(h)$, dann existiert ein (eideutig bestimmter) Gruppenhomomorphismus $\phi: G \to H$ mit $\phi(g) = h$

*Das heißt, dass ein [[Gruppenhomomorphismus]] eine zyklische Gruppe mit Ordnung $n$ immer auf eine andere zyklische Gruppe mit der Ordnung eines Teilers von $n$ abbildet.*
*Ist $G$ aber unendlich groß, dann kann ich $G$ auf jede andere Zyklische Gruppe abbilden. Entweder eine unendliche oder eine unendliche, wobei man G dann bildlich um die Uhr von $H$ wickelt*[^3]

### Kommutativität
Jede Zyklische Gruppe ist auch eine [[Abelsche Gruppe]]

#Carter #Algebra 

[^1]: Carter - Aufgabe 4.25 
[^2]: Gerkmann - Satz 3.5
[^3]: Gerkmann - Proposition 3.11