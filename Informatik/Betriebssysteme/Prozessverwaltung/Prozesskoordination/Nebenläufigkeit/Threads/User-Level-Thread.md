# Beschreibung
Ein **User-Level-Thread** ist ein [[Thread]], der vom [[Prozess|Anwendungsprozess]] verwaltet wird.
Das Benutzerprogramm hat dazu meistens einen eigenen [[Scheduler]].

Das Betriebssystem ist sich über dieser Threads nicht bewusst.

# Bewertung
## Vorteile
- Können in jedem Betriebsystem implementiert und ausgeführt werden
- Prozesse benötigen keine Privilegien
- Das Scheduling kann von einem eigenen Scheduler verwaltet werden

## Nachteile
- Wird ein Thread blockiert (d.h. er wartet auf ein Ereignis), so blockiert der gesamte Prozess
- Können in einer Mltiprozessorumgebung nicht parallel ausgeführt werden[^1]

#Betriebssysteme 

[^1]: https://www.tutorialspoint.com/user-level-threads-and-kernel-level-threads