## Beschreibung
Eine [[Formale Sprache|Sprache]] liegt in der Klasse der Funktion $f$, wenn es eine nicht-deterministische [[Turingmaschine]] gibt, die alle Wörter schneller akzeptiert oder verwirft als durch $f$ gegeben ist.

## Definition
Für eine Funktion $f: \mathbb{N} \to \mathbb{N}$ sei die Klasse $NTIME(f(n))$ genau die Menge der Sprachen, für die es eine nicht-deterministische, stets anhaltende [[Mehrband-Turingmaschine|Mehrband-TM]] $M$ gibt mit $L(M)=L$ und $ntime_M(w) \leq f(|w|)$ für alle $w \in \Sigma^*$