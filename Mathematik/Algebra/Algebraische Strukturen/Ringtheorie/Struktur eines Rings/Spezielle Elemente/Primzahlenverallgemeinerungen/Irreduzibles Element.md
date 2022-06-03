# Beschreibung
Die Irreduziblen Elemente sind die Analogons der [[Primzahl|Primzahlen]] für allgemeine Ringe.

# Definition
Sei $R$ ein [[Ring]]. Ein Element $p \in R$ wird irreduzibel genannt, wenn $p$ weder eine [[Einheit]] noch Null ist und die Implikation:
$$p = ab \implies a \in R^\times \text{ oder } b \in R^\times$$
Für alle $a, b \in R$ erfüllt ist. Alle anderen Elemente (außer Null) werden als **reduzibel** bezeichnet.[^1]

*In den Rationalen Zahlen sind alle Zahlen irreduzibel, da alle Zahlen Einheiten sind. Das gleiche Argument gilt natürlich auch bei anderen Körpern.* Irreduzible Elemente finden vor allem bei [[Polynomring]] Einsatz. Dort sind sie genau das [[Irreduzibles Polynom]].

# Eigenschaften
## Gemeinsame Eigenschaften
- Assoziierte Element sind gemeinsam [[Irreduzibles Element|irreduzibel]] oder gemeinsam reduzibel
- Assoziierte Element sind gemeinsam [[Primelement|Primelemente]] oder gemeinsam keine Primelemente


# Übung
## Zth Klausur 2019 Aufgabe 7
![[Zth Klausur 2019 Aufgabe 7.png]]
### a)
Sei $|\cdot|$ die komplexe Norm, die man auf $\Z[\sqrt{-3}]$ definieren kann. Die komplexe Norm erfüllt die Eigenschaft $|ab| = |a||b|$.
Alle Elemente $\alpha \in \Z[\sqrt{-3}]$ haben $|\alpha|\geq 1$ für $\alpha \neq 0$. 
Eine Einheit muss die Eigenschaft $ab = 1$ und damit $|ab| = |a||b| = 1$ erfüllen. Für $a$ mit $|a|>1$ kann es kein Inverses geben. Damit sind $\{-1, 1\}$ die einzigen Einheiten.

Angenommen, $2$ wäre reduzibel, dann gäbe es eine Zwelegung von $2 = ab$, wobei $a, b\in \Z(\sqrt 3)$ keine Einheiten sind. Für Elemente, die keine Einheiten gilt aber $|a| \geq \sqrt 3 > 1$ oder $|a|\geq 2$
Ein Produkt von zwei Nicht-Einheiten $ab$ hat also immer einen größeren Betrag als $2$.

### c)
Das Ideal $(\sqrt{-3}, 2)$ enthält $(2)$ enthält aber nicht $1$ und ist damit ein größeres Ideal, das nicht das $1$-Ideal ist.


## Zth Klausur 2019 Aufgabe 8
![[Zth Klausur 2019 Aufgabe 8.png]]

### b)
$p|p^2 = q_1q_2$, d.h. $p\mid q_1$ (o.E.)
In dem Fall muss aber $q_1/p$ eine Einheit sein. Wenn nicht, dann würde $q_1$ in zwei Nicht-Einheiten zerfallen, was der Irreduzibilität widerspricht.

Wir befinden uns in einem Integritätsbereich, also gilt die Kürzungsregel. Teile $p$ auf beiden Seiten und erhalte $p = \frac{q_1}{p}q_2$
$p \mid p = \frac{q_1}{p}q_2 \implies p \mid \frac{q_1}{p}$ oder $p \mid q_2$
- Fall 1: $q_1$ zerfällt in $\frac{q_1}{p^2}p*p$, weshalb es nicht irreduzibel sein kann.
- Fall 2: $p \mid q_2$, welcher durch Ausschlussprinzip übrig bleibt.

Da $q_1, q_2$ irreduzibel sind, gibt es für sie eine Zerlegung zu $p$ und einer weiteren Einheit:
$q_1 = pe_1, q_2 = pe_2$
Damit gilt $q_1 = q_2e_1e_2^{-1}$, womit sie assoziiert sind.


#Zahlentheorie 

[^1]: Gerkmann - Definition 10.3