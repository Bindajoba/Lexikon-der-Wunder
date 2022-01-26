## Beschreibung
Eine [[Formale Sprache|Sprache]] liegt in der Klasse der Funktion $f$, wenn es eine [[Turingmaschine|Deterministische Turingmaschine]] gibt, die alle Wörter schneller akzeptiert oder verwirft als durch $f$ gegeben ist.

## Definition
Für eine Funktion $f: \mathbb{N} \to \mathbb{N}$ sei die Klasse $TIME(f(n))$ genau die Menge der Sprachen, für die es eine deterministische, stets anhaltende Mehrband-TM $M$ gibt mit $L(M)=L$ und $time_M(w) \leq f(|w|)$ für alle $w \in \Sigma^*$