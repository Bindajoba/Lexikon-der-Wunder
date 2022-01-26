## Beschreibung
Aus dem charakteristischen Polynom lässt sich der Lösungsraum einer homogenen [[Skalare lineare Differentialgleichung|skalaren linearen DGL höherer Ordnung]] mit konstanten und reellen Skalaren errechnen.

## Definition
Betrachte das DGL 
$$x^{(k)}(t) + a_kx^{(k-1)} ... a_2x' + a_1x = 0 \tag{1}$$

Dann ist das charakteristische Polynom der DGL: 

$$p(z):=z^k + a_{k-1}z^{k-1}+...+a_1z+a_0$$

## Verwendung
Mit dem charakteristischen Polynom lässt sich der Lösungsraum von $(1)$ aus den Nullstellen bestimmen.

Ist $\rho \in \mathbb{R}$ eine m-Fache Nullstelle von p, so sind die m Funktionen
$$e^{\rho t}, te^{\rho t}, ..., t^{m-1}e^{\rho t}$$ linear unabhängige Lösungen von $(1)$.

Ist $\rho + i\sigma \in \mathbb{C}\backslash\mathbb{R}$ eine m-Fache Nullstelle von p, ist ist auch $\rho - i\sigma$ eine m-fache Nullstelle.
In dem Fall sind die 2m Funktionen
$$e^{\rho t}cos(\sigma t), te^{\rho t}cos(\sigma t), ..., t^{m-1}e^{\rho t}cos(\sigma t)$$ und 
$$e^{\rho t}sin(\sigma t), te^{\rho t}sin(\sigma t), ..., t^{m-1}e^{\rho t}sin(\sigma t)$$ linear unabhängige Lösungen von $(1)$.

#Mathe-IV 