TARGET DECK: Universität::Mathematik::Algebra

![[ZthKL2018.pdf]]

# Aufgabe 4
## c)
$x^6 = x^4(x^2+2)-2x^4$
$-2x^4 = -2x^2(x^2+2)+4x^4$
$4x^2 = 4(x^2+2)-8$

# Aufgabe 5
## a)
$48 = 2^4 * 3$
$(Z/48\Z)^\times = (Z/2\Z)^\times \times (Z/4\Z)^\times \times (Z/2\Z)^\times$

Siehe [[Prime Restklassengruppe]]

## b)
Nein, denn alle Elemente haben Ordnung 4.

# Aufgabe 6
## b)
Es ist kein [[Primideal]], da $5 = (2+i)(2-i)$ in Faktoren zerfällt, die nicht in $(5)$ liegen.

## c)
In einem Integritätsbereich sind alle Hauptideale eines Primelements Primideale.
Die Gaußschen Zahlen bilden nach VL einen euklidischen Ring und damit einen Hauptidealring. Da sind die Primelemente genau die irreduziblen Elemente.
$3$ ist irreduzibel. Wäre es in zwei Nichteinheiten aufteilbar $ab = 3$, dann wäre $9=h(3) = h(a)h(b)$, wobei $h(a), h(b)> 0$, da es keine Einheiten sind. Die einzige Faktorzerlegung von $9$ ist aber $3*3$, d.h. $h(a) = h(b)= 3$. Nach Definition der Höhenfunktion müsste $3$ eine Summe zweier Quadrate sein, also $x^2+y^2 = 3$. Aus $x^2 \leq 3$ folgt aber $x=1 \implies x^2=1 \implies y^2 = 2$. $2$ ist aber keine Quadratzahl.

# Aufgabe 7
## b)
Zeige $I+J = (1)$
Es gilt $-9 \in (3)$ und $5 = (2-i)(2+i) = -i(2+i)^2 \in(2+i)$
Damit $10-9 = 1 \in I+J$

| $t_i$ | $s_i$ | $r_i$ | $q_i$ |
| ----- | ----- | ----- | ----- |
| 1     | 0     | 3     |       |
| 0     | 1     | 2+i   |       |
| 1     | -1    | 1-i   | 1     |
| -i    | 1+i   | 1     | i     |
- $3 = 1(2+i) +(1 - i)$
- $2+i = i(1-i)+1$

Die beiden Zahlen sind also teilerfremd.

# Aufgabe 8
## b)
Ein Element in einem Integritätsbereich muss auch irreduzibel sein.
Angenommen $pq$ wäre prim, dann auch irreduzibel. Aber es hat eine Nichteinheitenzerlegung $pq$ (Prime Elemente sind keine Einheiten), ist also reduzibel.

## c)
$100 = 2^2*5^2 = -(1+i)^4(2+i)^2(2-i)^2$

$h(1+i) = 2$, eine Primzahl, also gibt es keine Zerlegung in zwei Nicht Einheiten $a, b$, sodass $h(ab) = h(a)h(b) = 2$

$h(2 \pm i) = 5$, eine Primzahl, also gibt es keine Zerlegung in zwei Nicht Einheiten $a, b$, sodass $h(ab) = h(a)h(b) = 5$

Die genannten Elemente sind damit irreduzibel. In einem faktoriellen Ring (und damit auch im gegebenen euklidischen Ring) sind [[Irreduzibles Element|irreduzible Elemente]] die [[Primelement|Primelemente]].


#Zahlentheorie 


