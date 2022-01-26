## Beschreibung
Eine [[Formale Sprache]] ist regulär, wenn sie eine reguläre Grammatik besitzt.

## Definition
Eine [[Formale Sprache]] ist regulär, wenn es eine [[Reguläre Grammatik]] gibt, die sie erzeugt.

## Eigenschaften
### Pumping Lemma
Reguläre Sprachen erfüllen das [[Pumping Lemma|Pumping Lemma für reguläre Sprachen]]

### Abgeschlossenheit
- Die regulären Sprachen sind abgeschlossen bzgl. [[Formale Sprache|Vereinigung]]
Die Vereinigung der Sprachen zu den [[Regulärer Ausdruck|regulären Ausdrücken]] $\alpha_1, \alpha_2$ kann durch den regulären Ausdruck $(\alpha_1|\alpha_2)$ erzeugt werden 
- Die regulären Sprachen sind abgeschlossen bzgl. [[Formale Sprache|Produkt]]
Das Produkt der Sprachen zu den [[Regulärer Ausdruck|regulären Ausdrücken]] $\alpha_1, \alpha_2$ kann durch den regulären Ausdruck $\alpha_1\alpha_2$ erzeugt werden 
- Die regulären Sprachen sind abgeschlossen bzgl. [[Formale Sprache|Kleeneschem Abschluss]][^1]
Der Kleenesche Abschluss der Sprache zum [[Regulärer Ausdruck|regulären Ausdruck]] $\alpha_1$ kann durch den regulären Ausdruck $(\alpha_1)^*$ erzeugt werden 
- Die regulären Sprachen sind abgeschlossen bzgl. [[Formale Sprache|Schnitt]]
Schneidet man zwei Sprachen, dann ist der Schnitt durch den [[Produktautomat]] notierbar, also regulär
- Die regulären Sprachen sind abgeschlossen bzgl. [[Formale Sprache|Komplementbildung]] zu $\Sigma^*$
In dem man die Endzustände eines Automaten umdreht, erhält man genau das Komplement der Sprache

### Entscheidbarkeit
- Das [[Leehrheitsproblem]] ist [[Entscheidbarkeit|entscheidbar]][^2]
Eine reguläre Sprache ist leer, wenn ihr [[Deterministischer Endlicher Automat|DFA]] keinen Weg vom Anfang zum Ende hat
- Das [[Endlichkeitsproblem]] ist entscheidbar[^3]
Eine Sprache ist endlich, wenn ihr Automat keine [[Pumping Lemma|Schleife]] auf dem Weg vom Anfang zum Ende enthält
- Das [[Schnittproblem]] ist entscheidbar[^4] 
Der Schnitt zweier Sprachen ist leer, wenn ihr [[Produktautomat]] das Leerheitsproblem erfüllt 
- Das [[Äquivalenzproblem]] ist entscheidbar[^5]
Zwei reguläre Sprachen sind gleich, wenn ihr [[Minimalautomat]] gleich ist.

## Beispiele
- Jede [[Kontextfreie Sprache]] über einem unären [[Alphabet]] $\Sigma = \{a\}$ ist **regulär**

#FSK 

[^1]: Sabel - Theorem 4.12.4
[^2]: Sabel - Satz 4.13.1
[^3]: Sabel - Satz 4.13.2
[^4]: Sabel - Satz 4.13.3
[^5]: Sabel - Satz 4.13.4