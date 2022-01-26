TARGET DECK: Universität::Informatik::Betriebssysteme

## Beschreibung
Unterprogramme sind [[Programm|Programme]], welche von einem anderen Programm mehrfach ausgeführt werden können.


## Unterteilung
Q: Welche zwei Arten von Unterprogrammen gibt es?
A: - Offenes Unterprogramm
- Geschlossenes Unterprogramm/Prozedur
<!--ID: 1642897217838-->


### Offenes Unterprogramm
Um das Unterprogramm auszuführen wird sein Quellcode (*vermutlich vom Betriebssystem*) in das ausführende Programm kopiert. Dies wird bei enfachen Arithmetischen Operationen gemacht, z.B. $|x|$ oder $x^2$.

Dies wird bei kleinen Funtionsaufrufen

**Nachteile:**
- Kopieren d.h. Duplizieren des Unterprogramms erfordert Speicherplatz zum Speichern
- Da die Sprungadressen beim Kopieren ungültig werden, müssen diese nachträglich verändert werden
- Nachträgliche Modifikationen am Unterprogramm müssen an jedem Vorkommen des Unterprogramms vorgenommen werden

Q: Nenne zwei Nachteile, die die ausschließliche Verwendung von offenen Unterprogrammen mit sich zieht
A: - Erhöht den Speicherplatz
- Nachträgliche Modifikationen
- Anpassung von Sprungandressen
<!--ID: 1642897218017-->


### Geschlossenes Unterprogramm/Prozedur
Siehe [[Prozedur]]





#Betriebssysteme 