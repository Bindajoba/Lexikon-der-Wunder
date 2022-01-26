Die McCabe Metrik hat eine interessante Art dem Problem der [[Software-Metrik]] zu begegnen.
McCabe misst Komplexität, indem er er die Verzweigtheit des Codes untersucht.


## Definition
### Zyklomatische Komplexität
Dazu wird der Code in ein [[Kontrollflussdiagramm]] und von da in einen [[Kontrollflussgraph|Kontrollflussgraphen]] umgewandelt.

![[McCabe-Metrik.png]]

Fügt man vom Endpunkt eine Kante zum Startpunkt hinzu lässt sich aus dem Graphen die [[Zyklomatische Zahl]] ermitteln:
$$V(Z) = |E|-|N|+2$$
Für [[Stark Zusammenhängender Graph|stark zusammenhängende Graphen]], wobei $E$ die Anzahl der Kanten und $N$ die Anzahl der Knoten ist.

Die Zyklomatische Zahl wird in diesem Kontext als **Zyklomatische Komplexität** bezeichnet.

Diese zyklomatische Zahl hat zufällig genau die Eigenschaft, dass sie ein gutes Maß für Verzweigung ist.
*Setze Beispielsweise eine Funktion in der if Anweisung ein. Es kommt ein Konten und eine Kante hinzu - der Code wird nicht verzeigter und die zyklomatishce Zahl nicht größer.*

Tatsächlich gilt für diese Art von Graphen sogar: Die **zyklomatische Komplexität** ist stets um eins größer als die Anzahl der Verzweigungen.

### Zyklomatische Komplexität mehrerer Komponenten
Besteht ein Programm aus mehreren Komponenten/Funktionen, so ist die **Zyklomatische Komplexität** des Programms als die Summe der **zyklomatischen Komplexität** seiner Unterkomponenten definiert.

*Die Funktionen lassen sich auch als Zusammenhanglose Graphen betrachten. In diesem Fall nennt man diese Struktur einen [[Wald (Graphentheorie)]] und die Definition des [[Zyklomatische Zahl|Zyklomatischen Zahl]] ergibt daruaf das gleiche Ergebnis wie die Summe seiner Einzelteile.*

#Softwaretechnik 