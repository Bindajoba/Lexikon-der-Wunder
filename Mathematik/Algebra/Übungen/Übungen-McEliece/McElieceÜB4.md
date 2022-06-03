TARGET DECK: Universität::Mathematik::Algebra

# Aufgabe 1
Zeige: Die Relation $a \equiv_m b$ definiert durch $m \mid (a-b)$ ist eine Äquivalenzrelation.

- Reflexivität: $m \mid (a-a)$
- Symmetrie: $m \mid (a-b) \implies m \mid -(a-b)$
- Transitivität: $m \mid (a-b)$ und $m \mid (b-c) \implies m \mid (a-b)+(b-c) = (a-c)$

Siehe: 
- [[Kongruenz (Ring)]]
- [[Äquivalenzrelation]]

# Aufgabe 2
Zeige, dass die Multiplikation $\overline a \cdot \overline b$ in $\mod m$ nicht vom Repräsentanten $a, b$ abhängt.
Alle Repräsentanten von $\overline a$ sind aus einem Repräsentanten ableitbar: $a+mn, n\in \Z$.
Seien $a+mn_a, b+mn_b$ beliebige Repräsentanten.
$$(a+mn_a)(b+mn_b) = ab + (an_b+bn_a)m + n_an_bm^2 \equiv_m ab$$
Siehe auch:
- [[Kongruenz (Ring)]]

# Aufgabe 3
$0 \equiv_m 1 \iff m = 1$ In dem Fall besteht der [[Ring]] nur aus einem Element $\overline 0 = \overline 1$. Das ist nach VL kein [[Körper]].

# Aufgabe 4
Zeige, dass ein [[Ring]] mit [[Nullteiler]] kein [[Körper]] sein kann.
In einem Körper ist Division definiert und eindeutig. Angenommen, es gibt $ab = 0$, was ist dann $0/a$. $0?, b?$

# Aufgabe 5
$x^2+1 \equiv 1 \iff x^2 \equiv -1$

# Aufgabe 6
Zeige, dass in einem Integritätsbereich gilt:
$grad(fg) = grad(f)+grad(g)$.

$fg = (ax^n + ...)(bx^m + ...) = (abx^{nm}+...)$, wobei $ab \neq 0$, da es sonst einen Nullteiler $\neq 0$ gäbe.

# Aufgabe 7
Zeige: Der Rest einer Polynomdivision $a(x) = q(x)b(x)+r(x)$ ist eindeutig

Bei der Polynomdivision gilt $grad(r(x)) < grad(b(x))$. Angenommen, es gibt zwei mögliche Reste $r_1(x), r_2(x)$ sodass
$$a(x) = q_1(x)b(x)+r_1(x) =  q_2(x)b(x)+r_2(x)$$
Dann gilt $(q_1(x)-q_2(x))b(x) = r_2(x)-r_1(x)$ also $r_1(x) \equiv r_2(x) \mod b(x)$
Entsprechend muss es ein $g$ geben, sodass $r_1 = r_2 + gb$.
Da aber $grad(gb) = grad(g)+grad(b) \geq grad(b)$ für $g \neq 0$ und damit $grad(r_1) \geq grad(gb) \geq grad(b)$, was gegen die Voraussetzung spricht, deshalb ist $g=0$ und damit $r_1 = r_2$.

# Aufgabe 8
$(x^2+x)(x^2+x+1) = (x^4+x^3+x^2+x^3+x^2+x) = x^4+x^2+x = 0$

# Aufgabe 9
## a)
Gebe eine Multiplikationsregel für die Elemente aus $\F_{16}$ gegeben durch das Minimalpolynom $x^4+x+1$
In $\F_2(x)/(x^4+x+1)$ sind alle Elemente durch ein Polynom von maximal drittem Grad repräsentierbar. Der Dadurch erzeugte Körper bildet einen $4$-dimensionalen Vektorraum.

Im Ring gilt die Regel: $\overline{x^4} = \overline{x+1}$
Für die Multiplikation zweier Polynome gilt:
$(a_1x^3+b_1x^2+c_1x+d_1)(a_2x^3+b_2x^2+c_2x+d_2)$
$= a_1a_2x^6+(a_1b_2+b_1a_2)x^5+ (a_1c_2+b_1b_2+c_1a_2)x^4(a_1d_2+b_1c_2+c_1b_2+d_1a_2)x^3$
$+(b_1d_2+c_1c_2+d_1b_2)x^2+(c_1d_2+d_1c_2)x+d_1d_2$
$= a_1a_2(x^3+x^2)+(a_1b_2+b_1a_2)(x^2+x)+ (a_1c_2+b_1b_2+c_1a_2)(x+1)(a_1d_2+b_1c_2+c_1b_2+d_1a_2)x^3$
$+(b_1d_2+c_1c_2+d_1b_2)x^2+(c_1d_2+d_1c_2)x+d_1d_2$
$=(a_1a_2+a_1c_2+b_1b_2+c_1a_2)x^3+(a_1a_2+a_1b_2+b_1d_2+c_1c_2+d_1b_2)x^2+$$+(a_1b_2+b_1a_2+a_1c_2+b_1b_2+c_1a_2+c_1d_2+d_1c_2)x+(a_1c_2+b_1b_2+c_1a_2+d_1d_2)$

## b)
Erstelle eine Logarithmustafel
- $x = x$
- $x^2 = x^2$
- $x^3 = x^3$
- $x^4 = x+1$
- $x^5 = x^2+x$
- $x^6 = x^3+x^2$
- $x^7 = x^4+x^3 = x^3+x+1$
- $x^8 = x^5+x^4 = x^4+x^2+x = x^2+1$
- $x^9 = x^3+x$
- $x^{10} = x^4+x^2 = x^2+x+1$
- $x^{11} = x^3+x^2+x$
- $x^{12} = x^4+x^3+x^2 = x^3+x^2+x+1$
- $x^{13} = x^4+x^3+x^2+x = x^3+x^2+1$
- $x^{14} = x^4+x^3+x = x^3+1$
- $x^{15} = x^4+x = 1$

Wir erhalten die Logarithmustabelle:

| $\beta$ | $\log_\alpha\beta$ |
| ------- | ------------------ |
| 0000    | -                  |
| 0001    | 0                  |
| 0010    | 1                  |
| 0011    | 4                  |
| 0100    | 2                  |
| 0101    | 8                  |
| 0110    | 5                  |
| 0111    | 10                 |
| 1000    | 3                  |
| 1001    | 14                 |
| 1010    | 9                  |
| 1011    | 7                  |
| 1100    | 6                  |
| 1101    | 13                 |
| 1110    | 11                 |
| 1111    | 12                 |

# Aufgabe 10
Beschreibe den [[Körper]] $\Z[i]/(1+i)$ vollständig.
Nehme eine beliebige gaußsche Zahl $\alpha$.
Hat sie einen Betrag größer als $1+i$, dann kann man $\alpha$ durch $1+i$ dividieren und der Rest $r$ ist kongruent zu $\alpha$.
D.h. $r + (1+i) = \alpha + (1+i)$.

![[McElieceÜB4-10.png]]
Alle Elemente, die auf den Punkten des Rasters liegen sind zu einander kongruent, da sich sich um $(a+bi)(1+i)$ unterscheiden. Ebenso sind Punkte mit der gleichen Position bezüglich eines dieser Quadrate zueinander kongruent.
Die einzigen Punkte in einem Quadrat, die nicht kongruent zueinander sind, sind $0$ und $1$. Also ist der resultierende Körper isomorph $\F_2$.

# Aufgabe 11
Beschreibe $\F_3[x]/(x^2-x-1)$ mit einer Adidtions und Multiplikationstabelle.
$x^2-x-1$ ist irreduzibel. Damit ist $\F_3[x]/(x^2-x-1)$ ein Körper.
Für die Polynome mit Grad $< 3$ sind nicht zueinander kongruent, denn wären sie es, dann müssten sie sich um ein Vielfaches ($\neq 0$) von $x^2-x-1$ unterscheiden, was nicht geht, solange beide Grad $<3$ haben sollen.

Polynome mit Grad $\geq$ 3 sind wegen wiederholter Polynomdivision kongruent zu einem Polynom von Grad $<3$.
Mit den Polynomen von Grad $3$ haben wir also ein Repräsentantensystem der Elemente der Faktorgruppe $\F_3[x]/(x^2-x-1)$ gefunden. Diese Polynome können wir durch ihre Koeffizienten beschreiben.

Additionstafel

| 000 | 001 | 002 | 010 | 011 | 012 | 020 | 021 | 022 | 100 | 101 | 102 | 110 | 111 | 112 | 120 | 121 | 122 | 200 | 201 | 202 | 210 | 211 | 212 | 220 | 221 | 222 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| 001 |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |
| 002 | 000 |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |
| 010 |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |
| 011 |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |
| 012 |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |
| 020 |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |
| 021 |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |
| 022 |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |
| 100 |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |
| 101 |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |
| 102 |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |
| 110 |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |
| 111 |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |
| 112 |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |
| 120 |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |
| 121 |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |
| 122 |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |
| 200 |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |
| 201 |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |
| 202 |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |
| 210 |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |
| 211 |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |
| 212 |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |
| 220 |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |
| 221 |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |
| 222 |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |

 Und so weiter. Die Multiplikation ist interessanter:

| *   | 000 | 001 | 002 | 010 | 011 | 012 | 020 | 021 | 022 | 100 | 101 | 102 | 110 | 111 | 112 | 120 | 121 | 122 | 200 | 201 | 202 | 210 | 211 | 212 | 220 | 221 | 222 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| 000 | 000 | 000 | 000 | 000 | 000 | 000 | 000 | 000 | 000 | 000 | 000 | 000 | 000 | 000 | 000 | 000 | 000 | 122 | 200 | 201 | 202 | 210 | 211 | 212 | 220 | 221 | 222 |
| 001 | 000 | 001 | 002 | 010 | 011 | 012 | 020 | 021 | 022 | 100 | 101 | 102 | 110 | 111 | 112 | 120 | 121 | 122 | 200 | 201 | 202 | 210 | 211 | 212 | 220 | 221 | 222 |
| 002 | 000 | 002 | 001 | 020 | 022 | 021 | 010 | 012 | 011 | 200 | 202 | 201 | 220 | 222 | 221 | 210 | 212 | 211 | 100 | 102 | 101 | 120 | 122 | 121 | 110 | 112 | 111 |
| 010 | 000 | 010 | 020 | 100 | 110 | 120 | 200 | 210 | 220 | 011 | 021 | 001 | 111 | 121 | 101 | 211 | 221 | 201 | 022 | 002 | 012 | 122 | 102 | 112 | 222 | 202 | 212 |
| 011 | 000 | 011 | 022 | 110 | 121 | 102 | 220 | 201 | 212 | 111 | ... | 	    |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |
| 012 |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |
| 020 |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |
| 021 |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |
| 022 |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |
| 100 |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |
| 101 |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |
| 102 |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |
| 110 |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |
| 111 |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |
| 112 |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |
| 120 |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |
| 121 |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |
| 122 |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |
| 200 |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |
| 201 |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |
| 202 |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |
| 210 |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |
| 211 |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |
| 212 |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |
| 220 |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |
| 221 |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |
| 222 |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |     |





$\newcommand{\Q}{\mathbb Q}$
$\newcommand{\R}{\mathbb R}$
$\newcommand{\C}{\mathbb C}$
$\newcommand{\F}{\mathbb F}$
$\newcommand{\Z}{\mathbb Z}$
$\newcommand{\N}{\mathbb N}$
$\newcommand{\a}{\alpha}$

#McEliece  


