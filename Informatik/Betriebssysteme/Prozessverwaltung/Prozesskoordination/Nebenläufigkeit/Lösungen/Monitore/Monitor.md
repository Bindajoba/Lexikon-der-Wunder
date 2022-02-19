TARGET DECK: Universität::Informatik::Betriebssysteme

# Beschreibung
Die Synchronisation wird nicht durch eine externe [[Semaphor]], sondern durch die Datenstruktur erledigt, auf die man zugreift.

**Hoare'sche Monitore** fassen Daten, darauf definierte Operationen und die Zugriffsynchronistation (für [[Prozess|Prozesse]]) zusammen.

# Visualisierung
Stell dir ein Formel 1 Wagen vor. Diesem Wegen stehen verschiedene Operationen zur Verfügung, z.B. fahren, blinken, Scheibenwischer betätigen, hupen, ...
In einen Formel 1 Wagen passt aber immer nur eine Person gleichzeitig hinein. Damit kann von dieser Person nur eine Operation gleichzeitig betätigt werden.

*Das ist wie bei Java. Da gibt es ein Objekt (Formel 1 Wagen), in das nur eine Person gleichzeitig hinein kann.*

Q: Was ist das Linnhoff-Bild zu Monitoren?
A: Ein Formel 1 Wagen
<!--ID: 1643668654173-->



# Definition
Ein Monitor ist ein Objekt, das sich im wesentlichen aus einer Menge von Prozeduren auf gegebenfalls gemeinsam genutzten Daten zusammensetzt.
Entscheidend ist, dass der Monitor - zu jedem Zeitpunkt - stets nur von (höchstens) einem Prozess genutzt werden darf.
*Daraus folgt nach Linnhoff, dass die Prozesse eines Monitors atomar ablaufen.*


# Struktur
## Außenstruktur
Irgendwie muss gewährleistet werden, dass trotz der Tatsache, dass nur ein Prozess gleichzeitig im Monitor sitzen darf, alle [[Prozess|Prozesse]] an die Reihe kommen.
Dazu verwendet man Warteschlangen. Es gibt Warteschlangen für:
1. Prozesse, die den Monitor gerade verlassen haben (wozu auch immer das nötig ist)
2. Prozesse, die den Monitor normal betreten wollen
3. Prozesse, die auf eine Bedingung (seitens des Monitors) warten, bevor sie eintreten.
Für jede Bedingung gib es eine eigene Warteschlange.
![[Monitor Beispie.png]]

Q: Aus welchen 3 Typen von Warteschlangen besteht der Monitor?
A: - Ausgangsschlange nach dem Monitor
- Eingangsschlange für normal wartende Prozesse
- Engangsschlange für auf Bedingungen wartende Prozesse
<!--ID: 1643668654282-->


## Innenstruktur
Nun soll darauf eingegangen werden, worus der Monitor im Inneren besteht. Siehe dazu den blauen Kast im unteren Bild:
![[Monitor Strukur.png]]
Man sieht, der Monitor besteht aus den Bestandteilen:
1. **Lokale Daten**
Daten, auf die von den Prozessen in der Monitor-Klasse zugegriffen wird.
2. **Bedingungsvariablen**
Für jede Bedingung wird eine Warteschlange erstellt
3. **Prozeduren**
Atomare [[Prozedur|Prozeduren]], sie können jedoch durch cwait() unterbrochen werden.
4. **Initialisierungscode**
Initialisierung der Lokalen Daten

*cwait(Bedingung) bedeutet Conditional Wait. Es stoppt den Prozess und bewegt ihn in die entsprechende Warteschlange. Der Prozess wird fortgesetzt, wenn die Bedingung erfüllt ist und der Monitor frei ist. Das Gegnstück dazu ist csignal(Bedingung).*

Q: Aus welchen Innenbestandteilen besteht der Monitor? ([[Monitor]])
A: 1. Lokale Daten
2. Bedingungsvariablen
3. Prozeduren
4. Initialisierungscode
<!--ID: 1643668654387-->



# Beispiele
## Monitor in Java
Mit dem Schlüsselwort **synchronized**, kann man eine Objektmethode, Klassenmethode oder einen Block schützen.
Das heißt, dass die Methode nur von einem einzigen [[Thread]] gleichzeitig aufgerufen werden kann. Das wird bewerkstelligt, indem die Methode einen Platz für einen Lock hat, welches von einem Thread belegt werden kann.

Der Lock wird aufgehoben, wenn
- die synchronisierte Methode verlassen wird
- eine Ausnahme erfolgt
- ein wait() Aufruf getätigt wird

Q: Mit welchem Schlüsselwort kann man in Java auf einem Objekt einen Monitor erstellen?
A: synchronized
<!--ID: 1643668654499-->




#Betriebssysteme 