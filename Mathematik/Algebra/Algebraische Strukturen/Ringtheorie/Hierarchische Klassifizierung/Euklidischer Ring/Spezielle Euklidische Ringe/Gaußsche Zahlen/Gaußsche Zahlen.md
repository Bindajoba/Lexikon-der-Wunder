TARGET DECK: Universität::Mathematik::Algebra

# Beschreibung
Die Gaußschen Zahlen sind alle komplexen Zahlen, mit ganzzahligen imaginären/reellen Werten.


# Definition
Alle Zahlen der Form
$$\{a+bi: a, b, \in \Z\}$$

# Eigenschaften
Die Gaußschen Zahlen sind ein [[Euklidischer Ring]].

**Beweis nach Gerkmann**
Sei eine Höhenfunktion durch $h: x+iy \mapsto x^2+y^2$ gegeben. 
Zu zeigen sind zwei Voraussetzungen:
- Die Höhenfunktion ist für Werte $\neq 0$ ungleich $\in \N$ (offensichtlich)
- Für alle $\alpha, \beta \in \Z[i]$ gibt es eine Division mit Rest, d.h. ein $q, r \in \Z[i]$ mit $\alpha = q\beta+r$ und $h(r) < h(\alpha)$ oder $r=0$

Zweites ist erfüllt, wenn :
$r = 0$ oder $h(r) = h(\alpha-q\beta) < h(\beta)$
Dividiere $\alpha = a+bi$ und $\beta = c+di$ ganz normal.
$$\frac{\alpha}{\beta} = \frac{a+bi}{c+di} = \frac{(a+bi)(c-di)}{c^2+d^2} = \frac{ac+bd}{c^2+d^2}+i\frac{bc-ad}{c^2+d^2} =: t + is$$
$t, s$ sind rationale Zahlen. Runde zur nächsten ganzen Zahlen, und bezeichne sie mit $t_0, s_0$. Dann gilt $|t-t_0| \leq \frac{1}{2}, |s-s_0| \leq \frac{1}{2}$.
Setze nun $q = t_0 + is_0$.
Dann gilt $h(r) = h(\alpha-q\beta) = h(\beta)h((\frac{\alpha}{\beta}-q)) = h(\beta)h((t-t_0)+i(s-s_0))$$=h(\beta)((t-t_0)^2+(s-s_0)^2) \leq h(\beta) \frac{1}{2} \leq h(\beta)$

Alternativ kann man auch meinen Beweis verwenden:
$h(z)$ gibt in gewissem Maße den Betrag von $z$ zurück. Nicht wirklich, denn es fehlt noch eine Wurzel. Nichtsdestotrotz steigt $h(z)$ mit dem Betrag von $z$.

Versuche $\alpha = q\beta + r$ zu zeigen, indem man alle Werte $q\beta$ betrachtet und überprüft, ob es einen gibt, für den gilt $|\alpha-q\beta| < |\beta|$.
Versuche $q\beta$ zu visualisieren: $q\beta = (q_r+iq_i)\beta = q_r\beta + iq_i\beta$ also eine Summe aus einer ganzzahligen Skalierung von Beta und einer dazu senkrecht stehenden ganzzahligen Skalierung von $i\beta$.
Alle möglichen Punkte von $q\beta$ bilden ein Punktgitter auf den Komplexen Zahlenebene
![[Gaussche Zahlen Höhenfunktion.png]]
Der Wert $\alpha$ muss in einem dieser entstandenen Quadrate liegen. In jedem Quadrat gibt es immer einen Eckpunkt, der weniger weit als $|\beta|$ entfernt ist. Damit gilt $|\alpha-q\beta| < |\beta|$ und in Folge $h(\alpha-q\beta) < h(\beta)$.

# Übungen
## McEliece Aufgabe 3-6
### a)
Zeige, dass $1+i, 2+i, 3, 3+2i, 7$ [[Primelement|Primelemente]] sind.

Es gilt $h(ab)=h(a)h(b)$. Desweiteren $h(a) = 1$ genau dann wenn $a$ eine Einheit. Ist also $h(ab)$ eine Primzahl, dann muss $a$ ein Primelement sein.
- $h(1+i) = 2$
- $h(2+i) = 5$
- $h(3) = 9$, die einzige Zerlegung von $9$ ist $3\cdot 3$. Wenn $3$ kein Primelement ist, dann muss es Produkt von $a, b$ mit $h(a) = h(b) = 3$.
Die einzigen Elemente mit $h(a) \leq 3$ sind $0, 1, 1+i$ und ihre assoziierten Elemente.
- $h(3+2i) = 13$ ist Primzahl
- $h(7) = 49$ gleiches Argument wie bei $h(3)$

### b)
Zeige, dass $5, 13, 17$ keine Primelemente sind.
$$5 = (2+i) \cdot (2-i)$$$$13=(3+2i)\cdot(3+-2)$$$$17 = (4+i)(4-i)$$
## McEliece Aufgabe 3-8
Faktorisiere die folgenden Zahlen
- $8 = (1+i)^3(i-1)$
- $8+4i = (1+i)^2(1-i)^2(2+i)$
- $10=(1+i)(1-i)(2+i)(2-i)$
- $12 = (1+i)^2(1-i)^23$
- $45+3i = 3(15+i)$
$h(15+i) = 226 = 2 \cdot 113$
Wenn $15+i$ also teilbar ist, dann durch $1+i$. Tatsächlich, wir erhalten $15+i = (1+i)(8-7i)$.
- $60 = 12\cdot 5 = 3 \cdot 4 \cdot 5 = (1+i)^2(1-i)^23\cdot 5$

## Zth Klausur 2019 Aufgabe 6
### a)
$h(1+i) = 1^2+1^2 = 2$.
Die Höhenfunktion ist eine Funktion auf den Natürlichen Zahlen (für Werte nicht $0$).
Desweiteren gilt $h(ab) = h(a)h(b)$.
Wäre also $2$ in zwei Nicht-Einheiten zerlegbar, dann dürfte $h(1+i)=2$ nicht prim sein, was es aber ist.
Gleiches für $h(2+i)$ und $h(7) = 49$ muss einer Summe zweier Quadrate sein. Alle möglichen Summen durchzuprobieren geht ganz schnell.

### b)
$i$ ist in den Gaußschen Zahlen eine Einheit, denn $i * (-1) = 1$.
$1+i = i(1-i)$ und $1-i = -i(1+i)$

### c)
$35i = 5*7*i = (2+i)(2-i)7i$


#Zahlentheorie 


