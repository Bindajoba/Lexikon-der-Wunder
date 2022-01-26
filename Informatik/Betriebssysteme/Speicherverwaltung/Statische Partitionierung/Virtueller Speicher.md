## Beschreibung
Der [[Hauptspeicher]] und andere Speicher wie Festplatten, USB, etc sind physisch getrennte Gegenstände.

Man kann aber alle Speichereinheiten zum [[Hintergrundspeicher]] zusammenfassen.
Der [[Hauptspeicher]] ist dann ein Teil des [[Hintergrundspeicher]].

Die Konstruktion eines riesigen Speichers, bei dem die einzelnen Speichermedien unwichtig werden, nennt man **Virtueller Speicher**

# Maschinenadresse
Wie kann der Hauptspeicher auf Daten im [[Hintergrundspeicher]] zugreifen? Dzu wird eine spezielle Adressierung benötigt. Diese funktioniert auf der [[Modellmaschine MI]] wie folgt:
- MI hat Frames mit der Größe $2^{9} = 512$
- MI hat einen Arbeits-/Hauptspeicher von Größe $1GB = 2^{30}$
- Somit hat MI $2^{21}$ [[Frame|Frames]]
- Der Hintergrundspeicher ist 4 mal so groß wie der Hauptspeicher 
![[Maschinenandressierung.png]]
*Durch die ersten vier Bits hat man genug Länge, um alle Pages im Hintergrundspeicher zu adressieren.*

Welches Pgae in welchem Frame sitzt, läst sich an einer Speichertabelle ablesen, die auf dem Computer gespeichert ist.
![[Virueller Speicher Speichertabelle.png]]
*Beobachte, dass der Hintergrundspeicher längere Adressen hat. Das liegt daran, das der Hintergrundspeicher mehr Adressen besitzt.*





#Betriebssysteme 