## Beschreibung
Die Krümmung beschreibt, wie gekrümmt ein [[Weg]] an einem bestimmten Punkt ist.

## Definition
Die legt man an eine Kurve einen [[Kreis]] so an, dass er die Kurve tangiert und zusätzlich die gleiche Krümmung hat, so ist die Krümmung an diesem Punkt der Kehrwert des Kreisradius.

Es fällt auf: Je kleiner der angelegte Wert, desto stärker die Krümmung.

## Eigenschaften
### Krümmung unter analytischen Funktionen
Die Krümmung einer Kurve wird unter einer [[Analytische Funktion]] verändert. Wie das an einem Punkt $p$ aussieht, lässt sich damit errechnen:
$$\tilde\kappa = \frac{1}{|f'(p)|}\left(Im\left(\frac{f''(p)\hat\xi}{f'(p)}\right) + \kappa\right)$$
wobei $\hat\xi$ der die komplexe Tangente an $p$ mit Betrag 1 ist.

### Krümmung der reellen Achse unter analytischen Funktionen
Das ist ein Spezialfall des vorherigen Ergebnisses. Setzt man alle nötigen Parameter ein, erhält man die Formel:
$$\tilde\kappa = \frac{Im\left(\frac{f''(p)}{f'(p)}\right)}{|f'(p)|}$$ oder
$$\tilde\kappa = \frac{Im\left(\overline{f'(p)}f''(p)\right)}{|f'(p)|^3} = \frac{Im\left(\overline{v}\dot v\right)}{|v|^3}$$ wobei $v$ die Geschwindigkeit eines Teilches beschreibt, welches entlang der Kurve wandert.


### Krümmung zweidimensionaler Kurven
Der obere Fall gleicht sehr einer Parametrisierten Kurve. Desweiteren fällt uns ins Auge, dass $Im\left(\overline{v}\dot v\right)$ das komplexe [[Kreuzprodukt]] von $v$ mit $\dot v$ ist.

Damit erhält man eine neue Formel:
$$\tilde\kappa = \frac{|\overline{v} \times \dot v|}{|v|^3}$$ 

### Krümmung mehrdimensionaler Kurven
In einem Raum mit mindestens 3 dimensionen kann man ein Kurvenstück durch die Bewegungs und Krümmungsrichtung durch eine Ebene darstellen. Anhand dieser Ebene kann man die obere Formel verwenden, um die Krümmung zu erhalten.


#Needham 