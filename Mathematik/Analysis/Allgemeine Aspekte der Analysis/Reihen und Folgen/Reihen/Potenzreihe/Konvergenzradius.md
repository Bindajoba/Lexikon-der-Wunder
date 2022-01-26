## Definition
Es sei 
- $(X, ||\cdot||)$ ein $\mathbb{C}$-[[Banachraum]]
- $a \in \mathbb{C}$
- $(c_n)_{n\in \mathbb{N}_0}$ eine [[Folge]] in X

Sei $\sum\limits_{n=0}^\infty c_n(z-a)^n$ eine [[Potenzreihe]] zum **Entwicklungspunkt** $a$

Ist $L:=\underset{n\to \infty}{\overline{\lim}} \sqrt[n]{||c_n||}$, dann heißt 
$$\rho := \begin{cases} 0 & \text{falls } L = \infty \\ \frac{1}{L} &\text{falls } L \in ]0, \infty[ \\ \infty & \text{falls } L = 0 \end{cases}$$ der **Konvergenzradius** von der Potenzreihe.[^1]

## Eigenschaften
### Konvergenz
Die [[Potenzreihe]] $\sum\limits_{n=0}^\infty c_n(z-a)^n$ ist für alle $z \in \mathbb{C}$
- mit $|z-a| < \rho$ [[Absolute Konvergenz|absolut konvergent]]
- mit $|z-a| > \rho$ divergent[^2]

## Sätze
### Quotientenkriterium
Siehe [[Quotientenkriterium]]

### Wurzelkriterium


#Mathe-I 

[^1]: Zenk - Definition 6.3.1
[^2]: Zenk - Satz 6.3.3