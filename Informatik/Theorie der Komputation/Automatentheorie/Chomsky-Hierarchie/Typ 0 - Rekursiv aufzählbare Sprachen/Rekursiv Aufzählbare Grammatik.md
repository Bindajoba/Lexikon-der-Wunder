## Definition
Eine [[Grammatik]] $G$ $G$ wird immer vom **Typ 0** (auch **rekursiv aufzählbar**, **Semientscheibare Grammatik**) gennannt.

Eine rekursiv aufzählbare Grammatik ist der Allgemeinste Fall einer [[Grammatik]] 
Rekursiv Aufzählbare Sprachen sind der nullte Typ von Sprachen der [[Chomsky-Hierarchie]] 

*Solche Grammatiken werden rekursiv aufzählbar gennant, da man alle Wörter durch Rekursion bestimmen könen sollte.* [^1]

## Eigenschaften
### Erzeugte Sprache
EIne rekursiv aufzählbare Grammatik erzeugt eine [[Rekursiv Aufzählbare Sprache]]

### Anzahl von Rekursiv Aufzählbaren Grammatiken
Jede Grammatik zu einem [[Alphabet]] $\Sigma$ bestimmt sich durch endlich viele Variablen $V$, endlich viele Produktionen $P$  und einen Startwert $S$. 
Es ist also möglich alle möglichen Grammatiken aufzuzählen.
Somit ist die Menge aller **Rekursiv aufzählbarer Grammatiken** abzählbar unendlich. [^1]

### Verkürzung von Wörtern
Eine Typ 1 Grammatik erlaubt keine verkürzende Regeln, während eine Typ 0 Grammtik dies im Normalfall erlaubt.

Will man also wissen, ob ein Wort der Länge $n$ durch eine Typ 1 Grammatik erzeugt wird, kann man die Suche beenden, wenn die Satzform länger als $n$ ist.
Bei Typ 0 Grammatiken ist das nicht der Fall.

![[Ableitung Wortlänge.png]]

#FSK 

[^1]: Sabel 3.2.2