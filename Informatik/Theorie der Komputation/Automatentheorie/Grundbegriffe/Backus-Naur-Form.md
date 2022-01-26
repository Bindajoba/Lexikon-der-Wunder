## Beschreibung
Die Backus-Naur-Form ist eine Notation, um die Definition von Produktionsregeln einer [[Grammatik]] zu erleichtern und zu kompaktifizieren.

Sie wurde von [[John Backus]] und [[Peter Naur]] entwickelt.

## Definition
Sei $G = (V, \Sigma, P, S)$ eine [[Kontextfreie Grammatik|Typ 2-Grammatik]]
1. Statt $A \to w_1, ..., A \to w_n$ schreibt man 
$A \to w_1 | ... | w_n$
*D.h. $w_1$ oder $...$ oder $w_n$*
2. Statt $A \to uvw$ und $A \to uw$ schreibt man
$A \to u[v]w$
3. Statt $A \to uv$, $A \to uBv$ und $B \to v|B$ schreibt man
$A \to u\{v\}w$ 

Grammatiken in EBNF sind äquivalent zu Typ 2-Grammatiken, stellen also genau die [[Kontextfreie Sprache|kontextfreien Sprachen]] dar.[^1]

#FSK 

[^1]: Sabel - Definition 3.6.1