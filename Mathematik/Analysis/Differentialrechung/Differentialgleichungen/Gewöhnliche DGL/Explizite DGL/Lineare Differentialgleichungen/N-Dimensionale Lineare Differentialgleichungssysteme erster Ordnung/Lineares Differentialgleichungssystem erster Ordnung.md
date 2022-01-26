# Lineares Differentialgleichungssystem erster Ordnung
## Beschreibung
Ein lineares homogenes Differentialgleichungssystem ist ein [[Reelle Zahlen|reelles]] [[Lineares Differentialgleichungssystem|lineares DGL]]  bei dem die Steigung der Variablen linear oder affin linear von den Werten aller Variablen abhängen.

Ein lineares homogenes Differentialgleichungssystem ist ein **[[Reelles Lineares Differentialgleichungssystem]] erster Ordnung**.

Es ist die Verallgemeinerung einer [[Lineares Differentialgleichungssystem erster Ordnung mit konstantem Koeffizienten]]

# Lineares Homogenes Differentialgleichungssystem erster Ordnung
## Beschreibung

Ein lineares homogenes Differentialgleichungssystem ist ein [[Reelle Zahlen|reelles]] [[Lineares Differentialgleichungssystem|lineares DGL]]  bei dem die Steigung der Variablen linear von den Werten aller Variablen abhängen.


## Definition
Sei $A: I \to M_n(\mathbb{K})$ eine $n$-dimensionale matrixwertige Funktion.

Ein lineares homogenes Differentialgleichungssystem hat die Form:
$$x' = A(t)x \tag{1}$$

wobei $A(t)$ eine reelle Matrix-Funktion ist.

## Lösung

Die Lösung des DGL $(1)$ zum [[Startwertproblem]] $x(\tau)=\xi$ ist
$$\Phi(t-\tau)\xi$$ wobei $\Phi(t)$ die [[Fundamentalmatrix]] von $(1)$ ist.

### Eindeutigkeit
Sei
- $I\subset \mathbb{R}$
- $A_i: I \to M_d(\mathbb{K})$
- $g: I \to \mathbb{K}$
 
Das linearen (In-)Homogenen Differentialgleichungssystems $$x^{(k)} = A_{k-1}(t)x^{(k-1)} + ... + A_1(t)x' + g(t)$$ zum [[Startwertproblem]] $x(\tau) = \xi$ hat eine eindeutige maximale Lösung $\lambda_{(\tau, \xi)}: I \to \mathbb{R}^d$.[^3]


## Stabilität
Ist eine Lösung [[Attraktivität|attraktiv]], dann ist sie auch [[Stabilität|stabil]] und damit [[Asymptotische Stabilität|asymptotisch stabil]].

Sei $\Lambda$ die [[Übergangsmatrix]] von $(1)$.
Dann sind alle Lösungen von $(1)$ genau dann [[Stabilität|stabil]], wenn es für ein $T_0 > a$ ein $\beta > 0$ gibt mit
$$\underset{t\geq \tau}{\sup} ||\Lambda(t, T_0)|| < \beta$$

## Attraktivität
Sei $\Lambda$ die [[Übergangsmatrix]] von $(1)$.
Dann sind alle Lösungen von $(1)$ genau dann [[Attraktivität|attraktiv]], wenn für ein $T_0 > a$ 
$$\underset{t \to \infty}{\lim} ||\Lambda(t, T_0)|| = 0$$


# Lineares Inhomogenes Differentialgleichungssystem erster Ordnung
## Beschreibung
Ein **n-dimensionales lineares inhomogenes Differentialgleichungssystem erster Ordnung** ist ein mehrdimensionales [[Differentialgleichung|Differentialgleichungssystem]], bei dem die **k-te Ableitung** der Variablen affin linear von den Werten und niedrigerer Ableitungen aller Variablen abhängen.

## Definition
Seien
- $I \subseteq \mathbb{R}$
*$I$ ist der Definitionsbereich von $A$*
- $A\in C(I, M_n(\mathbb{R}))$ eine [[Matrix|matrixwertige]] [[Stetigkeit|Stetige Funktion]]
- $g\in C(I, M_n(\mathbb{R}))$ eine [[Matrix|matrixwertige]] [[Stetigkeit|Stetige Funktion]]

Ein lineares Differentialgleichungssystem hat die Form:
$$x' = A(t)x + g(t) \tag{1}$$

wobei $g \neq 0$, sonst nennt man $(1)$ ein **Homogenes Differentialgleichungssystem erster Ordnung**

## Lösung
### Existenz und Eindeutigkeit
Die Lösung des linearen Differentialgleichungssystems $(1)$ zum [[Startwertproblem]] $x(\tau) = \xi$ ist eindeutig.[^1]
### Lösungsraum

Die Lösungen von $(1)$ bilden einen $n$-dimensionalen affinen Vektorraum
Das folgt aus der Eigenschaft, dass jede Lösung zu einem $n$-dimensionalen Startwert einzigartig ist
Diesen Raum nennt man einen Lösungsraum: $\text{Lös}_g	:= \{\varphi\in C^1(I, \mathbb{K}): \varphi \text{ löst } (1)\}$

Hat man eine Lösung $\varphi_g(t)$ von $(1)$ zu einem beliebigen Startpunkt gefunden, dann kann man den Lösungsraum $Lös_g$ berechnen. 
Dazu muss man $\varphi_g(t)$ zum Lösungsraum $\text{Lös}_0$ des **Lineares Homogenes Differentialgleichungssystem erster Ordnung** $$x' = A(t)x$$ addieren.

### Lösung mit Variation der Konstanten
Siehe ([[Variation der Konstanten]])


### Lösung mit Fundamentallösung
Die Lösung des DGL $(1)$ zum [[Startwertproblem]] $x(\tau)=\xi$ ist gegeben durch:

$$\lambda_{(\tau, \xi)} = Y(t)\xi+Y(t)\int\limits_\tau^t{Y(s)^{-1}g(s) \,ds}$$wobei $Y(t)$ die [[Lineare Homogene MatrixDGL|Matrix-DGL]] $Y'(t) = A(t)Y(t)$ ist.

Merke: Diese Methode ist sehr kompliziert.

### A(t) ist konstant oder nilpotent oder so
Sei $A\in M_d(\mathbb{K})$ eine Matrix. Die globale Lösung der DGL $x' = Ax + g(t)$ zum  [[Startwertproblem]] $x(\tau) = \xi$ errechnet sich durch:

$$\lambda_{(\tau, \xi)}(t)=e^{tA}\xi+\left(\frac{e^{tA}-1}{A}\right)g(t)$$ dabei ist $$\frac{e^{tA}-1}{A} = \sum\limits_{n=0}^\infty \frac{t^{n+1}}{(n+1)!}A^n$$[^4]

*Diese Lösungsmethode ist vermutlich sinnvoll, wenn man mit nilpotenten Matrizen zu tun hat oder wenn man sehr wenig Lust auf Integrieren hat. Normalerweise nutzt man einfach Variation der Konstanten*

## Stabilität
Ein lineares inhomogenes Differentialgleichungssystem $(1)$ ist genau dann [[Stabilität|stabil]], wenn die Nulllösung $$\nu: \begin{array} &]a, \infty[ &\to &\mathbb{K}^d\\
t &\mapsto &0\end{array}$$ des **Lineares Homogenes Differentialgleichungssystem erster Ordnung** $x' = A(t)x$ stabil ist.

## Attraktivität
Ein lineares inhomogenes Differentialgleichungssystem $(1)$ ist genau dann [[Attraktivität|attraktiv]], wenn die Nulllösung $$\nu: \begin{array} &]a, \infty[ &\to &\mathbb{K}^d\\
t &\mapsto &0\end{array}$$ des [[Lineares Differentialgleichungssystem erster Ordnung|linearen inhomogenen Differentialgleichungssystems]] $x' = A(t)x$ attraktiv ist.

#Mathe-IV

[^1]: FLD, Zenk: Satz 19.1.4
[^2]: FLD, Zenk: Satz 19.1.5 
[^3]: Zenk - Satz 19.1.4
[^4]: Zenk - Satz 19.2.8
[^5]: Zenk - Satz 19.4.6