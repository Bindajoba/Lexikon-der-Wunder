## Beschreibung
Auf der [[Riemannsche Zahlensphäre]] kann man eine Metrik auf $\hat{\mathbb{C}}$ definieren:
 
## Definition
$$d: \begin{array}{rcl}\hat{\mathbb{C}} \times \hat{\mathbb{C}} &\to& [0, \infty[ \\ (w, z) & \mapsto & ||Q(w)-Q(z)||_2 \end{array}$$ wobei $Q$ die Umkehrabbildung der [[Stereographische Projektion]] ist.

Verkürzt:
Für $w, z \in \hat{\mathbb{C}}$ gilt:
$$d(z, w) = \begin{cases} \frac{2|w-z|}{\sqrt{(1+|w|^2)(1+|z|^2)}} & \text{für } w,z \in \mathbb{C} \\ \frac{2}{\sqrt{1+|z|^2}} & \text{für } z \in \mathbb{C}, w = \infty \end{cases}$$

## Eigenschaften
### Kehrbrucheigenschaft
Für $w, z \in \mathbb{C}\backslash \{0\}$ gilt $d(w, z) = d(\frac{1}{w}, \frac{1}{z})$ und $d(0, z) = d(\frac{1}{z}, \infty)$

### Zentrum unendlich
1. Ist $r > 0$, so hat $K_{\hat{\mathbb{C}}}(\infty, r)$ die Form $K_{\hat{\mathbb{C}}}(\infty, r) = \hat{\mathbb{C}}\backslash K_r$, wobei $K_r \subset \mathbb{C}$ eine bestimmte kompakte Menge ist.
2. Ist $K \subseteq \mathbb{C}$ kompakt, so gibt es ein $R>0$, sodass $K_{\hat{\mathbb{C}}}(\infty, r) \subseteq \hat{\mathbb{C}}\backslash K$ ist
