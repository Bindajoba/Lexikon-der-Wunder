# Beschreibung
Gibt an, wie groß die Erweiterung ist.

# Definition
Ist $L|K$ eine [[Körpererweiterung]], dann definieren die beiden Abbildungen
$$+: L \times L \to L, (\alpha, \beta) \mapsto \alpha + \beta$$
und 
$$\cdot: K \times L \to L, (a, \alpha) \mapsto a\alpha$$
eine $K$-[[Vektorraum|Vektorraumstruktur]] auf $L$

Beispiel: $\mathbb{C}$ kann als zweidimensionaler $\mathbb{R}$-Vektorraum betrachtet werden. Dabei bezeichnet man $[L:K] = dim_K L$ als den **Grad der Körpererweiterung**, auch $[L:K]= \infty$ ist als Wert zugelassen. Ist $[L:K]$ endlich, dann nennt man $L | K$ eine [[Endliche Körpererweiterung]][^1]

# Eigenschaften
## Gradformel
Seien $L|K$ und $M|L$ endliche Körpererweiterungen. Dann ist auch die Körpererweiterung $M|K$ endlich und es gilt
$$[M : K] = [M:L]\cdot[L:K]$$



## Grad 1
Es gilt $[L:K] = 1$ genau dann, wenn $L = K$.[^2]

**Beweis:**
Ist $[L:K] = 1$, dann ist $L$ ein 1-dimensionaler $K$-Vektorraum, hat also die gleiche Struktur wie einfach nur $K$

# Aufgaben
## Klausur 2019 Aufgabe 5
Bestimmte den Erweiterungsgrad von $K := \Q(\sqrt 2, \sqrt[3]2:\Q)$. Dabei darf verwendet werden dass $x^2-2$ und $x^3-2$ Minimalpolynome in $\Q$ sind.

$\Q(\sqrt[3]{2})$ ist ein Zwischenkörper von $K|\Q$, also gilt die Gradformel
$$[K:\Q] = [K : \Q(\sqrt[3]2)] \cdot [\Q(\sqrt[3]2): \Q]$$
Das hintere ist $3$, da $x^3-2$ das Minimalpolynom von $\sqrt[3] 2$ ist.
Das vordere ist $2$, da die Nullstellen $\pm\sqrt 2$ nicht in $\Q(\sqrt[3]2)$ liegen, womit $x^2-2$ das Minimalpolynom von $\sqrt2$ ist.
Wären die Nullstellen $\pm \sqrt2 \in \Q(\sqrt[3]2)$, dann wäre $\Q(\sqrt 2)$ ein Zwischenkörper von $\Q(\sqrt[3]2)|\Q$
Dann muss aber der Erweiterungsgrad $[\Q(\sqrt2):\Q] = 2$ ein Teiler von $[\Q(\sqrt[3]2)]: \Q = 3$, was ein Widerspruch ist.




#Algebra 

[^1]: Gerkmann - Definition 11.10
[^2]: Böhm - Bemerkung 7.2.3





