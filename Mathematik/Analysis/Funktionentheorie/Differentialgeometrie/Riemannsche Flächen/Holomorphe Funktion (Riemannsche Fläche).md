## Beschreibung
Diese Art von Holomorphen Funktionen verallgemeinern die übliche [[Analytische Funktion|Holomorphe Funktion]]. 

Die neuen Holomophen Funktionen sind Funktionen die auf einer [[Riemannsche Fläche]] komplex differenzierbar sind.

## Definition
Es seien
- $X$ und $Y$ [[Riemannsche Fläche|Riemannsche Flächen]].
- $f:X \to Y$ eine [[Stetigkeit|stetige Abbildung]]

$f$ ist **holomorph**, wenn für jedes Paar von Karten $\varphi:U_X \to U_Y$ von $X$ und $\psi:U_Y \to V_Y$ von $Y$ mit $f(U_X) \subseteq U_Y$ die Abbildung
$$\psi \circ f \circ \varphi^{-1}:V_X \to V_Y$$ [[Analytische Funktion|holomorph]] ist.

### Biholomorphie
Siehe [[Biholomorphe Funktion]]

## Charaktierisierende Eigenschaften
### Charakterisierende Eigenschaft I
Es seien
- $X$ und $Y$ [[Riemannsche Fläche|Riemannsche Flächen]].
- $f:X \to Y$ eine [[Stetigkeit|stetige Abbildung]]

$f$ ist genau dann **holomorph**, wenn es für jedes $x \in X$ eine Karte $\varphi_x: U_x \to V_x$ um $x$ und eine Karte $\psi_{f(x)}: U_{f(x)} \to V_{f(x)}$ um $f(x)$ mit $f(U_x) \subseteq U_{f(x)}$ gibt, sodass$$\psi \circ f \circ \varphi^{-1}:V_X \to V_Y$$ [[Analytische Funktion|holomorph]] ist.


## Eigenschaften
### Offenheit
Ist $f: X \to Y$ **holomorph** und nicht konstant, dann ist $f$ eine [[Offene Abbildung]]

## Beispiele
### Meromorphe Erweiterung
Es sei 
- $\emptyset \neq U \subseteq \mathbb{C}$
- $f: U\backslash P(f) \to \mathbb{C}$ **meromorph**

Dann ist 
$$\hat{f}: \begin{array}{rcl} U &\to& \hat{\mathbb{C}} \\ 
z & \mapsto & \begin{cases} f(z) & \text{für } z \in U \backslash P(f) \\ \infty & \text{für } z\in P(f) \end{cases}\end{array}$$

eine **holomorphe Funktion**, wenn man $U$ und $\hat{\mathbb{C}}$ als Riemannsche Flächen auffasst.[^1]

[^1]: Zenk - Lemma 24.3.5


#Mathe-IV 