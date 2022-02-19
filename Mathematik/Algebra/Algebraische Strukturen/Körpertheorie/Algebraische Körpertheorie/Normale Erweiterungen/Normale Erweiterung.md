TARGET DECK: Universität::Mathematik::Algebra

# Beschreibung
Eine spezielle Form einer [[Körpererweiterung]].

# Definition
Eine [[Algebraische Erweiterung]] $L|K$ heißt normal, wenn folgende Bedingung erfüllt ist:
Ist $f \in K[x]$ ein [[Irreduzibles Polynom|irreduzibles Polynom]], das in $L$ eine Nullstelle besitzt, dann zerfällt $f$ über $L$ in Linearfaktoren.[^1]

# Charakterisierungen
Sei $K$ ein [[Körper]], und seien $\tilde K \supseteq L \supseteq K$ [[Körpererweiterung|Erweiterungen]] von $K$, wobei $L|K$ endlich und $\tilde K$ [[Algebraisch Abgeschlossener Körper|algebraisch abgeschlossen]] ist. 
Dann ist $L|K$ genau dann normal, wenn
- Es gibt ein nicht-konstantes Polynom $f \in K[x]$, so dass $L$ der Zerfällungskörper von $f$ über $K$ ist. ODER
- Es gilt $Hom_K(L, \tilde K) = Aut_K(L)$[^3]

## Normalteiler
Eine Erweiterung ist normal, wenn seine zugehörige [[Galoisgruppe]] ein Normalteiler ist oder so. Siehe [[Hauptsatz der Galoistheorie]].

# Hinreichende Bedingungen
Wenn ein [[Körper]] $K$ alle $p$-ten Wurzeln der Einheit enthält und wenn $a^p \in K$ aber $a \notin K$, dann ist $K(a)$ eine [[Normale Erweiterung]] von $K$

# Beispiele
Sei $K$ ein Körper und $L|K$ eine Erweiterung von Grad 2. Dann ist $L|K$ normal.[^2]

*Beweis:*
o.E. sei $f$ normiert. Dann gilt $f = \mu_{\alpha, K} \implies [K(\alpha): K] = grad(f)$...

#Algebra 

[^1]: Gerkmann - Definition 16.1
[^2]: Gerkmann - Proposition 16.2  
[^3]: Gerkmann - Satz 16.3
