## Beschreibung
Die **Ackermannfunktion** wurde von [[Wilhelm Ackermann]] erfunden. Es ist eine Funktion, die sehr schnell wächst.
Die Ackermannfunktion soll die Folge $x+y, x\cdot y, x^y, ...$ repräsentieren.[^1] Leider wird in der Informatik die "einfachere" Variation von Péter benutzt, bei der dieser Zusammenang nicht ersichtlich wird.

## Definition

Die Ackermannfunktion ist definiert durch:
$$a: \begin{array}{rcl}\mathbb{N}_0 \times \mathbb{N}_0 & \to & \mathbb{N}_0 \\
	(x,y) &\mapsto &\begin{cases} 
		y+1 & \text{falls } x=0\\
		a(x-1,1) & \text{falls } x \neq 0 \text{ und } y = 0\\
		a(x-1, a(x, y-1)) & \text{falls } x>0 \text{ und } y > 0\\
	\end{cases}
\end{array}$$

## Eigenschaften
### Totalität
Da erst der erste Paramater und dann der zweite Parameter immer kleiner wird, ist terminiert die Rekursion für alle Startwerte

### Berechenbarkeit
Die Ackermannfunktion ist [[WHILE-Berechenbarkeit|WHILE-berechenbar]] aber nicht [[LOOP-Berechenbarkeit|LOOP-berechenbar]]

### Monotonie
Die Ackermannfunktion erfüllt folgende Monotonie-Eigenschaften:
- $y < a(x, y)$
- $a(x, y) < a(x, y+1)$
- $a(x, y+1) \leq (x+1, y)$
- $a(x, y) < a(x+1, y)$
- Falls $x leq x'$ und $y \leq y'$, dann gilt auch $a(x, y) \leq a(x', y')$

#FSK 

[^1]: https://de.wikipedia.org/wiki/Ackermannfunktion 