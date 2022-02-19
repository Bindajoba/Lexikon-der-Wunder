TARGET DECK: Universität::Informatik::Betriebssysteme

# Beschreibung
Petri-Netze sind zur Modellierung von nebenläufigen, assynchronen [[Prozess|Prozessen]] geeignet. Sie veranschaulichen Vorgänge und ermöglichen eine Ableitung von Eigenschaften des modellierten Systems.
Zum Beispiel kann damit Formalisiert werden, wann ein System in eine [[Verklemmung]] kommt.

Q: Was ist ein Petrinetz?
A: Ein Graph, um Nebenläufige Systeme zu modellieren und visualisieren.
<!--ID: 1642897214749-->


# Definition
## Netz
Sei $X = (S \cup T, F)$ ein [[Graph|endlicher Graph]] mit $S \cap T \neq \emptyset$
Dann heißt $X$ Netz genau dann, wenn
1. $S$ eine endliche Menge $S = \{s_1, ..., s_m\}$ von **Stellen**,
2. $T$ eine endliche Menge $T = \{t_1, ..., t_n\}$ von **Transitionen**
3. $F \supseteq (S \times T) \cup (T \times S)$ eine Menge von Kanten, die nur zwischen Stellen und Transitionen verlaufen

*Wenn man die Transitionen als Beschriftungen von Kanten bezeichnet, die beliebig viele Stellen mit beliebig vielen anderen Stellen verbindet, wird das Netz zu einer Verallgemeinerung eines Graphen*

## Stellen/Transitions-System
Ein Stellen/Transitions-System ist ein 6-Tupel $Y= (S, T, F, K, W, M_0)$ bestehend aus einem Netz $(S \cup T, F)$ sowie den Abbildungen
1. $K: S \to \mathbb{N} \cup \{\infty\}$, durch die jeder Stelle eine Kapazität zugeordnet wird
2. $W: S \to \mathbb{N}$, durch die jeder Kante ein Kantengewicht zugeordnet wird
3. $M: S \to \mathbb{N}$ ([[Markierung]]), durch die jeder Stelle eine Anzahl von Marken (Token) zugeordnet wird.
*Werden die Stellen nummeriert, so kann die aktuelle Markierung durch einen Vektor dargestellt werden.*

Dabei kann eine Stelle nie mehr Marken aufnehmen als ihre Kapazität erlaubt, d.h. $M(s) \leq K(s)$ für alle $s\in S$
$M_0$ heißt [[Anfangsmarkierung]] und stellt die Markierung dar, wie sie zu Beginn des durch das **Petri-Netz** modellierten Prozesses vorliegt.

Q: Welche zwei Arten von Knoten hat ein Petri-Netz?
A: - Stelle
- Transition
<!--ID: 1642897214905-->


# Beziehung zu Prozessen
Die Stellen eines Petri-Netzes repräsentieren z.B. Signale Daten, Speicher eines Objekts. Beim Speichern kann die Anzahl der Marken beispielsweise die ANzahl der im Speicher vorhandenen Objekte repräsentieren.
Die Transitionen des Objekts repräsentieren z.B. Ereignisse, Vorgänge, Berechnungsschritte oder Jobs, d.h. Aktionen.

## Modellierung von Exklusivem Zugriff
Will man exklusiven Zugriff modellieren, kann man das machen, indem man eine Stelle hinzufügt, die eine Marke hat, wenn gerade nicht auf die Ressource hinzugefügt wir und sonst leer ist.

# Beispiel
## Beispiel Kaffemaschine
Frau Linnhoff stellt sich Petrinetze gerne mit einer Kaffeemaschine vor Das Petrinetz sieht so aus:

![[Petrinetz Beispiel.png]]

Man erkennt mehrere Sachen am Bild:
- Die grünen Zahlen über den Stellen ist die Kapazität
- Die grünen Zahlen über den Transitionen sind das Kantengewicht
- Die Kugeln sind die Marken

Wendet man eine Transition an, z.B. starken Kaffe brühen, dann wird eine Markierung aus dem Wasser, zwei aus dem Kaffe und eine aus der Tasse entfernt. Außerdem wird eine volle Tasse der Kaffetasse hinzugefügt.

# Siehe auch
- [[Erreichbarkeitsgraph]]

#Betriebssysteme 