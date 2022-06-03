# Definition
Sei $R$ ein [[Ring]] und $I \subseteq R$ ein [[Ideal]]. Dann ist die Menge der [[Nebenklasse (Ring)|Nebenklassen]] $R/I$ mit den [[Verknüpfung auf Nebenklassen (Ring)]] ein Ring, den man als **Faktorring** beeichnet.

Das ist im Grunde die gleiche Idee wie bei der [[Faktorgruppe]]

## Kanonische Epimorphismus
Es gibt einen Zusammenhang zwischen dem ursprünglichen Ring $R$ und einem **Faktorring** $R/I$.
Dieser Zusammenhang wird formalisiert durch den **kanonischen Epimorphismus** (siehe der [[Kanonischer Epimorphismus (Gruppe)]]) 


# Eigenschaften
## Isomorphie zu Körpern
Sei $L|K$ eine [[Körpererweiterung]], $\alpha \in L$ [[Algebraisches Element|algebraisch]] über $K$ und $f = \mu_{K, \alpha}$. Dann gibt es einen [[Körperisomorphismus|Isomorphismus]]
$$\bar\phi : K[x]/(f) \to K(\alpha), \bar\phi(g + (f)) = g(\alpha) \text{ für alle } g \in K[x]$$
Dabei bezeichnet $K(\alpha)$ den von $\alpha$ erzeugten Zwischenkörper der Erweiterung $L|K$, $(f)$ das von $f$ erzeugte [[Ideal]] und $K[x]/(f)$ ist ein [[Faktorring]] (der als Ergebnis einen Körper hat)[^3]

*Der Beweis erfolgt über den [[Homomophiesatz für Ringe]]. Die grundsätzliche Idee ist, dass jedes Polynom $g$ durch $f(\alpha)$ mit Rest teilbar ist, wenn der Grad größer gleich $grad(f)$ ist. Man kann also jedes Polynom aus $K[x]$ teilen, bis ein Repräsentant $< grad(f)$ herauskommt. In diesen kann man $\alpha$ einsetzen. Abbildung gefunden.*[^4]

[^4]: Gerkmann - Satz 12.5

#Zahlentheorie 