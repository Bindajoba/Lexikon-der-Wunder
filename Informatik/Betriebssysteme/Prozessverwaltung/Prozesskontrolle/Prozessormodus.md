TARGET DECK: Universität::Informatik::Betriebssysteme

# Beschreibung
Ein [[Prozessor]] kann zwei verschiedene Modi einnehmen. Ein Modus hat die Rechte alles zu tun, was er will, der andere ist eingeschränkt.

Der Zustand des Modus wird in einem Ein-Bit-Register auf dem Prozessor gespeichert.
Dieses befindet sich im [[Programm-Statuswort]]

# Modi
Q: Welche 2 Prozessormodi gibt es?
A: - Systemmodus (Kernel Mode)
- Nutzermodus (User Mode)
<!--ID: 1643668652367-->



## Systemmodus (Kernel Mode)
Der Prozessor behandelt ein [[Programm#Kernelprogramme]].
Der Systemmodus ist privilegiert, d.h. er elaubt die Ausführung aller Operationen

Funktionen des Betriebssystems-Kerns
- Support-Funktionen
- Selbstverwaltungsfunktionen
	- Fehlermanagemant
	- Konfigurationsmanagemant
	- Accounting Management
	- Leistungsmanagement
	- Sicherheitmanagemant
- E/A-Managemant
- Speichermanagement
- Prozessmanagement

## Nutzermodus (User Mode)
Der Prozessor behandelt ein [[Programm#Benutzerprogramme]].
Der Nutzermodeus ist nicht privilegiert, d.h. ihm können Operationen verwehrt werden.

# Moduswechsel bei Unterbrechungsroutine
Bei einem Moduswechsel (z.b. durch einen [[Systemaufruf|System-Call]] oder einer [[Unterbrechung]]), muss der aktuelle Prozess pausiert und die Unterbrechung im [[Prozessormodus|Kernel-Modus]] behandelt werden.

Der Moduswechsel passiert in 3 Schritten
1. Aktualisierung und Sicherung der Zustandsinformationen des [[Prozesskontrollblock|Prozesskontrollblocks]] des gerade aktiven Prozesses
2. Durchführung des eigentlichen Moduswechsels durch Änderung eines Registers im [[Prozessor]]
3. Sprung zur Unterbrechungsroutine (Programmzähler wird auf dessen Anfangsadresse gesetzt)

*Wie ich es verstanden habe, ist die Fehlerbehandlung eine [[Prozedur]] des auslösenden Prozesses. Warum die Zustandsinformationen im Prozesskontrollblock gesichert werden müssen, verstehe ich nicht.*

Q: Wie bezeichnet man die Schnittstelle zwischen Anwendungsprogrammen und Betriebssystem, durch welche diese z.B. auf Ressource zugreifen können, auf welche sie keinen direkten Zugriff haben.
A: Systemaufruf
<!--ID: 1644309602104-->



Q: In welchen drei Schritten wird ein Moduswechsel durchführt?
A: 1. Sicherung des Prozesskontrollblocks
2. Moduswechsel
3. Sprung zur Unterbrechungsroutine
<!--ID: 1643668652518-->


Q: Was versteht man unter einem Kontextswitch ([[Kontextswitch]])?
A: Wechsel des Prozesses, ohne den den Prozessormodus zu verändern.
<!--ID: 1643668652656-->



#Betriebssysteme 