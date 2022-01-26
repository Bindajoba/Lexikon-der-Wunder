## Beschreibung
Um einen Prozess zu verwalten und zu kontrollieren, muss das Betriebssystem wissen:
1. Wo ist der Prozess gespeichert? (**Prozesslokalisierung**)
*Wo ist mein Rezept?*
2. Welche Werte haben die für das Prozessmanagement relevanten Attribute? (?)
*An welcher Stelle des [[Programm|Programms]] habe ich zuletzt aufgehört?*

## Vorgehen
### Prozesslokalisierung
Die Lokalisierung eines Prozesses hängt von der eingesetzten [[Speicherverwaltung]] ab.

### Prozessattribute im Prozesskontrollblock
Der Prozesskontrollblock (PCB) ist die bedeutenste Datenstruktur in der Prozessverwaltung. Es enthält die wesentlichen Informationen, die das Betriebssystem zur Kontrolle eines Prozesses benötigt

Bestandteile:
- Prozessidentifikation
- Prozesszustandsinfo
- Prozesskontrollinfos

Des weiteren gehören zur Struktur eines Prozesses noch dazu:
- User Stack
- Private User Adress Space (Programmdaten)
- Shared Adress Space


#Betriebssysteme 