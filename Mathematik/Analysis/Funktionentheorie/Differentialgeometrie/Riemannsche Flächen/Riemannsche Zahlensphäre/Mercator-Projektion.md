## Beschreibung
Die Mercator-Projektion ist eine Projektion einer [[Kugel]] auf eine Ebene.
Für ein Bild, betrachte den Wikipedia-Artikel[^2] oder MapMen[^1]

## Definition
### Komplexe Analysis
Wird die **Mercator-Projektion** als eine Funktion der [[Riemannsche Zahlensphäre]] auf die Komplexe Ebene betrachtet, findet man einige spannende Erkenntnisse.

Zuerst wird die Projektion als periodisch definiert. Geht man also immer nach Westen, kommt man wieder beim gleichen Ort an.

Vergleiche diese Projektion mit der [[Stereographische Projektion]]:
Bilde dazu Längen- und Breitenkreise mit den jeweiligen Projektionen ab.

Die **Mercator-Projektion** bildet Längenkreise auf senkrechte Geraden ab und Breitenkreise auf waagrechte Geraden.

Die **Stereographische Projektion** bildet Längenkreise auf Strahlen ab und Breitenkreise auf konzentrische Ursprungskreise.

Es sieht ganz so aus, als würde die Funktion $e^{-iz}$ bzw. $i\log(z)$ die Karten ineinander umwandeln.
Das ist tatsächlich der Fall.

## Eigenschaften
### Winkelerhaltung
Da die Mercatorprojektion eine Komposition aus der [[Stereographische Projektion]] und $\log$ ist, ist sie [[Konformität (Analysis)|konform]].

Die Schlussfolgerung davon habe ich auf Artifexian gepostet:
"*Ich habe endlich verstanden, wozu die Mercatorprojektion gut ist! In irgendeinem MapMen-Video hieß es, eine Linie auf einer Mercatorkarte ist eine Linie in echt. Das fand ich aber etwas komisch. Wenn man immer gerade aus laufen würde, dann würde man ja Großkreise um die Erde laufen. Aber wenn man eine Horizontale Linie, sagen wir durch Berlin ziehen würden, dann ist die Linie auf der Weltkugel kein Großkreis sondern ein Kleinkreis. "In echt in einer Linie laufen" habe ich also entweder falsch in Erinnerung oder es ist total missverständlich formuliert. Stattdessen gilt folgendes. Hält man einen Kompass in Gehrichtung und läuft so, dass die Kompassnadel immer in die gleiche Richtung zeigt, dann ist der durchlaufene Weg auf der Mercatorkarte eine Gerade.

Des Weiteren ist der Winkel zwischen Gehrichtung und Nordpolnadel genau der gleiche wie der Winkel zwischen Mercatorgerade und den senkrechten Parrallen. Das macht Navigation absurd einfach. Man zeichnet eine Strecke zwischen dem Start und Zielpunkt auf einer Mercatorkarte. Dann misst man den Winkel zwischen Strecke und den senkrechen Parallelen. Dann nimmt man einen Kompass, und geht so, dass die Gehrichtung und der Nordpol den gleichen Winkel haben. Und dann kommt man einfach beim Ziel an!"


#Needham 

[^1]: https://www.youtube.com/watch?v=jtBV3GgQLg8&t=205s
[^2]: https://de.wikipedia.org/wiki/Mercator-Projektion