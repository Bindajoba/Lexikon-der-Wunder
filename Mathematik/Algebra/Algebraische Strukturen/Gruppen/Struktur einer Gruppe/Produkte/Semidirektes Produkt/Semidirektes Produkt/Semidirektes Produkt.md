# Beschreibung
Führt man ein [[Äußeres Direktes Produkt (Gruppe)]] aus, erlaubt aber, dass die Pfeile des Cayley-Diagramms eines Faktors etwas getauscht werden, erhält man ein **Semidirektes Produkt**

![[Semidirektes Produkt Beispiel.png]]

Ist beim [[Inneres Direktes Produkt (Gruppe)]] nur eine Menge ein [[Normalteiler]], dann nennt man das Ergebnis ein **Semidirektes Inneres Produkt**

# Intuition
Wir haben bereits herausgefunden, dass alle möglichen [[Neuverkabelung|Neuverkabelungen]] eine [[Gruppe]] bilden.
Tatsächlich benötigt man aber noch nicht mal alle Neuverkabelungen, um eine Gruppe zu bilden. Häufig reicht nur ein Teil aus.
In beiden Fällen bildet das erzeugte [[Cayley-Diagramm]] ein Semidirektes Produkt $G \rtimes_\phi H$:
Die Neuverkabelungen von $G$ werden in die Knoten der Gruppe $H$ eingesetzt. 
Welche Verkabelung in welchen Knoten von $H$ reinkommt wird durch $\phi$ bestimmt. 
![[Semidirektes Produkt Intuition.png]]

Wir haben auch herausgefunden, dass Verkabelungen einfach nur [[Gruppenautomorphismus|Gruppenautomorphismen]] sind.
$\phi$ bildet also ein $h \in H$ auf einen [[Gruppenautomorphismus]] von $G$ ab


# Definition
## Äußeres Semidirektes Produkt
Seien $U, N$ Gruppen und $\phi: U \to Aut(N)$ ein Homomorphismus. Wir definieren auf $N\times U$ eine Verknüpfung $*$ durch
$$(n_1, u_1) * (n_2, u_2) = (n_1\phi(u_1)(n_2), u_1u_2) \text{ für } (n_1, u_1), (n_2, u_2) \in U\times N$$
Dann ist $(N \times U, *)$ eine Gruppe. Man nennt sie das äußere Produkt von N und U und bezeichnen sie mit $N \rtimes_\phi U$

*Es gibt noch ein inneres Semidirektes Produkt aber dass ist vom Resultat gliech dem äußeren.*


#Carter 