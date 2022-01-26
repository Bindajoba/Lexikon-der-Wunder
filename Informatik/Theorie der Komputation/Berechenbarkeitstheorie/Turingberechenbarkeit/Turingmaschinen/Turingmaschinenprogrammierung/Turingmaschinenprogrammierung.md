## Beschreibung
Man kann [[Mehrband-Turingmaschine|Mehrband-Turingmaschinen]] mit einander verketten. Dabei entstehen kompliziertere Mehrbandturing-Maschinen. Die Hintereinanderausführungen erlauben uns die Bausteine einer [[Imperative Programmierung|imperativen Programmiersprache]] aus Turingmaschinen zusammenzubauen.

## Grundlegendes
Menn $M$ eine 1-Band-Turingmaschine ist, dann schreiben wir $M(i, k)$ für die $k$-Band-TUringmaschine (mit $i \leq k$), die die Operationenen von $M$ auf dem i. Band durchführt und alle anderen Bänder unverändert lässt.
*Ich glaube, hier ist von zwei verschiedenen Turingmaschinen die Rede, mich irritiert es, dass für beide das Zeichen $M$ verwendet wird.
Denke an so was wie $M(i, k) = M$*

Wenn $k$ nicht von Bedeutung (und groß genug gewählt werden kann) , schreiben wir $M(i)$ statt $M(i, k)$
*Das muss man aber zum Glück nicht verstehen, weil im Folgenden die Notation vereinfacht wird.*

### Wertezuweisung
$$Band \ i:= M$$ Bedeutet, dass dem $i$-ten Band durch die Turingmaschine $M$ operiert wird. Das ist das Äquivalent dazu, einen Wert in eine Variable zu speichern oder eine Operation auf eine Variable anzuwenden.

### Einfache Addition
$$Band\ i := Band \ i+1$$ Auf das Band $i$ wird 1 hinzuaddiert.

### Angepasste einfache Subtraktion
$$Band\ i := Band \ i-1$$ Vom Band $i$ wird 1 subtrahiert.
Ist die zu überschreibende Zahl schon null, dann bleibt sie null, da negative Zahlen nicht als Ausgabe einer TM erlaubt sind.

### 0 Überschreiben
$$Band\ i := 0$$ Überschreibt das Band $i$ mit 0.

### Werte kopieren
$$Band\ i := Band \ j$$ Überschreibt das Band $i$ mit den Werten aus Band $j$.


## Hintereinanderausführung
Wir wollen zwei TMs hintereinander ausführen und sie dazu zu einer neuen TM zusammenbauen.
Seien $M_1 = (Z_1, \Sigma, \Gamma_1, \delta_1, z_1, \square, E_1)$, $M_2 = (Z_2, \Sigma, \Gamma_2, \delta_2, z_2, \square, E_2)$ zwei k-Band-Turingmaschinen

Die Turingmaschine $M_1;M_2$ führt $M_1$ und $M_2$ hintereinander aus. Dazu wird:
- Erst $M_1$ ausgeführt
- Dann vom Endzustand von $M_1$ in den Startzustand $z_2$ von $M_2$ gewechselt
- Dann $M_2$ ausgeführt

*Beachte, dass beim Übergang von $M_1$ zu $M_2$ keine Veränderung des Schreiblesekopfes oder des Wortes auf dem Band passiert.*

**Konstruktion**
- O.B.d.A. $Z_1 \cap Z_2 = \emptyset$
- $M_1;M_2 = ((Z_1 cup Z_2), \Sigma, \Gamma_1 \cup \Gamma_2, \delta, z_1, \square, E_2)$ mit
$$\delta(z, (a_1, ..., a_k)) = \begin{cases} \delta_1(z, (a_1, ..., a_k)) & \text{falls } z\in Z_1\backslash E_1, (a_1, ..., a_k) \in \Gamma_1^k \\ \delta_2(z, (a_1, ..., a_k)) & \text{falls } z\in Z_2, (a_1, ..., a_k) \in \Gamma_2^k \\ (z, (a_1, ..., a_k), N) & \text{falls } z\in E_1, (a_1, ..., a_k) \in \Gamma_1^k\end{cases}$$

### Addition
Durch das $n$-malige Hintereinanderausführen von $Band\ i := Band \ i+1$ erhalten wir $$Band\ i := Band \ i+n$$

### Zyklen
Durch die Hintereinanderausführung kann man auch TMs zyklisch miteinander verketten.

### Verzweigung
Sei $M_0$ ein Turingautomat mit zwei Endzuständen. Dann können die beiden Zustände in jeweils unterschiedliche Automaten $M_1, M_2$ weiterführen. So kann $M_0$ als Verzweigung fungieren.

### Schleife
Aus Verzweigung und (zyklischer) Hintereinanderschaltung kann man eine Schleife konstruieren, die den Zykel verlässt, bis eine Bedingung erfüllt ist.
![[Schleife.png]]
Die Schleife dieses Beispiels nennen wir

***WHILE Band $i \neq 0$ DO $M$***

#FSK 