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

# Übungen
## Klausur 2019 Aufgabe 5
Bestimmte den Erweiterungsgrad von $K := \Q(\sqrt 2, \sqrt[3]2:\Q)$. Dabei darf verwendet werden dass $x^2-2$ und $x^3-2$ Minimalpolynome in $\Q$ sind.

$\Q(\sqrt[3]{2})$ ist ein Zwischenkörper von $K|\Q$, also gilt die Gradformel
$$[K:\Q] = [K : \Q(\sqrt[3]2)] \cdot [\Q(\sqrt[3]2): \Q]$$
Das hintere ist $3$, da $x^3-2$ das Minimalpolynom von $\sqrt[3] 2$ ist.
Das vordere ist $2$, da die Nullstellen $\pm\sqrt 2$ nicht in $\Q(\sqrt[3]2)$ liegen, womit $x^2-2$ das Minimalpolynom von $\sqrt2$ ist.
Wären die Nullstellen $\pm \sqrt2 \in \Q(\sqrt[3]2)$, dann wäre $\Q(\sqrt 2)$ ein Zwischenkörper von $\Q(\sqrt[3]2)|\Q$
Dann muss aber der Erweiterungsgrad $[\Q(\sqrt2):\Q] = 2$ ein Teiler von $[\Q(\sqrt[3]2)]: \Q = 3$, was ein Widerspruch ist.

## Klausur 2018 Aufgabe 7
### c)
Was ist $[\Q(\sqrt {15}, \sqrt {17}):\Q]$?
Das gilt wegen quadratfreien Zahlen. [[Quadratfreie Zahl]]

# Übungen
## Klausur 2016 Aufgabe 5
![[Klausur 2016 Aufgabe 5.png]]
### a)
$f$ ist über $\Q$ irreduzibel und normiert und hat Nullstelle $\alpha$, d.h. es ist Minimalpolynom und der Erweterungsgrad ist 4.

### b)
$\alpha^4 - \alpha -5 = 0 \implies \alpha^4= \alpha+5 \implies \alpha^7 = \alpha^4 + 5\alpha^3 = 5\alpha^3 + \alpha +5$

### c)
Wäre $g$ reduzibel, dann müsste ein Linearfaktor ein $\Q(\alpha)$-Polynom sein, das heißt eine Nullstelle liegt in $\Q(\alpha)$. Nenne diese Nullstelle $\gamma$
Damit wäre $\Q(\gamma)$ ein Zwischenkörper von $\Q(\alpha)|\Q$. Nach der Gradformel gilt
$$[\Q(\alpha):\Q] = [\Q(\alpha):\Q(\gamma)][\Q(\gamma):\Q]$$
Damit würde $4 = n \cdot 3$, was ein Widerspruch ist.


$[\Q(\alpha, \beta): \Q] = [\Q(\alpha, \beta):\Q(\alpha)][\Q(\alpha):\Q] = 3 \cdot 4$ 
Da $f$ Min.pol. in $\Q$ und $g$ Min.pol. in $\Q(\alpha)$.

## Alg Tut 11 Aufgabe 1
Bestimme den Grad vom Zerfällungskörper von $x^7-5$.

Man erhält den Zerfällungskörper indem $\Q$ durch alle Nullstellen von $f$ in $\C$ adjungiert wird.
D.h. Der Zerfällungskörper ist $L := \Q(\sqrt[7]5 \zeta, \sqrt[7]5 \zeta^2, ..., \sqrt[7]5 \zeta^7)$.

Behauptung: $L= \Q(\sqrt[7]5, \zeta)$
$\subseteq:$ Offensichtlich lässt sich jeder Erzeuger aus $\sqrt[7]5$ und $\zeta$ erzeugen.
$\supseteq:$ Gebe alle Elemente des Erzeugers von $L$ als Kombination von $\{\sqrt[7]5 \zeta, \sqrt[7]5 \zeta^2, ..., \sqrt[7]5 \zeta^7\}$ an:
$\sqrt[7]5 = \sqrt[7]5\zeta^7$
$\zeta = \sqrt[7]{5}\zeta / \sqrt[7]5\zeta^7 = \sqrt[7]5\zeta / \sqrt[7]5 = \zeta$

Sei $\alpha = \sqrt[7]5$
Zu Zeigen: $[L:\Q] = 42$
Da $\Q(\zeta)$ ein Zwischenkörper von $L|K$ ist gilt die Gradformel
$$[L:\Q] = [L:\Q(\zeta)]\cdot[\Q(\zeta):\Q]$$
Außerdem gilt:
$$[L:\Q] = [L:\Q(\alpha)]\cdot [\Q(\alpha):\Q]$$
Nach Angabe ist $[\Q(\zeta):\Q] = 6$
Da $f=\mu_{\Q, \alpha}$ Grad 7 hat, gilt $[\Q(\alpha): \Q] = 7$

Somit wird $[L:\Q]$ von $6$ und $7$ geteilt. $\implies [L:\Q]$ wird von $kgV(6, 7) =42$ geteilt.
$\implies [L:\Q] \geq 42$

Was ist $[L:\Q(\alpha)]$?
Sei $g$ das Minimalpolynom von $\sqrt[7]5$ in $\Q(\zeta)$
- $f \in \Q(\zeta)[x]$ und $f(\alpha) = 0 \implies f|g \implies grad(g) \leq grad(f) = 7 \implies [L:\Q(\alpha)] \leq 7$ 
$[L:\Q] = [L:\Q] = [L:\Q(\zeta)]\cdot[\Q(\zeta):\Q] = [L:\Q] \leq 7\cdot6 = 42$

D.h. $[L:\Q] = 42$




#Algebra 

[^1]: Gerkmann - Definition 11.10
[^2]: Böhm - Bemerkung 7.2.3





