# Lineares Differentialgleichungssystem erster Ordnung mit konstantem Koeffizietne
## Beschreibung
Ein **lineares homogenes Differentialgleichungssystem mit konstantem Koeffizieten** ist ein [[Lineares Differentialgleichungssystem erster Ordnung|lineares DGL erster Ordnung]] dessen Matrisxkoeffizient $A$ nicht von $t$ abhängt.


# Lineares Homogenes Differentialgleichungssystem erster Ordnung
## Beschreibung

Ein lineares homogenes Differentialgleichungssystem ist ein [[Reelle Zahlen|reelles]] [[Lineares Differentialgleichungssystem|lineares DGL]]  bei dem die Steigung der Variablen linear von den Werten aller Variablen abhängen.


## Definition
Sei $A \in M_d(\mathbb{K})$ eine $n$-dimensionale [[Matrix]].

Ein lineares homogenes Differentialgleichungssystem hat die Form:
$$x' = Ax \tag{1}$$


## Lösung
Sei $A\in M_d(\mathbb{K})$ eine Matrix. Die [[Fundamentalmatrix]] der Differentialgleichung $x' = Ax$ ist eindeutig, maximal und die [[Exponentialfunktion]] für Matrixwerte:

$$\lambda(t)=e^{tA}$$

Die Lösung, die das [[Startwertproblem]] $x(\tau) = \xi$ erfüllt ist:

$$\lambda_{(\tau, \xi)}(t) = e^{(t-\tau)A}\xi$$

## Stabilität
Ist eine Lösung [[Attraktivität|attraktiv]], dann ist sie auch [[Stabilität|stabil]] und damit [[Asymptotische Stabilität|asymptotisch stabil]].

Schreibe das charakteristische Polynom von $A$ in Nullstellenform.

$$\chi(t) = (-1)^k(\alpha_1-x)^{a_1}...(\alpha_m-x)^{a_m}$$ 

Alle Lösungen von $(1)$ sind genau dann [[Stabilität|stabil]], wenn
alle Eigenwerte die Bedingungen $Re(\alpha_i) \leq 0$ erfüllen oder im Fall $Re(\alpha_j) = 0$ die geometrische und algebraische Vielfachheit von $\alpha_j$ gleich sind. 


## Attraktivität
Schreibe das charakteristische Polynom von $A$ in Nullstellenform.

$$\chi(t) = (-1)^k(\alpha_1-x)^{a_1}...(\alpha_m-x)^{a_m}$$ 

Alle Lösungen von $(1)$ sind genau dann [[Attraktivität|attraktiv]], wenn alle Eigenwerte die Bedingungen $Re(\alpha_i) < 0$ erfüllen.

# Lineares Inhomogenes Differentialgleichungssystem erster Ordnung mit konstantem Koeffizienten
## Beschreibung
Ein **lineares inhomogenes Differentialgleichungssystem mit konstantem Koeffizieten** ist ein [[Lineares Differentialgleichungssystem erster Ordnung|lineares DGL erster Ordnung]] dessen Matrixkoeffizient $A$ nicht von $t$ abhängt.


## Definition
Seien
- $I \subseteq \mathbb{R}$
*$I$ ist der Definitionsbereich von $A$*
- $A\in M_d(\mathbb{R}))$ eine [[Matrix]]
- $g\in C(I, M_n(\mathbb{R}))$ eine [[Matrix|matrixwertige]] [[Stetigkeit|Stetige Funktion]]

Ein lineares Differentialgleichungssystem hat die Form:
$$x' = Ax + g(t) \tag{1}$$

wobei $g \neq 0$, sonst nennt man $(1)$ ein **Homogenes Differentialgleichungssystem erster Ordnung**

## Lösung
### Existenz und Eindeutigkeit
Die Lösung des linearen Differentialgleichungssystems $(1)$ zum [[Startwertproblem]] $x(\tau) = \xi$ ist eindeutig.[^1]

### Lösungsraum
Die Lösungen von $(1)$ bilden einen $n$-dimensionalen affinen Vektorraum
Das folgt aus der Eigenschaft, dass jede Lösung zu einem $n$-dimensionalen Startwert einzigartig ist
Diesen Raum nennt man einen Lösungsraum: $\text{Lös}_g	:= \{\varphi\in C^1(I, \mathbb{K}): \varphi \text{ löst } (1)\}$

Hat man eine Lösung $\varphi_g(t)$ von $(1)$ zu einem beliebigen Startpunkt gefunden, dann kann man den Lösungsraum $Lös_g$ berechnen. 
Dazu muss man $\varphi_g(t)$ zum Lösungsraum $\text{Lös}_0$ des **Lineares Homogenes Differentialgleichungssystem erster Ordnung** $$x' = Ax$$ addieren.

### Lösung mit Variation der Konstanten
Dieses Lösungsverfahren wird am beliebtesten angewendet:

Siehe ([[Variation der Konstanten]])


## Stabilität
Ist eine Lösung [[Attraktivität|attraktiv]], dann ist sie auch [[Stabilität|stabil]] und damit [[Asymptotische Stabilität|asymptotisch stabil]].

Ein lineares inhomogenes Differentialgleichungssystem $(1)$ ist genau dann [[Stabilität|stabil]], wenn die Nulllösung $$\nu: \begin{array} &]a, \infty[ &\to &\mathbb{K}^d\\
t &\mapsto &0\end{array}$$ des **Linearen Homogenen Differentialgleichungssystems erster Ordnung** $x' = A(t)x$ stabil ist.

## Attraktivität
Ein lineares inhomogenes Differentialgleichungssystem $(1)$ ist genau dann [[Attraktivität|attraktiv]], wenn die Nulllösung $$\nu: \begin{array} &]a, \infty[ &\to &\mathbb{K}^d\\
t &\mapsto &0\end{array}$$ des [[Lineares Differentialgleichungssystem erster Ordnung|linearen inhomogenen Differentialgleichungssystems]] $x' = A(t)x$ attraktiv ist.

#Mathe-IV

[^1]: FLD, Zenk: Satz 19.1.4
[^2]: FLD, Zenk: Satz 19.1.5 
[^3]: Zenk - Satz 19.1.4
[^4]: Zenk - Satz 19.2.8
[^5]: Zenk - Satz 19.4.6