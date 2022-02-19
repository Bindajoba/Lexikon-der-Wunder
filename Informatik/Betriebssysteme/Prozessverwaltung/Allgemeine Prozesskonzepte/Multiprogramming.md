TARGET DECK: Universität::Informatik::Betriebssysteme

## Beschreibung
**Multiprogramming** ist eine Form [[Prozess|Prozesse]] auszuführen.
Zwischen Prozesse wird durch Unterbrechungen hin und her gewechselt.

Das Gegenstück ist [[Multiprogramming]]

Q: Was versteht man unter Multiprogramming?
A: Mehrere Prozesse Prozesse werden gleichzeitig auf einem Prozessor ausgeführt.
<!--ID: 1643668652075-->


Q: Was ist der Hauptvorteil von Multiprogramming?
A: Die CPU-Auslastung ist höher.
<!--ID: 1643668652214-->




## Funktionsweise
### Prozesswechsel
Seien A, B, C Prozesse. Ein Betirebssystem nach Multiprogramming führt alle gleichzeitig aus, indem schnell zwischen den Prozessen gewechselt wird.

Dies wird bewerkstelligt, indem man Programm A startet und im (willkürlich) 6 [[Zeitquantum|Zeitquanten]] gibt, um zu terminieren. 
Terminiert A nicht, wird der [[Dispatcher]] (ein Programm im Speicher) ausgeführt, um zum nächsten Prozess B zu wechseln.
Dazu wird der [[Prozesskontext]] von A gespeichert. Ist A nach Durchlaufen aller anderen Prozesse wieder an der Reihe, wird der Prozesskontext wieder geladen.


## Eigenschaften
### Vorhersehbarkeit
Man kann nicht vorhersehen, in welcher Reihenfolge, Prozesse ausgeführt werden. Der Ablauf ist nicht reproduzierbar.

#Betriebssysteme 