TARGET DECK: Universität::Informatik::SWT

# Beschreibung
Die Anforderungsanalyse soll feststellen, welche Anforderungen der Auftraggeber an die zu erstellende Software hat und wie man diese am besten für die Softwareingenieure formuliert.

Im engeren Sinne ist die Anforderungsanalyse eine sukzessive Verfeinerung der Anforderungen bis die Software Konzeptionisiert werden kann.[^1] 

Q: Was ist das Ziel der Anforderungsanalyse? [[Anforderungsanalyse]]
A: Anforderungen sukzessive zu verfeinern, bis man eine Software daraus entwerfen kann.
<!--ID: 1641730454604-->


Q: Was versteht man unter dem Begriff der (Fach-)Domäne? ([[Anforderungsanalyse]])
A: Das Anwendungsumfeld und der Verwendungszweck der Software (z.B Videospiel, Messenger, Social Media) 
<!--ID: 1641730454690-->


Q: Was ist das Ziel der Domänenanalyse? ([[Anforderungsanalyse]])
A: Möglichst viele Anforderungen aus der Domäne der Software zu generieren.
<!--ID: 1641730454777-->


# Varianten
In der SWT-Vorlesung wurden uns zwei Varianten vorgestellt. Eine ist besonders für [[Objektorientierte Programmierung|objektorientierte Programme]] geeignet. Die andere kann auch für andere Paradigmen verwendet werden.

## Objektorientierte Anforderungsanalyse (Seemann)
Diese Anforderungsanalyse folgt den Schritten, die von Seemann und von Gudenberg beschrieben wurden. Sie fokussiert stark auf die Verwendung von UML-Diagrammen zur Generierung von Anforderungen.

Die Analyse gliedert sich in zwei Bestandteile:
- Das Finden von Objekten
- Das Strukturieren von Objekten

Wichtigste Aufgabe der Analyse ist es Objekte zu finden, die für die Software relevant sind.
Dazu kann man eine [[CRC-Karte]] aller schon bekannten Klassen anfertigen.

Die CRC-Karten werden dann in einem soganannten Analyse-[[Klassendiagramm]] miteinander verbunden.

Q: Was sind die zwei Bestandsteile der Analyse beim OOAD?
A: - Finden von Objekten
- Strukturieren von Objekten
<!--ID: 1641730454938-->


Q: Welche Stufe des Klassendiagramms sollte das bei der Analyse (OOAD) erzeugte Klassendiagramm besitzen?
A: Analyse-Klassendiagramm
<!--ID: 1641730455073-->



## Traditionelle Anforderungserhebung (Nicht zwingend objektorientiert)
Siehe [[Anforderungserhebung (Broy)]]


## Methoden der Methoden zur Anforderungsfindung
Broy und Kuhrmann stellen einige Methoden vor, mit denen man auf Basis der entdeckten Anforderungen Systeme entwickeln kann.
In manchen dieser Methoden werden immer noch neue Anforderungen aufgedeckt. In anderen ist die Implementierung von Funktionsfähigem Code eher im Vordergrund.


Diese Methoden passen daher irgendwie nicht so gut in den Artikel der Anforderungsanalyse. Für ihren eigentlichen Standpunkt habe ich zwei Vorschläge:
- Mit den Methoden soll man von der Anforderungsanalyse zum [[Systementwurf]] übergehen
- Die Methoden stehen über Anforderungsanalyse und System entwurf.
D.h. Anforderungsanalyse und System müssen in die Methoden eingebettet werden.
*Ich habe gemerkt, dass der Stoff hier nicht relevant ist. Somit ist die Fragestellung egal. Ich will meine Zeit zurück!*

Die Methoden sind
- [[Design Thinking]]
- [[Feature-Driven Development]]


#Softwaretechnik 

[^1]: https://www.isyde.de/unser-know-how/anforderungsanalyse