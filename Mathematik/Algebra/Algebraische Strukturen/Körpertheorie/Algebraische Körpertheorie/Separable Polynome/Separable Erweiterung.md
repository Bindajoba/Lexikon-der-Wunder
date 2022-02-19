TARGET DECK: Universität::Mathematik::Algebra

$\newcommand{\Q}{\mathbb Q}$
$\newcommand{\R}{\mathbb R}$
$\newcommand{\C}{\mathbb C}$
$\newcommand{\F}{\mathbb F}$
$\newcommand{\Z}{\mathbb Z}$


# Beschreibung



# Definition
Wir nennen die [[Körpererweiterung]] $L|K$ **separabel**, wenn jedes $\alpha \in L$ über $K$ [[Separables Element|separabel]] ist.

# Hinreichende Voraussetzungen
## Erweiterungen von Körper mit Charakteristik 0
Ist $K$ ein Körper der [[Charakteristik (Ring)|Charakteristik]] $0$, dann ist jede [[Algebraische Erweiterung]] $L|K$ separabel.[^1]

## Erweiterungen endlicher Körper
Ist $K$ ein [[Endlicher Körper]], dann ist jede algebraische Erweiterung $L|K$ separabel.[^2]


# Eigenschaften
## Quantifizierung der Separabilität
Sei $L|K$ eine endliche Erweiterung und $\tilde K$ ein algebraisch abgeschlossener Erweiterungskörper von $L$. Dann gilt
$$|Hom_K(L, \tilde K)| \leq [L:K]$$
mit Gleichheit genau dann, wenn die Erweiterung $L|K$ separabel ist.

*Die Anzahl der Homomorphismus besagt irgendwie, wie seperabel eine Erweiterung ist.*[^3]

## Anzahl Zwischenkörper
Jede endliche, separable Erweiterung $L|K$ besitzt nur endlich viele [[Zwischenkörper]].

# Beispiele
## Inseparables Beispiel
Sei $p$ eine Primzahl. $\F_p[t] = $ Polynomring über $\F_p$.
$\F_p(t) = $ rationaler Funktionenkörper über $\F_p =$ Quotientenkörper von $\F_p[t] = \{\frac{u}{v}: u, v \in \F_p[t], v \neq 0\}$

Dann ist $\F_p(t) | \F_p(t^p)$ eine algebraische aber inseparable Erweiterung.



#Algebra 


[^1]: Gerkmann - Satz 16.9
[^2]: Gerkmann - Satz 16.10
[^3]: Gerkmann - Proposition 16:11
