# Beschreibung
Zelluläre Automaten sind Manschinen, bei denen das Verhalten einer Zelle im nächsten Zeitabschnitt durch seine lokale Umgebung bestimmt ist. 


# Definition
[[Conways Spiel des Lebens]] lässt sich zum Konzept des Zellulären Automaten verallgemeinern:
*Es ist nicht wirklich eine Verallgemeinerung, da hier die Knoten auf immer gleich viele Nachbarn beschränkt sind.*

Sei $G = (V, E)$ ein [[Ungerichteter Graph]] mit dem [[Graphengrad]] $d \in \N$.
Ein Zustand $x \in \mathcal{X}$ ist eine Abbildung von Knoten auf die Werte $\{0, 1\}$.
Sei $x_t$ ein [[Zustand (Zellulärer Automat)]] zum Zeitschritt $t \in \N$. The Entwicklung eines Zustands $x_t$ zum nachfolgenden Zustand $x_{t+1}$ ist [[Determinismus|deterministisch]] gegeben durch die Werte der [[Nachbarschaft (Graphentheorie)]] und
$$f: V^{d+1} \times \{0, 1\}^{d+1} \to \{0, 1\}$$
Der nachfolgende Zustand ist dann.
$$x_{x+1}(v) = f(\{(w, x_t(w): w\in nachbarschaft(v) \cup \{v\})\})$$
Ein Tupel $(G, f, x_S)$ wird **Zellulärer Automat** genannt mit Initialzustand $x_S \in \mathcal{X}$.

*Aus der Definition geht nicht hervor, wie zwischen Richtungen der Knoten unterschieden werden kann. Vielleicht geht das auch nur beim [[1D Zellulärer Automat]]*

# Klassifizierungen nach Wolfram
- Uniform (Uniformity)
- Repetetiv (Repetition)
- Zufällig (Random)
- Complex (Complexity)

![[Klassifizierung Automaten.png]]


# Beispiel
## Conways Spiel des Lebens
Siehe [[Conways Spiel des Lebens]]


# Vorkommen
![[Anwendung Schnecke.png]]



#Natural-Computing