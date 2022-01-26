## Beschreibung
Die Umlaufzahl beschreibt, wie oft sich eine [[Komplexe Stückweise Differenzierbare Schleife]] um einen Punkt dreht.

## Definition
Sei
- $a\in \mathbb{C}$ der Punkt, um den die Umlaufzahl berechnet werden soll.
- $\gamma: [\alpha,\beta] \to \mathbb{C}\backslash\{a\}$ eine [[Komplexe Stückweise Differenzierbare Schleife|komplexe stückweise differenzierbare Schleife]]

Die **Umlaufszahl von $a$ bezüglich $\gamma$** errechnet sich aus:
$$n(a, \gamma) := -i\frac{1}{2\pi}\int\limits_\gamma{\frac{1}{z-a}\,dz} \in \mathbb{Z}$$[^1]

## Berechnung
### Einfach durchlaufene Schleife
Die Umlaufzahl einer einfach durchlaufenen Schleife kann [[Algorithmus zur Berechnung der Umlaufzahl einfach durchlaufener Schleifen|durch Konstruktion von Kreisen an der Spur der Schleife berechnet werden]].

## Eigenschaften
### Summenwege
Die Umlaufzahl einer Summe von differenzierbaren Schleifen, ist die Summe der jeweiligen Umlaufszahlen

*Das steht nicht ganz so im Skript. Das Skript ist etwas allgemeiner aber das ist wohl die wichtigste Schlussfolgerung.*

### Rückwärtswege
Die Umlaufszahl einer rückswärts durchlaufenen Schleife ist die Negierung der Schleife
[^2]

### UZ bei Zusammenhängenden Mengen
Die Funktion
$$n(\gamma, \cdot): \begin{array}{rcl}\mathbb{C}\backslash Spur(\gamma) &\to& \mathbb{Z} \\ a & \mapsto & n(\gamma, a)\end{array}$$ ist auf jeder [[Zusammenhängende Menge|zusammenhängenden]] Teilmenge konstant und damit [[Stetigkeit|stetig]].[^3]

### Inneres
Die Umlauffzahl ist in allen Punkten des [[Innere einer Schleife|Inneren]] von $\gamma$ nicht 0[^4]

### Äußeres
Auf jeder unbeschränkten Zusammenhangskomponente von $\mathbb{C}\backslash Spur(\gamma)$ ist die Umlaufzahl 0.[^4]

#Mathe-IV 

[^1]: Zenk -  Definition 22.2.1
[^2]: Zenk - Bemerkung 22.2.3
[^3]: Zenk - Lemma 22.2.5
[^4]: Zenk - Korrolar 22.2.6