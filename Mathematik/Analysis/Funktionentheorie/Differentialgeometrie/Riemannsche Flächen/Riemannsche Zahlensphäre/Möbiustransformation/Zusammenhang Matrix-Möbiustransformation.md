## Beschreibung
Beim Rechnen fält uns auf, dass die Multiplikation von [[Matrix|Matrizen]] und die [[Verknüpfung]] von [[Möbiustransformation|Möbiustransformationen]] viele Parallelen haben.
Desweiteren sieht die [[Inverse (Matrix)]] aus wie die [[Umkehrabbildung]].

Das bringt uns auf die Idee, zu jeder Möbiustransformation eine äquivalente Matrix zu finden:
$$M(z) = \frac{az-b}{cz-d} \longleftrightarrow [M] = \begin{bmatrix} a & b \\ c & d \end{bmatrix}$$
Leider ergibt sich dadurch ein Problem:
Ist $k$ eine [[Komplexe Zahlen|komplexe Zahl]], dann entspricht die Matrix $k[M]$ der gleichen Möbiustransformation wie $[M]$.
Beschränkt man die Möbiustransformationen aber auf [[Normalisierte Möbiustransformation|normalisierte]], dann gibt es zu jeder Möbiustransformation $M(z) = \frac{az+b}{cz+d}$ nur die Matrizen $[M] = \begin{bmatrix} a & b \\ c & d \end{bmatrix}$ und $-[M] = \begin{bmatrix} -a & -b \\ -c & -d \end{bmatrix}$

## Erklärung
Aber woher kommt dieser überraschende Zusammenhang?

Beschreibe einen Urbildpunkt und seinen Bildunkt in [[Homogene Koordinaten|homogenen Koordinaten]] $z = \frac{\mathfrak{z}_1}{\mathfrak{z}_2}$,  $w = \frac{\mathfrak{w}_1}{\mathfrak{w}_2}$.
Multipliziere des Urbildpunkt mit der Matrix:
$$\begin{bmatrix}\mathfrak{z}_1 \\ \mathfrak{z}_2 \end{bmatrix} \mapsto \begin{bmatrix}\mathfrak{w}_1 \\ \mathfrak{w}_2 \end{bmatrix} = \begin{bmatrix} a & b \\ c & d\end{bmatrix} \begin{bmatrix}\mathfrak{z}_1 \\ \mathfrak{z}_2 \end{bmatrix} = \begin{bmatrix}a\mathfrak{z}_1 + b\mathfrak{z}_2\\c\mathfrak{z}_1 +  d\mathfrak{z}_2 \end{bmatrix} $$
Bezieht man diese Abbildung auf das Verhältnis $z = \frac{\mathfrak{z}_1}{\mathfrak{z}_2}$ zurück, erhält man:
$$z = \frac{\mathfrak{z}_1}{\mathfrak{z}_2} \mapsto w = \frac{\mathfrak{w}_1}{\mathfrak{w}_2} = \frac{a\mathfrak{z}_1 + b\mathfrak{z}_2}{c\mathfrak{z}_1 +  d\mathfrak{z}_2} = \frac{a(\mathfrak{z}_1 / \mathfrak{z}_2) + b}{c(\mathfrak{z}_1/\mathfrak{z}_2) +  d} = \frac{az+b}{cz+d}$$
Die Möbiustransformation ist also genau das Anwenden der äquivalenten Matrix auf den Punkt in homogenen Koordinaten.

## Eigenvektoren-Fixpunkte
Ein [[Eigenvektor]] erfüllt die Gleichung
$$\begin{bmatrix} a & b \\ c & d \end{bmatrix} \begin{bmatrix} \mathfrak{z}_1 \\ \mathfrak{z}_2 \end{bmatrix} = \lambda \begin{bmatrix} \mathfrak{z}_1 \\ \mathfrak{z}_2 \end{bmatrix} =  \begin{bmatrix}\lambda \mathfrak{z}_1 \\\lambda \mathfrak{z}_2 \end{bmatrix}$$
D.h.
$$M(z) = M(\frac{\mathfrak{z}_1}{\mathfrak{z}_2}) = \frac{\lambda\mathfrak{z}_1}{\lambda\mathfrak{z}_2} = z$$
Eigenvektoren der Matrix sind also [[Fixpunkt|Fixpunkte]] der [[Möbiustransformation]] 

#Needham 