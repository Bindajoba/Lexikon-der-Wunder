## Beschreibung
Das **Pumping-Lemma** ist eine Eigenschaft, die von [[Reguläre Sprache|regulären]] und [[Kontextfreie Sprache|kontextfreien Sprachen]] erfüllt wird, und deshalb zum Widerlegen dieser genutzt werden kann.

Das Pumping-Lemma ist ein Spezialfall von [[Ogdens Lemma]]

## Definition für Reguläre Sprachen
Sei $L$ eine reguläre Sprache. Dann gilt die Pumping Eigenschaft:

Es gibt ein $n \in \mathbb{N}_0$, sodass jedes [[Wort]] $z \in L$ mit Mindestlänge $n$ hat (d.h. $|z| \geq n$) als $z = uvw$ geschrieben werden kann, sodass gilt:
- $|uv| \leq n$
- $|v| \geq 1$
- für alle $i \geq 0: uv^iw \in L$
Die Zahl $n$ nennt man auch die Pumping Konstante der Sprache L.

*Die Intuition:
Angenommen die Sprache ist eine reguläre Sprache.. Dann kann sie durch einen [[Deterministischer Endlicher Automat|Deterministischen Endlichen Automaten]] $M$ dargestellt werden kann. Erhält man aus einem solchen Automaten ein [[Wort]], welches länger ist als die Zahl der Zustände von $M$, dann muss irgendwo ein Zustand mindestens zweimal durchlaufen worden sein.
Deshalb muss der Automat eine Schleife haben. In dem Fall kann die Schleife 0, 1, 2 oder n-mal durchlaufen werden, und ergibt immer ein Wort in der Sprache.
Falls nicht, dann besteht ein Widerspruch, und die Sprache kann nicht regulär sein.*[^1]

*Es gibt [[Formale Sprache|Formale Sprachen]], die das Pumping Lemma erfüllen, aber nicht regulär sind:
z.B. $\{a^kb^lc^l:k,l\in \mathbb{N}\}$*

## Umkehrung für Reguläre Sprachen
Sei $L$ eine [[Formale Sprache]]. Dann gilt die Pumping Eigenschaft nicht, wenn:

Für alle $n \in \mathbb{N}_0$ gibt es ein [[Wort]] $z \in L$ mit Mindestlänge $n$ (d.h. $|z| \geq n$) und für jede Zerlegung $z = uvw$ mit:
- $|uv| \leq n$
- $|v| \geq 1$

gilt:
Es gibt ein $i \geq 0: uv^iw \notin L$

Insbesondere ist $L$ dann keine [[Reguläre Sprache]] mehr.
Die Aussage folgt aus Negation der oberen.[^2]

## Definition für Kontextfreie Sprachen
Sei $L$ eine [[Kontextfreie Sprache]]. Dann gilt die Pumping Eigenschaft:

Es gibt ein $n \in \mathbb{N}_0$, sodass jedes [[Wort]] $z \in L$ mit Mindestlänge $n$ hat (d.h. $|z| \geq n$) als $z = uvwxy$ geschrieben werden kann, sodass gilt:
- $|vwx| \leq n$
- $|vx| \geq 1$
- für alle $i \geq 0: uv^iw \in L$
[^3]

*Im Skript gibt es eine hervorragende Illustration, warum das gilt. Die Grundidee ist: Wenn man bei einer Grammatik in [[Chomsky-Normalform]], die n Nicht-Terminale besitzt (n+1)-Ableitungsschritte durchführt, muss irgendeinen Nichtterminal in der [[Ableitung eines Wortes]] zweimal vorkommen.
Logischerweise muss es eine Schleife geben, die $A$ enthält.
Das bedeutet aber auch, dass diese Schleife kein mal, ein mal oder mehrmals durchlaufen werden kann. Das Teilwort, das durch das mehrmalige Durchlaufen der Schleife durch $A$ entsteht ist $v$ das Teilwort links neben $A$  und $x$ das Teilwort rechts neben $A$.
$u, y$ ist das Teilwort vor der Schleife.
$w$ ist das Teilwort nach der Schleife.*

## Umkehrung für Kontextfreie Sprachen
Sei $L$ eine [[Kontextfreie Sprache]]. Dann gilt die Pumping Eigenschaft nicht, wenn:

Für alle $n \in \mathbb{N}_0$ gibt es ein [[Wort]] $z \in L$ mit Mindestlänge $n$ (d.h. $|z| \geq n$) und für jede Zerlegung $z = uvwxy$ mit:
- $|uvx| \leq n$
- $|vx| \geq 1$

gilt:
Es gibt ein $i \geq 0: uv^iwx^iy \notin L$

Insbesondere ist $L$ dann keine [[Reguläre Sprache]] mehr.
Die Aussage folgt aus Negation der oberen.[^2]

## Eigenschaften
- Sei $L_1$ eine Teilmenge der Sprache $L_2$ 
Erfüllt $L_1$ das Pumping-Lemma, dann erfüllt auch $L_2$ das Pumping Lemma.


#FSK 

[^1]: Sabel - Lemma 4.9.1
[^2]: Sabel - Lemma 4.9.3
[^3]: Sabel - Lemma 5.1.4