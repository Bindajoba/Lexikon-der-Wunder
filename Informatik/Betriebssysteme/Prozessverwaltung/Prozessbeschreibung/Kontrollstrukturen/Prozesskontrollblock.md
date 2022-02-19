## Bestandteile


### Prozessidentifikation
Der Prozessindentifikator enthält
- Seinen eigenen numerischen identifikator (Prozess-ID, PID)
- PID des [[Prozess|Elternprozesses]]
*Damit ist nicht das Programm gemeint, das dieses als Unterprogramm hat, das ist was ganz anderes!*
- ID des Eigentümers/Nutzers des Programms

### Prozesszustandsinformationen
Die Prozesszustandsinformationen enthalten genauere Informationen über die aktuellen [[Register]] und damit des [[Prozesskontext]] des [[Prozess|Prozesses]].

*Ein Programm kann während seiner Ausführung auf Prozessorregister zugreifen. Wird ein Programm suspendiert, müssen diese gespeichert werden, damit das Programm wieder reibungslos weiterlaufen kann.*
In der Regel gehört dazu der Stackpointer, Kontroll- und Statusregister, usw.


### Prozesskontrollinformationen
Die Prozesskontrollinfos speichern 
- Den Zustand des Prozesses [[7-Zustands-Prozessmodell|Zustand]]
- Die Priorität des Prozesses
	- Spezielle Daten, wie die Zeit, wie lange der Prozess schon wartet
	- [[Ereignis|Eregnisse]], auf die der Prozess wartet.


## Implementierung
![[Prozesskontrollblock.png]]

*Aber dann ist ja der Zustand im Stack und im PCB gespeichert!*

#Betriebssysteme 