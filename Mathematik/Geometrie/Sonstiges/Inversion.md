## Beschreibung
Die Inversion ist eine Methode eine Spiegelungsachse auf Kreisränder zu verallgemeinern.
Man spiegelt dabei das Äußere des [[Kreis|Kreises]] in das Innere und umgekehrt.

## Definition
### Komplexe Ebene


Sei 
- $K$ der Inversionskreis mit dem Mittelpunkt $q$ und dem Radius $R$

Dann ist
$$\mathcal{I}_K(z) = \frac{R^2}{\overline{z}-\overline{q}}+q$$[^1]

Dividiert man die Strecke $qz$ ihren Betrag $|qz|$ und multipliziert sie mit dem Radius $R$, erhält man einen Punkt, der auf $K$ und in der Richtung der ursprünglichen Strecke $qz$ liegt.
Tut man das erneut, erhält man das Bild von $z$ unter der Inversion an $K$.

Die gewöhnliche Inversion ist die Inversion am [[Einheitskreis]] und schreibt sich durch:
$$\mathcal{I} = \frac{1}{\overline{z}}$$

Die erste Formel habe ich mir aus der zweiten perfide hergeleitet. Ich habe mir die Inversion an $K$ so zerlegt:
- Verschiebe und Strecke $K$ auf den Einheitskreis
- Führe die gewöhnliche Inversion durch
- Verschiebe und Strecke zurück*

## Eigenschaften
Inversionen haben eine Menge Eigenschaften. Das war fast ein ganzes Kapitel von Needham. Hier die, auf die ich Lust hatte

### Bild einer Hyperbel
Sei $H$ die [[Hyperbel]] mit $x^2 + y^2 = 1$
Dann ergibt die Inversion der Hyperbel die [[Lemniskate]].

*Das Ergebnis erhält man durch einen kleinen Umweg. Das komplexe Quadrat von $H$ ist eine Gerade $x=1$, die Inversion davon ist ein [[Kreis]] durch 0 und 1 mit Durchmesser 1. Nimmt man davon die [[Holomorphe Wurzel|Wurzelfunktion]] erhält man die Lemniskate.* 

### Involutorisch
Die **Inversion** ist involutorisch (d.h. sie vertauscht zwei Punkte)

### Siehe auch
- Die Verallgemeinerung der Inversion: [[Schwarzsche Spiegelung|Spiegelung an einer beliebigen Kurve]]

#Needham

[^1]: Needham - Formel 3.4 