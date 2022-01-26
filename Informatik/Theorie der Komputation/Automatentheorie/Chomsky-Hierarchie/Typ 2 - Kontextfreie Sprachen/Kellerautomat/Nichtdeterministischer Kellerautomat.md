## Beschreibung
Ein **nichtdeterministischer Kellerautomat** (auch **pushdown automaton, PDA**) ist so etwas wie ein [[Nichtdeterministischer Endlicher Automat]], der um einen [[Keller]] (Stack) erweitert wurde.
Bei jedem Zustandwechsel kann das oberste Element des Kellers gelesen werden oder beliebig viele neue Objekte auf den Keller gelegt werden.
Das ermöglicht dem Automaten jetzt kompliziertere Dinge zu speichern.

## Definition
Ein (nichtdeterministischer) Kellerautomat ist ein [[Tupel]] $M = (Z, \Sigma, \Gamma, \delta, z_0, \#)$, wobei
- $Z$ ist eine endliche Menge von **Zuständen**
- $\Sigma$ ist das (endliche) Eingabe-[[Alphabet]]
- $\Gamma$ ist das (endliche) Kelleralphabet
- $\delta: Z \times (\Sigma \cup \varepsilon) \times \Gamma \to \mathcal{P}_e(Z \times \Gamma^*)$ ist die **Zustandsüberführungsfunktion**
- $z_0 \subseteq Z$ ist der **Startzustand**
- $\# \in \Sigma$ ist der **Startzustand** im Keller[^1]

*Der Keller het keine Endzustände. Das liegt daran, dass der Keller terminiert, wenn der Stapel leer ist. Das gegebene Wort wird genau dann akzeptiert.*

### Konfiguration eines Kellerautomaten
Die Konfiguration beschreibt den Kellerautomaten in einem bestimmten Moment der Wortverarbeitung. In der Konfiguration ist der aktuelle Zustand, die aktuellen Elemente im Keller und der Rest des noch zu lesenden Wortes.

Eine Konfiguration ist ein [[Tupel|Tripel]] $(z, w, W) \in Z \times \Sigma^* \times \Gamma^*$[^2]

### Transitionsrelation für PDA-Konfigurationen
Eine Transitionsrelation ist das Äquivalent zum [[Ableitung eines Wortes#Ableitungsschritt|Ableitungsschritt eines Endlichen Automaten]]. Es ist eine [[Relation]], die beschreibt, wie eine Konfiguration in die nächste übergeht.

Die **Transitionsrelation** $\vdash_M \subseteq (\Sigma^* \times \Gamma^*) \times (\Sigma^* \times \Gamma^*)$ ist definiert durch
- $(z, a_1...a_n, A_1...A_m)\vdash_M (z', a_2...a_n, W...A_m)$
falls $(z', W) \in \delta(z, a_1, A_1)$
*D.h. wenn es einen Zustandsübergang von $z$ zu $z'$ gibt, das Zeichen $A_1$ auf dem Keller liegt und nach dem Übergang die Zeichenkette $W$ auf den Keller gelegt wird*
- $(z, w, A_1...A_m)\vdash_M (z', a_2...a_n, W...A_m)$
falls $(z', W) \in \delta(z, \varepsilon, A_1)$
*D.h. wenn es einen Epsilon-Zustandsübergang von $z$ zu $z'$ gibt, das Zeichen $A_1$ auf dem Keller liegt und nach dem Übergang die Zeichenkette $W$ auf den Keller gelegt wird*

Insbesondere bezeichnet $\vdash_M^*$ die **reflexiv-transitive Hülle** von $\vdash_M$.
$\vdash_M^i$ beeichnet die **$i$-fache Anwendung** von $\vdash_M$
Ist $M$ bekannt, lässt man das $M$ weg und schreibt $\vdash$

### Akzeptierte Sprache
Die durch $M$ akzeptierte Sprache $L(M)$ ist definiert als
$$L(M) := \{w \in \Sigma^*:(z_0, w, \#) \vdash^* (z, \varepsilon, \varepsilon)\text{ für ein } z\in Z\}$$

## Umwandlungen
### Nichtdeterministischer Kellerautomat mit Endzuständen
Jeder **Kellerautomat** kann in einen [[Nichtdeterministischer Kellerautomat mit Endzuständen]] (und zurück) umgewandelt werden.

*Zum Automaten wird ein neuer Endzustand hinzugefügt. Außerdem wird unter den Stapel ein neues Symbol \$ hinzugefügt.
Von jedem Zustand kann man mit \$ zum Endzustand wechseln
Wäre der Stapel also eigentlich leer geworden, dann kann er ein den Endzustand wechseln.*

## Eigenschaften
**Kellerautomaten** erkennen genau die [[Kontextfreie Sprache]]

#FSK 

[^1]: Sabel - Definition 5.7.1
[^2]: Sabel - Definition 5.7.2