## Beschreibung
Die **holomorphe Wurzel** ist ist die Wurzel, definiert auf komplexe Zahlen

## Definition
Sei 
- $\emptyset \neq U \subseteq \mathbb{C} \backslash \{0\}$ ein [[Gebiet]]. 
- $\log: U \to \mathbb{C}$ ein [[Komplexe Logarithmusfunktion|Zweig des Logarithmus]]
- $b \in \mathbb{C}$

Dann heißt $\begin{array}{rrcl}z^b & U &\to &\mathbb{C} \\ & z & \mapsto & e^{b\log(z)}\end{array}$ ein **Zweig der b-ten Potenz auf $U$**[^1]


Sei 
- $\emptyset \neq U \subseteq \mathbb{C} \backslash \{0\}$ ein [[Gebiet]]
- $f: U \to \mathbb{C}$ eine nullstellenfreie, [[Analytische Funktion|holomorphe Funktion]].

Dann gibt 

Dann existiert für jedes $n \in \mathbb{N}$ eine holomorphe $n$-te Wurzel $g:U \to \mathbb{C} \backslash \{0\}$, sodass $(g(z))^n = f(z)$ für alle $z \in U$. [^1]

## Eigenschaften
Für $b \in \mathbb{Z}$ ist $z^b$ eindeutig. Für andere Werte aber nicht unbedingt[^2]

### Quotient zweier Wurzeln
Sei 
- $\emptyset \neq U \subseteq \mathbb{C} \backslash \{0\}$ ein [[Gebiet]].
- $g, h: U \to \mathbb{C}$ $n$-te Wurzeln von $f$.

Dann ist $\frac{g}{h}$ eine konstante Funktion, die nur die Werte $e^{\frac{2\pi i}{n}k} : k \in \{0, 1, ..., n-1\}$ annehmen kann.[^1]

### Wegintegral
Sei
- $S \subseteq \mathbb{C}\backslash [0, \infty[$ eine endliche Menge
- $f$ eine [[Rationale Funktion]], mit einem echt größeren Nennergrad.
Der Nenner von $f$ hat auf $\mathbb{R}$ keine Nullstelle
- Es sei $0 < Re(a) < 1$ Exponent einer [[Komplexe Potenz]]

Es sei $\begin{array}{rrcl}g: & \mathbb{C}\backslash ([0, \infty[ \cup S) & \to & \mathbb{C} \\ & z & \mapsto & f(z)z^{a-1} \end{array}$, dann gilt:

$$\int\limits_0^\infty f(t)t^{a-1} \, dt = - \frac{\pi e^{- i \pi a}}{\sin(\pi a)} \sum_{s \in S} Res(g, s)$$


#Mathe-IV 

[^1]: Zenk - Definition 23.3.7
[^2]: Zenk - Bemerkung 23.3.8 