
Seien $a_1, a_2 \in \mathbb{Z}$ und $a_2 \neq 0$. Dann terminiert die sukzessive Division mit Rest

$$\begin{align}a_1 &= q_1 a_2 + a_3 \\ 
a_2 &= q_2 a_3 + a_4 \\
\vdots\\
a_j &= q_j a_{j+1} + a_{j+2}\\
\vdots\\
a_{n-1} &= q_{n-1} a_{n} + 0
\end{align}$$
mit Rest $0$ und 
$$ggT(a_1, a_2) = a_n$$

**Ein Beispiel:**
$a_1 = 20$, $a_2=16$:
$$\begin{align}20 &= 1 \cdot 16 + 4 \\ 
16 &= 4 \cdot 4 + 0
\end{align}$$
d.h.
$$ggT(20, 16) = 4$$

**Beweis:**
*Terminierung*: Bei jeder Itereation wird $a_j$ echt kleiner, $a_n$ wird damit irgendwann null und terminiert.

*Ergebnis ist [[Teilbarkeit|Teiler]]*: Offensichtlich gilt $a_n | a_{n-1}$. $a_n$ teilt somit auch $a_{n-2} = q_{n-2}a_{n-1}+a_n$.
Dies lässt sich induktiv fortsetzen: $a_n$ teilt $a_1$ und $a_2$.

*Größter Teiler*: Ist $t$ ein von $a_1, a_2$, dann auch von $a_3 = a_1 - q_1a_2$ (Erhält man durch Umstellen der oberen Gleichungen).
Auch das lässt sich induktiv fortsetzen und $t$ ist ein Teiler von $a_n$. Die größte Zahl, die damit Teiler von $a_1$ und $a_2$ sein könnte, ist daher $a_n$, welche wie oben gezeigt ein Teiler von $a_1$ und $a_2$ ist.[^2]


[^2]: Böhm - Satz 2.3.2