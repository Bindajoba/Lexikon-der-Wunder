TARGET DECK: Universität::Informatik::SWT

## Beschreibung
Eine **Inspektion** ist die formellste der drei Prüfungsvarianten einer [[Manuelle Software Prüfung]].


Q: Was ist eine [[Inspektion]]? 
A: Code wird in formeller Umgebung von einer Gruppe langwierig überprüft. 
<!--ID: 1644996890336-->


## Vorgang
Die Inspektion lässt sich meistens in 6 Phasen aufteilen.

1. **Planungsphase**
Termin, Raum wird von einem Moderator vorbereitet.
2. **Überblicksphase**
Jeder Teilnehmende erhält spezielle Rollen
3. **Vorbereitungsphase**
Inspektoren begutachten den Code und notieren sich die gefundenen Fehler. Die Sitzung hat noch nicht angefangen! Die Fehler sind für den nächsten Schritt relevant
4. **Inspektionsphase**
Die gesammelten Ergebnisse werden zusammengetragen und gemeinsam bewertet. Jetzt werden die Rollen wichtig.
5. **Nacharbeitungsphase**
Die entdeckten Fehler im Code werden ausgebessert
6. **Überprüfungsphase**
Die Änderungen werden nachträglich überprüft

Wichtig ist, dass in einer Inspektion Fehler und keine Lösungen besprochen werden.

## Rollen
### Moderator
Der Moderator soll die Inspektion organisieren udn die Dominanz einzelner Inspektoren verhindern.
Desweiteren ist er dafür verantwortlich eine lockere positive Arbeitsatmossphäre zu erzeugen.


### Gutachter
Der Gutachter führt das Team durch den Programmcode. Dabei kommentiert er wichtige Punkte und Entscheidungen des Autors.
Die Art und Geschwindigkeit, des Gutachter beiflusst maßgeblich, wie gut Inspektoren Fehler entdecken können.
*Im Englischen wird der Gutachter Reader genannt, was mehr Sinn ergibt.*

### Autor
Der Autor nimmt in der Sitzung ein vollkommen passive Rolle ein. Dadurc soll er einen Blick von außen auf seinen Programmcode bekommen.
Außerdem wird der Autor dadurch ermutigt, seinen Code ästhetisch zu gestalten, wie es beim [[Walkthrough]] der Fall ist. (Externalisierung)

### Protokollführer
Der Protokollführer erstellt einen Prüfbericht und notiert die gefundenen Fehler

### Inspektor
Die Rolle des Inspektors wird auch vom Moderator, Gutachter und Protokollführer eingenommen, es können aber weitere Inspektoren hinzugezogen werden.