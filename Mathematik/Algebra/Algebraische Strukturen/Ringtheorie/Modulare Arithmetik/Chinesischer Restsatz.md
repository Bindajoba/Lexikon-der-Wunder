## Beschreibung
Der **Chinesische Restsatz** trifft eine Aussage, wann Zahlen mit einer geforderten Menge von [[Kongruenz (Ganze Zahlen)|Kongruenzen]] eine Lösung haben und welche Lösungen dies genau sind.

## Definition
### Enge Variante
Gesucht ist eine Zahl, welche kongruent zu $a_1, a_2, ..., a_r$ bezüglich modulo $n_1, n_2, ..., n_r$ sein soll.

Dabei sind $n_1, n_2, ..., n_r$ paarweise [[Teilerfremdheit|teilerfremde]] ganze Zahlen. (D.h. $ggT(n_1, n_2, ..., n_r) = 1$)

Formal:
$$\begin{align} x&\equiv a_1 \mod n_1 \\
\vdots\\
x &\equiv a_r \mod n_r\end{align}$$

Der Satz besagt, dass alle Lösung kongruent bezüglich $n=n_1 \cdot ... \cdot n_r$ sind.

*Die Bedingung, dass die Modulo teilerfremd seiene müssen, ergibt ziemlich viel Sinn. Versuche eine Zahl zu finden, welche Kongruent bazüglich $2$ und $3$ modulo $2$ ist. Offensichtich gibt es keine solche Zahl. Teilerfremdheit verhindert sowas.*

### Was in Algebra mal gemacht wurde
Sind $m, n \in \mathbb{N}$ teilerfremd, dann gilt $$\mathbb{Z}/(mn)\mathbb{Z} \cong \mathbb{Z}/(m)\mathbb{Z} \times \mathbb{Z}/(n)\mathbb{Z}$$

In der Übung haben wir gezeigt, dass die Rückrichtung auch gilt. Das heißt, 
$m, n \in \mathbb{N}$ sind genau dann teilerfremd, wenn gilt $$\mathbb{Z}/(mn)\mathbb{Z} \cong \mathbb{Z}/(m)\mathbb{Z} \times \mathbb{Z}/(n)\mathbb{Z}$$

### Ein dritter Chinesischer Restsatz
Sei $R$ ein Ring, $I_1, ..., I_m$ paarweise teilerfremde Ideale in $R$ und $I = I_1 \cdot ... \cdot I_m$. Dann gibt es einen [[Ringisomorphismus|Isomorphismus]]
$$\bar \phi : R/I \to (R/I_1) \times ... \times (R/I_m) \text{ mit } \bar \phi(a+I) = (a+I_1, ..., a+I_m) \text{ für alle } a\in R$$[^1]

# Übungen
![[Zth Klausur 2019 Aufgabe 4.png]]

### a)
$a \equiv 2\mod 5 \implies a \in \{..., 2, 7, 12, 17, 22, 27, 32, ...\}$
$a \equiv_7 3 \implies a = 17$ erfüllt die Gleichungen.

### b)
Aus a) und dem Chinesischem Restsatz können die ersten beiden Gleichungen zu $a \equiv_{35} 17$ zusammengefasst werden.
Wende den euklidischen Algorithmus auf $ggT(35, 19)$ an:
| $t_i$ | $s_i$ | $r_i$ | $q_i$ |
| ----- | ----- | ----- | ----- |
| 1     | 0     | 35    | -     |
| 0     | 1     | 19    | -     |
| 1     | -1    | 16    | 1     |
| -1    | 2     | 3     | 1     |
| 6     | -11   | 1     | 5     |

Das heißt $1 = 6 \cdot 35 -11\cdot 19$
Wir erhalten $6 \cdot 35 \equiv_{19} 1$ und $-11\cdot 19 \equiv_{35} 1$
Damit erfüllt $11 \cdot 6 \cdot 35 - 17 \cdot 11\cdot 19 = -1243$ beide Gleichungen.

### c)
$ggT(19, 35) = 1$. Nach Vorlesung kann man die beiden für b) verwendeten Gleichungssysteme zu einem zusammenfassen:
$$a \equiv_{19\cdot35}-1243$$
Die Lösungen davon sind genau $\{-1243+n\cdot19\cdot35:n\in \Z\}$

**Lösung**
*Weil die Zahlen $5, 7$ und $19$ paarweise teilerfremd sind und $665 = 5\cdot7 \cdot 19$ gilt, existiert nach dem Chinesischen Restsatz ein Ringisomorphismus $\Z/665\Z \to \Z/5\Z \times \Z/7\Z \times \Z/19\Z$ gegeben durch $\phi(a+665\Z) = (a+5\Z, a+7\Z, a+19\Z)$ für alle $a\in \Z$*

Die Lösung von Aufgabe b) erfüllt $\phi(-1243+665\Z) = (2+5\Z, 3+7\Z, 11+19\Z)$
Da $\phi$ injektiv sind die Zahlen $-1243+665\Z$ die einzigen Zahlen mit dieser Eigenschaft.


#Böhm #Algebra #Zahlentheorie 

[^1]: Gerkmann - Satz 8.5