## Beschreibung
Das Skalarprodukt ist eine [[Abbildung]], die zwei Vektoren eine Zahl/Skalar zuordnet.

## Definition
### Reelle Definition
Seien $p = \begin{pmatrix} p_1 \\ \vdots \\ p_n \end{pmatrix}, q = \begin{pmatrix} q_1 \\ \vdots \\ q_n \end{pmatrix}$ zwei reelle n-dimensionale Vektoren:

Dann ist das Skalarprodukt:
$$p \circ q = p_1q_1 + \dots + p_nq_n$$

### Komplexe Definition
Der erste Gedanke wäre das Produkt so zu definieren:
$$p \circ q = p_1q_1 + \dots + p_nq_n$$
Eine ziemlich wichtige Eigenschaft vom Standardskalarprodukt, ist aber dass das Produkt genau dann 0 ist, wenn man zwei orthogonale Vektoren multipliziert.

Das ist bei $\begin{pmatrix} 1\\ i \end{pmatrix} \circ \begin{pmatrix} 1\\ i \end{pmatrix} = 0$, was keinen Sinn ergibt sollte.

Stattdessen definiert man
$$p \circ q = \overline{p_1}q_1 + \dots + \overline{p_n}q_n$$


## Eigenschaften
### Orthogonale Vektoren (Reell)
Sind zwei Vektoren $p, q$ zueinander senkrecht, dann ist das $p \circ q = 0$.

### Orthogonale Vektoren (Komplex)
Für zwei komplexe Vektoren $\begin{pmatrix} p_1 \\ p_2\end{pmatrix}, \begin{pmatrix} q_1 \\ q_2\end{pmatrix}$ gilt:
$$\begin{pmatrix} p_1 \\ p_2\end{pmatrix} \circ \begin{pmatrix} q_1 \\ q_2\end{pmatrix} = \overline{p_1}q_1 + \overline{p_2}q_2 = 0 \iff \frac{q_1}{q_2} = - \frac{1}{\overline{\left(\frac{p_1}{p_2}\right)}}$$
$\frac{1}{\overline{z}}$ ist eine [[Inversion]] und mit $-z$ zusammen, erkennt man, dass das Produkt der Vektoren genau dann 0 ist, wenn $\frac{p_1}{p_2}$ und $\frac{q_1}{q_2}$ antipodal auf der [[Riemannsche Zahlensphäre]] liegen.

#Mathe-II 
#Needham 