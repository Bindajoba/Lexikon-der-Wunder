## Beschreibung
DIe Chomsky-Hierarchie ist eine hierarchische Klassifizierung von [[Grammatik|Grammatiken]] und [[Formale Sprache|formalen Sprachen]].
Sie wurde von [[Noam Chomsky]] vorgenommen und wurde nach ihm bennannt.

## Definition
### Definition Grammatik
- **Typ 0**: Jede Grammatik ist von Typ 0
- **Typ 1**: Eine Grammatik $G$ ist vom Typ 1 und wird kontextsensitiv gennannt, wenn für alle Produktionen $(l \to r) \in P$ gilt: $|l| \leq |r|$
- **Typ 2**: EIne Grammatik $G$ ist vom Typ 2 und wird [[Kontextfreie Grammatik|kontextfrei]] gennannt, wenn für alle Produktionen $(- \to r) \in P$ gilt: $a = A \in V$, 
D.h. die linken Seiten der Produktionen bestehen aus genau einer Variablen
- **Typ 3**: Eine Typ 2-Grammatik $G$ ist vom Typ 3 und wird [[Reguläre Grammatik|regulär]] genannt, wenn für alle Produktionen $(l\to r)$ gilt: $r$ ist von der Form $a$ oder von der Form $aA$ mit $a\in \Sigma, A \in V$, 
D.h., die rechte Seite bestehen aus einem Terminal, welchem optional eine Variable folgt.

### Definition Sprache
EIne [[Formale Sprache]] $L$ nennt man Typ 0, Typ 1, Typ 2 oder Typ 3, falls es eine Grammatik $G$ des entsprechenden Typen gibt, die diese Sprache erzeugt. ($L(G)=L$)[^1]  

### $\varepsilon$-Regel für Typ 1,2,3 Sprachen
Eine [[Grammatik]]  $G = (V, \Sigma, P, S)$ vom Typ 1, 2, 3 darf eine Produktion $(S \to \varepsilon)\in P$ enthalten, vorausgesetzt, dass keine rechte Seite einer Produktion in P, die Variable $S$ enthält.[^2]

## Hierarchie
Es gibt noch weitere Kriterien, mit denen sich eine [[Formale Sprache]] hierarchisch klassifizieren lassen kann.
Die Sprachen sind vom Allgemeinsten zum Speziellsten
- [[Formale Sprache]]
- [[Rekursiv Aufzählbare Sprache]]
- [[Entscheidbare Sprache]]
- [[Kontextsensitive Sprache]]
- [[Kontextfreie Sprache]]
- [[Reguläre Sprache]][^3]



#FSK 
[^1]: Sabel - Definition 3.2.1
[^2]: Sabel - Definition 3.2.4
[^3]: Sabel - 3.2.2