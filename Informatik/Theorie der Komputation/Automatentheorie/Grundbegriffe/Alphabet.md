## Definition
Ein Alphabet ist eine endliche, nicht-leere [[Menge]] von Zeichen.

Ein Alphabet wird oft mit $\Sigma$ bezeichnet.[^1]

## Operationen
### Alphabet hoch i
Seien $\Sigma$ ein Alphabet und $i\in \mathbb{N}_0$

$\Sigma^i$ wird so induktiv definitiert:
- $\Sigma^0 := \{\varepsilon\}$
- $\Sigma^k := \{ww^{k-1}:a\in\Sigma, w\in\Sigma^{i-1}\}$

### Kleenscher Abschluss für Alphabete
Der Kleensche Abschluss ist die Vereinigung aller **Alphabete hoch i**.

$$\Sigma^* := \bigcup_{i\in \mathbb{N}}\Sigma^i$$

Betrachtet man ein **Alphabet** als eine [[Menge]] von 1-Zeichen langen [[Wort|Wörtern]], dann ist ein Alphabet auch eine [[Formale Sprache]].
Der Kleensche Abschluss für Alphabete ist daher ein Spezialfall des [[Kleenscher Abschluss|Kleenschen Abschlusses für Sprachen]]


#FSK 
[^1]: Sabel - Definition 2.1.3