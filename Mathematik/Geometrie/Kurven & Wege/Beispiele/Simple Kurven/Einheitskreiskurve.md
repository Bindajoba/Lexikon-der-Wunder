TARGET DECK: Universität::Mathematik::Geometrie

# Beschreibung
Eine Einheitskreiskurve ist eine Kurve, die [[Gleichmäßige Kurve|gleichmäßig]] im Uhrzeigersinn alle Punkte des [[Einheitskreis]] durchläuft bis sie wieder am Anfangspunkt ankommt.

# Definition
## Standardkurve $\kappa_0$
Die Standard-Einheitskreiskurve $\kappa_0$ ist die Kurve, die beim Punkt $(1, 0)$ beginnt, [[Gleichmäßige Kurve|gleichmäßig]] im Uhrzeigersinn alle Punkte des [[Einheitskreis]] durchläuft bis sie wieder am Anfangspunkt ankommt.


## Periodische Fortsetzung
Die Kurve $\kappa_0: [0, 2\pi] \to \R^2$ lässt sich periodisch auf $\R$ fortsetzen, indem alle $2\pi$ der Wert von $\kappa_0$ verwendet wird. d.h. $\kappa(2\pi i + t) = \kappa_0 (t)$

# Eigenschaften
## Menge der Einheitskurven in $\R^2$
Da das [[Gleichmäßige Kurve|gleichmäßig]] Machen einer Kurve eindeutig ist, reicht schon ein Anfangspunkt auf dem Einheitskreis und eine Richtung (im oder gegen Uhrzeigersinn) aus, um eine Kurve zu bestimmen.
Alle Einheitskreiskurven haben also die Form $\kappa(\theta \pm t)$ für ein $\theta \in [0, 2\pi]$

## Zusammenspiel mit Rotationen
Verknüpft man Punkte der EInheitskurve mit einer [[Rotation (Geometrie)]], kann man einige lustige Eigenschaften herleiten.

$R_\theta(\kappa(0)) = R_\theta \begin{pmatrix}1\\0\end{pmatrix} = \kappa(\theta)$, weshalb:
$$R_\theta(\kappa(t)) = \kappa(\theta+t)$$
In Matrixschreibweise:
$$\begin{pmatrix} \cos(\theta)\cos(t) -\sin(\theta)\sin(t)  \\ \sin (\theta)cos(t) + \cos(\theta)\sin(t)\end{pmatrix}=\begin{pmatrix} \cos(\theta) & -\sin(\theta)  \\ \sin (\theta) & \cos(\theta)\end{pmatrix}\begin{pmatrix} \cos(t) \\ \sin (t)\end{pmatrix} = \begin{pmatrix} \cos(\theta + t) \\ \sin (\theta +t) & \end{pmatrix}$$
Was die Additionstheoreme von [[Sinus und Kosinus]] sind!!

#Geometrie



