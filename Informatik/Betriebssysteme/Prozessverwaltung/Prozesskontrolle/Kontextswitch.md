TARGET DECK: Universität::Informatik::Betriebssysteme

## Beschreibung
Beim [[Multiprogramming]] ist es üblich, dass zwischen Prozessen gewechselt wird. Wie das funktioniert soll nun erklärt werden. Also ein Prozesswechsel.

Es wird **Kontextswitch** genannt, da der [[Prozesskontext]] gewechselt wird. (Der Prozesskontext ist im [[Prozesskontrollblock]] gespeichert) 
Der Kontextswitch ist nicht zu Verwechseln mit dem [[Prozessormodus|Moduswechsel]]

Q: Wovon hängt der Aufwand von einem Kontextswitch im wesentlichen ab?
A: Von der Zahl der im Przozess invlvierten Register (diese müssen mit gespeichert werden.)
<!--ID: 1643668653096-->


## Vorgehen
Muss ein Prozess gewechselt werden, passiert folgendes
1. Aktualisierung und Sicherung des [[Prozesskontrollblock]]
D.h. Sicherung der Zustandsinformationen und Aktualisierung und Sicherung der Kontrollinformationen
2. Einfügen des Prozesskontrollblocks des bisherigen Prozesses in die Warteschlange des [[Scheduler|Schedulers]]
3. Auswahl eines anderen Prozesses zur Ausführung
4. Wiederherstellung und Aktualisierung des Prozesskontrollblocks des neuen Prozesses (Einschießlich der Änderung des Zustands auf "Running")

Q: Welche Aktionen muss das Betriebssystem bei einem Kontextswitch zwischen verschiedenen Prozessen vornehmen?
A: 1. Sicherung des Prozesskontrollblocks
2. Einfügen des Prozesskontrollblocks in die Scheduler-Warteschlange
3. Auswahl eines anderen Prozesses
4. Wiederherstellung des Prozesskontrollblocks des neuen Prozesses
<!--ID: 1643668653208-->


## Ursachen
- Externe Ereignisse verursachen [[Unterbrechung#Externe Unterbrechung Interrupt|Unterbrechung]] des aktuellen Programms
(z.B. I/O interrupt, memory fault, Drucker fertig, Tastatureingabe)
- Das aktuell laufende Programm verursacht einen Fehler und damit eine [[Unterbrechung]]
(z.B. Exception: Division durch 0)
- Ein Supervisor-Call ruft eine Betriebssystem-Funktion aus, wodurch der aktuelle Befehl unterbrochen wird.
(Üblicherweise weil der [[Scheduler]] wegen timeout einen neuen Prozess ausführen will)


#Betriebssysteme 