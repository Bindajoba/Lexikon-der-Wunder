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



#Böhm #Algebra #Zahlentheorie 

[^1]: Gerkmann - Satz 8.5