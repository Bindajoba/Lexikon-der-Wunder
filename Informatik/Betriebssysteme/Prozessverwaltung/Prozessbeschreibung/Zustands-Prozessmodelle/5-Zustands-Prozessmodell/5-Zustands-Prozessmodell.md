TARGET DECK: Universität::Informatik::Betriebssysteme

# Beschreibung
Das **5-Zustands-Modell** ist eine Weiterentwicklung des [[2-Zustands-Prozessmodell]].

Der Zustand 'not running' wird weiter differenziert in
- ready
- blocked

Damit besteht das Modell aus den Zuständen:
- new: der prozess wurde erzeugt, aber noch nicht durch das Betriebssystem zur Menge der ausführbaren Prozesse hnzugefügt 
(Es gibt aber nicht unbedingt genug Speicher, um das Programm zu laden)
- ready: Der Prozess ist zur Ausführung bereit 
- running: Der Prozess befindet sich in der Ausführung
- blocked: Der Prozess wartet auf ein Ereignis (z.B. Ende einer [[EA-Operation]]) und kann erst zur Ausführung kommen, wenn das Ereignis eingetreten ist
- exit: Der Prozess wurde durch das Betriebssystem aus der Menge der ausführbaren Prozesse entfernt

![[5-Zustands-Prozessmodell.png]]

Q: Welche Zustände hat das 5-Zustandsprozessmodell
A: - new
- ready
- running
- blocked
- exit
<!--ID: 1643668655367-->



## Weitere Funktionen
### Priorisierung
Um bestimmte Prozesse zu Priorisieren, kann die ready-queue in verschiedene Queues unterteilt werden.

### Auslagerung von Prozessen
Was passiert, wenn alle Prozesse auf ein Ereignis warten und kein Speicher für neue Prozesse da ist?

Für diesen Zweck werden Prozesse in andere Speicher ausgelagert ([[Swapping]]). Dieser wird in einen [[Virtueller Speicher]] gespeichert.

Ob ein Prozess aber im Hauptspeicher oder im Nebenspeicher gelagert ist, macht es nötig, die Zustände des Prozesses weiter aufzuteilen. Daraus entsteht das [[7-Zustands-Prozessmodell]]

## Realisierung
Statt einer Warteschlange werden zwei genutzt.

![[5-Zustands-Prozessmodell Realisierung.png]]

Für Ereignisse unterschiedlicher Art werden unterschiedliche Wartelisten verwendet. 

![[5-Zustands-Prozessmodell Realisierung 2.png]]

#Betriebssysteme 