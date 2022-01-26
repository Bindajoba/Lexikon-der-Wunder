## Beschreibung
Eine Strukturmetrik ist eine [[Software-Metrik]], die speziell für [[Objektorientierte Programmierung]] erstellt wurden.

Strukturmetriken zeichnen sich dadurch aus, dass sie Klassenverbünde als Ganzes untersuchen. Besonders wichtig ist die Analyse von Interaktionen zwischen Klassen.

Sie sind somit das Gegenstücker der [[Komponentenmetrik]]

## Definition
### Fan-In
Als Fan-In einer Klasse $C$, kurz $F_{in} (C)$ wird die Anzahl der Klassen bezeichnet, die direkt auf $C$ zugreifen.
Klassen mit einem hohen Fan-In Anteil sind in der Regel am unteren Ende der Software-Architektur angesiedelt

### Fan-Out
Als Fan-Out einer Klasse $C$, kurz $F_{in} (C)$ wird die Anzahl der Klassen bezeichnet, auf die $C$ zugreift.
Klassen mit einem hohen Fan-In Anteil sind in der Regel am oberen Ende der Software-Architektur angesiedelt

![[Strukturmetrik.png]]

### Strukturelle Komplexität einer Klasse
$$v_{HK}(C) = (F_{in}(C)F_{out}(C))^2$$
Die Komplexität untersucht aber nur Zugriffen nach und von außen. Will man die Komplexität der Klasse selbst messen, bruacht man eine passende [[Software-Metrik]] $v_{internal}$

Die angepasste Komplexitätsformel ist damit
$$v_{HS}(C) = v_{internal}(F_{in}(C)F_{out}(C))^2$$

### Strukturelle Komplexität des Programms
Die strukturelle Komplexität des Programms ist die Summe aller **Fan-Outs** 
$$s_CG = \sum_{i=1}^n F_{out}(C_i)^2$$
(*Wahrscheinlich, weil man sie sonst doppet zählen würde.*)

### Datenkomplexität
Die Datenkolexität berechnet sich wie folgt:
$$d_{CG} = \sum_{i = 1}^n \frac{IO(C_i)}{F_{out}(C_i)+1}$$
wobei $IO(C)$ die Anzahl der IO-Variablen von C beschreibt (*Vielleicht die Eingabe und Ausgabeargumente?*)

### Systemkomplexität
Die Summe der Datenkomplexität und der Strukturellen Komplexität ergibt die Komplexität $v_{CG}$:
$$v_{CG} = s_{SG} + d_{CG}$$

Teilt man die Komplexität durch die Anzahl der Teilkomponenten, erhält man die **relative Systemkomplexität**, also die Komplexität, die von jeder Komponente beigetragen wird.

#Softwaretechnik 