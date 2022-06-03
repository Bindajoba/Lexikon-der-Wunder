# Definition 
Eine Funktion $d: X \times X \to \R^+_0$, sodass für alle $x, y \in X$ gilt:
1) $d(x, y) = 0 \iff x = y$
2) $d(x, y) = d(y, x)$
3) $d(x, z) \leq d(x, y)+d(y, z)$

# Beispiele
## Euklidische Metrik
Der ist der kleinste Abstand zweier Punkte in $\R^n$.
$$d(x, y) := \sqrt{(x_1-y_1)^2+...+(x_n-y_n)^2}$$
## Manhattan Metrik
Abstände werden wie in Manhattan gemessen.
$$d(x, y) = |x_1-x_1|+...+|x_n+y_n|$$
## Paris-Metrik
Siehe [[Paris-Metrik]]

## Kausdorff-Abstand
Siehe [[Hausdorff-Abstand]]