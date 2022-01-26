## Beschreibung

Ein lineares Differentialgleichungssystem ist ein mehrdimensionales [[Differentialgleichung|Differentialgleichungssystem]], bei dem die Steigung der Variablen affin linear von den Werten aller Variablen abhängen.

Außerdem müssen die Variablen hier [[Reelle Zahlen|reell]] sein.
*Das ist im Allgemeinen nicht so, Herr Zenk ist in seinem Skript aber immer davon ausgegangen.*

Ein lineares Differentialgleichungssystem wird unterschiedlich behandelt, je nach dem ob es sich um ein Homogenes oder Inhomogenes Lineares Differentialgleichungssystem handelt.

Reelle Lineare Differentialgleichungsysteme sind Spezialfälle einer [[Explizite Differentialgleichung]]

## Definition Homogenes Lineares Differentialgleichungssystem
Seien
- $I \subseteq \mathbb{R}$
*$I$ ist der Definitionsbereich von $A_i$*
- $k \in \mathbb{N}$
*$k$ ist die Ordnung der DGL* 
- $A_i\in C(I, M_n(\mathbb{R}))$ eine [[Matrix|matrixwertige]] [[Stetigkeit|Stetige Funktion]] für $i \in \{0, ..., k-1\}$

Ein **n-Dimensionales Lineares Homogenes Differentialgleichungssystem k-ter Ordnung** hat die Form:
$$x^{(k)} = A_{k-1}(t)x^{(k-1)} + ... + A_1(t)x' \tag{1}$$

## Definition Inhomogenes Lineares Differentialgleichungssystem
Seien
- $I \subseteq \mathbb{R}$
*$I$ ist der Definitionsbereich von $A_i$*
- $k \in \mathbb{N}$
*$k$ ist die Ordnung der DGL* 
- $A_i\in C(I, M_n(\mathbb{R}))$ eine [[Matrix|matrixwertige]] [[Stetigkeit|Stetige Funktion]] für $i \in \{0, ..., k-1\}$
- $g\in C(I, M_n(\mathbb{R}))$ eine [[Matrix|matrixwertige]] [[Stetigkeit|Stetige Funktion]]

Ein **n-Dimensionales Lineares Inhomogenes Differentialgleichungssystem k-ter Ordnung** hat die Form:
$$x^{(k)} = A_{k-1}(t)x^{(k-1)} + ... + A_1(t)x' + g(t)$$

Wobei $g \neq 0$, sonst nennt man das DGL ein **Homogenes Lineares Differentialgleichungssystem**

## Strukturierung

| DGL                   | Eindimensional                                                                    | N-dimensional                                                                      |
| --------------------- | --------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------- |
| **Erste Ordnung**     | [[Skalare Lineare Differentialgleichung erster Ordnung\|Lin. DGL erster Ordnung]] | [[Lineares Differentialgleichungssystem erster Ordnung\|Lin. DGLS erster Ordnung]] | 
| **Beliebige Ordnung** | [[Skalare lineare Differentialgleichung\|Lin. DGL höherer Ordnung]]               | Lin. DGLS höherer Ordnung (also einfach lin. DGLS)                                 |

## Lösung
### Eindeutigkeit
Sei
- $I\subset \mathbb{R}$
- $A_i: I \to M_d(\mathbb{K})$
- $g: I \to \mathbb{K}$
 
Des linearen (In-)Homogenen Differentialgleichungssystems $$x^{(k)} = A_{k-1}(t)x^{(k-1)} + ... + A_1(t)x' + g(t)$$ zum [[Startwertproblem]] $x(\tau) = \xi$ hat eine eindeutige Lösung $\lambda_{(\tau, \xi)}: I \to \mathbb{R}^d$.[^1]

*Das folgt aus der Tatsache, dass solche Lösungen bei [[Lineares Differentialgleichungssystem erster Ordnung|Linearen (In-)Hmoogenen Gleichungssystemen]] erster Ordnung eindeutig sind, und sich die obere Gleichung in ein solches umwandeln lässt.*

### Umwandlung in Lineare Differentialgleichungssysteme erster Ordnung

Seien
- $I \subseteq \mathbb{R}$
*$I$ ist der Definitionsbereich von $A_i$*
- $k \in \mathbb{N}$
*$k$ ist die Ordnung der DGL* 
- $A_i\in C(I, M_n(\mathbb{R}))$ eine [[Matrix|matrixwertige]] [[Stetigkeit|Stetige Funktion]] für $i \in \{0, ..., k-1\}$

Eine **n-Dimensionales Lineares Homogenes Differentialgleichungssystem k-ter Ordnung**
$$x^{(k)} = A_{k-1}(t)x^{(k-1)} + ... + A_1(t)x' \tag{1}$$ kann in eine $nk$-dimensionales [[Lineares Differentialgleichungssystem erster Ordnung]] umgewandelt werden, indem:

Betrachte jede Ableitung von $x$ als eine eigene Variable:
$$\begin{array}{c} y_1 = x\\ y_2 = x' \\ \vdots \\ y_k = x^{(k-1)}  \end{array}$$ Dann gilt$$\begin{array}{c} y_1' = x' = y_2\\ y_2' = y_3 \\ \vdots \\ y_{k-1}' = y_{k} \\ y_k' = f(t, y_1, ..., y_k)  \end{array}\tag{2}$$ 

Eine gleiche Umwandlung gibt es auch bei ([[Explizite Differentialgleichung]])


## Eigenschaften


#Mathe-IV 

[^1]: FLD, Zenk: Satz 19.1.4 