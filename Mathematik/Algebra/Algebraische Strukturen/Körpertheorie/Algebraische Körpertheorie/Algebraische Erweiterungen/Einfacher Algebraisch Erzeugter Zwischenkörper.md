# Beschreibung
Eine weitere Spezifikation des [[Einfach Erzeugter Zwischenkörper]] mt der zusätzlichen Forderung, dass das erzeugende Element $\alpha$ [[Algebraisches Element|algebraisch]] sein muss.
Das Paar des Ursprünglichen Körpers und der [[Erzeugter Zwischenkörper]] bildet eine [[Algebraische Erweiterung]].

*Auch den Begriff habe ich mir ausgedacht, da er spezielle Eigenschaften hat.*

Offensichtlich ist dieser auch [[Einfache Erweiterung|einfach]]

# Eigenschaften
## Vektorraumeigenschaft
Sei $L|K$ eine [[Körpererweiterung]], $\alpha \in L$ algebraisch über $K, f = \mu_{L, \alpha}$ und $n = grad(f)$. Dann bilden die Elemente $1, \alpha, \alpha^2,..., \alpha^{n-1}$ eine Basis von $K(\alpha)$ als $K$-[[Vektorraum]].
Insbesondere gilt $[K(\alpha):K] = n$


## Isomorphie zu faktorisierten Polynomringen
Sei $L|K$ eine [[Körpererweiterung]], $\alpha \in L$ [[Algebraisches Element|algebraisch]] über $K$ und $f = \mu_{K, \alpha}$. Dann gibt es einen [[Körperisomorphismus|Isomorphismus]]
$$\bar\phi : K[x]/(f) \to K(\alpha), \bar\phi(g + (f)) = g(\alpha) \text{ für alle } g \in K[x]$$
Dabei bezeichnet $K(\alpha)$ den von $\alpha$ erzeugten Zwischenkörper der Erweiterung $L|K$, $(f)$ das von $f$ erzeugte [[Ideal]] und $K[x]/(f)$ ist ein [[Faktorring]] (der als Ergebnis einen Körper hat)[^3]

*Der Beweis erfolgt über den [[Homomophiesatz für Ringe]]. Die grundsätzliche Idee ist, dass jedes Polynom $g$ durch $f(\alpha)$ mit Rest teilbar ist, wenn der Grad größer gleich $grad(f)$ ist. Man kann also jedes Polynom aus $K[x]$ teilen, bis ein Repräsentant $< grad(f)$ herauskommt. In diesen kann man $\alpha$ einsetzen. Abbildung gefunden.*[^4]

[^4]: Gerkmann - Satz 12.5

#Algebra 