# Beschreibung
Der euklidische Algorithmus ist ein Algorithmus, um den [[Größter Gemeinsamer Teiler]] von zwei Zahlen zu bekommen. Er wurde anfangs von Euklid formuliert: Ziehe solange die kleinere Zahl von der größeren Zahl ab, bis zwei gleiche Zahlen übrigbleiben. Das ist der ggT.
Sei der Antike gab es aber einige Weiterentwicklungen und Verallgemeinerungen.


# Definition
## Einfacher Euklidischer Algorithums
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

## Verbesserter Algorithmus
Um die Linearkombination nicht durch mühsames und fehlerbehaftetes Rückrechnen zu erhalten, fügenn wir zwei neue Variablen $s_i, t_i$ hinzu, die die Skalare der Linearkombination geben.

Erläre en Algorithmus exemplarisch an diesem Beispiel. $ggT(a, b) = ggT(15, 35)$

| $i$  | $s_i$ | $t_i$ | $r_i$ | $q_i$ |
| ---- | ----- | ----- | ----- | ----- |
| $-1$ | $1$   | $0$     | $35$  | $-$   |
| $0$  | $0$   | $1$   | $15$  | $-$   |
| $1$  | $1$   | $-2$  | $5$  | $2$   |
| $2$  | $-3$  |  $7$     |  $0$     |  $3$     |

Das $r_i$, vor dem $r_i$, welches $0$ ist, gibt die richtige Lösung.

Die $s_i, t_i$ sind die Faktoren einer Linearkombination von $a, b$, mit $r_i$ als Ergebnis. D.h.
$$s_ia+t_ib=r_i$$
Daher ist es notwendig, dass die Werte in der ersten Zeile $1, 0$ und $0, 1$ sind.
In der vorletzen Zeile kann man damit die Linearkombination des $ggT(a, b)$ ablesen.

$s_i$ wird folgendermaßen berechnet:
$$s_{i} = s_{i-2} - s_{i-1}q_i$$
Im oberen Beispiel also zum Beispiel:
$$s_2 = s_{0}-s_{1}q_2 = 0-(1\cdot3) = -3$$
$t_i$ wird eigentlich genauso errechnet.
$$t_{i} = t_{i-2} - t_{i-1}q_i$$

# Übungen
## McEliece Aufgabe 2-5
Durch den Euklidischen Algorithmus erhält man ein Zahlenpaar $s, t$, sodass $ggT(a, b) = sa +tb$.
Dieses Zahlenpaar ist aber nicht eindeutig. Wie findet man alle Zahlenpaare?

Gesucht ist ein paar $x, y$, sodass $ggT(a, b) = ax + by$. Das ist eine Geradengleichung! Umstellen ergibt:
$$y = \frac{ggT(a, b)-ax}{b} =: f(x)$$
Die Punkte mit ganzzahligen Werten, durch die die Gerade verläuft sind genau die gesuchten Punkte. Wir kennen bereits das ganzzahlige Paar $(s, t) = (s, f(s))$.
Die Gerade hat eine Steigung von $-\frac{a}{b}$, kürzen wir den Bruch vollständig, dann $-\frac{a/ggT(a, b)}{b/ggT(a, b)}$. Nur alle $b/ggT(a, b)$ Schritte erhalten wir ein neues Paar. Die möglichen Paare sind damit $(s + n(b/ggT(a, b)), t)$

## McEliece Aufgabe 2-8
Zeige folgende Eigenschaften des euklidischen Algorithmus
1. $t_ir_{i-1}-t_{i-1}r_i = (-1)^ia$
2. $s_ir_{i-1}-s_{i-1}r_i = (-1)^ib$
3. $s_it_{i-1}-s_{i-1}t_i = (-1)^{i+1}$
4. $s_ia + t_ib = r_i$

### Teilaufgabe 1
Zeige mit vollständiger Induktion:
Induktionsanfang $(i = 0)$:
$$t_0r{-1}+t_{-1}r_0 = 0 + a = (-1)^0a$$
Induktionsschritt, zeige für $i+1$:
$$t_{i+1}r_{i}-t_{i}r_{i+1} = (t_{i-1}-t_iq_{i+1})r_{i}-t_{i}(r_{i-1}-q_{i+1}r_i) = t_{i-1}r_i-t_ir_{i-1} = (-1)(-1)^ia = (-1)^{i+1}a$$

### Teilaufgabe 2
Vermutlich genauso wie Teilaufgabe 1.

### Teilaufgabe 3
Zeige mit vollständiger Induktion:
Induktionsanfang $(i = 0)$:
$$s_it_{i-1}-s_{i-1}t_i = 0-1 = (-1)^1$$
Induktionsschritt, zeige für $i+1$:
$$s_{i+1}t_{i}-s_{i}t_{i+1} = (s_{i-1}-s_iq_{i+1})t_{i}-s_{i}(t_{i-1}-t_iq_{i+1}) = s_{i-1}t_i-s_it_{i-1} = (-1)(-1)^{i+1} = (-1)^{i+2}$$

### Teilaufgabe 4
Ich denke, man kann einfach das Ergebnis aus 1 und 2 einsetzen.
$$s_ia+t_ib = (-1)^i(s_i(t_ir_{i-1}-t_{i-1}r_i)+t_i(s_ir_{i-1}-s_{i-1}r_i))$$

## Zth Klausur 2018 Aufgabe 3
![[Zth Klausur 2018 Aufgabe 3.png]]
### a)
| $s_i$ | $t_i$ | $r_i$ | $q_i$ |
| ----- | ----- | ----- | ----- |
| 1     | 0     | 137   |       |
| 0     | 1     | 64    |       |
| 1     | -2    | 9     | 2     |
| -7    | +15      | 1     | 7     |

$1 = -7*137+15*64$

### b)
$1 = -7*137+15*64 \implies 15*64 = 1 + 7*137 \implies 15*64 \equiv_{137} 1$
Es ist eine Einheit, da es das Inverse $15$ besitzt.
$64^{-2} = (64^{-1})^2 = 15^2 = 225 = 88$





[^2]: Böhm - Satz 2.3.2


#Böhm #Zahlentheorie #McEliece 