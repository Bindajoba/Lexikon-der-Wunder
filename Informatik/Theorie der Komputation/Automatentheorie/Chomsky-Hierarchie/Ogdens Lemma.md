## Beschreibung
Das **Ogdens Lemma** ist eine Verallgemeinerung des [[Pumping Lemma#Definition für Kontextfreie Sprachen|Pumping Lemmas für Kontextfreie Sprachen]]. Beim Pumping Lemma gibt es solche Bedingungen wie: $vwx$ hat höchstens $n$-Zeichen.
Das Ogdens-Lemma zählt aber nicht zwingend alle Zeichen sondern nur bestimmte. Die obere Bedingung hat dann eher das Aussehen: $vwx$ hat höchstens $n$ $a$'s.

Jede [[Kontextfreie Sprache]] erfüllt **Ogdens Lemma**

## Definition
Sei $L$ eine [[Kontextfreie Sprache]]. Dann gilt die Pumping Eigenschaft:

"Markiere" die Zeichen $\sigma \subseteq \Sigma$ diese Zeichen werden wir zählen.
Es gibt ein $n \in \mathbb{N}_0$, sodass jedes [[Wort]] $z \in L$, welches mindestens $n$ Zeichen aus $\sigma$ hat (d.h. $\sum_{a\in \sigma} \#_a(z)\geq n$ als $z = uvwxy$ geschrieben werden kann, sodass gilt:
- $vwx$ enthält maximal $n$ Zeichen aus $\rho$
- $vx$ enthält mindestens $n$ Zeichen aus $\rho$
- für alle $i \geq 0: uv^iwx^iy \in L$[^1]

#FSK 

[^1]:  Sabel - Lemma 5.4.7