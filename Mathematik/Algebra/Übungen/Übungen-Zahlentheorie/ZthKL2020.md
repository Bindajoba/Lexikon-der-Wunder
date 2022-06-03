TARGET DECK: Universität::Mathematik::Algebra

# Aufgabe 1
## a)
4

## b)
- Faktorielle Ringe
- Hauptidealringe
- Euklidische Ringe
- Körper

## c)
- ii
- iii

## d)
125

## e)
- i
- ii
- v

# Aufgabe 2
## a)
- $R$ ist ein Ring
Die Differenz von zwei Elementen liegt wieder in dem Ring
Das Produkt liegt wieder in dem Ring
Es hat $1 = \frac{1}{3^0}$ und $0 = \frac{0}{3^0}$-Element
- $R \subset \R$ offensichtlich
- $1$ ist in beiden Ringen gleich.

## b)
- $\subseteq:$ $\Z$ und $\frac{2}{3}$ liegen in $R$
- $\supseteq:$ Jedes Element aus $R$ ist aus $\Z$ und $\frac{2}{3}$ erzeugbar


# Aufgabe 3
## a)
Für $3 \in (3)$ und $\frac{1}{3^1}\in R$:
$3 \cdot \frac{1}{3^1} \in R$, d.h. $(1) \subseteq (3)$
$(1)$ ist das größte Ideal, also $(1) = (3)$.

## b)
$(5) \neq (1)$, denn dazur müsste $1 \in (5)$ aber es gibt kein $\alpha \in R$ mit $\alpha5 = \frac{5a}{3^n} \neq 1$, da Zähler und Nenner für alle $n \in \N_0$ nicht gleich sind. (da der Nenner nicht den Faktor $5$ enthält).

Ideale werden aus einer Menge erzeugt.
Angenommen, wir fügen zur erzeugenden Menge ein Element $\frac{a}{3^n}$ hinzu. D.h. $J = (\frac{a}{3^n}, 5)$
Dann ist auch $a = \frac{a}{3^n}\cdot 3^n\in 3^n$. gilt $ggT(a, 5) = 1$, dann ist $1 \in J$, also $J = (1)$.

Gilt $ggT(5, a) \neq 1 \implies ggT(5, a) = 5 \implies a$ ist Vielfaches von $5$. Dann gilt aber $a \in (5)$ und damit $\alpha \in (5) \implies J=(5)$.

Durch das hinzufügen von Elementen zur Erzeugermenge ergrößert man nicht das Ideal. Daher ist $(5)$ ein maximales Ideal.

# Aufgabe 4
## a)
$239$ ist eine Primzahl. $45$ hat damit ein multiplikatives Inverses.
Bestimme diesen indem $ggT(239, 45)$ mit dem euklidischen Algorithmus bestimmt wird.

| $s_i$ | $t_i$ | $r_i$ | $q_i$ |
| ----- | ----- | ----- | ----- |
| 1     | 0     | 239   |       |
| 0     | 1     | 45    |       |
| 1     | -5    | 14    | 5     |
| -3    | 16    | 3     | 3     |
| 13    | -69   | 2     | 4     |
| -16   | 85      | 1     | 1     |

Also $85*45-16*239 = 1$
$85$ ist damit das multiplikative Inverse modulo $239$.

## b)
$48 = 3 * 2^4$
$(\Z/48\Z)^\times = \Z/2\Z \times \Z/2\Z  \times \Z/4\Z$
Erster Schritt folgt aus dem Chinesischen Restsatz. Zweiter Schritt nach VL zu primer Restklassengruppe.

# Aufgabe 5

## a)
- $x^6 = x^3(x^3+2)-2x^3$
- $-2x^3 = -2(x^3+2)+4$

D.h. $x^6 \equiv 4 \mod (f)$
$\alpha^6 = x^6 + (f) = 4+(f) = 4(1+(f)) = 4\cdot 1_R$

## b)
$x^4 = x(x^3+2)-2x \implies x^4 \equiv -2x$
$\alpha^4+\alpha^2 = (x^4+x^2)+(f) = (x^2-2x)+(f)$

## c)
Das Polynom $x^3+2$ kann nach Satz über rationale Nullstellen nur die Nullstellen $\pm\frac{1}{2}$ aber das sind keine Nullstellen. Da das Polynom Grad $3$ hat, würde es als reduzibles Polynom in einen Linearfaktor zerfallen, wodurch eine Nullstelle in $\Q$ läge. Das kann aber wie oben gesagt nicht der Fall sein, also ist $f$ irreduzibel.

Sei $\beta$ eine Nullstelle von $f$. Da $f$ irreduzibel und normiert udn damit Minimalpolynom von $\beta$ ist, gilt nach VL die Isomrphie: $\Q[x] \cong \Q(\beta)$, es handelt sich also um einen Körper. (Da $\Q$ ein Körper.)


# Aufgabe 6 
Nutze den Euklidischen Algorithmus

| $s_i$ | $t_i$ | $r_i$ | $q_i$ |
| ----- | ----- | ----- | ----- |
| 1     | 0     | 41    |       |
| 0     | 1     | 37    |       |
| 1     | -1    | 4     | 1     |
| -9    | 10      | 1     | 9     |

Also $10*37-9*41 = 1$
Demnach gilt 
- $10*37 \equiv_{41} 1$
- $10*37 \equiv_{37} 0$
- $-9*41 \equiv_{37} 1$
- $-9*41 \equiv_{41} 0$

Die Zahl $23*10*37-21*9*41$ erfüllt die oberen Kongruenzen
$23*10*37-21*9*41 = 761$

$41*37 = 1517$. Damit erfüllt $761+1517 = 2278$ auch die oberen Kongruenzen.

# Aufgabe 7
## a)
Sei $h$ die Höhenfunktion aus der VL auf den Gaußschen Zahlen.
$h(4+i) = 16+1 = 17$. Die Primelemente der Gaußschen Zahlen sind genau die irreduzible Elemente. Wäre $4+i$ reduzibel, dann gäbe es zwei Nichteinheiten $a, b \in \Z[i]$ mit $h(4+i) = h(ab) = h(a)h(b) = 17$, wobei $h(a), h(b) > 1$. Aber $17$ ist eine Primzahl, die einzige Zerlegung ist daher $17 = 1*17$.
Somit ist $4+i$ irreduzibel und damit auch ein Primelement.

*Alternativ $h(4+i) = 17$ ist Primzahl, also ist $4+1$ nach VL irreduzibel*

Angenommen $7$ ist reduzibel, dann gilt $h(ab) = h(a)h(b) = h(7) = 49$. Die einzige Zerlegung von $49$ in Nichteinheiten ist $7*7 \implies h(a) = h(x+yi) = x^2+y^2= 7$. $7$ ist aber keine Summe von Quadraten, dazu kann man alle Möglichkeiten durchgehen, die kleinere Summen ergeben.
- $1^2+1^2 = 2$
- $1^2+2^2 = 5$
- $2^2+2^2 = 8$

keine $7$ mit dabei ):


$13 = (2+3i)(2-3i)$

## b)
$70 = 2*3*5 = -i(1+i)^2*3*(2+i)(2-i) = i(1+i)*(-2)*3*(2+i)(2-i)$

![[ZthKL2020.pdf]]
# Aufgabe 8
## a)
$\C[x]$ ist ein Polynomring eines Körpers und damit ein Hauptidealring, da sind die Primideale und die maximalen Ideale gleich.
In einem Hauptideal ist jedes Ideal durch ein Element erzeugbar. Für ein Primideal muss dieses Element ein Primelement sein. Desweiteren ist ein Hauptidealring ein Faktorieller Ring, d.h. die Primelemente sind genau die Irreduziblen Elemente.

Die irreduziblen Elemente in $\C[x]$ sind genau die irreuziblen Polynome. In $\C$ sind aber alle Polynome von Grad $>1$ reduzibel. Damit sind die Linearfaktoren alle irreduzibel.
Elemente $z \in \C$ bilden keine Maximalen Ideale, da alle kontanten Terme Einheiten sind und damit $(1)$ erzeugen.

Die irreduziblen Elmente bilden die Primideale $\{(ax+b):a, b \in \C\}$.

## b)
$p$ ist ein Primelement. D.h. $p \mid p^2 = q_1q_2 \implies p \mid q_1$ oder $p \mid q_2$. O.E wähle $p \mid q_1$
Da wir uns in einem Integritätsbereich aufhalten gilt die Kürzungsregel. $\implies p = \frac{q_1}{p}q_2$.
$p$ ist als Primelement in einem Integritätsbereich auch ein Irreduzibles Element. d.h. $p = \frac{q_1}{p}q_2 \implies p \mid \frac{q_1}{p}$ oder $p \mid q_2$.
Im ersten Fall hätte $q_1$ die Faktoren $p$ und $p$. $p$ ist als Primelement keine Einheit, d.h. $q_1$ hat eine Zerlegung in zwei Nichteinheiten.
Damit folgt $p \mid q_2$

Es gilt also $p \mid p_1$ und $p \mid q_2$.
Demnach gibt es ein $e_1, e_2$ mit $q_1 = e_1p$ und $q_2 = e_2p$.
Da $q_1, q_2$ irreduzibel sind, müssen $e_1, e_2$ Einheiten sein. Damit sind $q_1, q_2$ assoziiert zu $p$ und zu sich selbst. 

#Zahlentheorie 




