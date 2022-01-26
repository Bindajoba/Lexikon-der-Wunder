# Definition
Sei $G$ eine [[Abelsche Gruppe]] und $m \in \mathbb{N}$
1. Man nennt $G[m] = \{g \in G: mg = 0_G\}$ die **$m$-Torsionsgruppe** von $G$
2. Die Teilmenge $Tor(G) = \bigcup_{n\in \mathbb{N}} G[n]$ wird die **Torsionsuntergruppe** von $G$ genannt[^1]

*Die Torsionsgruppe ist so etwas wie der Zyklische Anteil einer Gruppe.*

## Torsionsfreiheit
Sei $G$ eine [[Endlich Erzeugte Gruppe|endlich erzeugte]] abelsche Gruppe
1. Wir bezeichnen $G$ als **torsionsfrei**, wenn $Tor(G) = \{0_G\}$ gilt
2. Die Gruppe $G$ ist frei, wenn für ein $r \in \mathbb{N}_0$ ein Isomorphismus zwischen $G$ und $(\mathbb{Z}^r, +)$ existiert, wobei $\mathbb{Z}^0 = \{0\}$ gesetzt wird

Jede **freie Gruppe** ist auch **torsionsfrei** (*und wie ich glaube, umgekehrt*)


# Eigenschaften
### Zerlegung von Torsionsuntergruppen
Sei $G$ eine abelsche Gruppe
1. Sind $m, n$ [[Teilerfremdheit|teilerfremd]], dann gilt $G[mn] \cong G[m] \times G[n]$
2. Sei $n\in \mathbb{N}$ mit $G[n] = G$, und sei $n = \prod_{i=1}^r p_i^{e_t}$ die [[Primfaktorenzerlegung]] von $n$
Dann ist $G[p_1^{e_1}] \times ... \times G[p_r^{e_r}]$[^2]


#Algebra 

[^1]: Gerkmann - Definition 6.2
[^2]: Gerkmann - Satz 6.7