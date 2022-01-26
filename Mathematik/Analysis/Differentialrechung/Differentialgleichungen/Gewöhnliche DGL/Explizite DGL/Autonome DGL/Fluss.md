## Beschreibung
In Physiksimulationen ist die Lösung nur von initialen Anfangsbedingungen abhängig, nicht aber von der Zeit.
Die Funktion, die als Eingabe eine Anfangsbedingung und eine Zeit nimmt, eine Zustand ausgibt und eine [[Autonome Differentialgleichung]] löst, nennt man Fluss.

## Definitionen
Sei
- $D \subseteq \mathbb{K}^d$ ein offener und zusammenhängender Raum von [[Zustand|Zuständen]]
-  Sei $v: D \to \mathbb{K}^d$ die lokal lipschitzstetige rechte Seite der DGL

Der **Fluss** des autonomen Systems $$x'=v(x)$$ ist
$$\varphi: \begin{array}{rcl}J_\xi \times D & \to & \mathbb{K}^d\\(t, x)& \mapsto & \lambda_{(0, \xi)}(t)\end{array}$$

### Phasenfluss
Betrachtet man statt der Veränderung eines Punktes im Laufe der Zeit, alle Punkte gleichzeitig, dann nennt man das den [[Phasenfluss]].

## Eigenschaften
### Zusammenhang mit Einparametrigen Gruppen
Bei [[Phasenfluss]] wurde erklärt, wie ein [[Phasenfluss]] das gleiche ist wie eine Transformation $g^t$.
Ein Fluss ist dann die Transformation eines Punktes $g^tx$ im Bezug zur Zeit 


#Mathe-IV #Arnold 