## Beschreibung
Die **Greibach-Normalform** fordert eine spezielle Form der Produktionen einer [[Kontextfreie Grammatik]]. Die Chomsky-Normalform erleichtert die Formulierung von Algorithmen.
Sie ist benannt nach [[Sheila Greibach]]  

## Definition
Eine [[Kontextfreie Grammatik]] ist in **Greibach-Normalform**, wenn Produktionen die Form
- $A\to aB_1B_2...B_n \in P$ (mit $n \in \mathbb{N}_0, a\in \Sigma$ und $B_i\in V$)  
*Bestehen also aus einem Terminal und null oder mehreren Nicht-Terminalen*

haben.[^1]

## Herstellen der Greibach-Normalform
Sei $G$ eine Grammatik in [[Chomsky-Normalform]]
Da $G$ in Chomsky-Normalform ist, hat jede Produktion die Form $A \to BC$
Eine Idee wäre, einfach immer die Produktionsregel auf das erste Nicht-Terminal anzuwenden (siehe [[Kontextfreie Grammatik#Inlining von Produktionen|Inlining von Produktionen]]), bis dieses irgendwann zum Terminal wird. Dann wäre die Greibach-Normalform gegeben.

Es kann allerdings passieren, dass die Produktionen eine Schleife bilden und die Produktionsregeln unendlich oft auf erste Terminal anwendet.

Die richtige Lösung sieht man hier unten. (Bemerkung: die Nicht-Terminale werden durchnummeriert, damit alle einfach referenziert werden können)

![[Greibach-Normalform Algorithmus.png]]

#FSK 

[^1]: Sabel - Definition 5.3.1

