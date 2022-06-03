# Beschreibung
Das Minimalpolynom einer [[Algebraisches Element|Algebraischen Zahl]] $\alpha \in K$ ist das [[Polynom (Ring, Körper)]] des kleinsten Grades, welches $\alpha$ als Nullstelle hat.

# Definition
Sei $L|K$ eine [[Körpererweiterung]] und sei $\alpha \in L$ algebraisch über $K$. Dann gibt es ein eindeutig bestimmtes, normiertes Polynom $f \in K[x], f\neq 0$ minimalen Grades mit $f(\alpha) = 0$. Man nennt $f$ das **Minimalpolynom** von $\alpha$ über $K$.

Es wird mit $\mu_{K, \alpha}$ bezeichnet.[^1]

# Charakterisierende Eigenschaften
## [[Irreduzibles Polynom]]
Ich denke, die Minimalpolynome sind genau die [[Irreduzibles Polynom]]. Sicher bin ich mir aber nicht.

# Eigenschaften
## Zusammenhang mit anderen Polynomen
Für ein Minimalpolynom $\mu_{K, \alpha}$ gilt:
- Das Polynom $\mu_{K, \alpha}$ ist [[Irreduzibles Polynom|irreduzibel]]
- Ist $g \in K[x]$ ein Polynom mit $g(\alpha) = 0$, dann folgt $f|g$
- Ist $g \in K[x]$ ein weiteres normiertes, [[Irreduzibles Polynom]] mit $\alpha$ als Nullstelle, dann folgt $f = g$

## Keine Nullstellen im Bezugskörper
Sei $\mu_{K, \alpha}$ ein Minimalpolynom. Dann hat es keine Nullstellen in $K$.
Hätte es eine solche Nullstelle $n$, könnte man $\mu_{K, \alpha}$ durch $(x-n)$ polynomdividieren.
Das Ergebnis ist restlos und wie man am Algorithmus erkennen kann, müssen die  Koeffizienten des Ergbnisses wieder in $K$ liegen, womit $\mu_{K, \alpha}$ nicht reduzibel ist. 

# Beispiele
## Wurzel 2 + 3
Finde das [[Minimalpolynom]] von $\sqrt 2+ \sqrt 3$.
$(x-\sqrt 2 - \sqrt 3) \to ((x-\sqrt 2)^2 - 3) = x^2 - 2\sqrt 2 x + 2 -3 = (x^2-1)-2\sqrt 2x$
$\to (x^2-1)^2-8x^2 = x^4-10x^2+1$

Man kann prüfen: $\sqrt 2 + \sqrt 3$ bildet einen $4$-dimensionalen Vektorraum und $\Q(\sqrt 2 + \sqrt 3)$ hat damit den Erweiterungsgrad $4$. Das gefundene Polynom ist also wirklich das Minimalpolynom


[^1]: Gerkmann - Definition 12.2