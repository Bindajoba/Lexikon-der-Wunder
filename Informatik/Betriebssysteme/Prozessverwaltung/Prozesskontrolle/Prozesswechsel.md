## Beschreibung
Beim [[Multiprogramming]] ist es üblich, dass zwischen Prozessen gewechselt wird. Wie das funktioniert soll nun erklärt werden.


## Vorgehen
Muss ein Prozess gewechselt werden, passiert folgendes
1. Aktualisierung und Sicherung des [[Prozesskontrollblock]]
D.h. Sicherung der Zustandsinformationen und Aktualisierung und Sicherung der Kontrollinformationen
2. Einfügen des Prozesskontrollblocks des bisherigen Prozesses in die Warteschlange des [[Scheduler|Schedulers]]
3. Auswahl eines anderen Prozesses zur Ausführung
4. Wiederherstellung und Aktualisierung des Prozesskontrollblocks des neuen Prozesses (Einschießlich der Änderung des Zustands auf "Running")

## Ursachen
- Externe Ereignisse verursachen [[Unterbrechung#Externe Unterbrechung Interrupt|Unterbrechung]] des aktuellen Programms
(z.B. I/O interrupt, emory fault, Drucker fertig, Tastatureingabe)
- Das aktuell laufende Programm verursacht einen Fehler und damit eine [[Unterbrechung]]
(z.B. Exception: Division durch 0)
- Ein Supervisor-Call ruft eine Betriebssystem-Funktion aus, wodurch der aktuelle Befehl unterbrochen wird.
(Üblicherweise weil der [[Scheduler]] einen neuen Prozess ausführen will)


#Betriebssysteme 