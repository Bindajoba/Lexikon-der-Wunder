## Beschreibung
Die **Chomsky-Normalform** fordert eine spezielle Form der Produktionen einer [[Kontextfreie Grammatik]]. Die Chomsky-Normalform erleichtert die Formulierung von Algorithmen.
Sie ist benannt nach [[Noam Chomsky]]

## Definition
Eine [[Kontextfreie Grammatik]] ist in **Chomsky-Normalform**, wenn Produktionen die Form
- $A\to a \in P$ (mit $a \in \Sigma$)  
- $A \to BC$ (mit $B, C \in V$) 

haben.[^1]

## Konstruktion
Jede [[Kontextfreie Grammatik]] kann auf folgende Weise in Chomsky-Normalform gebracht werden:
- [[Kontextfreie Grammatik|Entferne die Einheitsproduktionen]]
- Ersetze Alle Terminalsymbole $a$, die auf der rechten Seite, aber nicht allein stehen durch eine Variable $A_a$ und füge die Produktion $A_a \to a$ hinzu
- Übrig bleiben die Produktionsformen $A \to a$ und $B \to B_1...B-n$
Zerlege die Produktion $B \to B_1...B-n$ durch Einführen neuer Variablen:
$B \to B_1C_1$, $C_1 \to B_2C_2$, ..., $C_{n-2} \to B_{n-1}C_{n-1}$, $C_{n-1} \to B_{n-1}$

![[Chomsky-Normalform KonstruktionKonstruktion.png]][^3]

## Eigenschaften
### Ableitung
Die [[Ableitung eines Wortes]] nimmt in der Chomsky-Normalform das Aussehen eines Binärbaumes an. 
![[Chomsky-Normalform Baum.png]][^2]

#FSK 

[^1]: Sabel - Definition 5.2.1
[^2]: Sabel - Beispiel 5.2.3
[^3]: Sabel - 5.2.2