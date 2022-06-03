# Beschreibung
Der erzeugter Zwischenkörper $K(a)$ ist der kleinste [[Erweiterungskörper]], der $a$ enthält.

*Diese Definition lässt sich sehr leicht mit dem Ausdruck $K[a]$ verwechseln. $K[a]$ ist der [[Erzeugter Teilring|kleinste Erweiterungsring]] von $K$, der $a$ enthält. $K$ ist nämlich als Körper auch ein Ring.*


# Definition
## Kleinster Zwischenkörper
Sei $\tilde L|K$ eine Körpererweiterung und $S \subseteq \tilde L$ eine Teilmenge. Dann gibt es einen eindeutig bestimten Zwischenkörper $L$ von $\tilde L|K$ mit den Eigenschaften
1. $L \supseteq S$
2. Für jeden weiteren Zwischenkörper $L'$ von $L'|K$ mit $L' \supseteq S$ gilt $L' \supseteq L$

Insgesamt ist $L$ also der kleinste Zwischenkörper von $L|K$ mit der Eigenschaft $L \supseteq S$.[^1]

Der obere Körper $L$ wird mit $K(S)$ bezeichnet.


# Eigenschaften
## Vereinigung von Erzeugern
Es gilt
$$K(S \cup T) = K(S)(T)$$[^2]

## Quotientenkörper des Erzeugten Teilrings
Der Körper $K(\alpha_1, ..., \alpha_n)$ ist der Quotientenkörper des [[Integritätsbereich]] $K[\alpha_1, ..., \alpha_n]$.[^4]


# Beispiel
## Einfach erzeugter Zwischenkörper
Ein [[Einfach Erzeugter Zwischenkörper]] ist ein Körper, der nur durch ein Element erweitert wird.

Sei $\tilde L|K$ eine Körpererweiterung und $a \in \tilde L$. Dann gilt
$$K(a) = \left\{\frac{f(a)}{g(a)}:f, g \in K[x], g(a) \neq 0\right\}$$
wobei $K[x]$ der [[Polynomring]] über $K$ ist


#Algebra 

[^1]: Gerkmann - Satz 11.7
[^2]: Gerkmann - Proposition 11.8
[^3]: Gerkmann - Satz 12.5
[^4]: Böhm - Lemma 7.5.3