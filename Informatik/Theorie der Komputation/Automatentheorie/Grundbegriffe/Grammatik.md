## Beschreibung
Grammatiken sind endliche Mengen von Regeln der Form
$$\text{"linke Seite"} \to \text{"rechte Seite"}$$
Mit Grammatiken kann man ein [[Formale Sprache]] definieren [^1]

## Definition 
Eine **Grammatik** ist ein 4-Tupel $G=(V, \Sigma, P, S)$ wobei

- $V$ ist eine endliche Menge von [[Nichterminal|Nichterminalen]]
- $\Sigma$ ist ein [[Alphabet]] von Zeichen (auch Terminale gennannt)
- $P$ ist eine endliche [[Menge]] von **Produktionen** (auch Regeln gennannt)
- $S\in V$ ist das Startsymbol (auch Startvariable gennannt)[^1]

### Produktion
Eine Produktion aus $P$ hat die Form $l \to r$
Wobei
- Die Linke Seite $l\in(V\cup \Sigma)^+$ aus mindestens einem Terminal oder nicht-Terminal besteht
*Komischerweise verbietet die Definition nicht, dass auf der linken Seite nur ein nicht Terminal steht*
- Die Rechte Seite $r\in(V\cup \Sigma)^*$ aus einer Kombination von Terminalen und nicht-Terminal besteht.

Man kann Produktionen auch als Tupel $(l, r)$ auffassen, dann gilt $(l, r) \subseteq (V\cup \Sigma)^+ \times (V\cup \Sigma)^*$

### Satzform
Eine Zeichenkette, die aus Terminalen und nicht-Terminalen besteht, nennt man **Satzform**


## Operationen
### Wortübergang
Seien $u, v$ Satzformen 

#FSK 
[^1]: Sabel - Definition 3.1.1