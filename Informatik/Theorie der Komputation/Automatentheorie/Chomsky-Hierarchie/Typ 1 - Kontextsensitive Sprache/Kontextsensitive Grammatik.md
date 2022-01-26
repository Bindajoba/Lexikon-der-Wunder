## Definition
Eine Grammatik $G$ ist vom **Typ 1** (auch **kontextsensitiv**, **monoton**) genannt, wenn für alle Produktionen $(l \to r) \in P$ gilt: $|l| \leq |r|$

Eine kontextsensitive Grammatik ist ein Spezialfall einer [[Rekursiv Aufzählbare Grammatik|rekursiv aufzählbaren Grammatik]] und die Verallgemeinerung der [[Kontextfreie Grammatik]].

## Eigenschaften
### Erzeugte Sprache
Ene Kontextsensitive Grammatik erzeugt mindestens eine [[Kontextsensitive Sprache]]. 

### Verkürzung von Wörtern
Eine Typ 1 Grammatik erlaubt keine verkürzende Regeln, während eine [[Rekursiv Aufzählbare Sprache|Typ 0 Grammatik]] dies im Normalfall erlaubt.

Will man also wissen, ob ein Wort der Länge $n$ durch eine Typ 1 Grammatik erzeugt wird, kann man die Suche beenden, wenn die Satzform länger als $n$ ist.
Bei Typ 0 Grammatiken ist das nicht der Fall.

![[Ableitung Wortlänge.png]][^1]

### Wortproblem
Aus dem oberen Grund ist das [[Wortproblem]] bei einer **kontextsensitiven Grammatik** für alle Wörter [[Entscheidbarkeit|entscheidbar]].
 
 
## Umformungen
DIe Grammatik kann auf viele Arten umgewandelt werden, ohne, dass die erzeugte Sprache anders ist.


 
 ### Sharing von Satzformen
Sei $G = (V, \Sigma, P, S)$ eine CFG, die Produktionsregeln der Form 
- $A \to w_1 ... w_n \in P$ (mit Satzformen $w_i$)
bestizt. Dann kann man die Satzformen $w_i$ durch neue Variablen $B_i$ ersetzen. Die Grammatik erhält die Produktionen:
- $A \to B_1 ... B_n \in P$
- $B_1 \to w_1, ..., B_n \to w_n$
Die erzeugt Sprache verändert sich dann nicht.

### Aufteilen der rechten Seite (eine Variable links)
Eine Produktion der Form $A \to B_1B_2...B_n$ kann aufgeteilt werden in 
- $A \to B_1C_1$
- $C_1\to B_2C_2$
- ...
- $C_{n-2} \to B_{n-1}B_n$


### Aufteilen der rechten Seite (zwei Variablen links)
Eine Produktion der Form $A_1A_2 \to B_1B_2...B_n$ kann aufgeteilt werden in 
- $A_1A_2 \to B_1C_2$
- $C_2 \to B_2C_3$
- ...
- $C_{n-2} \to B_{n-2}C_{n-1}$
- $C_{n-1} \to B_{n-1}B_n$


### Aufteilen beider Seiten
*Es könnte sein, dass ich hier Sachen brutal missachte.*
Eine Prouktion der Form $A_1A_2...A_n \to B_1B_2...B_m$ (mit $n \leq m$) kann aufgeteilt werden in 
- $A_1A_2 \to B_1C_2$
- $C_2A_3 \to B_2C_3$
- $C_3A_4 \to B_3C_4$
- ...
- $C_{n-2}A_{n-1} \to B_{n-2}C_{n-1}$
- $C_{n-1}A_n \to B_{n-1}B_nB_{n+1}...B_m$

Dann sehen die Ableitungsschritte so aus:
$$A_1A_2...A_n \to B_1C_2A_3...A_n \to B_1B_2C_3A_4...A_n \to B_1B_2...B_{n-2}C_{n-1}A_n...A_m\to B_{n-1}B_nB_{n+1}...B_m$$
Die letzte Ableitung der Reihe kann auf der rechten Seite mehr als 2 Variablen haben. Die können noch weiter unterteilt werden


### Kuroda Normalform
Jede **Kontextsensitive Grammatik** kann in [[Kuroda-Normalform]] gebracht werden.[^2]

### Inlining von Produktionen
Sei $G = (V, \Sigma, P, S)$ eine CFG, die Produktionsregeln der Form 
- $A \to uBv \in P$
- $B \to w_1 | ... | w_n$ (mit Satzformen $w_i$)
besitzt. Dann kann man $A \to uBv$ durch $A \to uw_1v | ... | uw_nv$ ersetzen

 Formell:
 $$G' = (V, \Sigma, P\backslash \{A \to uBv\} \cup \{A \to uw_1v | ... | uw_nv\}, S)$$ Dann erzeugen $G$ und $G'$ dieselbe Sprache $L(G) = L(G')$



#FSK 

[^1]: Sabel - Beispiel 3.2.2
[^2]: Sabel - Satz 6.1.2