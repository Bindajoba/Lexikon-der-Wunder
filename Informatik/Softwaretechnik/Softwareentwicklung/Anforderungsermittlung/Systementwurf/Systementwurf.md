TARGET DECK: Universität::Informatik::SWT

# Beschreibung
Der Systementwurf folgt der [[Anforderungsanalyse]]. Er befasst sich mit dem Entwurf des Systems.

# Schritte
Q: Welche vier Schritte durchläuft man beim Systementwurf (OOD)
A: 1. Systemarchitektur festlegen
2. Klassenentwurf
3. Schnittstellen spezifizieren
4. Detailentwurf
<!--ID: 1645543054200-->






## Entwurf nach Seemann
### Systemarchitektur festlegen
Am Ende der [[Anforderungsanalyse]] mussten bereits Aspekte konkreten Realisation in Betracht gezogen werden.

Bei der Festlegung der Systemarchitektur betrachtet man üblicherweise die Klassen, die man in der Analyse gefunden hat und identifiziert jede Klasse mit einer Softwarekomponente.
Dann sucht man die Klassen die als Schnittstellen zwischen den Komponenten fungieren.

Oft muss man aber keine Klassen zusammenfassen.sen zu erhalten. Die Aufgaben der Klassen der Analyse sind häufig so umfangreich, dass sie zu einem gesamten Subsystem aufgespalten werden können.

Die nun erhaltenen Subsysteme des Systems können zu einer Architektur neustrukturiert werden. Die gewählte Architektur kann einigen beliebten Mustern folgen. (z.B. dem [[Drei-Schichten-Modell]])

### Klassenentwurf
Zu jeder Analyseklassen werden eine oder mehrere Entwurfklassen erstellt.
Dem Namen nach zu urteilen, erhalten Klassendiagramme wohl jetzt die nächste [[Klassendiagramm#Varianten|Detailstufe]]. 

### Schnittstellen spezifizifieren
Nächster Schritt ist, die Schnittstellen zwischen Klassen zu verfeinern und zu spezifizieren.
Dabei muss man eventuell auf Interaktionsdiagramme (wie [[Sequenzdiagramm]] oder [[Kommunikationsdiagramm]]) zurückgreifen.

In dieser Phase wird man viele Erkenntnisse über die Kommunikation von Klassenteilen habe, weshalb das Klassendiagramm großen Änderungen unterworfen sein könnte.

### Detailentwurf
Das Klassendiagramm wird erst jetzt auf die Möglichkeiten der verwendeten Programmiersprache angepasst. Hat man Mehrfachvererbung im Diagramm, verwendet aber java, so muss das Diagramm durch interfaces angepasst werden 



#Softwaretechnik 


