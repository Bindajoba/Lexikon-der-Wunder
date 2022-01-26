TARGET DECK: Universität::Informatik::Betriebssysteme

# Beschreibung
Speicherverwaltung hat üblicherweise die Motivation, dass der [[Hauptspeicher]] nicht ausreicht, um alle Programme zum Laufen zu befähigen. Das Problem wird behoben, indem ein Hintergrundspeicher dazugenommen wird. Dieser muss aber verwaltet werden.

Die Speicherverwaltung ist dafür zuständig Daten aus dem Hauptspeicher in den Hintergrundspeicher zu laden.



# Anforderungen
Es werden fünf Anforderungen an die Speicherverwaltung gestellt:
1. **Relocation** (Wiederfindung)
Eine Datenstruktur soll dafür dienen, dass ein [[Prozess]] genau die Sachen wiederfindet, die er abgelegt hat.
2. **Protection**
Jder Prozess muss gegen ungewollte EInmischungen anderer Prozesse geschützt werden
3. **Sharing**
Es muss einen öffentlichen Datenbereich zugegriffen werden können
4. **Logical Organization**
Der Hauptspeicher ist immer als linearer (1-dimensionaler) Adressraum organisiert, der aus einer Folge von Bits besteht.
5. **Physical Organization**
Umfasst die Einteilung ein Hauptspeicher (schneller Zugriff) und Hintergrundspeicher (langsamer und billiger)



Q: Anforderungen an eine Speicherverwaltung
A: - Relocation
- Protection
- Sharing
- Logical Organization
- Physical Organization

# Variationen der Partitionierung
Beim Partitionieren gibt es grundsätzlich zwei Herangehensweisen:

Q: Welche grundsätzlichen drei Herangehensweisen der Partitionierung gibt es? ([[Speicherverwaltung]])
A: - Feste Partitionierung
- Dynamische Partitionierung
- Hybride Partitionierung

## Feste Partitionierung
*Der Speicher wird wie ein Hotel in feste Räume partitioniert.*
Nachteil: Dadurch kann es sein, dass manche dieser Räume nie aufgefüllt werden, es entsteht [[Interne Fragmentierung]].

Die Räume müssen nicht unbedingt gleich große Räume haben.
Programme müssen immer kleiner oder gleich der Partition sein. (Passt das Programm nicht in den Speicher, dann muss es vom Programmierer in kleinere Teilprogramme zerlegt werden.)

### Paging
Der Speicher wird in feste Blöcke partitioniert und ein [[Prozessimage]] in aneinander grenzenden Blöcken gespeichert. Sind die Blöcke gleich groß, so spricht man von [[Page|Pages]]

*Anscheinend müssen diese Blöcke aber nicht immer angrenzend sein.*

Wird ein Prozess gestartet, werden die Pages des Prozesses aus dem [[Hintergrundspeicher]] in den [[Hauptspeicher]] geladen.
Danach werden sie in den Hintergrundspeicher zurücktransportiert.


## Dynamische Partitionierung
*Die Wände des Hotels sind verschiebbar. d.h. Speicherpartitionen können variabel groß sein.*
Nachteil: Der Speicher kann so partitioniert sein, dass in die Räume zwischen den Daten kein neues Programm passt, es entsteht eine [[Externe Fragmentierung]]

Grundidee ist, dass man so viel Platz reserviert, wie viel man braucht, und dann erst die Trennwand zieht.
Um die Probleme der genannten externen Fragmentierung zu mindern, kann man entweder die Partitionen der Prozesse zusammenschieben (Compaction) oder die Speicherplätze schlau verteilen.
Hier für gibt es die Drei Strategien
- Best-Fit: Suche die kleinste Lücke, in die der Prozess passt
- First-Fit: Nimm vorne die erste passende Lücke
- Next-Fit: Nimm ab letzter Belegung die nächster passende Lücke

Q: Was sind die drei simplen Strategien zur dynamischen Partitionierung?
A: - Best-Fit
- First-Fit
- Next-Fit

### Segmentierung
Der Prozess wird als zusammenhängender Block in aufeinanderfolgenden Speicherzellen (des [[Hauptspeicher]]) abgelegt.

Wird ein neuer Prozess abgelegt, wird der erste Prozess nicht entfernt. So muss bei einer erneuten Ausführung vom ersten Prozess nicht alles neu geladen werden.

Das Betriebssystem muss dabei stets wissen, wo im [[Hintergrundspeicher]] bzw. [[Hauptspeicher]] das [[Prozessimage]] abgelegt ist.

## Hybride Partitionierung
Vereint Methoden und Nachteile beider Partitionierungen, man erhält interne und externe Partitionierung. 

Zum Beispiel [[Buddy-System]]



# Definition


#Betriebssysteme 


