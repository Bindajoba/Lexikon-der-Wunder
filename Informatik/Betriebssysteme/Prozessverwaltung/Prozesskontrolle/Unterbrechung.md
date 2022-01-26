## Beschreibung
Eine Unterbrechung ist das Maschinenkonzept für die Behandlung nicht [[Determinismus|deterministischer]] Abläufe
Eingerade aktiver Prozess wird dabei unterbrochen und eine Unterbrechungsbehandlungsroutine eingeschoben.

Analog wie bei [[Prozedur|Prozeduraufrufen]] müssen Informationen über den gerade aktiven Prozess gespeichert werden, um später an der Stelle fortfahren zu können.
Üblicherweise wird bei katastrophalen Fehlern aber der [[Prozess]], weshalb dieses Vorgehen oft nicht nötig ist.  

## Unterscheidung
### Externe Unterbrechung (Interrupt)
Eine externe Unterbrechung wird durch Ereignisse außerhalb des zu unterbrechenden Prozesses ausgelöst, wie Signale von E/A-Geräten oder Zeitgebern. (z.B. Der Drucker ist fertig)

Der Prozessor [[Moduswechsel|wechselt]] dann automatisch in den [[Prozessormodus|Kernel Modus]], bearbeitet den Interrupt und kehrt dann zur vorherigen Arbeit zurück

Dies geschieht über einen sogenannten Interrupt Request, der durch eine Signalfolge an die CPU realisiert wird.[^1]


### Interne Unterbrechung
Sie wird vom ausgeführten Prozess selbst ausgelöst und kann zur Ursache z.B. eine arithmetische Ausnahme haben. SIe bewirkt ebenfalls eine Unterbrechung der CPU und die Aktivierung der Unterbrechungsbehandlung im Systemkern. (Die Unterbrechungsbehandlung findet ebenfalls im Kernel-Modus statt)

*Der Prozessor wechselt in den Kernelmodus, bearbeitet die Unterbrechung und kehrt dann zum Program zurück*


## Konflikte bei Unterbrechungen
Bei der Abarbeitung von Unterbrechungen kann es zu Konflikten kommen. Ursachen sind:
1. Während der Unterbrechensbehandlung treten weitere Unterbechungen auf
2. Es treffen gleichzeitig mehrere Unterbrechungenswünsche ein

Lösung des Konflikte durch Hierarchien:
- Nutzerprozesse = Prio 0
- Externe Unterbrechungen = bis zu Prio 31 (bei 5 Prio-Bits)

Interne Unterbrechungen haben die gleiche Priorität wie der Prozess, der ihn wirft. 
Unterbrechungen werden nur bei höherer Priorität unterbrochen.

Die Priorität eines Programms wird im [[Interrupt Priority Level]] oder IPL, Teil des Prozessstatuswortes im [[Prozesskontrollblock]] gespeichert.

#Betriebssysteme 

[^1]: https://www.youtube.com/watch?v=xHu7qI1gDPA&t=34s