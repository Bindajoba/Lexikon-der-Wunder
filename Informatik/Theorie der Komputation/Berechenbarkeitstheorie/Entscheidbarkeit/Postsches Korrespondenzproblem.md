## Beschriebung
Das Postsche ist ein einfaches aber [[Entscheidbare Sprache|unentscheidbares]] Problem.
Kann man eine Menge von Dominos so aneinander hängen, dass oben und unten das gleiche Wort steht?
![[PCP Domos.png]][^1]



## Definition
Sei ein Alphabet $\Sigma$ und eine (endliche) [[Folge]] von Wortpaaren $K = \{(x_1, y_1), ..., (x_k, y_k)\}$ mit $x_1, y_i \in  \Sigma^+$.

Das **Postsche Korrespondenzproblem** (**k**) ist die Frage, ob es für die gegebene Folge $K$ eine Folge von Indizes $i_1, ..., i_m$ mit $i_j \in \{1, ..., k\}$ gibt, sodass $x_{i_1}...x_{i_m} = y_{i_1}...y_{i_m}$

### Modifiziertes Postsches Korrespondenzproblem
(x_k, y_k)\}$ mit $x_1, y_i \in  \Sigma^+$.

Das **Modifizierte Postsche Korrespondenzproblem** (**k**) ist die Frage, ob es für die gegebene Folge $K$ eine Folge von Indizes $i_1 = 1$ und $i_2, ..., i_m$ mit $i_j \in \{1, ..., k\}$ gibt, sodass $x_{i_1}...x_{i_m} = y_{i_1}...y_{i_m}$

## Eigenschaften
Das **Postsche Korrespondenzproblem** und des **Modifizierte Postsche Korrespondenzproblem** sind [[Entscheidbare Sprache|unentscheidbar]] aber trotzdem [[Semientscheidbare Sprache|semi-entscheidbar]]

### Binäres PCP
Das **Postsche Korrespondenzproblem** über dem Alphabet $\Sigma$ mit $|\Sigma| = 2$ ist unentscheidbar

### Unäres PCP
Das **Postsche Korrespondenzproblem** über dem Alphabet $\Sigma$ mit $|\Sigma| = 1$ ist entscheidbar

### PCP mit k Spielsteinen
- Das **Postsche Korrespondenzproblem** zu einer Folge $K$ der Länge 1 oder 2 ist entscheidbar
- Das **Postsche Korrespondenzproblem** zu einer Folge $K$ der Länge $\geq 5$ ist unentscheidbar
- Die Enscheidbarkei des **Postschen Korrespondenzproblems** zu einer Folge $K$ der Länge 3 oder 4 ist bisher [[PCP 3-4 Steine|unbekannt]].

## Beispiel
![[PTP.png]]



#FSK 

[^1]: https://www.youtube.com/watch?v=VZNN1OGoqr8