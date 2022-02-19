# Beschreibung
Ein Ringpuffer ist eine zyklische Datenstruktur, welche einen Puffer mehr hat als es Elemente besitzt

# Funktionsweise
Daten werden in einer Zyklischen Datenstruktur gespeichert.
Es gibt zwei Zeiger. Einen zum einsetzen von Daten an einer Stelle und einen zum herausnehmen von Daten an einer Stelle.

- Fügt man dem Ringpuffer etwas hinzu, wandert der in-Zeiger weiter
- Entnimmt man dem Ringpuffer etwas, geht der Out Zeiger einen Schritt weiter

Das Feld, bei dem sich der in-Zeiger befindet muss immer leer sein. Der in-Zeiger kann sich nicht auf ein volles Feld bewegen.  


![[Ringpuffer.png]]

# Nutzen
Mit einem Ringpuffer kann das [[Erzeuger-Verbraucher-Problem]] für einen Erzeuger und einen Verbraucher zu einem [[Unabhängige und Abhängige Abläufe|unabhängigen Ablauf]] gemacht werden

Wir erkennen, dass der Stapel leer ist, wenn der in und out-Zeiger gleich sind und voll, wenn man nur noch ein Element hinzufügen müsste, damit in und out gleich sind.
Wir programmieren:

![[Ringpufferbeispiel.png]]

Da hier in und out unterschiedliche Variablen sind, die unabhängig voneinander beschrieben werden, kann es nich zu einem [[Kritischer Abschnitt|Kritischen Abschnitt]] kommen.


#Betriebssysteme 