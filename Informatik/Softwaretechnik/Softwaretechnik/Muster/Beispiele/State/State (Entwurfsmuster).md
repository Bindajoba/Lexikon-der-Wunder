TARGET DECK: Universität::Informatik::SWT

# Beschreibung
State ist ein [[Entwurfsmuster (Softwaretechnik)]].
Es dient dazu Methoden eines Objekts in unterschiedlichen Zuständen zu modellieren.



# Struktur
Folgendes Beispiel illustriert den Verwendungszweck
Eine TCP-Verbindung soll unterschiedlich reagieren, abhängig davon, ob die Verbindung offen, listening oder closed ist.

TCP hat ein Objekt TCPState gespeichert, welcher den aktuellen Zustand der Verbindung repräsentiert. Das Ausführen der Open(), Close() Methode in der TCPState ist nun an den aktuellen Zustand angepasst.

![[State Beispiel.png]]

![[State Struktur.png]]


#Softwaretechnik 


