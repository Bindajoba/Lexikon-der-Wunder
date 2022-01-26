TARGET DECK: Universität::Informatik::Betriebssysteme

## Beschreibung
Ein Prozess ist ein [[Programm]] in Ausführung. Er kann als Eigentümer und Verwalter von (eigenen) Ressourcen betrechtet werden.
Prozesse verfügen über einen Bereich im Hauptspeicher und kann über zugeordnete E/A-Geräte, E/A-Kanäle und Dateien verfügen.

Ein Programm wird zum Prozess, wenn es in den [[Hauptspeicher|Speicher]] geladen wird, einen [[Prozesskontext]] erhält und gestartet wird.

Q: Was ist ein Prozess? ([[Prozess]])
A: Ein Programm in Ausführung
<!--ID: 1642897217464-->


### Thread
Der Teil eines Prozesses, der sich um die Erfüllung einer Aufgabe und weniger um die Verwaltung von Ressourcen kümmert, dann kann man Prozesse als [[Thread]] bezeichnen.

*Dummerweise wird genau dann wenn man von Threads redet Prozess gesagt, was bedeuten könnte, dass die Wörter nicht ganz so gut differenzierbar sind*

## Erzeugung
Prozesse können von anderen Prozessen gestartet werden. Ersteres nennt man dann Kindprozesse

Siehe [[Prozesserzeugung]]

## Terminierung
Prozesse können terminieren, indem sie angehalten werden oder an die Rücksprung-Anweisung kommen


## Struktur eines Prozesses im Hintergrundspeicher
- [[Prozesskontrollblock]]
- User Stack
- Private User Adress Space (Programmdaten)
- Shared Adress Space

## Prozessdescriptor
Der Prozessdeskriptor enthält alle Daten, um einen Prozess vollständig zu beschreiben.

**Bestandteile eines Prozessdescriptor in [[Modellmaschine MI|MI]]**
- Eindeutiger Name des Prozesses
- Der Name des Benutzers, dem der Prozess zugeordnet ist
- Zugeordneter Rechenkern
- Spezifikation des Ereignisses, auf das der Rechenkern wartet
- Ablaufpriorität des Prozesses

## Prozesswechsel
Siehe [[Prozesswechsel]]

#Betriebssysteme 