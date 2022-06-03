TARGET DECK: Universität::Mathematik::Algebra

# Beschreibung
Ein [[Endlicher Körper]] mit $p^n$ Elementen.


# Eigenschaften
## Existenz & Eindeutigkeit
Sei $p$ eine Primzahl und $n\in N$. Dann gibt es einen Körper mit $p^n$ Elementen und je zwei Körper mit $p^n$ Elementen sind zueinander [[Körperisomorphismus|isomorph]].

*Konkret ist der Körper mit Größe $p^n$ der Zerfällungskörper eines [[Körper von Primzahlgröße]] $p$ zum Polynom $x^{p^n}-x \in P[x]$. Der Zerfällungskörper ist immer eindeutig also sind die Körper gleich.*

## Algebraischer Abschluss und seine Teilkörper
Sei $p$ eine prim und $\mathbb{F}_p^{alg}$ ein algebraischer Abschluss von $\mathbb{F}_p$ (ein algebraischer Abschluss ist bis auf Isomorphie eindeutig.)
1. Für jedes $n \in \mathbb{N}$ gibt es genau einen Teilkörper $\mathbb{F_{p^n}} \subseteq \mathbb{F}_p^{alg}$ mit $p^n$ Elementen
2. Für $m, n \in \mathbb{N}$ gilt $\mathbb{F}_{p^m} \subseteq \mathbb{F}_{p^n}$ genau dann, wenn $m$ ein Teiler von $n$ ist

*Für $\mathbb{F}_2$:*
Sei $\mathbb{F}_2^{alg}$ der algebraische Abschluss von $\mathbb{F_2}$.
1. Für jedes $n \in \mathbb{N}$ gibt es genau einen Teilkörper $\mathbb{F}_{2^n}$ mit $2^n$ Elementen
2. Für $m, n \in \mathbb{N}$ gilt $\mathbb{F}_{2^m} \subseteq \mathbb{F}_{2^n}$ genau dann, wenn $m$ ein Teiler von $n$ ist

## Nullstellen des Polynoms
Die Elemente des p-Körpers $\F_{p^n}$ sind genau die Nullstellen des Polynoms $x^{p^n}-x$.
Desweiteren erfüllen alle Elemente die Gleichung $x^{p^n} = x$.

**Beweis:**

## Konjugierte Elemente
[[Konjugierte Elemente]] sind $p$-Potenzen voneinander

**Beweis:**
Potenziert man das Minimalpolynom mit $p$:
$$\begin{align}f(x)^p &= (x^n + a_{n-1}x^{n-1}+...+xa_1+a_0)^p \\
&= x^{np} + a_{n-1}^px^{(n-1)p}+...+x^pa_1^p+a_0^p \\
&= x^{np} + a_{n-1}x^{(n-1)p}+...+x^pa_1+a_0\\
&=f(x^p)\end{align}$$
Es gilt dann $f(x)^p = 0 \iff f(x^p) = 0$
Durch mehrfache Anwendung erhalten wir außerdem $x^{p^2}, x^{p^3}, ...$ als konjugierte Elemente. 

*Die Potenzierung ist doch genau der [[Frobenius-Automorphismus]]*

# Beispiele
## Körper mit p Elemente
Siehe [[Körper von Primzahlgröße]]


# Übungen
## Klausur 2019?
![[Klausur 2018 Aufgabe 6.png]]
### a)
Die Zwischenkörper erhält man nach VL aus den Teilern des Exponenten $8$ und aus Vielfachen des Exponenten $2$.
Möglich sind $\F_8, \F_4, \F_2$ also drei

### b)
$|K^\times| = 256-1 = 255 = 5 \times 51 = 17 \times 5 \times 3$
Alle endlichen Untergruppen Multiplikativer Gruppen sind zyklisch. $K^\times$ ist damit isomorph zu $C_{255}$.
Die Untergruppen einer zyklischen Gruppe sind nur die zyklischen Gruppen, deren Ordnung 255 teilt. (Diese sind dann eindeutig)
Aus Kombination der Primfaktoren von $255$ erhält man $1, 3, 5, 15, 17, 51, 85, 255$ also $8$ verschiedene Untergruppen.

## Checkliste Gerkmann
### Aufgabe 1
Warum hat $\F_2$ keine nicht-normalen algebraischen Erweiterungen?

Nach VL ist $\F_{2^n}$ der Zerfällungskörper von $x^{p^n}-x$ und zugleich dessen Nullstellenmenge. Sei $\alpha \in \F_{2^n}$, dann teilt das Minimalpolynom von $\alpha$ das obere Polynom womit alle anderen Nullstellen des Polynoms auch in dem Oberkörper liegen. Das Polynom zerfällt.

### Aufgabe 2
Sei $K$ ein p-Körper und $L$ ein Zerfällungskörper eines Polynoms $f$ vom Grad $n \in \N$. Welchen Grad kann die Erweiterung $[L:K]$ haben?

Als Zerfällungskörper ist $L|K$ normal und da $K$ ein endlicher Körper ist, auch separabel. Damit ist die Erweiterung eine [[Galois-Erweiterung]].
Jede Galoiserweiterung eines p-Körpers ist zyklisch. Desweiteren muss sie eine Teilmenge von $S_n$ sein. Damit kann sie maximal Ordnung $n$ haben.

## Klausur 2016 Aufgabe 6
![[Klausur 2016 Aufgabe 6.png]]
### a)
In p-Körpern gilt Freshmans Dream:
$x^6+1 = (x^3+1)^2$
$x^6+1 = (x^2+1)^3$

### b)
Der Körper hat die Ordnung $p^2-1 = (p-1)(p+1)$
Da $p$ ungerade Primzahl ist, sind die beiden Produkte gerade. D.h. $4 |p^2-1$
Da $p$ Primzahl $>3$ ist, ist $p$ nicht durch $3$ teilbar, also muss einer der anliegenden Zahlen durch $3$ teilbar sein. Damit ist $3 \mid p^2-1$.
Damit teilt auch $ggT(3, 4) = 12 \mid p^2-1$. 

### c)
Nach b) gibt es immer ein Element $\alpha$ der Ordnung $12$.
Es gilt also $\alpha^{12} = 1 \implies \alpha^{12}-1 = (\alpha^6-1)(\alpha^6+1) = 0$
Angenommen $\alpha^6-1 = 0$, dann hätte $\alpha$ nicht Ordnung $12$.
Also $\alpha^6+1 = 0$. damit löst $\alpha$ das Polynom aus der Aufgabenstellung

$\alpha \in \F_{p^2}$, weshalb $\F_p(\alpha)$ ein Zwischenkörper von $\F_{p^2}|\F_p$ ist und nur Erweiterungsgrad $1$ oder $2$ haben kann.
- Im Fall $[\F_p(\alpha):\F_p] = 2$, dann teilt das Minimalpolynom $g$ mit Grad 2 das Polynom $x^6+1$, dann ist das Polynom reduzibel.
- Im Fall $[\F_p(\alpha):\F_p] = 1$, dann ist $\alpha \in \F_p$ und $(x-\alpha)$ teilt $x^6+1$ und das Polynom ist reduzibel.

## McElice Übung 5-7
Sei $\F_{49}$ der Körper, der durch $x^3-3$ erzeugt wird. Sei $\alpha$ das Element, welches zu der Kongruenzklasse $x \mod x^2-3$ korrespondiert.

### a)
Was ist die Ordnung von $\alpha$?
Die Multiplikative Gruppe hat die Ordnung $48 = 2^4 * 16$

- $x$
- $x^2 \cong 3$
- $x^3 \cong 3x$
- $x^4 \cong 3x^2 \cong9 \cong 2$
- $x^5 \cong 2x$
- $x^6 \cong 2x^2 \cong 6$
- $x^7 \cong 6x$
- $x^8 \cong 6x^2 \cong 18 \cong 4$
- $x^{12} = 2*4 = 1$

Die Ordnung von $\alpha$ ist $12$ oder ein Teiler. Es kann aber wie man sieht kein Teiler sein, ist also $12$.

### b)
Finde eine [[Primitivwurzel]] und beschreibe $\alpha$ als Potenz davon.
Verwende $\alpha +1$. Was ist die Ordnung von $\alpha+1$.
- $\alpha + 1$
- $(\alpha+1)^2 = \alpha^2 + 2\alpha+1 = 2\alpha+4$
- $(\alpha+1)^3 = (2\alpha^2+6\alpha+4) = 6\alpha+3$
- $(\alpha+1)^4= (4\alpha^2+16\alpha+16) = 2\alpha$
- $(\alpha+1)^7 = 5\alpha^2+6\alpha = 6\alpha+1$
- $(\alpha+1)^8= 4\alpha^2 = 5$
- $(\alpha+1)^{12}=3\alpha$
- $(\alpha+1)^{16}= 25 = 4$
- $(\alpha+1)^{32} = 2$
- $(\alpha+1)^{48} = 1$
- $(\alpha+1)^{20}= 8\alpha = \alpha$

Gefunden!
Es gilt $\alpha = (\alpha+1)^{20}$

### c)
Finde das Minimalpolynom von $\alpha+1$.
Das Minimalpolynom berechnet sich aus den 2 konjugierten Werten.
$$\begin{align}(x-(\alpha+1))(x-(\alpha+1)^7) &= (x-(\alpha+1))(x-(6\alpha+1))\\
&= x^2-((\alpha+1)+(6\alpha+1))x+(\alpha+1)(6\alpha+1)\\
&=x^2-2x+5\end{align}$$

## McEliece Übung 5-8
Erzeuge $\F_{27}$ mit dem Minimalpolynom $x^3+2x+1$. Liste alle Elemente und finde für alle Elemente das Minimalpolynom und die Ordnung.

Sei $\alpha$ eine Nullstelle des Polynoms. Dann gilt $x^3 = -2x-1 = x+2$

| Potenz | Element | Ordnung | Minimalpolynom  |
| ------ | ------- | ------- | --------------- |
| -      | 000     | -       | $x$             |
| 0      | 001     | 1       | $x-1$           |
| 13     | 002     | 2       | $x-2$           |
| 1      | 010     | 26      | $x^3+2x+1$      |
| 9      | 011     | 26      | $x^3+2x+1$      |
| 3      | 012     | 26      | $x^3+2x+1$      |
| 14     | 020     | 13      | $x^3+x+2$       |
| 16     | 021     | 13      | $x^3+x+2$       |
| 22     | 022     | 13      | $x^3+x+2$       |
| 2      | 100     | 13      | $x^3+x^2+x+2$   |
| 21     | 101     | 26      | $x^3+x^2+2x+1$  |
| 12     | 102     | 13      | $x^3+x^2+2$     |
| 10     | 110     | 13      | $x^3+x^2+2$     |
| 6      | 111     | 13      | $x^3+x^2+x+2$   |
| 11     | 112     | 26      | $x^3+x^2+2x+1$  |
| 4      | 120     | 13      | $x^3+x^2+2$     |
| 18     | 121     | 13      | $x^3+x^2+x+2$   |
| 7      | 122     | 26      | $x^3+x^2+2x+1$  |
| 15     | 200     | 26      | $x^3+2x^2+x+1$  |
| 25     | 201     | 26      | $x^3+2x^2+1$    |
| 8      | 202     | 13      | $x^3+2x^2+2x+2$ |
| 17     | 210     | 26      | $x^3+2x^2+1$    |
| 20     | 211     | 13      | $x^3+2x^2+2x+2$ |
| 5      | 212     | 26      | $x^3+2x^2+x+1$  |
| 23     | 220     | 26      | $x^3+2x^2+1$    |
| 24     | 221     | 13      | $x^3+2x^2+2x+2$ |
| 19     | 222     | 26      | $x^3+2x^2+x+1$  |




Die Einheitengruppe von $\F_{27}$ hat $26 = 2 * 13$ Elemente
- $\alpha^2$
- $\alpha^3=\alpha+2$
- $\alpha^4 = \alpha^2+2\alpha$
- $\alpha^5 = 2\alpha^2+\alpha+2$
- $\alpha^6 = \alpha^2 + \alpha + 1$
- $\alpha^7 = \alpha^2 + 2\alpha+2$
- $\alpha^8 = \alpha^4+4\alpha^3+4\alpha^2 = \alpha^2+2\alpha+4\alpha+8+4\alpha^2 = 2\alpha^2+2$
- $\alpha^9 = \alpha+1$
- $\alpha^{10} = \alpha^2+\alpha$
- $\alpha^{11} = \alpha^2+\alpha+2$
- $\alpha^{12} = (\alpha^2+2\alpha)(2\alpha^2+2) =2\alpha^4+\alpha^3+2\alpha^2+\alpha = 2\alpha^2+\alpha+\alpha+2+2\alpha^2+\alpha = \alpha^2+2$
- $\alpha^{13} = \alpha^3+2\alpha = 2$
- $\alpha^{14} = 2\alpha$
- $\alpha^{15} = 2\alpha^2$
- $\alpha^{16} = 2\alpha+1$
- $\alpha^{17} = 2\alpha^2+\alpha$
- $\alpha^{18} = \alpha^2+2\alpha+1$
- $\alpha^{19} = 2\alpha^2 + 2\alpha + 2$
- $\alpha^{20} = 2\alpha^2 + \alpha + 1$
- $\alpha^{21} = \alpha^2+1$
- $\alpha^{22} = 2\alpha+2$
- $\alpha^{23} = 2\alpha^2+2\alpha$
- $\alpha^{24} = 2\alpha^2+2\alpha+1$
- $\alpha^{25} = 2\alpha^2 + 1$
- $\alpha^{26} = 1$

Nebenrechungen:
$(\alpha+1)^2 =\alpha^2+2\alpha+1 = 0$
$(\alpha^9, \alpha^{9*3}, \alpha^{9*3*3}) = \alpha^9, \alpha^1, \alpha^3$ sind konjugiert und teilen das gleiche Min-Polynom
$(x-\alpha^2)(x-(\alpha^2+\alpha+1))(x-(\alpha^2+2\alpha+1)) = (x-\alpha^2)(x^2-((\alpha^2+\alpha+1)+(\alpha^2+2\alpha+1))x + (\alpha^2+\alpha+1)(\alpha^2+2\alpha+1))$
$=(x-\alpha^2)(x-(\alpha^2+\alpha+1))(x-(\alpha^2+2\alpha+1)) = (x-\alpha^2)(x^2-(2\alpha^2+2)x + (2\alpha+1))$
$= (x^3-2x^2+((2\alpha+1+(2\alpha^4+2\alpha^2)))x)$





$\newcommand{\Q}{\mathbb Q}$
$\newcommand{\R}{\mathbb R}$
$\newcommand{\C}{\mathbb C}$
$\newcommand{\F}{\mathbb F}$
$\newcommand{\Z}{\mathbb Z}$
$\newcommand{\N}{\mathbb N}$
$\newcommand{\a}{\alpha}$


#Algebra 


