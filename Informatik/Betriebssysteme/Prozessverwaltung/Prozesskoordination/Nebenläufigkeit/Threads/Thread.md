# Beschreibung
Der Teil eines [[Prozess|Prozesses]], der sich um die Erfüllung einer Aufgabe und weniger um die Verwaltung von Ressourcen kümmert, dann kann man Prozesse als **Thread** bezeichnen.

**Threads** können aber auch allgemeiner als Einheiten, die eine gewisse Aufgaben erledigen verstanden werden. Nach der Definition kann es innerhalb eines Prozesses mehrere Threads geben

# Eigenschaften
Threads eines Prozesses
- Teilen sich den gleichen Adressraum
- Haben gemainsamen Zugriff auf Speicher und Ressourcen d. Prozesses
- Haben eigenen Stack für lokale Variablen
- Haben einen eigenen Deskriptor

# Zustände
Threads können einen der drei Zustände
- Ready
- Running oder
- Blocked
einnehmen.

*Bemerke, dass Threads nicht suspendiert werden können. Das liegt daran, dass der Adressraum mit dem ausführenden Prozess geteilt wird und daher nicht nicht seperat suspendiert werden können.*

# Thread-Arten
- [[User-Level-Thread]]
- [[Kernel-Level-Thread]]


#Betriebssysteme 