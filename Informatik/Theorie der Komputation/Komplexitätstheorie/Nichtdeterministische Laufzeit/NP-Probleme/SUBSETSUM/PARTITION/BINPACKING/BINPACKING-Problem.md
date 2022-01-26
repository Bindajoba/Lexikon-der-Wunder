Gegeben: Natürliche Zahlen $a_1, a_k \in \mathbb{N}$, die Behältergröße $b \in \mathbb{N}$ und die Anzahl der Behälter $m$

Gefragt: Gibt es eine totale Funktion $assign: \{1, ..., k\} \to \{1, ..., m\}$, sodass für alle $j \in \{1, ..., m\}$ gilt: $\sum\limits_{assign(i) = j} a_i \leq b$
Kann man alle gegebenen Zahlen so auf die Behäter aufteilen, sodass keiner der Behälter überläuft?

## Eigenschaften
- BINPACKING ist [[NP-Vollständigkeit|NP-vollständig]]
Das folgt aus [[Reduktion (Sprache)|Reduktion]] vom [[PARTITION-Problem]]