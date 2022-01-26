## Beschreibung
Wird eine Startvariable unter der Anwendung der [[Grammatik|Produktionsregeln]] in ein [[Wort]] überführt, dann nennt man die Folge dahin eine **Ableitung**

## Definition
### Ableitungsschritt
Wird eine [[Grammatik|Satzform]] mit einer [[Grammatik|Produktions]] in eine neue [[Grammatik|Satzform]] überführt, dann nennt man das einen **Ableitungsschritt**

Sei $u, v \in \Sigma^*$ [[Grammatik|Satzformen]] 
Gibt es zwei weitere "Kontext"-Satzformen $w_1, w_2 \in \Sigma^*$
mit 
- $u = w_1lw_2$
- $v = w_1rw_2$
- $(l \to r) \in P$

Dann schreibt man den Ableitungsschritt als [[Relation]] $u \Rightarrow_G v$
"$u$ geht unter Grammatik $G$ unmittelbar in $v$ über"[^1]

### Mehrfacher Ableitungsschritt
Die [[Relation]] $u \Rightarrow_G^* v$ beschreibt die 0- oder mehrfache Anwendung von $u \Rightarrow_G v$[^1]

### Ableitung 
Eine endliche Folge von **Satzformen** $(w_0, w_1, ..., w_n)$ für die gilt:
- $w_0 = S$
- $w_n \in \Sigma^*$
- $w_{i-1} \Rightarrow_G w_i$ für $i = 1, ..., n$
nennt man Ableitung von $w_n$[^1]

*Eine Ableitung wird aber in Realität trotzdem immer mit Pfeilen dazwischen dargestellt.*

### Linksableitung
Eine Linksableitung ist eine Ableitung, in der immer die linkeste Variable ersetzt wird.
*Die Reihenfolge, in der man ableitet macht bei [[Rekursiv Aufzählbare Grammatik|Typ 0]] und [[Kontextsensitive Grammatik|Typ 1 Grammatiken]] einen Unterschied, da die Produktionen vom Kontext abhängen*[^1]

### Rechtsableitung
Eine Rechtsableitung ist eine Ableitung, in der immer die rechteste Variable ersetzt wird.

#FSK 

[^1]: Sabel - Definition 3.1.1