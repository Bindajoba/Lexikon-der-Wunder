TARGET DECK: Universität::Mathematik::Algebra

# Aufgabe 1
## a)
$(1, 1), (1, 2)$

## b)
Nein es ist schon kein Integritätsbereich, da $(0, 1)(1, 0) = (0, 0)$, es also mindestens 3 Nullteiler gibt.

## c)
$\{(1, 0), (0, 0)\}=((1, 0))$ ist nach VL ein [[Ideal]], das aus $(1, 0)$ erzeugt wird.


, denn durch das addieren zwei beliebiger dieser Elemente erhält man wieder eines der beiden Elemente.
Außerdem gilt für $(a, b)\in R: (a, b)(1, 0) = (1, 0)$ oder $(0, 0)$.
*Wie macht man das in einer Klausursituation? Verknüpfungstabelle?*

## d)
$1(1, 1) = (1, 1), 2(1, 1) = (0, 2), 3(1, 1) =(1, 0) = 4(1, 1)=(0, 1), 5(1, 1) = (1, 2), 6(1, 1) = 0$
Die Charakterisitk ist also $6$.

# Aufgabe 2
Keine Lust...

# Aufgabe 3
## a)
Die ganzen Zahlen mit Betrag und die Gaußschen Zahlen mit $h(a+bi) = a^2+b^2$

## b)
| $t_i$ | $s_i$ | $r_i$ | $q_i$ |
| ----- | ----- | ----- | ----- |
| 1     | 0     | 911   | -     |
| 0     | 1     | 437   |       |
| 1     | -2    | 37    | 2     |
| -11   | 23    | 30    | 11    |
| 12    | -25   | 7     | 1     |
| -59   | 123   | 2     | 4     |
| 189   |  -394     | 1     | 3     |

Also gilt $189*911-394*437 = 1$, d.h. $394*437 \equiv_{911} 1$
$394$ ist das Inverse.

# Aufgabe 4
## b)
Finde die Lösung mit dem Euklidischen Alg.
Suche $a,b$ sodass $15a+92b = 1$.


| $t_i$ | $s_i$ | $r_i$ | $q_i$ |
| ----- | ----- | ----- | ----- |
| 1     | 0     | 92    | -     |
| 0     | 1     | 15    | -     |
| 1     | -6    | 2     | 6     |
| -7    | 43      | 1     | 7     |

Das heißt $43*15-7*92 = 1$
Wir erhalten daraus die Zahl: $47*43*15 - 3*7*92 = 28383$
$32203 = 276$ erfüllt die Kongruenzen.

# Aufgabe 5
## b)
$\Z[i]$ ist Hauptideal, d.h. jedes Ideal, auch $3, 2-i$


Nach VL wird das Produktideal $IJ$ aus den möglichen Produkten von den Erzeugern von $I$ und $J$ erzeugt, d.h. $IJ = (3+3i, 18, 3+i, 12-6i)$
Damit ist auch $2i \in IJ$, damit auch $3+i + i(2i) = 1+i$
Die Menge kann umgeschrieben werden zu:
$IJ = (3+3i, 18, 3+i, 12-6i) = (2, 1+i) = (1+i)$
Da $1+i$ ein Teiler von $2$ ist.

# Aufgabe 6
## a)
$f$ ist i m Körper $\F_2$ ein [[Irreduzibles Polynom]] und normiert und damit Minimalpolynom einer seiner Nullstelle $\alpha$.
Nach Zahlentheorie VL gibt es dann einen Isomorphismus von $R/(f)$ nach $\F_2(\alpha)$, einem Körper.

## b)
$g+(f) = h+(f) \iff (g-h)+(f) = (f) \iff (g+h) \in (f) \iff (g-h)$ Vielfaches von $f$.
Da $f$ irreduzibel ist, reicht es, dass $g-h$ die gleiche Nullstelle wie $f$ hat.
Das gilt genau dann, wenn $g$ und $h$ beim Einsetzen einer Nullstelle von $f$ den gleichen Wert annehmen.

## c)
$x^4 = x(x^3+x+1)-(x^2+x)$
D.h. 
$\alpha^4 = x^4+(f) = (-x^2-x)+(f) =(x^2+x)+(f)$
Die Koeffizienten kann man sich jetzt ablesen.

# Aufgabe 7
## a)
$132 = 66*2 = 2^2*3*11$
$(\Z/132\Z)^\times = \Z/2\Z \times \Z/2\Z \times \Z/10\Z$

## b)
- $3^2 = 9$
- $3^4 = 81 = 13$
- $3^8 = 16$
- $3^{16} = 1$

$3$ ist eine Primitivwurzel, wenn $3$ ein Erzeuger der multiplikativen Gruppe isomorph $\Z/16\Z$ ist, das heißt Ordnung 16 hat.
Die Ordnung der Elemente in $\Z/16\Z$ muss die Gruppenordnung $16$ teilen. Um zu zeigen, dass $3$ eine Primitivwurzel ist, ist es ausreichend zu zeigen, dass es nicht Ordnung $1, 2, 4, 8$ hat. Das habe ich oben gemacht. Also hat $3$ Ordnung $16$.

- $2^2 = 4$
- $2^4 = 16$
- $2^8 = 1$

Zwei hat Ordnung $8$.

![[ZthKL2017.pdf]]
# Aufgabe 8
## b)
$p$ ist Primelemente, das heißt es teilt, $a, b$ oder $c$. O.E. $p \mid a$. Wir können in einem Integritätsbereich kürzen und erhalten. $q = bc$.
$q$ ist als Primelement irreduzibel, das heißt $b$ oder $c$ ist eine Einheit.



#Zahlentheorie 


