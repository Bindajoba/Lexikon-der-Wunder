# Beschreibung
Diese Art des [[Polynom]] ist als Element eines [[Polynomring]] definiert.

# Definiton
## Formale Ableitung
Die Formale Ableitung entspricht der [[Ableitung]]. Im Gegensatz zu ihr ist diese aber nur durch eine formale Anwendung der Ableitungsregeln definiert.

Sei $K$ ein [[Körper]] und $f = \sum_{k=0}^n a_k x^k \in K[x]$, mit $n \in \mathbb{N}_0$ und $a_i \in K$.
Dann nent man 
$$f' = \sum_{k=1}^n k a_{k-1}x^{k-1}$$
die **formale Ableitung** von $f$[^1]

# Eigenschaften
## Zerfallen in Linearfaktoren
Sei $K$ ein Körper, $f \in K[x]$ ein Polynom vom Grad $n \geq 1$ und $L$ ein Erweiterungskörper von $K$, über dem $f$ in Linearfaktoren zerfällt. Dann sind die folgenden beiden Aussagen äquivalent
- Es gilt $ggT(f, f') = 1$ in $K[x]$
- Das Polynom $f$ besitzt in $L$ nur einfache Nullstellen, d.h. es ein $a \in K^\times$ und $n$ verschiedene Elemente $a_1, ..., a_n \in L$, sodass $f = a \prod_{i=1}^n(x-a_i)$

*Hätte ein Polynom keine einfachen Nullstellen, dann hätte die Nullstelle die Form eines kritischen Punktes an der Nullstelle. Damit hätte die Ableitung auch an der Stelle eine Nullstelle und der ggT der beiden Funktionen wäre nicht 1.*

#Zahlentheorie 

[^1]: Gerkmann - Definition 15.2