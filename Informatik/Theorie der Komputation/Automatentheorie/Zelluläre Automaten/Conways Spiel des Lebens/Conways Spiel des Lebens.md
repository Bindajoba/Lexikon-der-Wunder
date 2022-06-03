# Definition
Sei $G = (V, E)$ ein [[Ungerichteter Graph]] mit Knoten $V$ und Kanten $E \subseteq V \times V$.


Ein Zustand $x \in \mathcal{X}$ ist eine Abbildung der Knoten auf $\{tod, lebendig\}$
Zustände werden sich mit steigender Zeit verändern. Deshakb wird mit $x_t$ zwischen den Zeitpunkten unterschieden. 

Wir definieren die Anzahl der lebendigen Knoten um einen Knoten $v$ zu einem Zeitpunkt durch [[Nachbarschaft (Graphentheorie)]] $$|v|_{x_t} := \{w:w \in nachbarschaft(v) \land w_t(w) = lebendig\}$$

Die Evolution eines Zustandes $x_t$ in einen Zustand $x_{t+1}$ ist gegeben durch
$$x_{t+1}(v) = \begin{cases} 
	tot &\text{falls $|v|_{x_t} \leq 1$}, \\
	x_t(v) &\text{falls $|v_{x_t}| = 2$} \\
	lebendig &\text{falls $|v_{x_t}| = 3$} \\
	tot &\text{falls $|v_{x_t}| \geq 4$} 
	\end{cases}$$
für alle Knoten $v \in V$

# Strukturen
Bei Conways spiel des Lebens entstehen viele Interessante Strukturen:

## Still Lifes
Diese Verändern sich nicht
![[Stillleben.png]]

## Oscillators
![[Oscillator.png]]

## Spaceships
![[Spaceships.png]]

## Guns
Eine Gun kann Glider schießen.
![[Gun 1.png]]

## Turingmaschine
Mit dem Spiel des Lebens können sogar [[Turingmaschine|Turing Maschinen]] nachgebaut werden:
![](https://conwaylife.com/w/images/4/49/Turingmachine_large.png)

