## Beschreibung 
Das [[Polynom]] kennt man schon aus der Schule


## Charaktiersierungen
### Charakterisierung I
$$F: \begin{array}{rcl} \hat{\mathbb{C}}&\to &\hat{\mathbb{C}} \\ z& \mapsto& \begin{cases} f(z) &\text{für } z \in \mathbb{C} \\ \infty &\text{für } z = \infty \end{cases} \end{array}$$ genau dann eine holomorphe Fortsetzung von $f$, wenn $f$ ein Polynom ist.

### Charakterisierung II
$f$ ist genau dann ein Polynom, wenn es keine [[Transzendente Funktion]] ist.

## Eigenschaften
### Ganze Funktion
Polynome sind [[Ganze Funktion|ganz]]

### Abschätzung
Alles was unten steht musste ich neu schreiben, weil ich den Text im Clipboard verloren habe. Seitdem habe ich die Clipboard-Geschichte aktiviert. 

Es sei $p: \begin{array}{rcl} \mathbb{C} & \to & \mathbb{C}\\ z & \mapsto & a_nz^n+...+a_1z+a_0 \end{array}$ ein Polynom vom Grad $n$
Dann gibt es zu jedem $\varepsilon \in ]0,1[$ ein $\rho_\varepsilon \geq 1$, sodass für alle $z \in \mathbb{C}$ mit $|z| \geq \rho_\varepsilon$ gilt:
$$(1-\varepsilon)|a_n||z^n| \leq |p(z)| \leq (1+\varepsilon)|a_n||z^n|$$

*Die Intuition des Satzes ist, dass das Verhalten und damit der Betrag eines Polynoms im Unendlichen nur von der Potenz mit dem höchsten Grad und dessen Vorfaktor abhängt.

Betrachtet man daher ein Monom mit gleichem Grad aber etwas kleinerem Vorfaktor und entfernt sich vom 0-Punkt, dann ist das der Betrag des Monoms ab einer bestimmten Entfernung $\rho_\varepsilon$ kleiner als $|p(z)|$.
Gleiches gilt auch für größere Vorfaktoren.* [^1]

### Nullstellen
Siehe [[Fundamentalsatz der Algebra]]

### Zählen von Nullstellen
Ein Polynom $p(z)$ lässt sich in die Nullstellenform bringen. Die einzelnen Produkte der Nst.form haben das Aussehen $(z-a)$, geben also den (komplexen) Abstand zwischen $a$ und $z$ an.

Das Polynom gibt als das Produkt der Verbindungsstrecken der Nullstellen zu $z$ zurück.

Man bewege nun $z$ entlang einer Schleife die einmal um genau 2 Nullstellen $a$ und $b$ gewickelt ist.

Die Verbindungsstrecken zu $a$ und $b$ erleben beide eine Umrundung. Und da beim komplexen Produkt Winkel addiert werden, muss sich die Kurve, die das Bild $p(z)$ zeichnet zweimal um $0$ winden!
Es ist offensichtlich, dass somit gilt: 

Windet sich eine einfache [[Schleife]] $\Gamma$ einmal um $m$ Nullstellen von $p(z)$, dann gilt für die [[Umlaufzahl]] $n(p(\Gamma), 0) = m$

*Dieses Verhalten gilt auch bei analytischen Funktionen und wird da als das [[Argumentprinzip]] bezeichnet.*


### Schwerpunkt der Nullstellen
Verschiebt man ein Polynom um einen Parameter $q$, bleibt der [[Schwerpunkt]] der Nullstellen gleich.

### Wertemenge
Für jedes Polynom $p$ mit Grad $n \geq 1$ gilt: $p(\mathbb{C}) = \mathbb{C}$[^2]

### Gleiche Funktionswerte
Für jedes Polynom $p$ mit Grad $n \geq 1$ gilt:
Für jedes $w \in \mathbb{C}$ besitzt $p^{-1}(\{w\})$ höchstens $n$ Elemente[^2]

#Mathe-IV 
#Needham 

[^1]: Lemma 22.6.3
[^2]: Zenk - Lemma 26.2.1