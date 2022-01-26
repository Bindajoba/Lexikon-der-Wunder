## Beschreibung
Die **Schwarzsche Spiegelung** ist eine Verallgemeinerung der gewöhnlichen [[Achsenspiegelung]] oder der [[Inversion]].

Sie erlaubt es, Punkte an einer "ausreichend glatten" Kurve zu spiegeln.

## Herleitung
Bildet eine [[Analytische Funktion]] eine Gerade $L$ auf eine andere Gerade $\tilde L$ ab, so bildet sie zwei Punkte, die symmetrisch zu $L$ sind auf zwei Punkte ab, die symmetrisch zu $\tilde L$ sind.

Zum Beispiel:
$sin(z)$ bildet die reelle Achse auf $[-1, 1]$ ab.
Demnach gilt:
$$\overline{\sin(z)} = \overline{(\frac{e^{iz} - e^{-iz}}{2i})} = \frac{e^{i \overline z} - e^{-i\overline z}}{-2i} = \sin(\overline z)$$
D.h. das Spiegelbild von $z$ wird auf das Spiegelbild von $f(z)$ abgebildet

Dieser Sachverhalt gilt aber auch für andere Syymetrien: Bildet eine Funktion z.B. eine Gerade auf einen Kreis ab, dann wird da ebenfalls die Symmetrie beibehalten.

Bildet eine Funktion eine Gerade auf irgendeine Kurve ab, dann könnte man die Spiegelpunkt dieser Kurve so definieren.  

## Definition
Sei $K$ eine [[Analytische Kurve]] mit der [[Schwarzsche Funktion|Schwarzschen Funktion]] $\mathcal{S}_K$.

Dann ist die **Schwarzsche Spiegelung** $$\mathcal{R}_K(z)=\overline{\mathcal{S}_K(z)}$$

Man erkennt leicht, dass Punkte von $K$ auf sich selbst abgebildet werden.

#Needham 