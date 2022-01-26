## Beschreibung
Langsam werden es immer mehr von diesen Sätzen. Diese werden hier alle zusammengefasst.

### Residuensatz
Sehe [[Residuensatz]]

### Zählen von Nullstellen
Sei
- $\emptyset \neq U \subseteq \mathbb{C}$ [[Offene Menge|offen]]
- $f: U \to \mathbb{C}$ auf keiner [[Zusammenhangskomponente]] von $U$ konstant $0$
- $N:=\{z \in U: f(z)=0\}$ ist die Menge der Nullstellen von $f$
- $\gamma: [0,1] \to U$ [[Nullhomologie|nullhomolog]] in $U$ mit $Spur(\gamma) \cap N = \emptyset$

Dann ist
$$\int\limits_\gamma \frac{f'(z)}{f(z)}\, dz = 2 \pi i \sum\limits_{a\in N}n(\gamma, a)\omega(f, a)$$[^4]

*Das hat nicht wirklich mit Residuen zu tun, der Satz ieht aber ganz ähnlich aus, deshalb ist er hier drin.*

### Polynomquotient
Seien
- $p, q \in \mathbb{C}[X]$ [[Polynom (Komplexe Analysis)|Polynome]]
- $q$ habe auf $\mathbb{R}$ keine [[Nullstelle]] und der Grad von $q$ sei um mindestens 2 größer als der von $p$. 

Dann ist $\frac{p}{q}|_\mathbb{R} \in L^1(\mathbb{R})$ und es gilt:
$$\int\limits_\mathbb{R} \frac{p(x)}{q(x)} = 2 \pi i \sum_{Im \ z > 0} Res(\frac{p}{q}, z)$$[^5]

### Reelles Integral I 
Sei 
- $S \subseteq \mathbb{C}\backslash \mathbb{R}$ eine endliche Menge
- $f: \mathbb{C} \backslash S \to \mathbb{C}$ analytisch mit $\underset{|z| \to \infty}{\lim} |f(z)| = 0$
- $a \in \mathbb{R} \backslash \{0\}$ 
- $g: \begin{array}{rcl}\mathbb{C} \backslash S & \to & \mathbb{C} \\ z & \mapsto & f(z)e^{iaz} \end{array}$

Dann gilt:
$$\lim\int\limits_{-\infty}^\infty f(x)e^{iax} dx = \begin{cases} 2\pi i \sum_\limits{Im (z)>0} Res(g, z) & \text{für } a>0 \\ -2\pi i \sum_\limits{Im (z)>0} Res(g, z) & \text{für } a<0 \end{cases}$$

#Mathe-IV 

[^4]: Zenk - Lemma 23.4.1
[^5]: Zenk - Lemma 23.5.1