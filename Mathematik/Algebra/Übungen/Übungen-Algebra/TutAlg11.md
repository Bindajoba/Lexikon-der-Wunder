![[blatt11.pdf]]]

# Aufgabe 0
## a)
$f$ zerfällt in Linearfaktoren. Der Zerfällungskörper wird von den Nullstellen des Polynoms erzeugt.
$\Q$ ist kein Zerfällungskörper von $x^2-3=(x-\sqrt 3)(x+\sqrt 3)$, $\sqrt 5$ ist keine Nullstelle.

## b)
Nein, man kann $K$-Linearfaktoren zu $f$ multiplizieren und die resultierende Funktion hat den gleichen Zerfällungskörper.

## c)
- Erweiterung $L|K$ ist algebraisch
- Körper $L$ ist alg. abgeschlossen (d.h., dass jedes $K$-Polynom mindestens eine Nullstelle in $L$ haben muss)

## d)
Der Körper $K^\times$ ist eine zyklische Gruppe der Ordnunf $p^n-1$.
$\implies \alpha^{p^n-1} = 1$ und $\alpha^{p^n} = \alpha$
$\implies \alpha^{p^n}-\alpha = \alpha-\alpha = 0$

## e)
$[K:P] = n$
Teilkörper $M$ von $K$ ist ein Zwischenkörper von $K|P$ und damit ein $P$-Vektorraum mit einer Dimension $d <\infty$
Dieser $P$-VR ist isomorph zu $P^d: |M| = |P|^d + p^d$.
$K$ als endl-dim- $M$-VR:
...

# Aufgabe 1
![[blatt11.pdf]]

## a)
Siehe [[Erweiterungsgrad]]
## b)
$L \to \mathbb{R}$
$x^7-5$ hat nur eine Reelle Nullstelle und nach dem Prinzip Nullstelle auf Nullstelle müssten alle Nullstellen von $f$ auf die einzige Reelle Nullstelle $\alpha$ abbilden. Damit wäre der Körperhomomorphismus nicht injektiv, was der Tatsache widerspricht, das diese es immer sind.
Somit gibt es keinen Homomorphimus.


$L \to \Q(\zeta)$
Da $[L:\Q] = [L:\Q(\zeta)]\cdot[\Q(\zeta):\Q] = [L:\Q(\zeta)] \cdot 6 = 42 \implies  [L:\Q(\zeta)] = 7$
Das Minimalpolynom von $\alpha$ hat also Grad 7.
$f$ ist normiert, hat $\alpha$ als Nullstelle und muss daher das Minimalpolynom in $\Q(\zeta)$ sein.
Ist $f$ irreduzibel, dann hat es keine Nullstellen in $\Q(\zeta)$.
Hätte es eine Nullstelle $n \in \Q(\zeta)$, dann könnte man per Polynomdivision. $f:(x-n)$ dividieren. Es kommt ein restloses Ergbnis zustande. Insbesondere sind die Koeffizienten wieder in $\Q(\zeta)$.
Somit wäre $f$ ein Produkt von zwei Polynomen und kann somit nicht irreduzibel sein (Widerspruch!)

Nach dem Prinzip Nullstellen auf Nullstellen muss die Nullstelle $\alpha \in L$ auf eine Nullstelle in $\Q(\zeta)$ abgebildet werden, was nicht möglich ist.

$L$

