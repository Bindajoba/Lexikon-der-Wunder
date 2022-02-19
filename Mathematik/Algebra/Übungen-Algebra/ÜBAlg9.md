# Aufgabe 1
a)

$\alpha = \sqrt[3]{2 + \sqrt{2}}$
$2 + \sqrt{2}$ ist die Lösung von $x^3 - (2+\sqrt{2}) = (x^3 - 2) - \sqrt{2}$
Probiere: $((x^3 - 2) - \sqrt{2})((x^3 - 2) + \sqrt{2}) = (x^3-2)^2 - 2 = x^6 - 4x^3 + 2$

$[\mathbb{Q}(\alpha): \mathbb{Q}] = 6$
$x^6 - 4x^3 + 2$ ist normiert, hat Grad $6=[\mathbb{Q}(\alpha): \mathbb{Q}]$ und Nullstelle $\alpha$ und ist damit Minimalpolynom von $\alpha$ in $\mathbb{Q}$.

$\mathbb{Q} \subseteq \mathbb{Q}(\alpha)$ und $\sqrt{2} = \alpha^3 -2 \implies \mathbb{Q}(\alpha) | \mathbb{Q}(\sqrt{2})|\mathbb{Q}$

Damit gilt die Gradformel:
$$[\mathbb{Q}(\alpha):\mathbb{Q}] = [\mathbb{Q}(\alpha):\mathbb{Q}(\sqrt{2})]\cdot[\mathbb{Q}(\sqrt{2}):\mathbb{Q}]$$
Aus $[\mathbb{Q}(\alpha):\mathbb{Q}] = 6$ und $[\mathbb{Q}(\sqrt{2}):\mathbb{Q}] = 2$ folgt $[\mathbb{Q}:\mathbb{Q}(\sqrt{2})] = 3$
$x^3 - (2+\sqrt{2})$ ist normiert, hat Grad $3$ und Nullstelle $\alpha$ und ist damit Minimalpolynom von $\alpha$ in $\mathbb{Q}(\sqrt{2})$

b)

Offensichtlich ist $\gamma$ eine Nullstelle von $f(x) = x^3 + x+ 1$.
0 und 1 sind keine Nullstellen von $f$. Damit ist $f$ irreduzibel in $\mathbb{F}_2$. 
$\implies f = \mu_{\mathbb{F}_2, \gamma}$
Der Erweiterungsgrad von $\mathbb{F}_2(\gamma)|\mathbb{F}_2$ ist durch den Grad des Minimalpolynoms von $\gamma$ gegeben: $[\mathbb{F}_2(\gamma) : \mathbb{F}_2] = 3$.

Damit ist $\mathbb{F}_2(\gamma) = \{a + b\gamma + c\gamma^2: a,b,c \in \mathbb{F}_2\}$
Obere Menge zerlegt sich in $\{0, 1\}$ und $S = \{\gamma, \gamma+1,\gamma^2, \gamma^2+1, \gamma^2 +\gamma, \gamma^2+\gamma+1\}$

Behauptung: Für alle $\alpha \in S$ ist $[\mathbb{F}_2(\alpha):\mathbb{F}_2] = 3$.
$\mathbb{F}_2(\alpha)$ ist ein Zwischenkörper von $\mathbb{F}_2(\gamma)$ und $\mathbb{F}_2$.
Damit gilt nach der Gradformel:
$$[\mathbb{F}_2(\gamma):\mathbb{F}_2] = [\mathbb{F}_2(\gamma):\mathbb{F}_2(\alpha)]\cdot[\mathbb{F}_2(\alpha):\mathbb{F}_2]$$
Es gilt: $[\mathbb{F}_2(\gamma):\mathbb{F}_2] = 3$, damit teilt $[\mathbb{F}_2(\alpha):\mathbb{F}_2]$ die Zahl 3. D.h. $[\mathbb{F}_2(\alpha):\mathbb{F}_2] \in \{1, 3\}$.

Aus $[\mathbb{F}_2(\alpha):\mathbb{F}_2] = 1$ würde $\mathbb{F}_2(\alpha) =\mathbb{F}_2$ folgen, also $[\mathbb{F}_2(\alpha):\mathbb{F}_2] = 3$.
Finde nun alle Kandidaten für reduzible Polynome von Grad 3, diese sind
- $f(x) = x^3+x+1$
- $g(x) = x^3 + x^2 +1$

Setz nun alle $\alpha \in S$ ein und berücksichtige: $\gamma^3 = \gamma + 1 \implies \gamma^4 = \gamma^2+\gamma \implies \gamma^5 = ...$
- $f(\gamma + 1) = (\gamma+1)^3+(\gamma+1)+1 = \gamma^3 + \gamma^2 + \gamma + 1 + \gamma = \gamma^3 + \gamma 2 +1 = ...$ (scheint keine Nullstelle zu sein)
- $g(\gamma+1) = (\gamma+1)^3+(\gamma+1)^2+1 = 0$
$g$ ist Minimalpolynom von $\gamma+1$, führe das Verfahren für alle Elemente fort.





