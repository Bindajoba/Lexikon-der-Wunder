## Definition
Eine **Formale Sprache** $L$ über dem [[Alphabet]] $\Sigma$ ist eine Teilmenge vom [[Kleenscher Abschluss|Kleenschen Abschluss]] $\Sigma^*$.
$$L \subseteq \Sigma^*$$
## Operationen
Seien $L_1, L_2$ **Formale Sprachen** zum Alphabet $\Sigma$

*Formale Sprachen sind auch nur [[Wort]]-Mengen, daher funktionieren viele Operatoren, wie man es erwarten würde* 
### Vereinigung
$L_1 \cup l_1$ ist die [[Vereinigung]] von $L_1$ und $L_2$
### Schnitt
$L_1 \cap l_1$ ist der [[Schnitt]] von $L_1$ und $L_2$
### Komplement
$\overline{L_1} = \Sigma^* \backslash L_1$ ist das [[Komplement]] von $L_1$ bzgl. $\Sigma^*$

### Produkt
$L_1 \circ L_2 = L_1L_2 := \{uv : u \in L_1 \text{ und }v\in L_2\}$
also alle möglichen Konkatenationen mit Wörtern aus $L_1$ und $L_2$[^1]

### Kartesisches Produkt
$L_1 \times l_1$ ist das [[Kartesisches Produkt|Kartesische Produkt]] von $L_1$ und $L_2$[^2]

### Sprache hoch i
Analog zu [[Alphabet|Alphabet hoch i]] definieren wir den gleichen Operator auch für Sprachen

Sei $L$ eine Sprache und $i \in methbb{N}$ Dann ist
$$L^0:=\{\varepsilon\}$$$$L^i:=\{L\circ L^{i-1}\}$$$$L^+ := \bigcup_{i\in \mathbb{N}}\Sigma^i$$

### Kleenscher Abschluss
Sei $L$ eine Sprache. Dann ist
$$L^* := \bigcup_{i\in \mathbb{N}_0}\Sigma^i$$ der Kleensche Abschluss (benannt nach [[Stephen Cole Kleene]])

## Eigenschaften
### Grammatik
Nicht jede **formale Sprache** besitzt eine [[Grammatik]].

### Menge an Sprachen
Es gibt [[Überabzählbarkeit|überabzählbar unendlich]] viele Sprachen.

Denn:
Betrachte die Reellen Zahlen zwischen 0 und 1. In der binären Zahlendarstellung können diese als unendlich lange Nachkommazahl aus 0 und 1 definiert werden.

Jedem dieser Zahlen kann man jetzt auf folgende Weise eine Formale Sprache $L$ mit Alphabet $a$ zuordnen.
- Ist die erste Nachkommastelle eine 1, dann ist $a^1$ in der Sprache enthalten $a^1 \in L$
- Ist die i-te Nachkommastelle eine 1, dann ist $a^i$ in der Sprache enthalten $a^i \in L$

Da zwei unterschiedliche Zahlen $x, y \in ]0,1[$ sich in ihren Nachkommazahlen unterscheiden müssen, sind die erzeugten Sprachen auch verschieden.
Somit gibt es mehr **Formale Sprachen** als Zahlen zwischen 0 und 1. Es gibt überabzählbar viele.


Es gibt abzählbar unendlich viele Wörter

## Hierarchien
### Chomsky-Hierarchie
Siehe [[Chomsky-Hierarchie]]

### Berechenbarkeitshierarchie
1. Alle Sprachen
2. [[Semientscheidbare Sprache|Semi-entscheidbare Sprachen]]
3. [[Entscheidbare Sprache|Entscheidbare Sprachen]]
4. [[LOOP-Berechenbarkeit|LOOP-berechenbare Sprachen]]
5. [[Komplexitätsklasse NP|NP-Sprachen]]
6. [[Komplexitätsklasse P|P-Sprachen]]


#FSK 

[^1]: Sabel - Definition 2.1.10
[^2]: Sabel - Bemerkung 2.1.11