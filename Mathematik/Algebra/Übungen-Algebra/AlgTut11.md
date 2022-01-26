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
Man erhält den Zerfällungskörper indem $\Q$ durch alle Nullstellen von $f$ in $\C$ adjungiert wird.
D.h. Der Zerfällungskörper ist $L := \Q(\sqrt[7]5 \zeta, \sqrt[7]5 \zeta^2, ..., \sqrt[7]5 \zeta^7)$.

Behauptung: $L= \Q(\sqrt[7]5, \zeta)$
$\subseteq:$ Offensichtlich lässt sich jeder Erzeuger aus $\sqrt[7]5$ und $\zeta$ erzeugen.
$\supseteq:$ Gebe alle Elemente des Erzeugers von $L$ als Kombination von $\{\sqrt[7]5 \zeta, \sqrt[7]5 \zeta^2, ..., \sqrt[7]5 \zeta^7\}$ an:
$\sqrt[7]5 = \sqrt[7]5\zeta^7$
$\zeta = \sqrt[7]{5}\zeta / \sqrt[7]5\zeta^7 = \sqrt[7]5\zeta / \sqrt[7]5 = \zeta$

Sei $\alpha = \sqrt[7]5$
Zu Zeigen: $[L:\Q] = .$
Da $\Q(\zeta)$ ein Zwischenkörper von $L|K$ ist gilt die Gradformel
$$[L:\Q] = [L:\Q(\zeta)]\cdot[\Q(\zeta):\Q]$$
Außerdem gilt:
$$[L:\Q] = [L:\Q(\alpha)]\cdot [\Q(\alpha):\Q]$$
Nach Angabe ist $[\Q(\zeta):\Q] = 6$
Da $f=\mu_{\Q, \alpha}$ Grad 7 hat, gilt $[\Q(\alpha): \Q] = 7$

Somit wird $[L:\Q]$ von $6$ und $7$ geteilt. $\implies [L:\Q]$ wird von $kgV(6, 7) =42$ geteilt.
$\implies [L:\Q] \geq 42$

Was ist $[L:\Q(\alpha)$?
Sei $g$ das Minimalpolynom von $\sqrt[7]5$ in $\Q(\zeta)$
- $f \in \Q(\zeta)[x]$ und $f(\alpha) = 0 \implies f|g \implies grad(g) \leq grad(f) = 7 \implies [L:\Q(\alpha)] \leq 7$ 
$[L:\Q] = [L:\Q] = [L:\Q(\zeta)]\cdot[\Q(\zeta):\Q] = [L:\Q] \leq 7\cdot6 = 42$

D.h. $L:\Q] = 42$

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

