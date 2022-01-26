## Beschreibung
Kontextfreie Sprachen sind eine Verallgemeinerung einer [[Reguläre Sprache]] und ein Spezialfall einer [[Kontextsensitive Sprache]]

Sie tauchen oft auf, wenn mit [[Wort|Palindromen]] oder Klammerungen gearbeitet wird.

## Eigenschaften
### Probleme
- Das [[Wortproblem]] ist für kontextfreie Sprachen [[Entscheidbarkeit|entscheidbar]] (siehe [[CYK-Algorithmus]]) 
- Das [[Leerheitsproblem]] ist für kontextfreie Sprachen [[Entscheidbarkeit|entscheidbar]]
Die Sprache liegt in Chmosky-Normalform vor. Dazu markiert man iterativ alle Variablen, die keine leer Sprache erzeugen (also erst $A \to a$, dann $B \to AC$) Ist am Ende die Startvariable $S$ unter den markierten Variablen enthalten, ist die Sprache nicht leer.[^1]
- Das [[Endlichkeitsproblem]] ist für kontextfreie Sprachen [[Entscheidbarkeit|entscheidbar]]
*Ist ein Wort länger als die Zahl der Zustände $n$ des Automaten in der Sprache, enthalten, dann muss, ein Zustand zweimal durchlaufen worden sein. Also muss es eine Schleife im Automaten geben.
Hat die Sprache also ein Wort der Länge $n \geq |z| < 2n$, dann muss die Sprache unendlich sein, sonst ist sie endlich.
Ob die Wörter enthalten sind, kann man mit dem Wortproblem prüfen.*[^2]

### Abgeschlossenheit
- Kontexfreie Sprachen sind unter der [[Formale Sprache#Vereinigung|Vereinigung]] [[Abgeschlossenheit von Operationen|abgeschlossen]]
- Kontexfreie Sprachen sind unter dem [[Formale Sprache#Produkt|Produkt]] [[Abgeschlossenheit von Operationen|abgeschlossen]]
- Kontexfreie Sprachen sind unter dem [[Formale Sprache#Kleenscher Abschluss|Kleenschen Abschluss]] [[Abgeschlossenheit von Operationen|abgeschlossen]]

### Schnitt mit regulärer Sprache
- Der Schnitt einer **kontextfreien Sprache** mit einer [[Reguläre Sprache|regulären Sprache]] ist **kontextfrei**

## Beispiele
- Die Sprache $L = \{a^jb^j\}$
- Die Sprache $L = \{w \in \{a, b\}^*: w \text{ ist Palindrom}\}$


#FSK 

[^1]: Sabel - Satz 5.9.1 
[^2]: Sabel - Satz 5.9.1