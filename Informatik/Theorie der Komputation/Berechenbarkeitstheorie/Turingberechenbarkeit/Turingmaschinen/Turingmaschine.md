## Beschreibung
Eine Turingmaschine ist eine imaginäre Maschine, die ein endliches Wort auf einem unendlich langem Band, auf dem das einzulesende Wort steht.
Die Machine wird durch einen Automaten gesteuert, der in Abhängigkeit zum Buchstaben auf dem Band seinen Zustand wechselt.

Die Turingmaschine kann sogar auf dem Band schreiben.
![[Bild_Turingmaschine.png]]

Die Turingmaschine wurde vom britischen Informatiker [[Alan Turing]] eingeführt

## Definition
 Eine Turingmaschine (TM) ist ein 7-Tupel 
 $$M=(Z, \Sigma, \Gamma, \delta, z_0, \square, E)$$ wobei:
 - $Z$ ist eine endliche Menge von Zuständen
 - $\Sigma$ ist das (endliche) Eingabealphabet
 - $\Gamma \supset \Sigma$ ist das (endliche) Bandalphabet
 - $\delta$ ist die (deterministische/nichtdeterministische) Zustandüberführungsfunktion
 - $z_0 \in Z$ ist der Startzustand
 - $\square \in \Gamma \backslash \Sigma$ ist das Blank-Symbol
 - $E \subseteq Z$ ist die Menge der Endzustände 

Landet die Turingmaschine in einem Endzustand, dann bleibt sie stehen und das Wort wird akzeptiert.
Je nach Zustandsübergangsfunktion kann eine Turingmaschine entweder **deterministisch** (**DTM**) oder **nichtdeterministisch** (**NTM**) sein

### Deterministische Zustandüberführungsfunktion
$\delta$ hat die Form $\delta(z, a) = (z', b, x)$.
Es wird also nur ein Zustand ausgegeben.

Das bedeutet:
Falls die TM im Zustand $z$ ist und das Zeichen $a$ an der aktuellen Position des Schreib-Lesekopfs ist, dann:
- Wechsle in Zustand $z'$
- Ersetze $a$ durch $b$ auf dem Band
- Falls $x=L$: Verschiebe den Schreib-Lesekopf eine Position nach Links
- Falls $x=N$: Lass den Schreib-Lesekopf stehen
- Falls $x=R$: Verschiebe den Schreib-Lesekopf eine Position nach Rechts

### Nicht-Deterministische Zustandüberführungsfunktion
$\delta: (Z \times \Gamma) \to \mathcal{P}(Z \times \Gamma \times \{L, R, N\})$
$\delta$ hat die Form $delta(z, a) = \{(z_1, b_1, x_1), ..., (z_n, b_n, x_n)\}$.
Es werden also mehrere Tupel ausgegeben.

Eine Deterministische Turingmaschine kann in eine Nichtterministische Turingmaschine und umgekehr umgewandelt werden.

### Konfiguration einer Turingmaschine
Eine [[Konfiguration]] einer TM ist ein Wort $k\in \Gamma^* Z \Gamma^*$
Es beschreibt 
- Das Teilwort links neben dem Schreib-Lese-Kopf
- Den aktuellen Zustand
- Das Teilwort rechts neben dem Schreib-Lese-Kopf

Der Schreibkopf steht aber auf dem ersten Symbol der rechten Hälfte. 

Die Startkonfiguration einer TM ist $z_0w$

### Startkonfiguration einer TM
Für ein Eingabewort $w$ ist die Startkonfiguration einer TM mit Startzustand $z_0$ das Wort $z_0w$

### Transitionsrelation
Eine Transitionsrelation ist das Äquivalent zum [[Ableitung eines Wortes#Ableitungsschritt|Ableitungsschritt eines Endlichen Automaten]]. Es ist eine [[Relation]], die beschreibt, wie eine Konfiguration in die nächste übergeht.

Die **Transitionsrelation** $\vdash_M \subseteq (\Sigma^* \times \Gamma^*) \times (\Sigma^* \times \Gamma^*)$ der (deterministischen/nichtdeterministischen) Turingmaschine ist definiert durch die folgenden Fälle:
- $b_1...b_mza_1...a_n \vdash_M b_1...b_mz'ca_2...a_n$, wenn $(z', c, N) =/\in \delta(z, a_1), m \geq 0, n \geq 1, z \notin E$
*Der Schreiblesekopf bleibt stehen*
- $b_1...b_mza_1...a_n \vdash_M b_1...b_mcz'a_2...a_n$, wenn $(z', c, L) =/\in \delta(z, a_1), m \geq 1, n \geq 1, z \notin E$
*Der Schreiblesekopf bewegt sich nach links?*
- $b_1...b_mza_1...a_n \vdash_M b_1...b_mcz'a_2...a_n$, wenn $(z', c, L) =/\in \delta(z, a_1), m \geq 1, n \geq 1, z \notin E$
*Der Schreiblesekopf bewegt sich nach links?*
- $b_1...b_mza_1 \vdash_M b_1...b_mca_2z'\square$, wenn $(z', c, R) =/\in \delta(z, a_1), m \geq 0, n \geq 2, z \notin E$
*Der Schreiblesekopf bewegt sich in ein unbeschriebenes Gebiet rechts des Wortes?*
- $za_1...a_n \vdash_M z'\square ca_2...a_n$, wenn $(z', c, L) =/\in \delta(z, a_1), m \geq 0, n \geq 2, z \notin E$
*Der Schreiblesekopf bewegt sich in ein unbeschriebenes Gebiet links des Wortes?*

Insbesondere bezeichnet $\vdash_M^*$ die **reflexiv-transitive Hülle** von $\vdash_M$.
$\vdash_M^i$ beeichnet die **$i$-fache Anwendung** von $\vdash_M$
Ist $M$ bekannt, lässt man das $M$ weg und schreibt $\vdash$

### Akzeptierte Sprache 
Die durch $M$ akzeptierte Sprache $L(M)$ ist definiert als
$$L(M) := \{w \in \Sigma^*:\exists u, v \in \Gamma^*, z \in E:z_0w \vdash uzv\}$$

## Eigenschaften
Die durch Turingmaschinen erkannten Sprachen sind genau die [[Unbeschränkte Sprache|Typ 0-Sprachen]]

#FSK #Natural-Computing 