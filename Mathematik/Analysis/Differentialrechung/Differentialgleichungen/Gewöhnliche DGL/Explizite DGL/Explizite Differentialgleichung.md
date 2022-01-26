## Beschreibung
Eine [[Gewöhnliche Differentialgleichung]] heißt *n-dimensionale explizite Differentialgleichung k-ter Ordnung*, wenn auf der linken Seite die $k$-te Ableitung von $x$ steht Gleichung null sind.

## Definition
Seien
- $k, n \in N$ 
*$k$ ist die höchste Ableitung der Gleichung*
*$n$ ist die Dimension von der Lösung*
- $U\subseteq \mathbb{R} \times \mathbb{K}^{kn}$ ein [[Gebiet]]
*$U$ ist der Defintionsbereich der Gleichung $f$*
- $f: U \to \mathbb{K^n}$

Eine Gleichung
$$x^k = f(t, x, x', ..., x^{(k-1)})\tag{1}$$ bzw.
$$\begin{array}{c}&x_1^{(k)} = f_1(t, x, x', ..., x^{(k-1)})=0 \\ &x_2^{(k)}=f_2(t, x, x', ..., x^{(k-1)})=0 \\ &\vdots \\ &x_n^{(k)}=f_n(t, x, x', ..., x^{(k-1)})=0 \end{array}$$

heißt n-dimensionale implizite Differentialgleichung k-ter Ordnung.


### Definition Lösung
Siehe [[Lösung]]

## Lösung
Seien
- $k, n \in N$ 
*$k$ ist die höchste Ableitung der Gleichung*
*$n$ ist die Dimension von der Lösung*
- $U\subseteq \mathbb{R} \times \mathbb{K}^{kn}$ ein [[Gebiet]]
*$U$ ist der Defintionsbereich der Gleichung $f$*
- $f: U \to \mathbb{K^n}$

Eine **n-Dimensionales Lineares Homogenes Differentialgleichungssystem k-ter Ordnung**
$$x^{(k)} = f(t, x, x', ..., x^{(k-1)}) \tag{1}$$ kann in eine $nk$-dimensionales [[Lineares Differentialgleichungssystem erster Ordnung]] umgewandelt werden:

Betrachte jede Ableitung von $x$ als eine eigene Variable:
$$\begin{array}{c} y_1 = x\\ y_2 = x' \\ \vdots \\ y_k = x^{(k-1)}  \end{array}$$ Dann gilt$$\begin{array}{c} y_1' = x' = y_2\\ y_2' = y_3 \\ \vdots \\ y_{k-1}' = y_{k} \\ y_k' = f(t, y_1, ..., y_k)  \end{array}\tag{2}$$ 

Ist $\mu = \begin{pmatrix} \mu_1 \\ \vdots \\ \mu_k \end{pmatrix}$ eine Lösung von $(2)$, dann ist $\mu_1 = x$ eine Lösung von $(1)$[^1]

### Existenzintervall
Das $I$ oben nennt man das **Lösungs- oder Existenzintervall** von $\lambda$ und $(2)$ die **Lösungsidentität**

#Mathe-IV 

[^1]: Satz 18.1.1