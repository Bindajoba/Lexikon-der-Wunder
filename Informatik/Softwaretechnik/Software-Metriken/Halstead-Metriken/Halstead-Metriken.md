
TARGET DECK: Universität::Informatik::SWT

## Beschreibung
Die Halstead-Metriken sind eine Sammlung von [[Software-Metrik|Software-Metriken]]. 
Sie versuchen Komplexität und andere Eigenschaften eines Codes zu bestimmen, indem [[Operator|Operatoren]] und [[Operand|Operanden]] in Funktionale Zusammenhänge gebracht werden.

Q: Was sind die [[Halstead-Metriken]]?
A: Sie sind eine Sammlung von Softwaremetriken, die versuchen Komplexität und andere Eigenschaften eines Codes zu bestimmen, indem Operatoren und Operanden in Funktionale Zusammenhänge gebracht werden.
<!--ID: 1645610669714-->


Q: Was ist ein Operator? ([[Halstead-Metriken]])
A: z.B. Schlüsselwörter, +, -, etc.
<!--ID: 1645610669823-->


Q: Was sind Operanden? ([[Halstead-Metriken]])
A: z.B. Bezeichner, Konstanten
<!--ID: 1645610669937-->


## Definitionen
$\eta_1 =$ Anzahl unterschiedlicher Operatoren
$\eta_2 =$ Anzahl unterschiedlicher Operanden
$\eta = \eta_1 + \eta_2 =$ Anzahl verschiedener Symbole
$N_1 =$ Gesamtzahl aller Operatoren
$N_2 =$ Gesamtzahl aller Operanden
$N = N_1 + N_2 =$ Gesamtzahl aller Operatoren und Operanden

### Anzahl der Ein- und Ausgaben
$\eta_2^* =$ Anzahl der Ein- und Ausgabeoperanden (Argumente)

Jeder Algorithmus wird mehr Operanden als $\eta_2^*$ benötigen, daher ist diese Zahl eine gute untere Grenze für die Operandenzahl $\eta_2$

### Größe des Minimalvokabulars
In einer fiktiven Programmiersprache können alle Algorithmen durch eine einzige Funktion $\Delta$ so vereinfacht werden:
$$\text{Operand}_1 = \Delta(\text{Operand}_2, \text{Operand}_3, ...)$$

In dieser Sprache sind $=$ und $\Delta$ die einzigen Operatoren.

Somit folgt für die Größe des Minimalvokabulars:
$$\eta^* = \eta_2^* + 2$$

### Volumen
Das Volumen ist die Gesamtlänge des Programms, multipliziert mit der Anzahl an [[Bit|bits]] die nötig wären, um jeden Operator/Operanden voneinander zu unterscheiden.
$$V = N \log_2 \eta$$

### Minimalvolumen
Das Minimalvolumen ist das kleinste Volumen, dass ein Programm haben kann:
$$V^*= \eta^* \log_2 \eta^*$$

### Level
Setzt man das Volumen eines Programms mit dem Minimalvolumen in Bezug, erhält man eine Maßzahl, wie weit die Implementierung von der Minimalimplementierung entfernt ist.

Da die Minimalimplementierung auf der Annahme basiert, das eine Funktion $\Delta$ den Algorithmus ausführt, gibt es auch den Abstraktionsgrad und damit die Transparenz des Software-Moduls an

$$L = \frac{V^*}{V}$$

Im optimalen Fall hat das Level einen Wert von 1.

### Durchschnittliche Wiederholungsrate von Operanden
Operanden sollten möglichst nicht wiederholt werden. Die Wiederholungsrate $P$ lässt sich messen mit:
$$P = \frac{N_2}{\eta_2}$$

### Level 2
Will man Level definieren, ohne Minimalvolumen zu verwenden, kann man sich auf die Annahme stützen, dass das Level eines Programms umgekehrt Proportional zu der Anzahl der verwendeten Operatoren sinkt.

Ein Programm mit nur 2 Operatoren soll dabei Level 1 haben:

$$\hat L \sim \frac{2}{\eta_1}$$

Das Level ist außerdem indirekt proportional zur durchschnittlichen Widerholungsrate von Operanden:

$$\hat L \sim \frac{1}{P}$$

Somit ergibt sich die neue Formel für das Level:

$$\hat L = \frac{2}{\eta_1 P}$$

### Schwierigkeit eines Programms
Ein Programm ist einfacher, je näher sein Level an ist. Folgerichtig ist ein Programm schwieriger je größer der Kehrwert von L ist:
$$D = \frac{1}{L}$$

Die Schwierigkeit kann auf Programmiersprachen angewendet werden.
Wähle dazu ein typisches Problem und messe die Schwierigkeiten der unterschiedlichen Implementierungen.

### Aufwand
Der Aufwand ist das Produkt aus Schwierigkeit und Volumen
$$E = V D = \frac{V^2}{V^*}$$

## Kritiken
- Unterscheidung zwischen Operator und Operand nicht immer möglich
- Die vier Anfangsparameter reichen nicht aus, um einen Aufschluss über komplzierte Eigenschaften des Codes zu erhalten

## Beispiel
![[Halstead-Matriken Beispiel.png]]

#Softwaretechnik 