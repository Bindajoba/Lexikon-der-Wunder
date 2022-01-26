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



#Algebra 

[^1]: Gerkmann - Satz 14.1

