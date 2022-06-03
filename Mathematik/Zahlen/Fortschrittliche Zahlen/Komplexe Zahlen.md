# Definition
## Konstruktion mit Faktorringen
Sei $R = R[x]$ ein [[Ring]] und $I = (x^2+1)$ ein [[Ideal]] $C = R/I$

Dann gilt die Gleichung $(x+I)(x+I) = (x^2+I) = ((x^2+1)-1)+I = (-1)+I$

Diese Eigenschaft erinnert uns daran, wie $i^2 = -1$. Tatsächlich ist dieser [[Faktorring]] [[Ringisomorphismus|isomorph]] zum Körper $\mathbb{C}$!
Die Isomorphie verstehen wir besser, wenn wir uns Addition und Multiplikation ansehen:

### Addition
Alle Elemente aus $R/I$ sind durch ein Polynom von Grad $0$ oder $1$ repräsentierbar. Würde man ein größeres Polynom nehmen, könnte man dieses durch $x^2+1$ dividieren und der Rest wäre kongruent zum urspünglichen.

Elemente aus $R/I$ haben also die Form: $(a+bx)+I = \overline{(a+bx)}$. Bei der Addition gilt $$\overline{(a+bx)}+\overline{(c+dx)} = \overline{(a+c)+(b+d)x}$$
### Multiplikation
$$\overline{(a+bx)}\cdot\overline{(c+dx)} = \overline{ac+(ad+bc)x+bdx^2}$$
Im ersten Absatz galt: $\overline{x^2+1} = \implies \overline{x^2} = \overline{-1}$. Daraus folgt
$$\overline{(a+bx)}\cdot\overline{(c+dx)} = \overline{(ac-bd)+(ad+bc)x}$$
Was genau wie die Multiplikation zweier komplexer Zahlen aussieht.



#Algebra #Mathe-I 