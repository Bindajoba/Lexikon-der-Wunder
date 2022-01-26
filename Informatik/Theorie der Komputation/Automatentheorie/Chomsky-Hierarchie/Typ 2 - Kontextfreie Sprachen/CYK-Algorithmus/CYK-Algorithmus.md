## Beschreibung
Der CYK-Algorithmus ist ein Algorithmus, um das [[Wortproblem]] für eine [[Kontextfreie Sprache]] in [[Laufzeit|polynomieller Zeit]] zu bestimmen.



## Algorithmus
Er funktioniert ungefähr so:
Die vorliegende Grammatik wird zur besseren  Handhabung erst in Chomsky-Normalform umgewandelt.

Der CYK soll herausfinden, ob ein [[Wort]] $w$ durch die Grammatik erzeugt wird.
Im ersten Schritt wird bestimmt, welche Buchstaben im Wort enthalten sind und welche Nichtterminale diese Buchstaben erzeugen.
Im zweiten Schritt wird überprüfft, welche Teilwörter der Länge 2 durch zwei der im ersten Schritt bestimmten Nichtterminale erzeugt werden können.
Im dritten Schritt wird überprüft, welche Teilwörter der Länge 3 durch die im ersten und zweiten Schritt bestimmten Nichtterminale erzeugt werden können.
Das geht so lange weiter, bis im letzten Schritt geprüft wird, durch welches Paar von Nicht-Terminale das Wort $w$ sich zusammensetzen lässt.
Gibt es eine Produktionsregel von der Startvariable zu diesem Nicht-Terminalpaar, dann ist das Wort in der Sprache enthalten.

Das Verfahren wird häufig durch eine Tabelle unterstützt

![[CYK-Algorithmus Algorithmus.png]][^1]

## Beispiel
Betrachte die [[Kontextfreie Sprache]] mit Produktionsregeln $P = \{S \to AC, A \to BE, E \to AD, C \to a, B\to b, D \to d\}$
Prüfe, ob das Wort $bbddc$ enthalten ist.
![[CYK.Algorithmus Beispiel 1.png]]![[CYK-Algorithmus Beispiel 1.2.png]]


#FSK 

[^1]: Sabel - Theorem 5.6.1