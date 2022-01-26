## Definition
Sei ein [[Alphabet]] $\Sigma$ gegeben.

Ein Wort $w = a_1...a_n$ über $\Sigma$ ist eine endliche Folge von Zeichen aus $\Sigma$  [^1]

### Leeres Wort
Ein Wort kann auch aus keinen Zeichen bestehen.
Dann ist es leer und wird mit $\varepsilon$ notiert.

### Präfix
Seien $u, v$ Wörter

$u$ ist ein Präfix von $v$, wenn es ein Wort $w$ über $\Sigma$ gibt, sodass $uw = v$

### Suffix
Seien $u, v$ Wörter

$u$ ist ein Suffix von $v$, wenn es ein Wort $w$ über $\Sigma$ gibt, sodass $uw = v$

### Teilwort
Seien $u, v$ Wörter

$u$ ist ein Teilwort von $v$, wenn es Wörter $w_1, w_2$ über $\Sigma$ gibt, sodass $w_1uw_2 = v$
## Operationen
### Länge eines Wortes
Sei $w$ ein Wort.

Dann bedeutet $|w|$ die Länge des Wortes

### Anzahl eines Buchstaben in einem Wort
Sei $w$ ein Wort und $a\in \Sigma$ ein Zeichen

Dann gibt $\#_a(w)\in \mathbb{N}_0$ zurück, wie oft das Zeichen im Wort enthalten ist. 

### Buchstabe im Index eines Wortes
Sei $w = a_1...a_n$ ein Wort.

Dann gibt $w[i]$ den Buchstaben $a_i$ zurück. 
Der Operator gibt also den $i$-ten Buchstaben eines Wortes zurück

### Länge eines Wortes
Sei $w$ ein Wort.

Dann bedeutet $|w|$ die Länge des Wortes

### Konkatenation
[[Konkatenation]]

### Umdrehen
Sei $w = a_1...a_n$ ein Wort.

$\overline{w} = a_n...a_1$ ist das rückwärtgelesene Wort.

Gilt $w = \overline{w}$, so ist das Wort ein **Palindrom**[^2]

Für alle Worte gilt $\overline{\overline{w}}=w$[^3]

#FSK 

[^1]: Sabel - Definition 2.1.3
[^2]: Sabel - Definition 2.1.6
[^3]: Sabel - Übungsaufgabe 2.1.9