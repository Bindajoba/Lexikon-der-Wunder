# Beschreibung
Dieser Artikel befasst sich mit den allgemeinen Polynomen.

Polynome sind ein stark untersuchtes Gebiet der Mathematik. Daher ist es kein Wunder, dass sie sich in vielen Bereichen wieder finden. Damit die Artikel nicht zu sehr aufschwellen, wird eine Unterteilung vorgenommen:
- [[Polynom (Komplexe Analysis)]]
- [[Polynom (Didaktik)]]
- [[Polynom (Ring, Körper)]]


# Definition
## Definition (Komplexitätstheorie)
Ein Polynom ist eine Funktion $p:\mathbb{N} \to \mathbb{N}$ der Form:
$$p(n)= \sum\limits_{i=0}^k {a_i \cdot nî} = a_kn^k + a_{k-1}n^{k-1} + ... + a_1n + a_0 $$

# Eigenschaften
Im folgenden werden einige Eigenschaften von Polynomen aufgelistet. Die meisten sind auch im Komplexen korrekt, stehen aber hier, weil sie auf reelle Zahlen anwendbar sind und damit für die Schule interessant sind.


## Summe der Nullstellen
Bei einem Polynom der Form
$$P_n(z)=a_nz^n + a_{n-1}z^{n-1} + \dots + a_1z + a_0$$
ist die Summe der [[Nullstelle|Nullstellen]] $-\frac{a_{n-1}}{a_n}$[^3]
 
## Produkt der Nullstellen
Bei einem Polynom der Form
$$P_n(z)=a_nz^n + a_{n-1}z^{n-1} + \dots + a_1z + a_0$$
ist das Produkt der [[Nullstelle|Nullstellen]] $-\frac{a_0}{a_n}$[^3]

## Satz über rationale Nullstellen
Sei $f(x) = a_nx^n+ ... + a_1x + a_0$ ein Polynom.
Hat $f$ eine (gekürzte), rationale Nullstelle $\frac{m}{n}$, dann gilt $n | a_n$ und $m|a_0$.

Damit kann überprüft werden, ob ein Polynom rationale Nullstellen besitzt. Wenn ja, können diese durch den Satz eingeschränkt werden.

Siehe [[Teilbarkeit]]


## Vereinfachte Form von Gleichungen
Jede Gleichung, welche nur aus Addition, Subtraktion, Multiplikation und Division besteht, kann als Lösung eines Polynoms umgeschrieben werden.

D.h. die Nullstellen des Polynoms sind genau die Lösungen der Gleichung.
*Das Lösen der Nullstellen, löst also alle Gleichungen mit den oberen Bedingungen.*

#Hadlock 

[^3]: https://www.mathsisfun.com/algebra/polynomials-sums-products-roots.html
 