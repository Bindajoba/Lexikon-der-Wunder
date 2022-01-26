## Beschreibung
Für einen [[Ungerichteter Graph|Graphen]] $G=(V, E)$ ist $V' \subseteq V$ eine **überdeckende Knotenmenge**, wenn jede Kante aus $E$ mindestens einen Knoten in $V'$ hat, d.h. für alle Knoten $u, v \in V: \{u, v\} \in E \implies u \in V' \vee v\in V'$

![[Überdeckende Knotenmenge.png]]

## Eigenschaft
- $G$ hat genau dann eine Überdeckende Knotenmenge der Größe $k$ wenn $G$ eine [[Unabhängige Knotenmenge]] der Größe $|V|-k$