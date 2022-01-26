## Definition
Eine [[Grammatik]] $G$ $G$ ist vom **Typ 2** bzw **kontextfrei** (**context-free grammar**, **CFG**) gennannt, wenn für alle Produktionen $(- \to r) \in P$ gilt: $a = A \in V$, 
D.h. die linken Seiten der Produktionen bestehen aus genau einer Variablen

Eine kontextfreie Grammatik ist ein Spezialfall einer [[Kontextsensitive Grammatik|kontextsensitiven Grammatik]] und die Verallgemeinerung einer [[Reguläre Grammatik]]
Kontextfreie Sprachen sind der zweite Typ von Sprachen der [[Chomsky-Hierarchie]] 

## Eigenschaften
### Erzeugte Sprache
EIne kontextfreie Grammatik erzeugt eine [[Kontextfreie Sprache]]

### $\varepsilon$-Produktionen
Fügt man einer kontextfreien Grammatik eine Produktion eine sogenannte $\varepsilon$-Produktion $A \to \varepsilon$ hinzu, so ist die erzeugte Sprache immer noch kontextfrei.[^1]

*Das folgt, indem man eine $\varepsilon$-Produktion zum Start der Sprache hinzufügt und dann die vorher hinzugefügte Produktion wieder entfernt.*[^2]

## Umformungen
### Inlining von Produktionen
Sei $G = (V, \Sigma, P, S)$ eine CFG, die Produktionsregeln der Form 
- $A \to uBv \in P$
- $B \to w_1 | ... | w_n$ (mit Satzformen $w_i$)
besitzt. Dann kann man $A \to uBv$ durch $A \to uw_1v | ... | uw_nv$ ersetzen

 Formell:
 $$G' = (V, \Sigma, P\backslash \{A \to uBv\} \cup \{A \to uw_1v | ... | uw_nv\}, S)$$ Dann erzeugen $G$ und $G'$ dieselbe Sprache $L(G) = L(G')$
 
 ### Sharing von Satzformen
Sei $G = (V, \Sigma, P, S)$ eine CFG, die Produktionsregeln der Form 
- $A \to w_1 ... w_n \in P$ (mit Satzformen $w_i$)
bestizt. Dann kann man die Satzformen $w_i$ durch neue Variablen $B_i$ ersetzen. Die Grammatik erhält die Produktionen:
- $A \to B_1 ... B_n \in P$
- $B_1 \to w_1, ..., B_n \to w_n$
Die erzeugt Sprache verändert sich dann nicht.

 ### Elimination von Links-Rekursion
 Sei $G = (V, \Sigma, P, S)$ eine CFG, die Produktionsregeln der Form 
- $A \to Au_1|...|Au_n|w_1|...|w_m$ (mit Satzformen $u_1, w_i$, wobei $w_i$ nicht mit $A$ beginnt)
besitzt. Dann die Produktionen durch folgende Produktionen ersetzen:
- $A \to w_1B_1 ... w_nB_n | w_1 | ... | w_n$
- $B \to u_1 | ... | u_n | u_1B | ... | u_nB \to w_n$
Die erzeugt Sprache verändert sich dann nicht.

*Die Idee ist, dass die ursprüngliche Grammatik Satzformen der Form $w_ju_{i1}...u_{ik}$* haben. Offensichtlich kann man das $w_j$ auch am Anfang erzeugen und die $u_i$ rekursiv danach. So wird die Linksrekursion los.
 
 ### Entfernen von Einheitsproduktionen
 Eine Einheitsproduktion ist eine Produktion der Form $A \to B$.
 Besitzt man eine solche Produktions, dann erhält man die Ableitungsschritte $A \Rightarrow B \Rightarrow$. Es ist klar, dass man auch gleich eine Produktion $A \to w$ nutzen könnte.
 
 Bilden die Einheitsproduktionen aber einen Kreis, dann muss man aufpassen, welche Produktion man entfernt, im schlimmsten Fall kann man manche Produktionen von der Startvariable nicht mehr erreichen.

Algorithmus 5 berücksichtigt dieses Problem
![[Entfernen von Einheitsproduktionen.png]] [^3]
 
 ### Umwandlung in Chomsky-Normalform
 Siehe [[Chomsky-Normalform]]
 
## Eigenschaften
### Ableitungen
Zu einem Wort gibt es immer eine [[Ableitung eines Wortes|Links- und Rechtsableitung]].

Vergleiche dies mit einer [[Kontextsensitive Grammatik]] bei der man nicht alle [[Wort|Wörter]] erreichen kann, wenn man immer die linkeste/rechteste [[Grammatik|Satzform]] ableitet.

Überhaupt ist es bei **Kontextfreien Grammatiken** egal, in welcher Reihenfolge man ableitet.

#FSK 

[^1]: Sabel - Definition 3.2.5
[^2]: Sabel - Satz 3.2.6
[^3]: Sabel - 5.2.1