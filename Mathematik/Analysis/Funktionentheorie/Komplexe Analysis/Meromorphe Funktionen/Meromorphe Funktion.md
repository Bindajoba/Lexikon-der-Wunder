## Beschreibung
**Meromorphe Funktionen** sind Verallgemeinerungen von [[Analytische Funktion|Holomorphen Funktionen]]. Sie wurden eingefürt, da der Kehrwert $\frac{1}{f}$ einer holomorphen Funktion nicht holomorph ist, da sie [[Pol|Pole]] an den [[Nullstelle|Nullstellen]] von $f$ hat.
Deshalb erlauben Meromorphe Funktionen Pole.

## Definition
Es sei
- $\emptyset \neq U \subseteq \mathbb{C}$ offen
- $P = P(f) \subseteq U$ eine Menge, die in $U$ keinen [[Häufungspunkt]] besitzt[^1]

Eine Funktion $f : U \backslash P(f) \to \mathbb{C}$, die auf $U \backslash P(f)$ analytisch ist und in jedem Punkt $a \in P(f)$ einen Pol besitzt heißt **meromorph**

### Polstellenmenge
$P(f)$ heißt **Polstellenmenge**[^1]

## Äquivalente Charaktierisierungen
### Äquivalente Charaktierisierung I 
Sei
- $S \subseteq U$ eine Menge ohne Häufungspunkt und $U$
- $f:U\backslash S \to \mathbb{C}$ analytisch
- kein $s \in S$ ist eine [[Wesentliche Singularität]]

Dann ist $f$ auf $U$ **meromorph** und durch analytisches Fortsetzen der [[Hebbare Singularität|Hebbaren Singularitäten]] in $S$ erhält man eine **Polstellenmenge**[^2]

## Eigenschaften
### C-Algebra
Sei $\emptyset \neq U \subseteq \mathbb{C}$ [[Offene Menge|offen]], dann bildet
$$\mathcal{M}(U) := \{f: U \backslash P(f) \to \mathbb{C}: f \text{ ist meromorph auf } U\}$$ zusammen mit punktweiser Addition und Multiplikation eine $\mathbb{C}$-[[Algebra]][^3]

### Körper
Ist $\emptyset \neq U \subseteq \mathbb{C}$ ein [[Gebiet]], dann ist $\mathcal{M}(U)$ ein [[Körper (Algebra)]]

### Ableitung
Die [[Ableitung]] einer **meromorphen Funktion** ist wieder **meromorph** und hat die gleiche **Polstellenmenge**[^4]





#Mathe-IV 

[^1]: Zenk - Definition 24.2.1
[^2]: Zenk - Bemerkung 24.2.2
[^3]: Zenk - Lemma 24.2.3
[^4]: Zenk - Lemma 24.2.4