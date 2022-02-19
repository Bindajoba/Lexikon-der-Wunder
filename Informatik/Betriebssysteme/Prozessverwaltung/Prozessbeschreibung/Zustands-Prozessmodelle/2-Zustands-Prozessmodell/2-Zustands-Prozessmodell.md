TARGET DECK: Universität::Informatik::Betriebssysteme

## Beschreibung
Im 2-Zustandsmodell können sicht [[Prozess|Prozesse]] in zwei Zuständen befinden:
- not running: Das Programm wird gerade nicht von der CPU gelesen
- running: Das Programm wird gerade von der CPU gelesen.

Q: Welche Zustände hat das 2-Zustandsprozessmodell
A: - running
- not running
<!--ID: 1643668655491-->



Ein Programm kann durch den [[Dispatcher]] aktiviert werden. 
![[2-Zustands-Prozessmodell.png]]

Programme im Zustand not running werden in einer Warteschlange gespeichert. Beim Suspendieren eines Programms wird dieses in die Warteschlange eingereiht.

#Betriebssysteme 