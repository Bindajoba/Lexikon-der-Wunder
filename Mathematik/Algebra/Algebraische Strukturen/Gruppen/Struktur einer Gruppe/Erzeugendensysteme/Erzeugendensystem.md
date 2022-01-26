## Beschreibung
Das Erzeugendensystem einer [[Gruppe]] ist eine Menge, mit der man die Gruppe eindeutig konstruieren kann.

Erzeugendensysteme werden durch geknickte Klammern ausgedrückt:
$$\langle a \rangle$$

Es klingt ganz danach, als ob das genau die Generatoren einer Gruppe sind.


## Definition
Sei $G$ eine Gruppe und $S \subset G$. $S$ ist dann ein **Erzeugendensystem** der [[Untergruppe]] $U$ wenn
1. $U \supset S$
2. Ist $V$ eine weitere Untergruppe von $G$ mit $V \supset S$, dann folgt $V \supset U$

Das bedeutet: $U$ ist die kleinste Untergruppe, die $S$ enthält

### Group Presentation
Statt das Zusammenspiel der Elemente aus einer Obergruppe zu erhalten, können diese auch explizit angegeben werden.
Z.B.
$$\langle r, f: r^3 = 1, f^2 = 1, frf=r^{-1}$$[^2]

## Berechnung
Sein $G$ eine Gruppe und $S \subset G$ eine Teilmenge.

Die Elemente von $\langle S \rangle$ sind gegeben durch:
$$\langle S \rangle = \{g_1^{\varepsilon_1}\cdot g_2^{\varepsilon_2} \cdot \dots \cdot g_r^{\varepsilon_r}|r \in \mathbb{N}_0, r_k \in S, \varepsilon_k \in \{-1, 1\} \text{ für } 1\leq k \leq r \}$$
[^1]


## Beispiele
*Für Erzeugendensysteme muss die Obergruppe immer mit angegeben werden!*

### Leeres Erzeugendessystem
In jeder Gruppe $G$ gilt:
$$\langle \emptyset \rangle = \{e_G\}$$

### Ganze Zahlen
Die Gruppe $(\mathbb{Z}, +)$ wird von $\{1\}$, ebenso $\{-1\}$, ebenso $\{2,3\}$ erzeugt.


#Algebra 
 
[^1]: Gerkmann - Satz 2.9
[^2]: Carter - Aufgabe 5.33