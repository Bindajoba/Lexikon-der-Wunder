## Beschreibung
Die **Cauchy-Riemannschen-Differentialgleichungen** sind 2 partielle [[Differentialgleichung|Differentialgleichungen]], welche eine [[Analytische Funktion]] charakterisieren.

## Herleitung
Interpretiert man eine komplexe Funktion $f = u + iv$ als eine Funktion, die eine Ebene auf eine andere Ebene abbildet, so beschreibt die [[Ableitung]] dieser Funktion das Lokale Verhalten in Form einer [[Lineare Abbildung|linearen Abbildung]].

Da eine analytische Funktion infinitessimale Figuren auf [[Ahnlichkeitabbildung|ähnliche]] infinitessimale Figuren abbildet, muss die lokale lineare Abbildung eine Drehstreckung sein.

Somit ist die Ableitung durch eine Matrix $$f'(x, y) = \begin{pmatrix} a & b \\ b & -a \end{pmatrix}$$ beschreibbar.
Bekanntermaßen berechnet sich die Ableitung mit der [[Jakobi-Matrix]]:
$$f'(x, y) = \begin{pmatrix} \partial_x u & \partial_y u \\ \partial_y v & \partial_y v \end{pmatrix}$$

Man kann damit folgende Gleichungen aufstellen:
$$\begin{align} \partial_x u &= \partial_y v \\ \partial_y v &= -\partial_y u  \end{align}$$

Da die Ableitung nur eine Drehstreckung ist, gibt jede Richtungsableitung die gleiche Drehstreckung. Leitet man also in Richtung der reellen Achse ab, so beschreibt die erhaltene komplexe Zahl die Ableitung vollständig:
$$f' = \partial_x f = \partial_x u + i\partial_x v$$
Das Substituieren der oberen Gleichungen in die jetzige ergibt die zweite Gleichung:
$$f' = \partial_y v - i \partial_y u = -i\partial_y f$$

## Variationen
Im oberen Fall wurden der Effekt einer [[Analytische Funktion]] in karthesischen Koordinaten beschrieben.
Das soll uns aber nicht aufhalten, andere Formen der Cauchy-Riemannschen Differentialgleichungen zu suchen.

### Kart.-Polar Form
Sei eine analytische Funktion 
$$f(x+iy) = R(x+iy)e^{\Psi(x + ix)}$$
Dann gilt
$$\begin{align} \partial_x R &= R \partial_y \Psi \\ \partial_y R &= -R \partial_x \Psi\end{align}$$

Das erhält man aus den oberen beiden Gleichungen:
$$f' = \partial_x f = \partial_x Re^{i \Psi} + iRe^{i\Psi}\partial_x \Psi $$
$$f' = -i\partial_y f = -i\partial_y Re^{i \Psi} + Re^{i\Psi}\partial_y \Psi $$
Setzt man Real und Imaginärteile der Gleichung gleich, so erhält man obigen Ausdruck.

### Polar Form
Macht man ein wenig Geometrie, erhält man eine kompakte Form der Gleichungen:
$$\partial_\theta f = i r \partial_r f$$
Grob bedeutet die Gleichung, die Bewegungsstrecke bei einer winzigen kreisbogenförmige Veränderung $\varepsilon$ $(\theta)$ senkrecht und $r$ mal so lang ist wie die Bewegungsstrecke bei einer winzigen, radialen Veränderung $\varepsilon$ $(r)$.
*Das $r$ mal kommt daher, dass sich die infinitesimale Winkeländerung $\partial_\theta$ durch das Produkt aus Kreissbogenlänge und Radius $\varepsilon r$ berechnet.
Das $r$ steht sozusagen bereits auf beiden Seiten der Gleichung*


### Polar-Kart. Form
Setzt man in die obere Gleichung $f = u + v$ ein, erhält man die Gleichungen:
$$\begin{align} \partial_\theta v &= r \partial_r u \\ \partial_\theta u &= -r \partial_r v\end{align}$$

### Polar-Polar Form
Setzt man in die obere Gleichung $f = Re^{i\Psi}$ ein, erhält man die Gleichungen:
$$\begin{align} \partial_\theta R &= -rR \partial_r \Psi \\ R\partial_\theta \Psi &= r \partial_r R\end{align}$$

#Needham 