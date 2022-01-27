## Beschreibung
Ein Programm ist eine Folge (Sequenz) von Befehlen. Ein Programm in Ausführung heißt [[Prozess]].

# Definition
## Softwaretechnik
Ein Programm ist eine in einer [[Programmiersprache]] verfasste Verarbeitungsvorschrift, die auf einem Computer unter Nutzung und Festlegung von Datenformaten ausgeführt werden kann 

## Funktionsweise
Wird ein Programm ausgeführt, erhält es einen zusammenhängenden Speicherbereich. (vermutlich im [[Hauptspeicher]])
Dieser wird [[Trace]] des Prozesses genannt und ist zunächst so lang wie die Anzahl der Befehle des Programms in [[Maschinencode]].

Der zusammenhängende Speicherbereich hat einen Anfangswert $\alpha$, an dem sich alle anderen Werte beziehen können.
Die erlaubt es innerhalb des Programms Speicheradressen zu benutzen, die bei 0 beginnen. ($\alpha$ wird dann vom Betriebssystem dazuaddiert.)

Dann wird das Programm von oben nach unten ausgeführt.

Hat man ein [[Multiprogramming]]-Prozessor wird zwischen den Programmen gewechselt. Mehr auf [[Multiprogramming]]

## Unterteilung
Programme des [[Betriebssystem|Betriebssystems]] sind in Kernel- und Benutzerprogramme unterteilbar

### Kernelprogramme
Kernalprogramme sind ein direkter Teil des Betriebssystems und laufen mit höherer Priorität als andere Programme

### Benutzerprogramme
Benutzerprogramme sind alle anderen Programme



#Betriebssysteme #Softwaretechnik 