TARGET DECK: Universität::Mathematik::Algebra

# Beschreibung
Nimmt man ein [[Polynom]] eines Körpers und erweitert den Körper nur um seine Nullstellen, dann erhält man den **Zerfällungskörper** des Polynoms.

# Definition
Sei $K$ ein [[Körper]] und $f \in K[x]$ ein nicht-konstantes Polynom. Dann existiert einen Erweiterungskörper $L$ von $K$ mit den beiden Eigenschaften
1. Das Poynom $f$ zerfällt über $L$ in Linearfaktoren
2. Sind $\alpha_1,...\alpha_r$ die Nullstellen von $f$ in $L$, dann gilt $L = K(\alpha_1,...,\alpha_r)$

Ein Erweiterungskörper von $L$ mit diesen Eigenschaften wird **Zerfällungskörper** von $f$ über $K$ genannt.[^1]

# Eigenschaften
Ist $K$ ein Körper und $S \subset K[x]$ eine beliebige (möglicherweise unendliche) Menge von nicht-konstanten Polynomen, dann gibt es einen Erweiterungskörper $L$ von $K$ mit der Eigenschaft, dass jedes Polynom $f \in S$ über $L$ in Linearfaktoren zerfällt, und dass $L = K(N)$ gilt, wobei
$$N = \{\alpha \in L : f(\alpha) = 0 \text{ für ein } f \in S\}$$
Die Menge der Nullstellen sämtlicher Polynome aus $S$ bezeichnet. Man nennt $L$ dann einen Zerfällungskörper von $S$ über dem Grundkörper $K$.

## Algebraische Erweiterung
Sei $K$ ein Körper und $S \subset K[x]$ eine beliebige Menge nicht-konstanter Polynome. Dann ist jeder Zerfällungskörper von $S$ eine [[Algebraische Erweiterung]] von $K$.

## Proposition
Sei $K$ ein Körper, $S \subseteq K[x]$ eine Menge nicht-konstanter Polynome und $\tilde L$ ein Erweiterungskörper von $K$ mit der Eigenschaft, dass jedes Polynom aus $S$ über $\tilde L$ in Linearfaktoren zerfällt. Dann enthält $\tilde L$ genau einen Zerfällungskörper $L_S$ von $S$ über $K$. Es handelt sich um den kleinsten Zwischenkörper von $\tilde L | K$ mit der angegebenen Eigenschaft: ist $L_1$ ein beliebiger Zwischenkörper mit dieser Eigenschaft, dann folgt $L_1 \supseteq L_S$

## Eindeutigkeit
Sei $K$ ein Körper und $S \subset K[x]$ eine Menge bestehten aus nicht-konstanten Polynomen. Sei $\phi: K \to \tilde K$ ein Isomorphismus von Körpern und $\tilde S = \{\phi(f): f \in S\}$. Sei $L$ ein Zerfällungskörper von $S$ und $\tilde L$ ein Zerfällungskörper von $\tilde S$. Dann gibt es eienn Isomorphismus $\psi: L \to \tilde L$ mit $\psi|_K = \phi$.

*d.h. Der Zerfällungskörper ist eindeutig!!!*

# Beispiele
## Polynom zu Zerfällungskörper finden
Angenommen, es gäbe ein Polynom $f$, von dem $\Q(\sqrt[3] 2)$ der Zerfällungskörper ist. Das Polynom kann nicht nur $(x-\sqrt[3]2)$ sein, also müsste sein Grad größer als $1$ sein.
Damit hätte die [[Galoisgruppe]] der Erweiterung $[\Q(\sqrt[3]2): \Q]$ mehr als ein Element, was einer vorherigen Aufgabe widerspricht.

# Übungen
## Klausur 2018 Aufgabe 5
![[Klausur 2018 Aufgabe 5.png]]
### a)
Die Nullstellen von $f$ sind $\pm\sqrt[4]17, \pm i\sqrt[4]17$. Der Zerfällungskörper entsteht durch Adjunktion der Nullstelle an $\Q$.
Offenseichtlich ist jede Nullstelle durch $\{\sqrt[4]17, i\}$ beschreibbar, d.h. $L \subseteq \Q(\sqrt[4]17, i)$
Desweiteren gilt $\frac{1}{17}i\sqrt[4]17 \cdot \sqrt[4]17^3 = i$ und $\sqrt[4]17 = \sqrt[4]17$: Deshalb $L \supseteq \Q(\sqrt[4]17, i)$

$\Q(\sqrt[4]17)$ ist ein Zwischenkörper von $L:\Q$. Es gilt die Gradformel:
$$[L : \Q] = [\Q(\sqrt[4]17, i) : \Q(\sqrt[4]17)][\Q(\sqrt[4]17):\Q]$$
Das Minimalpolynom von $\sqrt[4]17$ in $\Q$ ist $f$, also $[\Q(\sqrt[4]17):\Q]$. (da normiert und nach Aufgabenstellung irred.)
Das Minimalpolynom von $i$ in $\Q(\sqrt[4]17)$ ist $g(x) =x^2+1 = (x+i)(x-1)$. $g$ ist irred. denn die Nullstellen sind nicht-reell und liegen damit nicht in $\Q(\sqrt[4]17) \subseteq \R$ und $g$ ist normiert.
Damit ist $[\Q(\sqrt[4]17, i) : \Q(\sqrt[4]17)] = 2$ und $[L : \Q] = 2 \cdot 4 = 8$.


### b)
Angenommen, es hätte eine Nullstelle $\zeta \in L$. Dann wäre $\Q(\zeta)$ eine Erweiterung vom Grad drei und eine Zwischenerweiterung von $L|\Q$.
Damit muss $3$ ein Teiler von $[L:\Q]$ sein, was nicht geht und einen Widerspruch erzeugt.








#Algebra 

[^1]: Gerkmann - Satz 14.1

