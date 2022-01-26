## Definition
Eine [[Halbgruppe]] $(G, *)$ wird Monoid genannt, wenn sie ein Neutralelement besitzt.

Ein Monoid wird zur [[Gruppe]], wenn jedes Element ein Inverses besitzt.

### Monoid-Homomorphismus
Sind $(G, *)$ und $(H, \circ)$ Monoide, dann ist eine Abbildung, welche mit den Verknüpfungen verträglich ist, d.h.
$$\phi(g_1 * g_2) = \phi(g_1) \circ \phi(g_2)$$
und das neutrale Element erhält
$$\phi(e_G) = e_H$$
ein Monoid-Homomorphismus.

Vergleiche auch [[Homomorphismus]].
*Bemerke, dass ein nicht-neutrales Element auch auf ein neutrales Element abbilden kann.*

## Eigenschaften
### Umwandlung in Gruppe
Sei $(G, *)$ ein Monoid und $G^{\times} \subset G$ die Teilmenge der invertierbaren Elemente.
Dann ist $G^\times$ abgeschlossen unter der Verknüpfung $*$ und $(G^\times, *)$ ist eine [[Gruppe]]. Das Neutralelement $e_G$ von $G$ ist zugleich das Neutralelement von $G^\times$ [^1]

*Diesen Satz kann man Nutzen um leicht einen Beweis einer Gruppe zu erbringen*

## Beispiele
### Multiplikation der Ganzen Zahlen
Die Mulitplikation auf den ganzen Zahlen ist eine Monoid, da Monoide nicht notwendigerweise ein Inverses Element verlangen.


### Menge aller Funktionen
Sei $X$ eine Menge und $Map(X)$ die Menge der Abbildungen $X \to X$.
Für $f,g \in Map(X)$ ist die Komposition eine [[Assoziativität|assoziative]] Verknüpfung mit dem Neutralelement $id_X$.

Damit ist $(Map(X), \circ)$ ein Monoid



#Algebra 

[^1]: Gerkmann - Satz 1.13