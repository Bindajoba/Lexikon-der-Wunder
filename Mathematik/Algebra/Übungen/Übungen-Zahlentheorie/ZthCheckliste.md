TARGET DECK: Universität::Mathematik::Algebra

# Aufgabe 1
Was sind die [[Einheit|Einheiten]] der [[Ring]] $\Z, \Q, \Z/4\Z, \Z/5\Z, \Q[x]$?
- $\{1\}$
- $\Q\backslash \{0\}$
- $\{\overline 1\}$
- $\{\overline 1, 3\}$
- $\{1, 2, 3, 4\}$
- $\Q\backslash \{0\}$

# Aufgabe 2
Welche Beispiele für Ringe gibt es, die keine [[Integritätsbereich|Integritätsbereiche]] sind?
- $\Z/n\Z, n$ keine Primzahl
- $\Z/p_1\Z \times \Z/p_2\Z$
- $\Z \times \Z$
- Nullringe

Nullringe sind meiner Meinung nach schon Integritätsbereiche, denn die $0$ ist das einzige Element.

# Aufgabe 3
Warum gibt es für jeden Ring genau einen [[Ringhomormorphismus]] $\Z \to R$
Die $1$ muss auf die $1$ abbilden. Durch das Bild der $1$ ist der gesamte Ringhomomorphismus bestimmt.

# Aufgabe 4
Was ist über den [[Kern (Ring)]] eines Körperhomormophismus bekannt?
Ein [[Körperhomomorphismus]] ist injektiv. Desweiteren muss er die $0$ auf die $0$ abbilden. Damit ist der Kern immer $\{0\}$

# Aufgabe 5
Gibt es für jedes $n \in \N$ einen Ring der Charakteristik $n$? Ist es möglich, dass $R$ ein Integritätsbereich ist aber $char(R)  \neq 0$ gilt?
1. Ja, $\Z/n\Z$ ist ein Ring mit Charakteristik $n$.
2. Die Ringe $\Z/p\Z$ sind [[Integritätsbereich|integritätsbereiche]], haben aber [[Charakteristik (Ring)]] $p$.

# Aufgabe 6
Was ist die Form der Elemente eines [[Erzeugter Teilring|erzeugten Teilrings]] $R[c]$?
Sie haben die Form $\{a_0+a_ac+a_2c^2+...:a_0, ... \in R\}$.

# Aufgabe 7
Wenn $K$ ein [[Körper]] ist, was ist dann sein [[Quotientenkörper]]?
Natürlich wieder $K$! Alle Quotienten zweier Elemente von $K$ liegen schon in $K$.

# Aufgabe 8
Was sind die zu $7+5i$ [[Assoziierte Elemente]] im Ring der [[Gaußsche Zahlen|Gaußschen Zahlen]]
$7+5i$ mal $i, -1, -i$

# Aufgabe 9
Inwieweit ist der [[Größter Gemeinsamer Teiler|größte gemeinsame Teiler]] von Elementen in einem Integritätsbereich eindeutig bestimmt?
Sei $A$ eine Menge von Elementen.
Hat man einen $ggT(A)$ gegeben, dann sind die anderen die dazu assoziierten Elemente.

Aber was hat das mit Integritätsbereichen zu tun?
Versuche den $ggT$ von zwei Zahlen im Nicht-Integritätsbereich $R = \Z/4\Z$ zu finden. Stelle das durch eine Verknüpfungstabelle dar.

| *   | 0   | 1   | 2   | 3   |
| --- | --- | --- | --- | --- |
| 0   | 0   | 1   | 2   | 3   |
| 1   | 1   | 1   | 1   | 1   |
| 2   | 1   | 1   | 2   | 1   |
| 3   | 1   | 2   | 1   | 3    |

- Was ist $ggT(0, 0)$?
Die Zahl $a$, die $0$ und $0$ teilt und die von allen anderen Teilern geteilt wird.
Teiler von $0$: $0$ hat die Teiler $\{0, 1, 2, 3\}$, denn für $a \in \{0, 1, 2, 3\}: 0 = 0*a$
Aber nur $0$ wird von allen Zahlen geteilt.
- Was ist $ggT(2, 0)$
$0$ hat die Teiler $\{0, 1, 2, 3\}$, denn für $a \in \{0, 1, 2, 3\}: 0 = 0*a$
$2$ hat die Teiler $\{1, 2\}$
Die Zahl, die von allen gemeinsamen Teilern $\{1, 2\}$ geteilt wird ist $2$.

Das Problem mit Integritätsbereichen ist wahrscheinlich, dass die assoziierten Elemente sich nicht durch eine EInheit unterscheiden.

Probieren wir $\Z^2$. Oben hatten wir mit $ggT(0, 2) = 2$ kein Glück. Aber was ist, wenn wir uns etwas anderes ausdenken?
Was ist $ggT((1, 0), (0, 1), (0, 0))$? Vermutlich $1$

# Aufgabe 10
Welche Beispiele für [[Euklidischer Ring|euklidische Ringe]] sind bekannt?
- Polynomringe von Körpern
- $\Z$
- $\Z[i]$
- $\Z[\sqrt2]$
- Körper

# Aufgabe 11
Renn $R$ ein Ring und $a, b \in R$ sind, was sind die Elemente es [[Hauptideal|Hauptideals]] $(a)$? Wie sehen die Elemente von $(a, b)$ aus?
$$(a) = \{ra: r \in R\}$$
$$(a, b) = \{r_1a+r_2b: r\in R\}$$

# Aufgabe 12
In jedem Ring gibt es ein größtes und ein kleinstes Ideal. Gebe diese an:
- $(1), (0)$

# Aufgabe 13
Wie ist das [[Produktideal]] definiert?
$$IJ = \{ab: a \in I, b\in J\}$$

# Aufgabe 14
Wie begründet man im Ring $\Z[i]$ $I=(2+i, 3+i) = (1)$
$2+i, 3+i \in I \implies (3+i)-(2+i) = 1 \in I \implies (1) \subseteq I$. Da aber $(1)$ das größte Ideal folgt $I = (1)$ 


# Aufgabe 15
Zeige, durch überprüfen der definierenden Eigenschaft, dass $(7)$ in $\Z$ ein [[Primideal]] und auch ein [[Maximales Ideal]] ist. Zeige, dass $(8)$ weder Prim noch maximales Ideal ist.

$(7)$ ist ein Primideal, wenn für ein $ab \in (7)$ gilt $a \in (7)$ oder $b \in (7)$.  
$(7)= \{7n:n \in \Z\}$. Da $7$ eine Primzahl und damit Primelement in $\Z$ ist, gilt für $7n = ab$. $7 \mid a$ oder $7 \mid b$. Damit gilt auch $a \in (7)$ oder $b \in (7)$.

$(7)$ ist ein maximales Ideal.
Angenommen, man würde ein Element $a$ zum Erzeuger hinzufügen. Dann ist dieses Element entweder ein Vielfaches von $7$ oder nicht. Im ersten Fall gilt $a \in (7)$ also $(7) = (7, a)$.
Im zweiten Fall ist $ggT(7, a) = 1$ (da $7$ Primzahl und daher irreduzibel) und damit gilt $(7, a) = (1)$.

$(8)$ ist kein Primideal, denn es gilt $2*4 = 8$ aber $2, 4 \notin 8$.
$(8)$ ist kein Maximales Ideal, denn $(8)\subset (2) \subset (1)$.

# Aufgabe 16
Sei $R$ ein Ring, $a, b \in R$. Welche Bedingungen sind zur Gleichung $a+I = b+I$ äquivalent?
$a+I = b+I \iff (a-b)+I = I \implies (a-b) \in I \iff a \equiv b \mod I \iff (a-b) \equiv 0 \mod I$.

# Aufgabe 17
Gibt es ein Ideal $I$ mit der Eigenschaft, dass $a+I = b+I \iff a=b$ für alle $a, b \in R$ gilt? 
Ist es möglich, dass $a+I = b+I$ für alle $a, b \in R$ gilt? Falls ja, was ist $I$ dann für ein Ideal?
- Ja, das Ideal $(0)$ hat eine solche Eigenschaft
- Ja, das Ideal $(1)$ hat eine solche Eigenschaft

# Aufgabe 18
Gebe zwei verschiedene [[Repräsentantensystem (Nebenklassen von Ringen)|Repräsentantensysteme]] von $\Z/5\Z$ an.
$\{0, 1, 2, 3, 4\}$ oder $\{2, 3, 4, 5, 6\}$

# Aufgabe 19
Was kann über das [[Ideal]] $I$ gesagt werde, wenn der Faktorring $R/I$ ein [[Integritätsbereich]] bzw. ein Körper ist.
1. Das Ideal ist ein Primideal
2. Das Ideal ist ein Maximales Ideal

# Aufgabe 20
Was hat die [[Teilerfremdheit (Ideal)|Teilerfremdheit]] von [[Ideal|Idealen]] mit der [[Teilerfremdheit (Ring)|Teilerfremdheit]] von ganzen Zahlen zu tun?

Zwei Ideale $I, J$ sind Teilerfremd, wenn $I+J = (1)$
Zwei Hauptideale sind teilerfremd, wenn die erzeugenden Zahlen teilerfremd sind.
Enthalten die Ideale $I, J$ zueinander teilerfremde Zahlen, dann ist $I+J$ auch teilerfremd.
Sind $I, J$ teilerfremd, dann enthält $I+J$ sie zueinander teilerfremde Zahlen.

# Aufgabe 21
Gibt es ein $a \in \Z$ mit $a \equiv_{49} 3$ und $a \equiv_{50} 7$? Ja, da die moduli teilerfremd sind.
Gibt es ein $a \in \Z$ mit $a \equiv_{49} 3$ und $a \equiv_{56} 4$? Muss nicht sein, da $49$ und $56$ nicht teilerfremd sind.

Ein $a \in \Z$ mit $a \equiv_{49} 3$ erfüllt auch $a \equiv_7 3$
Ein $a \in \Z$ mit $a \equiv_{56} 4$ erfüllt auch $a \equiv_7 4$
Also kann es kein solches $a$ geben.

# Aufgabe 22
Wenn $R$ ein Integritätsbereich bzw. ein Körper ist, wie sieht die [[Einheitengruppe]] $(R[x])^\times$ des [[Polynomring|Polynomrings]] über $R$ aus?

- Integritätsbereich $(R[x])^\times = R^\times$
- Körper: $(R[x])^\times = R^\times = R\backslash \{0\}$

# Aufgabe 23
Welche Einschränkung muss man an den Grad eines Polynoms $f \in K[x]$ über einem Körper $K$ machen, damit aus der Nicht-Existenz von Nullstellen in $K$ die Irreduzibilität von $f$ in $K[x]$ folgt?
Der Grad muss $\leq 3$ sein.

Beispiel: $(x^2+1)(x^2+2)$

# Aufgabe 24
Wenn $R$ ein [[Faktorieller Ring]] und $K$ sein Quotientenkörper ist, kann es passieren, dass ein Polynom $f \in R[x]$ im Polynomring $K[x]$ aber nicht in $R[x]$ irreduzibel ist? Kann die umgekehrte Situation eintreten?
Ja, es kann passieren. $2x^2+1$ ist zum Beispiel in $\Z$ irreduzibel aber reduzibel in $\Q$. Umgekehrt geht das natürlich nicht. Der Quotientenkörper ist größer, daher werden dort mehr Polynome zerfallen als im Grundring.

# Aufgabe 25
Was besagt das [[Eisenstein-Kriterium]] bzw. das [[Reduktionskriterium]]?
Eisenstein: Alle Koeffizienten bis auf den ersten sind durch eine Primzahl $p$ teilbar. Der letzte ist nicht durch $p^2$ teilbar.
Reduktion: $f$ ist irreduzibel, wenn $f$ in einem Faktorring irreduzibel ist.

Zeige $f = x^7+2x+2$ und $g=x^3+x+1$.
$f$ ist nach Eisensteinkriterium irreduzibel. $g$ ist nach Satz über rationale Nullstellen irreduzibel. Man kann aber auch das Reduktionskriterium anwenden und zeigen, dass $g$ über $\Z/2\Z$ irreduzibel ist.







$\newcommand{\Q}{\mathbb Q}$
$\newcommand{\R}{\mathbb R}$
$\newcommand{\C}{\mathbb C}$
$\newcommand{\F}{\mathbb F}$
$\newcommand{\Z}{\mathbb Z}$
$\newcommand{\N}{\mathbb N}$
$\newcommand{\a}{\alpha}$

#Algebra 



