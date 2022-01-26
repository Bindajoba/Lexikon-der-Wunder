## Beschreibung
Die **Kuroda-Normalform** fordert eine spezielle Form der Produktionen einer [[Kontextsensitive Grammatik]]. Die Chomsky-Normalform erleichtert die Formulierung von [[Algorithmus|Algorithmen]].
Sie ist benannt nach [[Sige-Yuki Kuroda]]

## Definition
Eine [[Kontextsensitive Grammatik]] $G=(V, \Sigma, P, S)$ ist in **Kuroda-Normalform**, wenn die Produktionen die Form
- $A\to a \in P$
- $A \to B$
- $A \to BC$
- $AB \to CD$

haben, wobei $a \in \Sigma$ und $A, B, C, D \in V$[^1]

## Konstruktion
Jede [[Kontextsensitive Grammatik]] kann auf folgende Weise in Chomsky-Normalform gebracht werden:
- Ersetze Alle Terminalsymbole $a$, die auf der rechten Seite, aber nicht allein stehen durch eine Variable $A_a$ und füge die Produktion $A_a \to a$ hinzu
- Übrig bleiben die Produktionsformen $A \to a$, $A \to B_1...B-n$ und $A_1...A_n \to B_1...B_m$
[[Kontextsensitive Grammatik#Aufteilen der rechten Seite|Zerlege die Produktion]] $A \to B_1...B-n$ durch Einführen neuer Variablen
- [[Kontextsensitive Grammatik#Aufteilen beider Seite|Zerlege die Produktion]] $B \to B_1...B_m$ durch Einführen neuer Variablen
- Übrig bleiben Produktionen der Form $A \to a$, $A \to B_1B_2$, $A_1A_2 \to B_1B_2$ und $A_1A_2 \to B_1...B_m$
[[Kontextsensitive Grammatik#Aufteilen der rechten Seite zwei Variablen links|Zerlege die rechte Seite der letzten Form]].

Dann erhält man die Kuroda-Normalform

![[Kuroda-Normalform Algorithmus.png]]

## Eigenschaften
### Ableitung
Die [[Ableitung eines Wortes]] nimmt in der Chomsky-Normalform das Aussehen eines Binärbaumes an. 
![[Chomsky-Normalform Baum.png]][^2]

#FSK 