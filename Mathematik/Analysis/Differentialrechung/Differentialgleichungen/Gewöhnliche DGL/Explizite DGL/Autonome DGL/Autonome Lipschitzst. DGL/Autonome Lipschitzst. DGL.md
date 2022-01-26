## Beschreibung
Eine autonome lipschitzsteige Differentialgleichung ist eine [[Autonome Differentialgleichung]], dessen rechte Seite [[Lokale Lipschitzstetigkeit|lokal lipschitzstetig]]]]st.

Es handelt sich hierbei um einen Begriff, den ich mir ausgedacht habe, um Eigenschaften von autonomen DGLs besser auszudifferenzieren.

## Definition
Eine [[Autonome Differentialgleichung]] 
$$x' = v(x) \tag{1}$$ ist lipschitzstetig, wenn $v$ [[[[Lokale Lipschitzstetigke|lokal lipschitzstetig]] Lösung
### Existenzintervall[^1]
- Ist die [[Trajektorie|positive Halbtrajektorie]] $T^+(\xi)$ von $(1)$ in einer kompakten Teilmenge von D enthalten, so gilt $b(\xi)=\infty$
- Ist die [[Trajektorie|negative Halbtrajektorie]] $T^-(\xi)$ in einer kompakten Teilmenge von D enthalten, so gilt $a(\xi)=-\infty$
- Ist $b(\xi)<\infty$, so ist 
  - $T^+(\xi)$ unbeschränkt
*D.h. ein [[Fluss]] geht gegen Unendlich, bevor ein bestimmter Zeitpunkt erreicht wurde* oder
  - Der Rand von $D$ ist ist nichtleer und es gilt
$$\underset{t\nearrow {\xi}}{\lim} dist(\varphi(t, \xi), \partial D) = 0$$ *D.h. Die Trajektorie stößt an den Rand des Definitionsbereiches*

### Trajektorien
Seien
- $\xi, \nu \in D$ ein [[Zustand|Startzustand]]

Dann bildet
$$\xi \sim \nu \iff \text{Es existiert } \tau \in J_\xi \text{ mit } \nu=\varphi(\tau, \xi)$$ eine [[Äquivalenzklasse]].

Die Menge aller Trajektorien, das [[Phasenportrait]] bildet also eine [[Zerlegung]] von D.[^2]

Trajektorien eines Flusses haben genau eine der drei Formen: [^3]
1. DIe Trajektorie $T(\xi)$ ist einpunktig:
$J_\xi=]\-infty, \infty[$ und $\varphi(\cdot, \xi)$ ist konstant.
$\xi$ wird ist dann ein [[Ruhelage|kritischer Punkt]] und bestimmt sich aus der Lösung von $g(x)=0$
2. Die Trajektorie $T(\xi)$ ist eine geschlossene Kurve
$J_\xi=]\-infty, \infty[$ und $\varphi(\cdot, \xi)$ ist nicht konstant und periodisch.
3. Die Trajektorie $T(\xi)$ ist eine doppelpunktfreie Kurve ohne die Endpunkte
Dann ist der Fluss $\phi(\cdot, \xi)$ [[Injektivität|injektiv]]

### Stabilität
Sei $V: D \to \mathbb{R}$ eine [[Lyapunov-Funktion]] zu $(1)$ und $\xi \in D$ eine [[Ruhelage]], sodass:
1. $V(\xi)=0$
2. $V(x)>0$ für alle $x\in D\backslash\{\xi\}$
Dann ist $\xi$ eine [[Stabilität|stabile]] [[Ruhelage]].
[^4]

*Die Intuition ist hier ziemlich leicht aber das Verständnis schwer. $\xi$ ist der "energieärmste" Zustand, deshalb wollen alle anderen Zustände da hin. Wenn man aber genauer darüber nachdenkt, bricht das Bild auseinander*

### Asymptotische Stabilität

Seien
- $\xi \in D$ eine [[Ruhelage]]
- $V: D \to \mathbb{R}$ eine [[Lyapunov-Funktion]] zu $(1)$
mit:
1. $V(\xi)=0$
2. $V(x)>0$ für alle $x\in D\backslash\{\xi\}$
3. $grad V(x) \circ v(x) < 0$ für alle $x\in D\backslash\{\xi\}$
Dann ist $\xi$ eine [[Asymptotische Stabilität|asymptotisch stabile]] [[Ruhelage]].
[^5]
*Das Verständnis ist hier viel leichter. 
Die letzte Bedingung besagt, dass die Lypunov-Funktion entlang einer Trajektorie [[Monotonie|streng monoton fällt]] Wenn eine solche Lyapunovfunktion existiert, können Trajektorien keine geschlossenen Kurven geben, da die Lypunovfuntion dazu fallen und fallen müsste, bis sie mit einem anderen Wert wieder am Startpunkt ankommt.
Weil 0 der niedrigste Punkt der Funktion ist, können Funktionswerte der Lypunovfunktion in einer kleinen Umgebung mit wachsender Entfernung nur größer werden.
Da die Lypunovfunktion entlang der [[Trajektorie|Trajektorien]] aber kleiner wird, müssen sich die Trajektorien in dieser Umgebung auch in Richtung null bewegen. (Sonst würde die Lyapunovfunktion entlang der Trajektorien größer werden uder gleich bleiben.)*

### Instabilität
Seien
- $\xi \in D$ eine [[Ruhelage]]
- $V: D \to \mathbb{R}$ eine [[Lyapunov-Funktion]] zu $(1)$
mit:
1. $V(\xi)=0$
3. $grad V(x) \circ v(x) < 0$ für alle $x\in D\backslash\{\xi\}$
3. In jeder Umgebung $W$ von $\xi$ gibt es ein $x_W \in W$ mit $V(x_W)<0$

*Dieser Satz ist vermutlich am leichtesten zu verstehen.. 
Ein Punkt ist instabil, wenn sich die Lösung bei einer kleinen Veränderung des Startwert stark verändert.
Die zweite Bedingung besagt, dass die Lypunov-Funktion entlang einer Trajektorie [[Monotonie|streng monoton fällt]]
Auch hier kann es deshalb keine geschlossenen Kurven geben.
Eine Lösung die jetzt bei $x_W$ anfängt kann sich im Kreis drehen. Also muss sie sich in "Spirallinien" (Also einer Linie, sodass sie sich nicht selbst schneidet) entweder zum Kreis hin oder weg bewegen.
Hin geht nicht, da sonst die Lypunovfunktion aufgrund ihrer Stetigkeit irgendwann größer werden würde. 
Deshalb bewegt sich die Trajektorie von $\xi$ weg.*
[^6]
#Mathe-IV 

[^1]: Zenk - Satz 20.1.10
[^2]: Zenk - Satz 20.1.12
[^3]: Zenk - Satz 20.1.13
[^4]: Zenk - Satz 20.2.8
[^5]: Zenk - Satz 20.2.11
[^5]: Zenk - Satz 20.2.12
