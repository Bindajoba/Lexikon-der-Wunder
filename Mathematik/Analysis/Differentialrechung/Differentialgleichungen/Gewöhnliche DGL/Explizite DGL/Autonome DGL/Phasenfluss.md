## Beschreibung
Betrachtet man bei einer [[Autonome Differentialgleichung|autonomen Differentialgleichung]] statt der Veränderung eines Punktes im Laufe der Zeit (wie es beim [[Fluss]] impliziert ist), die Veränderung aller Punkte gleichzeitig, dann nennt man das den [[Phasenfluss]].

## Definition
Die Definition ist die gleiche wie beim [[Fluss]], nur fokussiert man sich eher auf das Ganze.

Sei
- $D \subseteq \mathbb{K}^d$ ein offener und zusammenhängender Raum von [[Zustand|Zuständen]]
-  Sei $v: D \to \mathbb{K}^d$ die lokal lipschitzstetige rechte Seite der DGL

Der **Phasenfluss** des autonomen Systems $$x'=v(x)$$ ist
$$\varphi: \begin{array}{rcl}J_\xi \times D & \to & \mathbb{K}^d\\(t, x)& \mapsto & \lambda_{(0, \xi)}(t)\end{array}$$

## Eigenschaften
### Zusammenhang mit Einparametrigen Gruppen
Ein **Phasenfluss** kann als [[Einparametrige Gruppe]] von [[Stetigkeit|stetigen]] [[Transformation|Transformationen]] verstanden werden, denn sie erfüllt alle dafür nötigen Eigenschaften:

- $\varphi(t + s, \cdot)$ ist äquivalent dazu, zu beobachten, was mit einem Anfangspunkt nach $t$ Zeiteinheiten passiert, dann stehen zu bleiben, den Punkt an dem man stehen geblieben ist als neuen Startpunkt zu wählen und dann um $s$ Zeiteinheiten weitersimulieren. 
- $\varphi(-t, \cdot)$ ist äquivalent dazu, einen Punkt $\xi$, der nach $t$ Zeiteinheiten den neuen Zustand $\xi'$ erreicht, an seinen Anfang zurück zu senden. (*Inverse*)

$\varphi(0, \cdot)$ beschreibt dabei die Null-Transformation, also die Identitätstranformation.

#Arnold 